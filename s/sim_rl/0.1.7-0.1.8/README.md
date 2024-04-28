# Comparing `tmp/sim_rl-0.1.7.tar.gz` & `tmp/sim_rl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim_rl-0.1.7.tar", max compression
+gzip compressed data, was "sim_rl-0.1.8.tar", max compression
```

## Comparing `sim_rl-0.1.7.tar` & `sim_rl-0.1.8.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0      754 2024-04-28 20:17:33.805495 sim_rl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    14209 2024-04-28 20:17:21.903473 sim_rl-0.1.7/README.md
--rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.7/sim_rl/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.7/sim_rl/__init__.py
--rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.7/sim_rl/agents/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:57.799129 sim_rl-0.1.7/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3593 2024-04-28 15:25:57.812081 sim_rl-0.1.7/sim_rl/agents/__pycache__/buffer.cpython-310.pyc
--rw-r--r--   0        0        0    13843 2024-04-28 15:25:57.804520 sim_rl-0.1.7/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc
--rw-r--r--   0        0        0     9252 2024-04-28 15:25:57.809029 sim_rl-0.1.7/sim_rl/agents/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.7/sim_rl/agents/buffer.py
--rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.7/sim_rl/agents/ddpg_agent.py
--rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.7/sim_rl/agents/model.py
--rw-r--r--   0        0        0   282094 2024-04-28 15:26:02.560345 sim_rl-0.1.7/sim_rl/agents/trained_agent.pt
--rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.7/sim_rl/agents/trained_ddpg_agent.pt
--rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.7/sim_rl/debug.py
--rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.7/sim_rl/dist/sim_rl-0.1.0.tar.gz
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.7/sim_rl/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.7/sim_rl/evaluation/convergence_evaluation/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.7/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
--rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.7/sim_rl/evaluation/convergence_evaluation/reward_plot.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.7/sim_rl/evaluation/decision_evaluation/__init__.py
--rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.7/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
--rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.7/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.7/sim_rl/evaluation/noise_evaluation/__init__.py
--rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.7/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.7/sim_rl/evaluation/robustness_evaluation/__init__.py
--rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.7/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/__init__.py
--rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot.png
--rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
--rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
--rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
--rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
--rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.7/sim_rl/foundations/__init__.py
--rw-r--r--   0        0        0      162 2024-04-28 15:25:54.662508 sim_rl-0.1.7/sim_rl/foundations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    31515 2024-04-28 15:25:54.670219 sim_rl-0.1.7/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc
--rw-r--r--   0        0        0    10353 2024-04-28 15:25:58.846613 sim_rl-0.1.7/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/__init__.py
--rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
--rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
--rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
--rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
--rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
--rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
--rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
--rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
--rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.7/sim_rl/foundations/core_functions.py
--rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.7/sim_rl/foundations/core_plotting.py
--rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.7/sim_rl/foundations/output_csv/action_dict.csv
--rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.7/sim_rl/foundations/output_csv/actor_loss.csv
--rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.7/sim_rl/foundations/output_csv/critic_loss.csv
--rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.7/sim_rl/foundations/output_csv/next_state_model_loss.csv
--rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.7/sim_rl/foundations/output_csv/reward_dict.json
--rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.7/sim_rl/foundations/output_csv/reward_model_loss.csv
--rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.7/sim_rl/foundations/output_csv/transition_proba.csv
--rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.7/sim_rl/main.py
--rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.7/sim_rl/Makefile
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.7/sim_rl/queue_env/__init__.py
--rw-r--r--   0        0        0      160 2024-04-28 15:25:57.816084 sim_rl-0.1.7/sim_rl/queue_env/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9916 2024-04-28 15:25:58.842612 sim_rl-0.1.7/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc
--rw-r--r--   0        0        0     5432 2024-04-28 15:25:57.819081 sim_rl-0.1.7/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc
--rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.7/sim_rl/queue_env/queue_base_functions.py
--rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
--rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.gitignore
--rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.readthedocs.yml
--rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/CHANGELOG.md
--rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/CITATION.cff
--rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/cliff.toml
--rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
--rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
--rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
--rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
--rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
--rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
--rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
--rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
--rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
--rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
--rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
--rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
--rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/conf.py
--rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/current_state.png
--rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/current_state1.png
--rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
--rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
--rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/fig.png
--rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/graph.rst
--rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/index.rst
--rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/installation.rst
--rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/make.bat
--rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/Makefile
--rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/modules.rst
--rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/my_network.png
--rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/my_network1.png
--rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/network.rst
--rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/overview.rst
--rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/queues.rst
--rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/requirements.txt
--rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/sim.png
--rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/sim1.png
--rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/store.png
--rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/store1.png
--rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
--rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/LICENSE.txt
--rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/MANIFEST.in
--rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/poetry.lock
--rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/pyproject.toml
--rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
--rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
--rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
--rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
--rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
--rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
--rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
--rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
--rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
--rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
--rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
--rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
--rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
--rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
--rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
--rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
--rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
--rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/README.rst
--rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/setup.py
--rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
--rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
--rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
--rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_network.py
--rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
--rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
--rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
--rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.7/sim_rl/queue_env/queueing_network.py
--rw-r--r--   0        0        0      191 2024-04-28 17:02:38.117430 sim_rl-0.1.7/sim_rl/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.7/sim_rl/rl_env/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:58.834087 sim_rl-0.1.7/sim_rl/rl_env/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    14513 2024-04-28 15:25:58.838089 sim_rl-0.1.7/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc
--rw-r--r--   0        0        0    16235 2024-04-28 17:01:26.321399 sim_rl-0.1.7/sim_rl/rl_env/RL_Environment.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.7/sim_rl/tuning/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:58.827199 sim_rl-0.1.7/sim_rl/tuning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6466 2024-04-28 15:26:00.355144 sim_rl-0.1.7/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc
--rw-r--r--   0        0        0     5627 2024-04-28 15:25:58.831079 sim_rl-0.1.7/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc
--rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.7/sim_rl/tuning/ray_tuning.py
--rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.7/sim_rl/tuning/wandb_tuning.py
--rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.7/sim_rl/user_config/configuration.yml
--rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.7/sim_rl/user_config/eval_hyperparams.yml
--rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.7/sim_rl/user_config/tuning_hyperparams.yml
--rw-r--r--   0        0        0    14629 1970-01-01 00:00:00.000000 sim_rl-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-04-28 20:19:03.558595 sim_rl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    14210 2024-04-28 20:18:48.158953 sim_rl-0.1.8/README.md
+-rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.8/sim_rl/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.8/sim_rl/__init__.py
+-rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.8/sim_rl/agents/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:57.799129 sim_rl-0.1.8/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3593 2024-04-28 15:25:57.812081 sim_rl-0.1.8/sim_rl/agents/__pycache__/buffer.cpython-310.pyc
+-rw-r--r--   0        0        0    13843 2024-04-28 15:25:57.804520 sim_rl-0.1.8/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc
+-rw-r--r--   0        0        0     9252 2024-04-28 15:25:57.809029 sim_rl-0.1.8/sim_rl/agents/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.8/sim_rl/agents/buffer.py
+-rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.8/sim_rl/agents/ddpg_agent.py
+-rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.8/sim_rl/agents/model.py
+-rw-r--r--   0        0        0   282094 2024-04-28 15:26:02.560345 sim_rl-0.1.8/sim_rl/agents/trained_agent.pt
+-rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.8/sim_rl/agents/trained_ddpg_agent.pt
+-rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.8/sim_rl/debug.py
+-rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.8/sim_rl/dist/sim_rl-0.1.0.tar.gz
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.8/sim_rl/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.8/sim_rl/evaluation/convergence_evaluation/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.8/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
+-rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.8/sim_rl/evaluation/convergence_evaluation/reward_plot.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.8/sim_rl/evaluation/decision_evaluation/__init__.py
+-rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.8/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
+-rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.8/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.8/sim_rl/evaluation/noise_evaluation/__init__.py
+-rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.8/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.8/sim_rl/evaluation/robustness_evaluation/__init__.py
+-rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.8/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/__init__.py
+-rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot.png
+-rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
+-rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
+-rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
+-rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
+-rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.8/sim_rl/foundations/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-28 15:25:54.662508 sim_rl-0.1.8/sim_rl/foundations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    31515 2024-04-28 15:25:54.670219 sim_rl-0.1.8/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc
+-rw-r--r--   0        0        0    10353 2024-04-28 15:25:58.846613 sim_rl-0.1.8/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/__init__.py
+-rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
+-rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
+-rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
+-rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
+-rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
+-rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
+-rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
+-rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
+-rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.8/sim_rl/foundations/core_functions.py
+-rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.8/sim_rl/foundations/core_plotting.py
+-rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.8/sim_rl/foundations/output_csv/action_dict.csv
+-rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.8/sim_rl/foundations/output_csv/actor_loss.csv
+-rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.8/sim_rl/foundations/output_csv/critic_loss.csv
+-rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.8/sim_rl/foundations/output_csv/next_state_model_loss.csv
+-rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.8/sim_rl/foundations/output_csv/reward_dict.json
+-rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.8/sim_rl/foundations/output_csv/reward_model_loss.csv
+-rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.8/sim_rl/foundations/output_csv/transition_proba.csv
+-rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.8/sim_rl/main.py
+-rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.8/sim_rl/Makefile
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.8/sim_rl/queue_env/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-28 15:25:57.816084 sim_rl-0.1.8/sim_rl/queue_env/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9916 2024-04-28 15:25:58.842612 sim_rl-0.1.8/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     5432 2024-04-28 15:25:57.819081 sim_rl-0.1.8/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc
+-rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.8/sim_rl/queue_env/queue_base_functions.py
+-rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
+-rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.gitignore
+-rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.readthedocs.yml
+-rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/CHANGELOG.md
+-rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/CITATION.cff
+-rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/cliff.toml
+-rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
+-rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
+-rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
+-rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
+-rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
+-rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
+-rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
+-rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
+-rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
+-rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
+-rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
+-rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
+-rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/conf.py
+-rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/current_state.png
+-rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/current_state1.png
+-rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
+-rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
+-rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/fig.png
+-rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/graph.rst
+-rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/index.rst
+-rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/installation.rst
+-rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/make.bat
+-rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/Makefile
+-rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/modules.rst
+-rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/my_network.png
+-rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/my_network1.png
+-rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/network.rst
+-rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/overview.rst
+-rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/queues.rst
+-rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/requirements.txt
+-rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/sim.png
+-rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/sim1.png
+-rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/store.png
+-rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/store1.png
+-rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
+-rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/LICENSE.txt
+-rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/MANIFEST.in
+-rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/poetry.lock
+-rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
+-rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
+-rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
+-rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
+-rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
+-rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
+-rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
+-rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
+-rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
+-rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
+-rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
+-rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
+-rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
+-rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
+-rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
+-rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
+-rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/README.rst
+-rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/setup.py
+-rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
+-rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
+-rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
+-rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_network.py
+-rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
+-rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
+-rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
+-rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.8/sim_rl/queue_env/queueing_network.py
+-rw-r--r--   0        0        0      191 2024-04-28 17:02:38.117430 sim_rl-0.1.8/sim_rl/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.8/sim_rl/rl_env/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:58.834087 sim_rl-0.1.8/sim_rl/rl_env/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    14513 2024-04-28 15:25:58.838089 sim_rl-0.1.8/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc
+-rw-r--r--   0        0        0    16235 2024-04-28 17:01:26.321399 sim_rl-0.1.8/sim_rl/rl_env/RL_Environment.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.8/sim_rl/tuning/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:58.827199 sim_rl-0.1.8/sim_rl/tuning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6466 2024-04-28 15:26:00.355144 sim_rl-0.1.8/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc
+-rw-r--r--   0        0        0     5627 2024-04-28 15:25:58.831079 sim_rl-0.1.8/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc
+-rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.8/sim_rl/tuning/ray_tuning.py
+-rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.8/sim_rl/tuning/wandb_tuning.py
+-rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.8/sim_rl/user_config/configuration.yml
+-rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.8/sim_rl/user_config/eval_hyperparams.yml
+-rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.8/sim_rl/user_config/tuning_hyperparams.yml
+-rw-r--r--   0        0        0    14630 1970-01-01 00:00:00.000000 sim_rl-0.1.8/PKG-INFO
```

### Comparing `sim_rl-0.1.7/pyproject.toml` & `sim_rl-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sim_rl"
-version = "0.1.7"
+version = "0.1.8"
 description = "Simulation Driven RL Package Utilized to Optimize Queueing Systems"
 authors = ["Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi <fatima.al-ani23@imperial.ac.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 torch = "2.2.0"
```

### Comparing `sim_rl-0.1.7/README.md` & `sim_rl-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,843 +47,843 @@
 000002e0: 6e20 4576 616c 7561 7469 6f6e 2a2a 3a20  n Evaluation**: 
 000002f0: 4465 6d6f 6e73 7472 6174 6573 2068 6f77  Demonstrates how
 00000300: 2074 6865 2061 6765 6e74 2072 6573 706f   the agent respo
 00000310: 6e64 7320 746f 2061 2073 6572 7665 7220  nds to a server 
 00000320: 6f75 7461 6765 2062 7920 6164 6a75 7374  outage by adjust
 00000330: 696e 6720 726f 7574 696e 6720 7072 6f62  ing routing prob
 00000340: 6162 696c 6974 6965 732e 0d0a 2020 2d20  abilities...  - 
-00000350: 2a2a 436f 6e66 6964 656e 6365 2045 7661  **Confidence Eva
-00000360: 6c75 6174 696f 6e2a 2a3a 2041 7373 6573  luation**: Asses
-00000370: 7365 7320 7468 6520 7374 6162 696c 6974  ses the stabilit
-00000380: 7920 616e 6420 7265 6c69 6162 696c 6974  y and reliabilit
-00000390: 7920 6f66 2074 6865 2061 6765 6e74 2061  y of the agent a
-000003a0: 6372 6f73 7320 6469 6666 6572 656e 7420  cross different 
-000003b0: 7472 6169 6e69 6e67 2073 6574 7570 730d  training setups.
-000003c0: 0a20 202d 202a 2a4e 6f69 7365 2045 7661  .  - **Noise Eva
-000003d0: 6c75 6174 696f 6e2a 2a3a 2045 7661 6c75  luation**: Evalu
-000003e0: 6174 6520 7468 6520 6566 6665 6374 206f  ate the effect o
-000003f0: 6620 656e 7669 726f 6e6d 656e 7461 6c20  f environmental 
-00000400: 6e6f 6973 6520 6f6e 2074 6865 2070 6572  noise on the per
-00000410: 666f 726d 616e 6365 206f 6620 7468 6520  formance of the 
-00000420: 6167 656e 740d 0a20 202d 202a 2a53 7461  agent..  - **Sta
-00000430: 7274 7570 2045 7661 6c75 6174 696f 6e2a  rtup Evaluation*
-00000440: 2a3a 2049 6465 6e74 6966 6965 7320 7468  *: Identifies th
-00000450: 6520 6275 726e 2d69 6e20 7065 7269 6f64  e burn-in period
-00000460: 206f 6620 7468 6520 6167 656e 740d 0a20   of the agent.. 
-00000470: 202d 202a 2a52 6f62 7573 746e 6573 7320   - **Robustness 
-00000480: 4576 616c 7561 7469 6f6e 2a2a 3a20 4173  Evaluation**: As
-00000490: 7365 7373 2072 6f62 7573 746e 6573 7320  sess robustness 
-000004a0: 6f66 2064 6563 6973 696f 6e73 2061 6372  of decisions acr
-000004b0: 6f73 7320 6d75 6c74 6970 6c65 2074 7261  oss multiple tra
-000004c0: 696e 6564 2061 6765 6e74 730d 0a0d 0a23  ined agents....#
-000004d0: 2320 5072 6572 6571 7569 7369 7465 730d  # Prerequisites.
-000004e0: 0a0d 0a42 6566 6f72 6520 7275 6e6e 696e  ...Before runnin
-000004f0: 6720 7468 6520 7369 6d75 6c61 7469 6f6e  g the simulation
-00000500: 732c 2065 6e73 7572 6520 796f 7520 6861  s, ensure you ha
-00000510: 7665 2074 6865 2066 6f6c 6c6f 7769 6e67  ve the following
-00000520: 2069 6e73 7461 6c6c 6564 3a0d 0a2d 2050   installed:..- P
-00000530: 7974 686f 6e20 3e3d 332e 3130 203c 332e  ython >=3.10 <3.
-00000540: 3132 0d0a 2d20 746f 7263 6820 3d20 2232  12..- torch = "2
-00000550: 2e32 2e30 220d 0a2d 206e 756d 7079 203d  .2.0"..- numpy =
-00000560: 2022 312e 3236 2e34 220d 0a2d 2070 616e   "1.26.4"..- pan
-00000570: 6461 7320 3d20 2232 2e32 2e30 220d 0a2d  das = "2.2.0"..-
-00000580: 2071 7565 7565 696e 675f 746f 6f6c 203d   queueing_tool =
-00000590: 2022 312e 322e 3522 0d0a 2d20 6d61 7470   "1.2.5"..- matp
-000005a0: 6c6f 746c 6962 203d 2022 332e 382e 3322  lotlib = "3.8.3"
-000005b0: 0d0a 2d20 7761 6e64 6220 3d20 2230 2e31  ..- wandb = "0.1
-000005c0: 362e 3322 0d0a 2d20 5079 5941 4d4c 203d  6.3"..- PyYAML =
-000005d0: 2022 362e 302e 3122 0d0a 2d20 7261 7920   "6.0.1"..- ray 
-000005e0: 3d20 7b20 7665 7273 696f 6e20 3d20 2232  = { version = "2
-000005f0: 2e39 2e32 222c 2065 7874 7261 7320 3d20  .9.2", extras = 
-00000600: 5b22 7472 6169 6e22 2c20 2274 756e 6522  ["train", "tune"
-00000610: 5d20 7d0d 0a2d 2074 7164 6d20 3d20 2234  ] }..- tqdm = "4
-00000620: 2e35 372e 3022 0d0a 2d20 7363 6970 7920  .57.0"..- scipy 
-00000630: 3d20 2231 2e31 322e 3022 0d0a 0d0a 2323  = "1.12.0"....##
-00000640: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
-00000650: 0a43 6c6f 6e65 2074 6865 2072 6570 6f73  .Clone the repos
-00000660: 6974 6f72 7920 616e 6420 696e 7374 616c  itory and instal
-00000670: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
-00000680: 6570 656e 6465 6e63 6965 733a 0d0a 0d0a  ependencies:....
-00000690: 6060 6062 6173 680d 0a67 6974 2063 6c6f  ```bash..git clo
-000006a0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-000006b0: 622e 636f 6d2f 616f 2d34 3230 2f73 696d  b.com/ao-420/sim
-000006c0: 5f72 6c2e 6769 740d 0a63 6420 7369 6d5f  _rl.git..cd sim_
-000006d0: 726c 0d0a 7069 7020 696e 7374 616c 6c20  rl..pip install 
-000006e0: 2d72 2072 6571 7569 7265 6d65 6e74 732e  -r requirements.
-000006f0: 7478 740d 0a60 6060 0d0a 0d0a 2323 2053  txt..```....## S
-00000700: 7465 7020 313a 2043 6f6e 6669 6775 7261  tep 1: Configura
-00000710: 7469 6f6e 0d0a 0d0a 2323 2320 456e 7669  tion....### Envi
-00000720: 726f 6e6d 656e 7420 5365 7475 700d 0a0d  ronment Setup...
-00000730: 0a23 2323 2320 2a2a 5175 6575 6569 6e67  .#### **Queueing
-00000740: 2045 6e76 6972 6f6e 6d65 6e74 2043 6f6e   Environment Con
-00000750: 6669 6775 7261 7469 6f6e 2a2a 0d0a 0d0a  figuration**....
-00000760: 5468 6520 7369 6d75 6c61 7469 6f6e 2065  The simulation e
-00000770: 6e76 6972 6f6e 6d65 6e74 2072 6571 7569  nvironment requi
-00000780: 7265 7320 7468 6520 666f 6c6c 6f77 696e  res the followin
-00000790: 6720 7061 7261 6d65 7465 7273 2074 6f20  g parameters to 
-000007a0: 6265 2064 6566 696e 6564 2069 6e20 7468  be defined in th
-000007b0: 6520 6063 6f6e 6669 6775 7261 7469 6f6e  e `configuration
-000007c0: 2e79 6d6c 602e 0d0a 0d0a 2d20 6061 646a  .yml`.....- `adj
-000007d0: 6163 656e 745f 6c69 7374 603a 2041 2064  acent_list`: A d
-000007e0: 6963 7469 6f6e 6172 7920 6465 6669 6e69  ictionary defini
-000007f0: 6e67 2074 6865 2061 646a 6163 656e 6379  ng the adjacency
-00000800: 206c 6973 7420 666f 7220 7468 6520 6e65   list for the ne
-00000810: 7477 6f72 6b20 746f 706f 6c6f 6779 2e0d  twork topology..
-00000820: 0a2d 2060 6d69 755f 6469 6374 603a 2041  .- `miu_dict`: A
-00000830: 2064 6963 7469 6f6e 6172 7920 6f66 2073   dictionary of s
-00000840: 6572 7669 6365 2072 6174 6573 2066 6f72  ervice rates for
-00000850: 2065 6163 6820 7365 7276 6963 6520 6e6f   each service no
-00000860: 6465 2069 6e20 7468 6520 6e65 7477 6f72  de in the networ
-00000870: 6b2e 0d0a 2d20 6074 7261 6e73 6974 696f  k...- `transitio
-00000880: 6e5f 7072 6f62 615f 616c 6c60 3a20 4120  n_proba_all`: A 
-00000890: 6469 6374 696f 6e61 7279 2064 6566 696e  dictionary defin
-000008a0: 696e 6720 7468 6520 7472 616e 7369 7469  ing the transiti
-000008b0: 6f6e 2070 726f 6261 6269 6c69 7469 6573  on probabilities
-000008c0: 2062 6574 7765 656e 206e 6f64 6573 2e0d   between nodes..
-000008d0: 0a2d 2060 6163 7469 7665 5f63 6170 603a  .- `active_cap`:
-000008e0: 2054 6865 2061 6374 6976 6520 6361 7061   The active capa
-000008f0: 6369 7479 206f 6620 7468 6520 6e6f 6465  city of the node
-00000900: 7320 6672 6f6d 206f 7574 7369 6465 2074  s from outside t
-00000910: 6865 206e 6574 776f 726b 2e0d 0a2d 2060  he network...- `
-00000920: 6465 6163 7469 7665 5f74 603a 2054 6865  deactive_t`: The
-00000930: 2064 6561 6374 6976 6174 696f 6e20 7468   deactivation th
-00000940: 7265 7368 6f6c 6420 666f 7220 7468 6520  reshold for the 
-00000950: 6e6f 6465 7320 6672 6f6d 206f 7574 7369  nodes from outsi
-00000960: 6465 2074 6865 206e 6574 776f 726b 2e0d  de the network..
-00000970: 0a2d 2060 6275 6666 6572 5f73 697a 655f  .- `buffer_size_
-00000980: 666f 725f 6561 6368 5f71 7565 7565 603a  for_each_queue`:
-00000990: 2041 2064 6963 7469 6f6e 6172 7920 7468   A dictionary th
-000009a0: 6174 2064 6566 696e 6573 2074 6865 2062  at defines the b
-000009b0: 7566 6665 7220 7369 7a65 2066 6f72 2065  uffer size for e
-000009c0: 6163 6820 7175 6575 652e 0d0a 2d20 6061  ach queue...- `a
-000009d0: 7272 6976 616c 5f72 6174 6560 3a20 4120  rrival_rate`: A 
-000009e0: 6c69 7374 2074 6861 7420 6465 6669 6e65  list that define
-000009f0: 7320 7468 6520 6172 7269 7661 6c20 7261  s the arrival ra
-00000a00: 7465 7320 666f 7220 616c 6c20 706f 7373  tes for all poss
-00000a10: 6962 6c65 2065 6e74 7279 206e 6f64 6573  ible entry nodes
-00000a20: 2e0d 0a2d 2060 6d61 785f 6167 656e 7473  ...- `max_agents
-00000a30: 603a 2041 2076 616c 7565 2074 6861 7420  `: A value that 
-00000a40: 6465 6669 6e65 7320 7468 6520 6d61 7869  defines the maxi
-00000a50: 6d75 6d20 6e75 6d62 6572 206f 6620 6167  mum number of ag
-00000a60: 656e 7473 2063 616e 2062 6520 6163 6370  ents can be accp
-00000a70: 6574 6564 2066 726f 6d20 6f75 7473 6964  eted from outsid
-00000a80: 6520 7468 6520 6e65 7477 6f72 6b20 666f  e the network fo
-00000a90: 7220 7468 6520 656e 7472 7920 6e6f 6465  r the entry node
-00000aa0: 732e 0d0a 2d20 6073 696d 5f6a 6f62 7360  s...- `sim_jobs`
-00000ab0: 3a20 4120 7661 6c75 6520 7468 6174 2064  : A value that d
-00000ac0: 6566 696e 6573 2074 6865 206e 756d 6265  efines the numbe
-00000ad0: 7220 6f66 206a 6f62 7320 6265 696e 6720  r of jobs being 
-00000ae0: 7369 6d75 6c61 7465 6420 6475 7269 6e67  simulated during
-00000af0: 2065 7665 7279 2073 696d 756c 6174 696f   every simulatio
-00000b00: 6e2e 0d0a 2d20 606d 6178 5f61 7272 5f72  n...- `max_arr_r
-00000b10: 6174 655f 6c69 7374 603a 2041 206c 6973  ate_list`: A lis
-00000b20: 7420 7468 6174 2064 6566 696e 6573 2074  t that defines t
-00000b30: 6865 206d 6178 696d 756d 2061 7272 6976  he maximum arriv
-00000b40: 616c 2072 6174 6520 666f 7220 616c 6c20  al rate for all 
-00000b50: 656e 7472 7920 7175 6575 6573 2e0d 0a2d  entry queues...-
-00000b60: 2060 656e 7472 795f 6e6f 6465 7360 3a20   `entry_nodes`: 
-00000b70: 4120 6c69 7374 2074 6861 7420 6465 6669  A list that defi
-00000b80: 6e65 7320 7468 6520 736f 7572 6365 2061  nes the source a
-00000b90: 6e64 2074 6172 6765 7420 7665 7274 6963  nd target vertic
-00000ba0: 6573 206f 6620 6561 6368 2065 6e74 7279  es of each entry
-00000bb0: 206e 6f64 652e 0d0a 0d0a 2020 2045 7861   node.....   Exa
-00000bc0: 6d70 6c65 3a0d 0a20 2020 6060 6079 616d  mple:..   ```yam
-00000bd0: 6c0d 0a20 2020 6d69 755f 6c69 7374 3a20  l..   miu_list: 
-00000be0: 200d 0a20 2020 313a 2030 2e32 3530 0d0a   ..   1: 0.250..
-00000bf0: 2020 2032 3a20 302e 3235 0d0a 2020 2033     2: 0.25..   3
-00000c00: 3a20 302e 3031 3530 300d 0a20 2020 343a  : 0.01500..   4:
-00000c10: 2031 3030 0d0a 2020 2035 3a20 312e 3230   100..   5: 1.20
-00000c20: 0d0a 2020 2036 3a20 302e 3031 3030 300d  ..   6: 0.01000.
-00000c30: 0a20 2020 373a 2031 300d 0a20 2020 383a  .   7: 10..   8:
-00000c40: 2030 2e31 3030 300d 0a20 2020 393a 2030   0.1000..   9: 0
-00000c50: 2e35 3030 0d0a 0d0a 2020 2061 646a 6163  .500....   adjac
-00000c60: 656e 745f 6c69 7374 3a0d 0a20 2020 303a  ent_list:..   0:
-00000c70: 205b 315d 0d0a 2020 2031 3a20 5b32 2c20   [1]..   1: [2, 
-00000c80: 332c 2034 5d0d 0a20 2020 323a 205b 355d  3, 4]..   2: [5]
-00000c90: 0d0a 2020 2033 3a20 5b36 2c20 375d 0d0a  ..   3: [6, 7]..
-00000ca0: 2020 2034 3a20 5b38 5d0d 0a20 2020 353a     4: [8]..   5:
-00000cb0: 205b 395d 0d0a 2020 2036 3a20 5b39 5d0d   [9]..   6: [9].
-00000cc0: 0a20 2020 373a 205b 395d 0d0a 2020 2038  .   7: [9]..   8
-00000cd0: 3a20 5b39 5d0d 0a20 2020 393a 205b 3130  : [9]..   9: [10
-00000ce0: 5d0d 0a0d 0a20 2020 6275 6666 6572 5f73  ]....   buffer_s
-00000cf0: 697a 655f 666f 725f 6561 6368 5f71 7565  ize_for_each_que
-00000d00: 7565 3a20 0d0a 2020 2030 3a20 3530 3030  ue: ..   0: 5000
-00000d10: 0d0a 2020 2031 3a20 3530 3030 0d0a 2020  ..   1: 5000..  
-00000d20: 2032 3a20 3530 3030 0d0a 2020 2033 3a20   2: 5000..   3: 
-00000d30: 3530 3030 0d0a 2020 2034 3a20 3530 3030  5000..   4: 5000
-00000d40: 0d0a 2020 2035 3a20 3530 3030 0d0a 2020  ..   5: 5000..  
-00000d50: 2036 3a20 3530 3030 0d0a 2020 2037 3a20   6: 5000..   7: 
-00000d60: 3530 3030 0d0a 2020 2038 3a20 3530 3030  5000..   8: 5000
-00000d70: 0d0a 2020 2039 3a20 3530 3030 0d0a 2020  ..   9: 5000..  
-00000d80: 2031 303a 2035 3030 300d 0a20 2020 3131   10: 5000..   11
-00000d90: 3a20 3530 3030 0d0a 2020 2031 323a 2035  : 5000..   12: 5
-00000da0: 3030 300d 0a0d 0a20 2020 7472 616e 7369  000....   transi
-00000db0: 7469 6f6e 5f70 726f 6261 5f61 6c6c 3a0d  tion_proba_all:.
-00000dc0: 0a20 2020 303a 207b 313a 2031 7d0d 0a20  .   0: {1: 1}.. 
-00000dd0: 2020 313a 207b 323a 2030 2e33 332c 2033    1: {2: 0.33, 3
-00000de0: 3a20 302e 3333 2c20 343a 2030 2e33 347d  : 0.33, 4: 0.34}
-00000df0: 0d0a 2020 2032 3a20 7b35 3a20 317d 0d0a  ..   2: {5: 1}..
-00000e00: 2020 2033 3a20 7b36 3a20 302e 352c 2037     3: {6: 0.5, 7
-00000e10: 3a20 302e 357d 0d0a 2020 2034 3a20 7b38  : 0.5}..   4: {8
-00000e20: 3a20 317d 0d0a 2020 2035 3a20 7b39 3a20  : 1}..   5: {9: 
-00000e30: 317d 0d0a 2020 2036 3a20 7b39 3a20 317d  1}..   6: {9: 1}
-00000e40: 0d0a 2020 2037 3a20 7b39 3a20 317d 0d0a  ..   7: {9: 1}..
-00000e50: 2020 2038 3a20 7b39 3a20 317d 0d0a 2020     8: {9: 1}..  
-00000e60: 2039 3a20 7b31 303a 2031 7d0d 0a20 2020   9: {10: 1}..   
-00000e70: 0d0a 2020 2061 6374 6976 655f 6361 703a  ..   active_cap:
-00000e80: 2035 0d0a 0d0a 2020 2064 6561 6374 6976   5....   deactiv
-00000e90: 655f 743a 2030 2e31 320d 0a0d 0a20 2020  e_t: 0.12....   
-00000ea0: 6172 7269 7661 6c5f 7261 7465 3a20 5b30  arrival_rate: [0
-00000eb0: 2e33 5d0d 0a0d 0a20 2020 6d61 785f 6167  .3]....   max_ag
-00000ec0: 656e 7473 3a20 696e 660d 0a0d 0a20 2020  ents: inf....   
-00000ed0: 7369 6d5f 6a6f 6273 3a20 3130 300d 0a0d  sim_jobs: 100...
-00000ee0: 0a20 2020 6d61 785f 6172 725f 7261 7465  .   max_arr_rate
-00000ef0: 5f6c 6973 743a 205b 302e 335d 0d0a 0d0a  _list: [0.3]....
-00000f00: 2020 2065 6e74 7279 5f6e 6f64 6573 3a0d     entry_nodes:.
-00000f10: 0a20 2020 2d20 5b30 2c20 315d 200d 0a20  .   - [0, 1] .. 
-00000f20: 2020 6060 600d 0a0d 0a23 2323 2320 2a2a    ```....#### **
-00000f30: 524c 2045 6e76 6972 6f6e 6d65 6e74 2050  RL Environment P
-00000f40: 6172 616d 6574 6572 732a 2a0d 0a0d 0a53  arameters**....S
-00000f50: 6574 2075 7020 7468 6520 524c 2065 6e76  et up the RL env
-00000f60: 6972 6f6e 6d65 6e74 2070 6172 616d 6574  ironment paramet
-00000f70: 6572 7320 696e 2060 6576 616c 5f68 7970  ers in `eval_hyp
-00000f80: 6572 7061 7261 6d73 2e79 6d6c 603a 0d0a  erparams.yml`:..
-00000f90: 0d0a 2d20 606e 756d 5f65 7069 736f 6465  ..- `num_episode
-00000fa0: 7360 3a20 5468 6520 6e75 6d62 6572 206f  s`: The number o
-00000fb0: 6620 6570 6973 6f64 6573 2074 6f20 7275  f episodes to ru
-00000fc0: 6e20 7468 6520 7369 6d75 6c61 7469 6f6e  n the simulation
-00000fd0: 2e0d 0a2d 2060 6e75 6d5f 6570 6f63 6873  ...- `num_epochs
-00000fe0: 603a 2054 6865 206e 756d 6265 7220 6f66  `: The number of
-00000ff0: 2065 706f 6368 7320 666f 7220 7472 6169   epochs for trai
-00001000: 6e69 6e67 2e0d 0a2d 2060 7469 6d65 5f73  ning...- `time_s
-00001010: 7465 7073 603a 2054 6865 206e 756d 6265  teps`: The numbe
-00001020: 7220 6f66 2074 696d 6520 7374 6570 7320  r of time steps 
-00001030: 696e 2065 6163 6820 6570 6973 6f64 652e  in each episode.
-00001040: 0d0a 2d20 6062 6174 6368 5f73 697a 6560  ..- `batch_size`
-00001050: 3a20 5369 7a65 206f 6620 7468 6520 6261  : Size of the ba
-00001060: 7463 6820 7573 6564 2069 6e20 7472 6169  tch used in trai
-00001070: 6e69 6e67 2e20 2844 6566 6175 6c74 2069  ning. (Default i
-00001080: 7320 6571 7561 6c20 746f 2074 696d 655f  s equal to time_
-00001090: 7374 6570 7329 0d0a 2d20 606e 756d 5f73  steps)..- `num_s
-000010a0: 696d 603a 2054 6865 206e 756d 6265 7220  im`: The number 
-000010b0: 6f66 2073 696d 756c 6174 696f 6e73 2074  of simulations t
-000010c0: 6f20 7275 6e20 6475 7269 6e67 2074 7261  o run during tra
-000010d0: 696e 696e 672e 0d0a 2d20 6074 6175 603a  ining...- `tau`:
-000010e0: 2043 6f65 6666 6963 6965 6e74 2066 6f72   Coefficient for
-000010f0: 2073 6f66 7420 7570 6461 7465 206f 6620   soft update of 
-00001100: 7468 6520 7461 7267 6574 2070 6172 616d  the target param
-00001110: 6574 6572 732e 0d0a 2d20 6061 6374 6f72  eters...- `actor
-00001120: 5f6c 7260 3a20 4c65 6172 6e69 6e67 2072  _lr`: Learning r
-00001130: 6174 6520 666f 7220 7468 6520 4163 746f  ate for the Acto
-00001140: 7220 6e65 7477 6f72 6b20 6f70 7469 6d69  r network optimi
-00001150: 7a65 722e 0d0a 2d20 6063 7269 7469 635f  zer...- `critic_
-00001160: 6c72 603a 204c 6561 726e 696e 6720 7261  lr`: Learning ra
-00001170: 7465 2066 6f72 2074 6865 2043 7269 7469  te for the Criti
-00001180: 6320 4e65 7477 6f72 6b20 6f70 7469 6d69  c Network optimi
-00001190: 7a65 722e 0d0a 2d20 6064 6973 636f 756e  zer...- `discoun
-000011a0: 7460 3a20 4469 7363 6f75 6e74 2066 6163  t`: Discount fac
-000011b0: 746f 7220 666f 7220 6675 7475 7265 2072  tor for future r
-000011c0: 6577 6172 6473 2e0d 0a2d 2060 706c 616e  ewards...- `plan
-000011d0: 6e69 6e67 5f73 7465 7073 603a 2054 6865  ning_steps`: The
-000011e0: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
-000011f0: 2064 7572 696e 6720 706c 616e 6e69 6e67   during planning
-00001200: 2e0d 0a2d 2060 706c 616e 6e69 6e67 5f73  ...- `planning_s
-00001210: 7464 603a 2053 7461 6e64 6172 6420 6465  td`: Standard de
-00001220: 7669 6174 696f 6e20 6f66 2074 6865 206e  viation of the n
-00001230: 6f72 6d61 6c20 6469 7374 7572 6261 6e63  ormal disturbanc
-00001240: 6520 6475 7269 6e67 2070 6c61 6e6e 696e  e during plannin
-00001250: 672e 0d0a 2d20 6061 6374 6f72 5f6e 6574  g...- `actor_net
-00001260: 776f 726b 603a 204e 6574 776f 726b 2061  work`: Network a
-00001270: 7263 6869 7465 6374 7572 6520 666f 7220  rchitecture for 
-00001280: 6163 746f 7220 6e65 7477 6f72 6b2e 0d0a  actor network...
-00001290: 2d20 6063 7269 7469 635f 6e65 7477 6f72  - `critic_networ
-000012a0: 6b60 3a20 4e65 7477 6f72 6b20 6172 6368  k`: Network arch
-000012b0: 6974 6563 7475 7265 2066 6f72 2063 7269  itecture for cri
-000012c0: 7469 6320 6e65 7477 6f72 6b2e 0d0a 2d20  tic network...- 
-000012d0: 6072 6577 6172 645f 6d6f 6465 6c60 3a20  `reward_model`: 
-000012e0: 4e65 7477 6f72 6b20 6172 6368 6974 6563  Network architec
-000012f0: 7475 7265 2066 6f72 2072 6577 6172 6420  ture for reward 
-00001300: 6d6f 6465 6c20 7573 6420 696e 2070 6c61  model usd in pla
-00001310: 6e6e 696e 672e 0d0a 6020 606e 6578 745f  nning...` `next_
-00001320: 7374 6174 655f 6d6f 6465 6c60 3a20 4e65  state_model`: Ne
-00001330: 7477 6f72 6b20 6172 6368 6974 6563 7475  twork architectu
-00001340: 7265 2066 6f72 206e 6578 7420 7374 6174  re for next stat
-00001350: 6520 6d6f 6465 6c20 7573 6564 2069 6e20  e model used in 
-00001360: 706c 616e 6e69 6e67 2e20 0d0a 0d0a 2020  planning. ....  
-00001370: 2045 7861 6d70 6c65 3a0d 0a20 2020 6060   Example:..   ``
-00001380: 6079 616d 6c0d 0a20 2020 6e75 6d5f 6570  `yaml..   num_ep
-00001390: 6973 6f64 6573 3a20 350d 0a0d 0a20 2020  isodes: 5....   
-000013a0: 7468 7265 7368 6f6c 643a 2031 300d 0a0d  threshold: 10...
-000013b0: 0a20 2020 6e75 6d5f 6570 6f63 6873 3a20  .   num_epochs: 
-000013c0: 3130 300d 0a0d 0a20 2020 7469 6d65 5f73  100....   time_s
-000013d0: 7465 7073 3a20 3330 0d0a 0d0a 2020 2062  teps: 30....   b
-000013e0: 6174 6368 5f73 697a 653a 2033 300d 0a20  atch_size: 30.. 
-000013f0: 2020 0d0a 2020 2074 6172 6765 745f 7570    ..   target_up
-00001400: 6461 7465 5f66 7265 7175 656e 6379 3a20  date_frequency: 
-00001410: 3130 300d 0a20 2020 0d0a 2020 2062 7566  100..   ..   buf
-00001420: 6665 725f 7369 7a65 3a20 3130 3030 300d  fer_size: 10000.
-00001430: 0a20 2020 0d0a 2020 206e 756d 5f73 696d  .   ..   num_sim
-00001440: 3a20 3130 0d0a 2020 200d 0a20 2020 7461  : 10..   ..   ta
-00001450: 753a 2030 2e35 0d0a 0d0a 2020 206e 756d  u: 0.5....   num
-00001460: 5f74 7261 696e 5f41 433a 2031 300d 0a20  _train_AC: 10.. 
-00001470: 2020 0d0a 2020 2063 7269 7469 635f 6c72    ..   critic_lr
-00001480: 3a20 302e 3031 0d0a 0d0a 2020 2061 6374  : 0.01....   act
-00001490: 6f72 5f6c 723a 2030 2e30 3030 310d 0a20  or_lr: 0.0001.. 
-000014a0: 2020 0d0a 2020 2064 6973 636f 756e 743a    ..   discount:
-000014b0: 2030 2e38 0d0a 2020 200d 0a20 2020 706c   0.8..   ..   pl
-000014c0: 616e 6e69 6e67 5f73 7465 7073 3a20 3130  anning_steps: 10
-000014d0: 0d0a 2020 200d 0a20 2020 706c 616e 6e69  ..   ..   planni
-000014e0: 6e67 5f73 7464 3a20 302e 310d 0a0d 0a20  ng_std: 0.1.... 
-000014f0: 2020 6163 746f 725f 6e65 7477 6f72 6b3a    actor_network:
-00001500: 0d0a 2020 202d 2036 340d 0a20 2020 2d20  ..   - 64..   - 
-00001510: 3634 0d0a 2020 202d 2036 340d 0a0d 0a20  64..   - 64.... 
-00001520: 2020 6372 6974 6963 3a0d 0a20 2020 2d20    critic:..   - 
-00001530: 3634 0d0a 2020 202d 2036 340d 0a20 2020  64..   - 64..   
-00001540: 2d20 3634 0d0a 0d0a 2020 2072 6577 6172  - 64....   rewar
-00001550: 645f 6d6f 6465 6c3a 0d0a 2020 202d 2033  d_model:..   - 3
-00001560: 320d 0a20 2020 2d20 3634 0d0a 2020 202d  2..   - 64..   -
-00001570: 2036 340d 0a20 2020 2d20 3332 0d0a 0d0a   64..   - 32....
-00001580: 2020 206e 6578 745f 7374 6174 655f 6d6f     next_state_mo
-00001590: 6465 6c3a 0d0a 2020 202d 2033 320d 0a20  del:..   - 32.. 
-000015a0: 2020 2d20 3634 0d0a 2020 202d 2036 340d    - 64..   - 64.
-000015b0: 0a20 2020 2d20 3332 0d0a 2020 2060 6060  .   - 32..   ```
-000015c0: 0d0a 0d0a 2323 2323 202a 2a54 756e 696e  ....#### **Tunin
-000015d0: 6720 436f 6e66 6967 7572 6174 696f 6e2a  g Configuration*
-000015e0: 2a0d 0a53 6574 2075 7020 7468 6520 6879  *..Set up the hy
-000015f0: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
-00001600: 696e 6720 7261 6e67 6573 2069 6e20 6074  ing ranges in `t
-00001610: 756e 696e 675f 7061 7261 6d73 2e79 6d6c  uning_params.yml
-00001620: 603a 0d0a 0d0a 2d20 606c 725f 6d69 6e2f  `:....- `lr_min/
-00001630: 6d61 7860 3a20 4d69 6e20 616e 6420 6d61  max`: Min and ma
-00001640: 7820 7261 6e67 6573 206f 6620 7468 6520  x ranges of the 
-00001650: 6c65 6172 6e69 6e67 2072 6174 6520 6265  learning rate be
-00001660: 696e 6720 7475 6e65 642e 0d0a 2d20 6065  ing tuned...- `e
-00001670: 706f 6368 735f 6c69 7374 603a 2041 206c  pochs_list`: A l
-00001680: 6973 7420 7468 6174 2064 6566 696e 6573  ist that defines
-00001690: 2074 6865 2072 616e 6765 206f 6620 706f   the range of po
-000016a0: 7373 6962 6c65 2065 706f 6368 7320 746f  ssible epochs to
-000016b0: 2074 7261 696e 2072 6577 6172 6420 6d6f   train reward mo
-000016c0: 6465 6c20 616e 6420 6e65 7874 2073 7461  del and next sta
-000016d0: 7465 206d 6f64 656c 2e0d 0a2d 2060 6261  te model...- `ba
-000016e0: 7463 685f 7369 7a65 603a 2041 206c 6973  tch_size`: A lis
-000016f0: 7420 7468 6174 2064 6566 696e 6573 2074  t that defines t
-00001700: 6865 2072 616e 6765 206f 6620 6261 7463  he range of batc
-00001710: 6820 7369 7a65 7320 746f 2073 616d 706c  h sizes to sampl
-00001720: 6520 6672 6f6d 2074 6865 2072 6570 6c61  e from the repla
-00001730: 7920 6275 6666 6572 2e0d 0a2d 2060 7461  y buffer...- `ta
-00001740: 755f 6d69 6e2f 6d61 7860 3a20 4d69 6e20  u_min/max`: Min 
-00001750: 616e 6420 6d61 7820 7261 6e67 6573 206f  and max ranges o
-00001760: 6620 7468 6520 736f 6674 2075 7064 6174  f the soft updat
-00001770: 6520 7061 7261 6d65 7465 7273 2e0d 0a2d  e parameters...-
-00001780: 2060 6469 7363 6f75 6e74 206d 696e 2f6d   `discount min/m
-00001790: 6178 603a 204d 696e 2061 6e64 206d 6178  ax`: Min and max
-000017a0: 2072 616e 6765 7320 6f66 2074 6865 2064   ranges of the d
-000017b0: 6973 636f 756e 7420 6661 6374 6f72 2066  iscount factor f
-000017c0: 6f72 2066 7574 7572 6520 7265 7761 7264  or future reward
-000017d0: 732e 0d0a 2d20 6065 7073 696c 6f6e 5f6d  s...- `epsilon_m
-000017e0: 696e 2f6d 6178 603a 204d 696e 2061 6e64  in/max`: Min and
-000017f0: 206d 6178 2072 616e 6765 7320 6f66 2074   max ranges of t
-00001800: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-00001810: 6174 696f 6e20 6f66 206e 6f72 6d61 6c20  ation of normal 
-00001820: 6469 7374 7572 6261 6e63 6573 2064 7572  disturbances dur
-00001830: 696e 6720 706c 616e 6e69 6e67 2e0d 0a2d  ing planning...-
-00001840: 2060 706c 616e 6e69 6e67 5f73 7465 7073   `planning_steps
-00001850: 603a 2041 206c 6973 7420 7468 6174 2064  `: A list that d
-00001860: 6566 696e 6573 2070 6f73 7369 626c 6520  efines possible 
-00001870: 7374 6570 7320 666f 7220 706c 616e 6e69  steps for planni
-00001880: 6e67 2e0d 0a2d 2060 7731 2f77 3260 3a20  ng...- `w1/w2`: 
-00001890: 5765 6967 6874 2070 6172 616d 6574 6572  Weight parameter
-000018a0: 7320 7468 6174 2069 6e66 6c75 656e 6365  s that influence
-000018b0: 2074 6865 2065 7870 6c6f 7261 7469 6f6e   the exploration
-000018c0: 2062 6574 7765 656e 206b 6579 2061 6e64   between key and
-000018d0: 2070 6572 6970 6865 7261 6c20 7374 6174   peripheral stat
-000018e0: 6573 2e0d 0a2d 2060 6e75 6d5f 6570 6973  es...- `num_epis
-000018f0: 6f64 6573 603a 2041 206c 6973 7420 7468  odes`: A list th
-00001900: 6174 2064 6566 696e 6573 2074 6865 2070  at defines the p
-00001910: 6f73 7369 626c 6520 6e75 6d62 6572 7320  ossible numbers 
-00001920: 6f66 2065 7069 736f 6465 7320 746f 2074  of episodes to t
-00001930: 7261 696e 2074 6865 2061 6765 6e74 732e  rain the agents.
-00001940: 0d0a 2d20 6074 696d 655f 7374 6570 7360  ..- `time_steps`
-00001950: 3a20 4120 6c69 7374 2074 6861 7420 6465  : A list that de
-00001960: 6669 6e65 7320 7468 6520 706f 7373 6962  fines the possib
-00001970: 6c65 206e 756d 6265 7220 6f66 2074 696d  le number of tim
-00001980: 6520 7374 6570 7320 6475 7269 6e67 2065  e steps during e
-00001990: 6163 6820 6570 6973 6f64 650d 0a0d 0a20  ach episode.... 
-000019a0: 2020 4578 616d 706c 653a 0d0a 2020 2060    Example:..   `
-000019b0: 6060 7961 6d6c 0d0a 2020 206c 6561 726e  ``yaml..   learn
-000019c0: 696e 675f 7261 7465 5f6d 6178 3a20 302e  ing_rate_max: 0.
-000019d0: 310d 0a20 2020 6c65 6172 6e69 6e67 5f72  1..   learning_r
-000019e0: 6174 655f 6d69 6e3a 2030 2e30 3031 0d0a  ate_min: 0.001..
-000019f0: 0d0a 2020 2065 706f 6368 735f 6c69 7374  ..   epochs_list
-00001a00: 3a0d 0a20 2020 2d20 3130 0d0a 2020 202d  :..   - 10..   -
-00001a10: 2031 300d 0a20 2020 2d20 3130 0d0a 0d0a   10..   - 10....
-00001a20: 2020 2062 6174 6368 5f73 697a 653a 0d0a     batch_size:..
-00001a30: 2020 202d 2031 360d 0a20 2020 2d20 3332     - 16..   - 32
-00001a40: 0d0a 2020 202d 2036 340d 0a0d 0a20 2020  ..   - 64....   
-00001a50: 7461 755f 6d69 6e3a 2030 2e30 3030 350d  tau_min: 0.0005.
-00001a60: 0a20 2020 7461 755f 6d61 783a 2030 2e30  .   tau_max: 0.0
-00001a70: 3032 0d0a 0d0a 2020 2064 6973 636f 756e  02....   discoun
-00001a80: 745f 6d69 6e3a 2030 2e31 0d0a 2020 2064  t_min: 0.1..   d
-00001a90: 6973 636f 756e 745f 6d61 783a 2030 2e33  iscount_max: 0.3
-00001aa0: 0d0a 0d0a 2020 2065 7073 696c 6f6e 5f6d  ....   epsilon_m
-00001ab0: 696e 3a20 302e 310d 0a20 2020 6570 7369  in: 0.1..   epsi
-00001ac0: 6c6f 6e5f 6d61 783a 2030 2e33 0d0a 0d0a  lon_max: 0.3....
-00001ad0: 2020 2070 6c61 6e6e 696e 675f 7374 6570     planning_step
-00001ae0: 733a 200d 0a20 2020 2d20 3130 0d0a 0d0a  s: ..   - 10....
-00001af0: 2020 206e 756d 5f73 616d 706c 653a 200d     num_sample: .
-00001b00: 0a20 2020 2d20 3530 0d0a 0d0a 2020 2077  .   - 50....   w
-00001b10: 313a 200d 0a20 2020 2d20 302e 350d 0a0d  1: ..   - 0.5...
-00001b20: 0a20 2020 7732 3a20 0d0a 2020 202d 2030  .   w2: ..   - 0
-00001b30: 2e35 0d0a 0d0a 2020 206e 756d 5f65 7069  .5....   num_epi
-00001b40: 736f 6465 733a 200d 0a20 2020 2d20 350d  sodes: ..   - 5.
-00001b50: 0a0d 0a20 2020 7469 6d65 5f73 7465 7073  ...   time_steps
-00001b60: 3a20 0d0a 2020 202d 2031 300d 0a20 2020  : ..   - 10..   
-00001b70: 0d0a 2020 206e 756d 5f74 7261 696e 5f41  ..   num_train_A
-00001b80: 433a 200d 0a20 2020 2d20 3130 0d0a 0d0a  C: ..   - 10....
-00001b90: 2020 2060 6060 0d0a 0d0a 2323 2053 7465     ```....## Ste
-00001ba0: 7020 323a 2052 756e 6e69 6e67 2053 696d  p 2: Running Sim
-00001bb0: 756c 6174 696f 6e73 0d0a 0d0a 2323 2320  ulations....### 
-00001bc0: 5472 6169 6e69 6e67 2041 6765 6e74 0d0a  Training Agent..
-00001bd0: 5468 6973 2063 6f6d 6d61 6e64 2073 7461  This command sta
-00001be0: 7274 7320 7472 6169 6e69 6e67 2074 6865  rts training the
-00001bf0: 2061 6765 6e74 2077 6974 6869 6e20 7468   agent within th
-00001c00: 6520 7369 6d75 6c61 7465 6420 7175 6575  e simulated queu
-00001c10: 6569 6e67 2065 6e76 6972 6f6e 6d65 6e74  eing environment
-00001c20: 2e20 5265 7375 6c74 7320 6172 6520 7361  . Results are sa
-00001c30: 7665 6420 696e 2060 2f66 6f75 6e64 6174  ved in `/foundat
-00001c40: 696f 6e73 2f6f 7574 7075 745f 6373 7660  ions/output_csv`
-00001c50: 2061 6e64 2060 2f66 6f75 6e64 6174 696f   and `/foundatio
-00001c60: 6e73 2f6f 7574 7075 745f 706c 6f74 7360  ns/output_plots`
-00001c70: 2e0d 0a0d 0a60 6060 6261 7368 0d0a 7079  .....```bash..py
-00001c80: 7468 6f6e 206d 6169 6e2e 7079 202d 2d66  thon main.py --f
-00001c90: 756e 6374 696f 6e20 7472 6169 6e20 2d2d  unction train --
-00001ca0: 636f 6e66 6967 5f66 696c 6520 7573 6572  config_file user
-00001cb0: 5f63 6f6e 6669 672f 636f 6e66 6967 7572  _config/configur
-00001cc0: 6174 696f 6e2e 796d 6c20 2d2d 7061 7261  ation.yml --para
-00001cd0: 6d5f 6669 6c65 2075 7365 725f 636f 6e66  m_file user_conf
-00001ce0: 6967 2f65 7661 6c5f 6879 7065 7270 6172  ig/eval_hyperpar
-00001cf0: 616d 732e 796d 6c20 2d2d 6461 7461 5f66  ams.yml --data_f
-00001d00: 696c 6520 6f75 7470 7574 5f63 7376 202d  ile output_csv -
-00001d10: 2d69 6d61 6765 5f66 696c 6520 6f75 7470  -image_file outp
-00001d20: 7574 5f70 6c6f 7473 202d 2d70 6c6f 745f  ut_plots --plot_
-00001d30: 6375 7276 6573 2054 7275 6520 2d2d 7361  curves True --sa
-00001d40: 7665 5f66 696c 6520 5472 7565 0d0a 6060  ve_file True..``
-00001d50: 600d 0a0d 0a23 2323 2048 7970 6572 7061  `....### Hyperpa
-00001d60: 7261 6d65 7465 7220 5475 6e69 6e67 0d0a  rameter Tuning..
-00001d70: 0d0a 4265 6c6f 7720 7072 6f76 6964 6573  ..Below provides
-00001d80: 2075 7365 7273 2074 776f 2074 7970 6573   users two types
-00001d90: 206f 6620 7475 6e69 6e67 2073 7472 6174   of tuning strat
-00001da0: 6567 6965 7320 7468 6174 2066 6561 7475  egies that featu
-00001db0: 7265 2064 6966 6665 7265 6e74 2066 756e  re different fun
-00001dc0: 6374 696f 6e61 6c69 7469 6573 2e0d 0a0d  ctionalities....
-00001dd0: 0a23 2323 2320 2a2a 5761 6e64 6220 5475  .#### **Wandb Tu
-00001de0: 6e69 6e67 2a2a 0d0a 0d0a 4120 6d61 6368  ning**....A mach
-00001df0: 696e 6520 6c65 6172 6e69 6e67 2064 6576  ine learning dev
-00001e00: 656c 6f70 6d65 6e74 2070 6c61 7466 6f72  elopment platfor
-00001e10: 6d20 7468 6174 2061 6c6c 6f77 7320 7573  m that allows us
-00001e20: 6572 7320 746f 2074 7261 636b 2061 6e64  ers to track and
-00001e30: 2076 6973 7561 6c69 7a65 2076 6172 6f75   visualize varou
-00001e40: 2061 7370 6563 7473 206f 6620 7468 6569   aspects of thei
-00001e50: 7220 6d6f 6465 6c20 7472 6169 6e69 6e67  r model training
-00001e60: 2070 726f 6365 7373 2069 6e20 7265 616c   process in real
-00001e70: 2d74 696d 652c 2069 6e63 6c75 6469 6e67  -time, including
-00001e80: 206c 6f73 7320 616e 6420 6163 6375 7261   loss and accura
-00001e90: 6379 2063 6861 7274 732c 2070 6172 616d  cy charts, param
-00001ea0: 6574 6572 2064 6973 7472 6962 7574 696f  eter distributio
-00001eb0: 6e73 2c20 6772 6164 6965 6e74 2068 6973  ns, gradient his
-00001ec0: 746f 6772 616d 7320 616e 6420 7379 7374  tograms and syst
-00001ed0: 656d 206d 6574 7269 6373 2e20 546f 2072  em metrics. To r
-00001ee0: 756e 2077 616e 6462 3a0d 0a0d 0a60 6060  un wandb:....```
-00001ef0: 6261 7368 0d0a 7079 7468 6f6e 206d 6169  bash..python mai
-00001f00: 6e2e 7079 202d 2d66 756e 6374 696f 6e20  n.py --function 
-00001f10: 7475 6e65 202d 2d63 6f6e 6669 675f 6669  tune --config_fi
-00001f20: 6c65 2075 7365 725f 636f 6e66 6967 2f63  le user_config/c
-00001f30: 6f6e 6669 6775 7261 7469 6f6e 2e79 6d6c  onfiguration.yml
-00001f40: 202d 2d70 6172 616d 5f66 696c 6520 7573   --param_file us
-00001f50: 6572 5f63 6f6e 6669 672f 6576 616c 5f68  er_config/eval_h
-00001f60: 7970 6572 7061 7261 6d73 2e79 6d6c 202d  yperparams.yml -
-00001f70: 2d64 6174 615f 6669 6c65 206f 7574 7075  -data_file outpu
-00001f80: 745f 6373 7620 2d2d 696d 6167 655f 6669  t_csv --image_fi
-00001f90: 6c65 206f 7574 7075 745f 706c 6f74 7320  le output_plots 
-00001fa0: 2d2d 706c 6f74 5f63 7572 7665 7320 5472  --plot_curves Tr
-00001fb0: 7565 202d 2d73 6176 655f 6669 6c65 2054  ue --save_file T
-00001fc0: 7275 6520 2d2d 7475 6e65 7220 7761 6e64  rue --tuner wand
-00001fd0: 6220 0d0a 6060 600d 0a0d 0a23 2323 2320  b ..```....#### 
-00001fe0: 2a2a 5261 7920 5475 6e69 6e67 2a2a 0d0a  **Ray Tuning**..
-00001ff0: 0d0a 416e 2069 6e64 7573 7472 7920 7374  ..An industry st
-00002000: 616e 6461 7264 2074 6f6f 6c20 666f 7220  andard tool for 
-00002010: 6469 7374 7269 6275 7465 6420 6879 7065  distributed hype
-00002020: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
-00002030: 6720 7768 6963 6820 696e 7465 6772 6174  g which integrat
-00002040: 6573 2077 6974 6820 5465 6e73 6f72 426f  es with TensorBo
-00002050: 6172 6420 616e 6420 6578 7465 6e73 6976  ard and extensiv
-00002060: 6520 616e 616c 7973 6973 206c 6962 7261  e analysis libra
-00002070: 7269 6573 2e20 4974 2061 6c73 6f20 616c  ries. It also al
-00002080: 6c6f 7773 2075 7365 7273 2074 6f20 6c65  lows users to le
-00002090: 7665 7261 6765 2063 7574 7469 6e67 2065  verage cutting e
-000020a0: 6467 6520 6f70 7469 6d69 7a61 7469 6f6e  dge optimization
-000020b0: 2061 6c67 6f72 6974 686d 7320 6174 2073   algorithms at s
-000020c0: 6361 6c65 2c20 696e 636c 7564 696e 6720  cale, including 
-000020d0: 4261 7965 7369 616e 204f 7074 696d 697a  Bayesian Optimiz
-000020e0: 6174 696f 6e2c 2050 6f70 756c 6174 696f  ation, Populatio
-000020f0: 6e20 4261 7365 6420 5472 6169 6e69 6e67  n Based Training
-00002100: 2061 6e64 2048 7970 6572 4261 6e64 2e20   and HyperBand. 
-00002110: 546f 2072 756e 2072 6179 2074 756e 696e  To run ray tunin
-00002120: 673a 0d0a 0d0a 6060 6062 6173 680d 0a70  g:....```bash..p
-00002130: 7974 686f 6e20 6d61 696e 2e70 7920 2d2d  ython main.py --
-00002140: 6675 6e63 7469 6f6e 2074 756e 6520 2d2d  function tune --
-00002150: 636f 6e66 6967 5f66 696c 6520 7573 6572  config_file user
-00002160: 5f63 6f6e 6669 672f 636f 6e66 6967 7572  _config/configur
-00002170: 6174 696f 6e2e 796d 6c20 2d2d 7061 7261  ation.yml --para
-00002180: 6d5f 6669 6c65 2075 7365 725f 636f 6e66  m_file user_conf
-00002190: 6967 2f65 7661 6c5f 6879 7065 7270 6172  ig/eval_hyperpar
-000021a0: 616d 732e 796d 6c20 2d2d 6461 7461 5f66  ams.yml --data_f
-000021b0: 696c 6520 6f75 7470 7574 5f63 7376 202d  ile output_csv -
-000021c0: 2d69 6d61 6765 5f66 696c 6520 6f75 7470  -image_file outp
-000021d0: 7574 5f70 6c6f 7473 202d 2d70 6c6f 745f  ut_plots --plot_
-000021e0: 6375 7276 6573 2054 7275 6520 2d2d 7361  curves True --sa
-000021f0: 7665 5f66 696c 6520 5472 7565 202d 2d74  ve_file True --t
-00002200: 756e 6572 2072 6179 5f74 756e 650d 0a60  uner ray_tune..`
-00002210: 6060 0d0a 0d0a 2323 2053 7465 7020 333a  ``....## Step 3:
-00002220: 2045 7870 6c6f 7265 2046 6561 7475 7265   Explore Feature
-00002230: 730d 0a0d 0a23 2323 2031 2e20 2a2a 4578  s....### 1. **Ex
-00002240: 706c 6f72 6520 4272 6561 6b64 6f77 6e20  plore Breakdown 
-00002250: 5363 656e 6172 696f 732a 2a0d 0a0d 0a54  Scenarios**....T
-00002260: 6869 7320 6665 6174 7572 6520 616c 6c6f  his feature allo
-00002270: 7773 2074 6865 2075 7365 7220 746f 2074  ws the user to t
-00002280: 7261 696e 2074 6865 2061 6765 6e74 2062  rain the agent b
-00002290: 6173 6564 206f 6e20 6375 7374 6f6d 6564  ased on customed
-000022a0: 2065 7870 6c6f 7261 7469 6f6e 2070 7265   exploration pre
-000022b0: 6665 7265 6e63 6573 2062 6574 7765 656e  ferences between
-000022c0: 206b 6579 2073 7461 7465 7320 616e 6420   key states and 
-000022d0: 7065 7269 7068 6572 616c 2073 7461 7465  peripheral state
-000022e0: 7320 7573 696e 6720 7765 6967 6874 2070  s using weight p
-000022f0: 6172 616d 6574 6572 2060 7731 5f6b 6579  arameter `w1_key
-00002300: 6020 616e 6420 6077 325f 7065 7269 7068  ` and `w2_periph
-00002310: 6572 616c 602e 2054 6865 2070 7572 706f  eral`. The purpo
-00002320: 7365 206f 6620 7468 6973 2066 6561 7475  se of this featu
-00002330: 7265 2069 7320 746f 2065 6e61 626c 6520  re is to enable 
-00002340: 7468 6520 6167 656e 7420 746f 206e 6f74  the agent to not
-00002350: 206f 6e6c 7920 6765 6e65 7261 7465 2068   only generate h
-00002360: 6967 6820 7265 7761 7264 7320 666f 7220  igh rewards for 
-00002370: 6b65 7920 7374 6174 6573 2062 7574 2061  key states but a
-00002380: 6c73 6f20 7669 7369 7420 616c 6c20 6272  lso visit all br
-00002390: 6561 646f 776e 2073 6365 6e61 7269 6f73  eadown scenarios
-000023a0: 2073 7566 6669 6369 656e 746c 7920 656e   sufficiently en
-000023b0: 6f75 6768 2e20 0d0a 0d0a 5365 7420 7570  ough. ....Set up
-000023c0: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-000023d0: 696e 2060 7573 6572 5f63 6f6e 6669 675c  in `user_config\
-000023e0: 6665 6174 7572 6573 5f70 6172 616d 735c  features_params\
-000023f0: 626c 6f61 636b 6167 655f 6578 706c 6f72  bloackage_explor
-00002400: 655f 7061 7261 6d73 2e79 6d6c 603a 0d0a  e_params.yml`:..
-00002410: 0d0a 2d20 6077 315f 6b65 7960 3a20 5765  ..- `w1_key`: We
-00002420: 6967 6874 2070 6172 616d 6574 6572 2074  ight parameter t
-00002430: 6f20 636f 6e74 726f 6c20 6661 766f 7220  o control favor 
-00002440: 6578 706c 6f72 696e 6720 6b65 7920 7374  exploring key st
-00002450: 6174 6573 2e0d 0a2d 2060 7732 5f70 6572  ates...- `w2_per
-00002460: 6970 6865 7261 6c60 3a20 5765 6967 6874  ipheral`: Weight
-00002470: 2070 6172 616d 6574 6572 2074 6f20 636f   parameter to co
-00002480: 6e74 726f 6c20 6661 766f 7220 6578 706c  ntrol favor expl
-00002490: 6f72 696e 6720 7065 7269 7068 6572 616c  oring peripheral
-000024a0: 2073 7461 7465 732e 0d0a 2d20 6072 6573   states...- `res
-000024b0: 6574 603a 2041 2062 6f6f 6c20 7661 6c75  et`: A bool valu
-000024c0: 6520 7468 6174 2063 6f6e 7472 6f6c 7320  e that controls 
-000024d0: 7768 6574 6865 7220 746f 2072 6573 6574  whether to reset
-000024e0: 2077 6569 6768 7420 7061 7261 6d65 7465   weight paramete
-000024f0: 7273 2064 7572 696e 6720 7472 6169 6e69  rs during traini
-00002500: 6e67 2e0d 0a2d 2060 7265 7365 745f 6672  ng...- `reset_fr
-00002510: 6571 7565 6e63 7960 3a20 4120 7661 6c75  equency`: A valu
-00002520: 6520 7468 6174 2064 6566 696e 6573 2074  e that defines t
-00002530: 6865 206e 756d 6265 7220 6f66 2065 7069  he number of epi
-00002540: 736f 6465 7320 6672 6571 7565 6e63 7920  sodes frequency 
-00002550: 746f 2072 6573 6574 2074 6865 2077 6569  to reset the wei
-00002560: 6768 7420 7061 7261 6d65 7465 7273 2e0d  ght parameters..
-00002570: 0a2d 2060 6e75 6d5f 6f75 7470 7574 603a  .- `num_output`:
-00002580: 2041 2076 616c 7565 2074 6861 7420 6465   A value that de
-00002590: 6669 6e65 7320 7468 6520 6e75 6d62 6572  fines the number
-000025a0: 206f 6620 746f 7020 616e 6420 6c65 6173   of top and leas
-000025b0: 7420 7265 7761 7264 2f76 6973 6974 7320  t reward/visits 
-000025c0: 7374 6174 6573 2074 6f20 706c 6f74 2069  states to plot i
-000025d0: 6e20 6120 6869 7374 6f67 7261 6d0d 0a2d  n a histogram..-
-000025e0: 2060 6f75 7470 7574 5f6a 736f 6e60 3a20   `output_json`: 
-000025f0: 4120 626f 6f6c 2076 616c 7565 2074 6861  A bool value tha
-00002600: 7420 6465 7465 726d 696e 6573 2077 6865  t determines whe
-00002610: 7468 6572 2074 6f20 6f75 7470 7574 2074  ther to output t
-00002620: 6865 206a 736f 6e20 6669 6c65 206f 6620  he json file of 
-00002630: 6b65 7920 7374 6174 6573 2061 6e64 2070  key states and p
-00002640: 6572 6970 6865 7261 6c20 7374 6174 6573  eripheral states
-00002650: 0d0a 2d20 606f 7574 7075 745f 6869 7374  ..- `output_hist
-00002660: 6f67 7261 6d60 3a20 4120 626f 6f6c 2076  ogram`: A bool v
-00002670: 616c 7565 2074 6861 7420 6465 7465 726d  alue that determ
-00002680: 696e 6573 2077 6865 7468 6572 2074 6f20  ines whether to 
-00002690: 6f75 7470 7574 2074 6865 2068 6973 746f  output the histo
-000026a0: 6772 616d 2074 6861 7420 7368 6f77 7320  gram that shows 
-000026b0: 7468 6520 7265 7761 7264 7320 616e 6420  the rewards and 
-000026c0: 7669 7369 7473 206f 6620 7468 6520 746f  visits of the to
-000026d0: 7020 616e 6420 6c65 6173 7420 7374 6174  p and least stat
-000026e0: 6573 2e0d 0a2d 2060 6f75 7470 7574 5f63  es...- `output_c
-000026f0: 6f76 6572 6167 655f 6d65 7472 6963 603a  overage_metric`:
-00002700: 2041 2062 6f6f 6c20 7661 6c75 6520 7468   A bool value th
-00002710: 6174 2064 6574 6572 6d69 6e65 7320 7768  at determines wh
-00002720: 6574 6865 7220 746f 206f 7574 7075 7420  ether to output 
-00002730: 7468 6520 6375 7272 656e 7420 636f 7665  the current cove
-00002740: 7261 6765 206d 6574 7269 632e 0d0a 0d0a  rage metric.....
-00002750: 546f 2072 756e 2074 6869 7320 6665 6174  To run this feat
-00002760: 7572 652c 206e 6176 6967 6174 6520 746f  ure, navigate to
-00002770: 2060 2f66 6f75 6e64 6174 696f 6e73 2f62   `/foundations/b
-00002780: 7265 616b 646f 776e 5f65 7870 6c6f 7261  reakdown_explora
-00002790: 7469 6f6e 6020 616e 6420 7275 6e3a 0d0a  tion` and run:..
-000027a0: 2020 2060 6060 6261 7368 0d0a 2020 2070     ```bash..   p
-000027b0: 7974 686f 6e20 6272 6561 6b64 6f77 6e5f  ython breakdown_
-000027c0: 6578 706c 6f72 6174 696f 6e2e 7079 0d0a  exploration.py..
-000027d0: 2020 2060 6060 0d0a 0d0a 2323 2320 322e     ```....### 2.
-000027e0: 202a 2a44 6563 6973 696f 6e20 4576 616c   **Decision Eval
-000027f0: 7561 7469 6f6e 2028 426c 6f63 6b61 6765  uation (Blockage
-00002800: 2044 656d 6f6e 7374 7261 7469 6f6e 7329   Demonstrations)
-00002810: 2a2a 0d0a 0d0a 5468 6973 2066 6561 7475  **....This featu
-00002820: 7265 2061 6c6c 6f77 7320 7468 6520 7573  re allows the us
-00002830: 6572 2074 6f20 7465 7374 2061 2074 7261  er to test a tra
-00002840: 696e 6564 2061 6765 6e74 2773 2070 6572  ined agent's per
-00002850: 666f 726d 616e 6365 206f 6e20 6120 7369  formance on a si
-00002860: 6d75 6c61 7465 6420 7365 7276 6572 2062  mulated server b
-00002870: 6c6f 636b 6167 6520 7175 6575 6569 6e67  lockage queueing
-00002880: 2065 6e76 6972 6f6e 6d65 6e74 2062 7920   environment by 
-00002890: 7669 7375 616c 697a 696e 6720 7468 6520  visualizing the 
-000028a0: 6368 616e 6765 7320 696e 2074 7261 6e73  changes in trans
-000028b0: 6974 696f 6e20 7072 6f62 6162 696c 6974  ition probabilit
-000028c0: 6965 732e 2054 6865 2070 7572 706f 7365  ies. The purpose
-000028d0: 206f 6620 7468 6973 2066 6561 7475 7265   of this feature
-000028e0: 2069 7320 746f 2073 686f 7720 686f 7720   is to show how 
-000028f0: 6566 6665 6374 6963 6520 7468 6520 7472  effectice the tr
-00002900: 616e 6965 6420 6167 656e 7420 6973 2061  anied agent is a
-00002910: 6374 696e 6720 6f6e 2062 7265 616b 646f  cting on breakdo
-00002920: 776e 2063 6173 6573 2e20 0d0a 0d0a 2d20  wn cases. ....- 
-00002930: 606e 756d 5f73 696d 603a 2044 6566 696e  `num_sim`: Defin
-00002940: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-00002950: 206a 6f62 7320 746f 2073 696d 756c 6174   jobs to simulat
-00002960: 6520 666f 7220 6561 6368 2074 696d 6520  e for each time 
-00002970: 7374 6570 2064 7572 696e 6720 7472 6169  step during trai
-00002980: 6e69 6e67 2e0d 0a2d 2060 7469 6d65 5f73  ning...- `time_s
-00002990: 7465 7073 603a 2044 6566 696e 6573 2074  teps`: Defines t
-000029a0: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
-000029b0: 6520 7374 6570 7320 746f 2070 6572 666f  e steps to perfo
-000029c0: 726d 2066 6f72 2065 6163 6820 6570 6973  rm for each epis
-000029d0: 6f64 652e 0d0a 2d20 6071 7565 7565 5f69  ode...- `queue_i
-000029e0: 6e64 6578 603a 2044 6566 696e 6573 2074  ndex`: Defines t
-000029f0: 6865 2071 7565 7565 2069 6e64 6578 2074  he queue index t
-00002a00: 6861 7420 7265 636f 7264 2074 6865 206d  hat record the m
-00002a10: 6574 7269 6373 2066 6f72 2e0d 0a2d 2060  etrics for...- `
-00002a20: 6d65 7472 6963 603a 2044 6566 696e 6573  metric`: Defines
-00002a30: 2074 6865 206d 6574 7269 6320 746f 2062   the metric to b
-00002a40: 6520 7265 706f 7274 6564 2066 6f72 2074  e reported for t
-00002a50: 6865 2073 656c 6563 7465 6420 7175 6575  he selected queu
-00002a60: 652e 0d0a 0d0a 546f 2075 7365 2074 6869  e.....To use thi
-00002a70: 7320 6665 6174 7572 652c 206e 6176 6967  s feature, navig
-00002a80: 6174 6520 746f 2060 2f65 7661 6c75 6174  ate to `/evaluat
-00002a90: 696f 6e2f 6465 6369 7369 6f6e 5f65 7661  ion/decision_eva
-00002aa0: 6c75 6174 696f 6e60 2061 6e64 2072 756e  luation` and run
-00002ab0: 3a0d 0a20 2020 6060 6062 6173 680d 0a20  :..   ```bash.. 
-00002ac0: 2020 7079 7468 6f6e 2064 6563 6973 696f    python decisio
-00002ad0: 6e5f 6576 616c 7561 7469 6f6e 2e70 790d  n_evaluation.py.
-00002ae0: 0a20 2020 6060 600d 0a0d 0a23 2323 2033  .   ```....### 3
-00002af0: 2e20 2a2a 5374 6172 7475 7020 4265 6861  . **Startup Beha
-00002b00: 7669 6f72 2049 6465 6e74 6966 6963 6174  vior Identificat
-00002b10: 696f 6e2a 2a0d 0a0d 0a54 6869 7320 6665  ion**....This fe
-00002b20: 6174 7572 6520 616c 6c6f 7773 2074 6865  ature allows the
-00002b30: 2075 7365 7220 746f 2076 6973 7561 6c69   user to visuali
-00002b40: 7a65 2077 6865 6e20 7468 6520 6275 726e  ze when the burn
-00002b50: 2d69 6e20 7065 7269 6f64 7320 656e 6420  -in periods end 
-00002b60: 6f6e 2074 6865 206c 6561 726e 696e 6720  on the learning 
-00002b70: 6375 7276 652e 200d 0a0d 0a53 6574 2075  curve. ....Set u
-00002b80: 7020 7468 6520 7061 7261 6d65 7465 7273  p the parameters
-00002b90: 2069 6e20 7468 6520 7363 7269 7074 3a0d   in the script:.
-00002ba0: 0a0d 0a2d 2060 7769 6e64 6f77 5f73 697a  ...- `window_siz
-00002bb0: 6560 3a20 5370 6563 6966 6965 7320 7468  e`: Specifies th
-00002bc0: 6520 6e75 6d62 6572 206f 6620 6461 7461  e number of data
-00002bd0: 2070 6f69 6e74 7320 7573 6564 2074 6f20   points used to 
-00002be0: 636f 6d70 7574 6520 7468 6520 6d6f 7669  compute the movi
-00002bf0: 6e67 2061 7665 7261 6765 206f 6620 7468  ng average of th
-00002c00: 6520 7265 7761 7264 732e 0d0a 2d20 6074  e rewards...- `t
-00002c10: 6872 6573 686f 6c64 603a 2044 6566 696e  hreshold`: Defin
-00002c20: 6573 2074 6865 206d 6178 696d 756d 2061  es the maximum a
-00002c30: 6363 6570 7461 626c 6520 6162 736f 6c75  cceptable absolu
-00002c40: 7465 2076 616c 7565 206f 6620 7468 6520  te value of the 
-00002c50: 6465 7269 7661 7469 7665 206f 6620 7468  derivative of th
-00002c60: 6520 736d 6f6f 7468 6564 2072 6577 6172  e smoothed rewar
-00002c70: 6473 2062 656c 6f77 2077 6869 6368 2061  ds below which a
-00002c80: 2072 6577 6172 6420 6973 2063 6f6e 7369   reward is consi
-00002c90: 6465 7265 6420 7374 6162 6c65 2e20 0d0a  dered stable. ..
-00002ca0: 2d20 6063 6f6e 7365 6375 7469 7665 5f70  - `consecutive_p
-00002cb0: 6f69 6e74 7360 3a20 5468 6520 6e75 6d62  oints`: The numb
-00002cc0: 6572 206f 6620 636f 6e73 6563 7574 6976  er of consecutiv
-00002cd0: 6520 6461 7461 2070 6f69 6e74 7320 7468  e data points th
-00002ce0: 6174 206d 7573 7420 616c 6c20 6265 2062  at must all be b
-00002cf0: 656c 6f77 2074 6865 2074 6872 6573 686f  elow the thresho
-00002d00: 6c64 2066 6f72 2074 6865 2072 6577 6172  ld for the rewar
-00002d10: 6473 2074 6f20 6265 2063 6f6e 7369 6465  ds to be conside
-00002d20: 7265 6420 6173 2068 6176 696e 6720 7374  red as having st
-00002d30: 6162 696c 697a 6564 2e20 0d0a 2d20 6065  abilized. ..- `e
-00002d40: 7069 736f 6465 603a 2053 7065 6369 6679  pisode`: Specify
-00002d50: 2077 6869 6368 2065 7069 736f 6465 2773   which episode's
-00002d60: 2072 6577 6172 6473 2074 6f20 616e 616c   rewards to anal
-00002d70: 797a 6520 6672 6f6d 2061 2064 6174 6173  yze from a datas
-00002d80: 6574 2e0d 0a0d 0a54 6f20 7065 7266 6f72  et.....To perfor
-00002d90: 6d20 7468 6520 6665 6174 7572 652c 206e  m the feature, n
-00002da0: 6176 6967 6174 6520 746f 2060 2f65 7661  avigate to `/eva
-00002db0: 6c75 6174 696f 6e2f 7374 6172 7475 705f  luation/startup_
-00002dc0: 6576 616c 7561 7469 6f6e 6020 616e 6420  evaluation` and 
-00002dd0: 7275 6e3a 0d0a 2020 2060 6060 6261 7368  run:..   ```bash
-00002de0: 0d0a 2020 2070 7974 686f 6e20 7374 6172  ..   python star
-00002df0: 7475 705f 6576 616c 7561 7469 6f6e 2e70  tup_evaluation.p
-00002e00: 790d 0a20 2020 6060 600d 0a0d 0a23 2323  y..   ```....###
-00002e10: 2034 2e20 2a2a 436f 6e76 6572 6765 6e63   4. **Convergenc
-00002e20: 6520 4576 616c 7561 7469 6f6e 2a2a 200d  e Evaluation** .
-00002e30: 0a0d 0a54 6869 7320 6665 6174 7572 6520  ...This feature 
-00002e40: 616c 6c6f 7773 2074 6865 2075 7365 7220  allows the user 
-00002e50: 7472 6169 6e20 6d75 6c74 6970 6c65 2076  train multiple v
-00002e60: 6572 7369 6f6e 7320 6f66 2074 6865 2061  ersions of the a
-00002e70: 6765 6e74 2066 6f72 2064 6966 6665 7265  gent for differe
-00002e80: 6e74 206e 756d 6265 7273 206f 6620 7472  nt numbers of tr
-00002e90: 6169 6e69 6e67 2065 7069 736f 6465 7320  aining episodes 
-00002ea0: 616e 6420 7468 656e 2065 7661 6c75 6174  and then evaluat
-00002eb0: 6520 7468 6520 7065 7266 6f72 6d61 6e63  e the performanc
-00002ec0: 6520 6f66 2065 6163 6820 6167 656e 7420  e of each agent 
-00002ed0: 6f6e 2074 6865 2073 696d 756c 6174 696f  on the simulatio
-00002ee0: 6e20 656e 7669 726f 6e6d 656e 742e 0d0a  n environment...
-00002ef0: 0d0a 5365 7420 7570 2074 6865 2070 6172  ..Set up the par
-00002f00: 616d 6574 6572 7320 696e 2074 6865 2073  ameters in the s
-00002f10: 6372 6970 743a 0d0a 0d0a 2d20 606e 756d  cript:....- `num
-00002f20: 5f65 7069 736f 6465 735f 6c69 7374 603a  _episodes_list`:
-00002f30: 2041 206c 6973 7420 7468 6174 2063 6f6e   A list that con
-00002f40: 7461 696e 7320 6469 6666 6572 656e 7420  tains different 
-00002f50: 6e75 6d62 6572 7320 6f66 2065 7069 736f  numbers of episo
-00002f60: 6465 7320 746f 2074 7261 696e 2074 6865  des to train the
-00002f70: 2061 6765 6e74 732e 0d0a 2d20 6074 696d   agents...- `tim
-00002f80: 6573 7465 7073 603a 2041 2076 616c 7565  esteps`: A value
-00002f90: 2074 6861 7420 6465 6669 6e65 7320 7468   that defines th
-00002fa0: 6520 6e75 6d62 6572 206f 6620 7469 6d65  e number of time
-00002fb0: 7374 6570 7320 746f 2074 7261 696e 2074  steps to train t
-00002fc0: 6865 2061 6765 6e74 2064 7572 696e 6720  he agent during 
-00002fd0: 6561 6368 2065 7069 736f 6465 2e0d 0a0d  each episode....
-00002fe0: 0a54 6f20 7275 6e20 7468 6973 2066 6561  .To run this fea
-00002ff0: 7475 7265 2c20 6e61 7669 6761 7465 2074  ture, navigate t
-00003000: 6f20 602f 6576 616c 7561 7469 6f6e 2f63  o `/evaluation/c
-00003010: 6f6e 7665 7267 656e 6365 5f65 7661 6c75  onvergence_evalu
-00003020: 6174 696f 6e60 2061 6e64 2072 756e 3a0d  ation` and run:.
-00003030: 0a20 2020 6060 6062 6173 680d 0a20 2020  .   ```bash..   
-00003040: 7079 7468 6f6e 2063 6f6e 7665 7267 656e  python convergen
-00003050: 6365 5f65 7661 6c75 6174 696f 6e2e 7079  ce_evaluation.py
-00003060: 0d0a 2020 2060 6060 0d0a 0d0a 2323 2320  ..   ```....### 
-00003070: 352e 202a 2a52 6f62 7573 746e 6573 7320  5. **Robustness 
-00003080: 4576 616c 7561 7469 6f6e 2a2a 200d 0a0d  Evaluation** ...
-00003090: 0a54 6869 7320 6665 6174 7572 6520 616c  .This feature al
-000030a0: 6c6f 7773 2074 6865 2075 7365 7220 746f  lows the user to
-000030b0: 2074 7261 696e 206d 756c 7469 706c 6520   train multiple 
-000030c0: 6167 656e 7473 2c20 616e 616c 797a 6520  agents, analyze 
-000030d0: 7468 6569 7220 6265 6861 7669 6f72 2c20  their behavior, 
-000030e0: 616e 6420 6361 6c63 756c 6174 6520 7374  and calculate st
-000030f0: 6174 6973 7469 6361 6c20 6d65 7472 6963  atistical metric
-00003100: 7320 6261 7365 6420 6f6e 2074 6865 6972  s based on their
-00003110: 2070 6572 666f 726d 616e 6365 2e0d 0a0d   performance....
-00003120: 0a53 6574 2075 7020 7468 6520 7061 7261  .Set up the para
-00003130: 6d65 7465 7273 2069 6e20 7468 6520 7363  meters in the sc
-00003140: 7269 7074 3a0d 0a0d 0a2d 2060 636f 6e66  ript:....- `conf
-00003150: 6964 656e 6365 5f6c 6576 656c 603a 2054  idence_level`: T
-00003160: 6865 2073 7461 7469 7374 6963 616c 2063  he statistical c
-00003170: 6f6e 6669 6465 6e63 6520 6c65 7665 6c20  onfidence level 
-00003180: 666f 7220 6361 6c63 756c 6174 696f 6e73  for calculations
-00003190: 2e0d 0a2d 2060 6465 7369 7265 645f 6572  ...- `desired_er
-000031a0: 726f 7260 3a20 5468 6520 7461 7267 6574  ror`: The target
-000031b0: 2065 7272 6f72 206d 6172 6769 6e20 666f   error margin fo
-000031c0: 7220 6573 7469 6d61 7469 6e67 2073 7461  r estimating sta
-000031d0: 7469 7374 6963 616c 2072 6571 7569 7265  tistical require
-000031e0: 6d65 6e74 732e 0d0a 2d20 606e 756d 5f72  ments...- `num_r
-000031f0: 756e 7360 3a20 4e75 6d62 6572 206f 6620  uns`: Number of 
-00003200: 7469 6d65 7320 746f 2074 7261 696e 2061  times to train a
-00003210: 6765 6e74 732e 0d0a 2d20 6074 696d 655f  gents...- `time_
-00003220: 7374 6570 7360 3a20 4e75 6d62 6572 206f  steps`: Number o
-00003230: 6620 7469 6d65 2073 7465 7073 2065 6163  f time steps eac
-00003240: 6820 6167 656e 7420 7275 6e73 2069 6e20  h agent runs in 
-00003250: 7468 6520 7369 6d75 6c61 7469 6f6e 2065  the simulation e
-00003260: 6e76 6972 6f6e 6d65 6e74 2e0d 0a2d 2060  nvironment...- `
-00003270: 6e75 6d5f 7369 6d60 3a20 4e75 6d62 6572  num_sim`: Number
-00003280: 206f 6620 7369 6d75 6c61 7469 6f6e 7320   of simulations 
-00003290: 746f 2072 756e 2069 6e20 7468 6520 656e  to run in the en
-000032a0: 7669 726f 6e6d 656e 742e 0d0a 0d0a 546f  vironment.....To
-000032b0: 2072 756e 2074 6869 7320 6665 6174 7572   run this featur
-000032c0: 652c 206e 6176 6967 6174 6520 746f 2060  e, navigate to `
-000032d0: 2f65 7661 6c75 6174 696f 6e2f 726f 6275  /evaluation/robu
-000032e0: 7374 6e65 7373 5f65 7661 6c75 6174 696f  stness_evaluatio
-000032f0: 6e60 2061 6e64 2072 756e 3a0d 0a20 2020  n` and run:..   
-00003300: 6060 6062 6173 680d 0a20 2020 7079 7468  ```bash..   pyth
-00003310: 6f6e 2072 6f62 7573 746e 6573 735f 6576  on robustness_ev
-00003320: 616c 7561 7469 6f6e 2e70 790d 0a20 2020  aluation.py..   
-00003330: 6060 600d 0a0d 0a23 2323 2036 2e20 2a2a  ```....### 6. **
-00003340: 4e6f 6973 6520 4576 616c 7561 7469 6f6e  Noise Evaluation
-00003350: 2a2a 200d 0a0d 0a54 6869 7320 6665 6174  ** ....This feat
-00003360: 7572 6520 616c 6c6f 7773 2074 6865 2075  ure allows the u
-00003370: 7365 7220 746f 2065 7661 6c75 6174 6520  ser to evaluate 
-00003380: 7468 6520 6566 6665 6374 206f 6620 656e  the effect of en
-00003390: 7669 726f 6e6d 656e 7461 6c20 6e6f 6973  vironmental nois
-000033a0: 6520 6f6e 2074 6865 2070 6572 666f 726d  e on the perform
-000033b0: 616e 6365 206f 6620 7468 6520 6167 656e  ance of the agen
-000033c0: 742e 0d0a 0d0a 5365 7420 7570 2074 6865  t.....Set up the
-000033d0: 2070 6172 616d 6574 6572 7320 696e 2074   parameters in t
-000033e0: 6865 2073 6372 6970 743a 0d0a 0d0a 2d20  he script:....- 
-000033f0: 6066 7265 7175 656e 6379 2060 3a20 5468  `frequency `: Th
-00003400: 6520 6c69 6b65 6c69 686f 6f64 206f 7220  e likelihood or 
-00003410: 6672 6571 7565 6e63 7920 6174 2077 6869  frequency at whi
-00003420: 6368 206e 6f69 7365 2069 7320 696e 7472  ch noise is intr
-00003430: 6f64 7563 6564 2074 6f20 7468 6520 7379  oduced to the sy
-00003440: 7374 656d 2e20 4974 206d 7573 7420 6265  stem. It must be
-00003450: 2061 2076 616c 7565 2062 6574 7765 656e   a value between
-00003460: 2030 2061 6e64 2031 2e20 5468 6973 2070   0 and 1. This p
-00003470: 6172 616d 6574 6572 2064 6574 6572 6d69  arameter determi
-00003480: 6e65 7320 686f 7720 6f66 7465 6e2c 2070  nes how often, p
-00003490: 726f 706f 7274 696f 6e61 6c6c 792c 206e  roportionally, n
-000034a0: 6f69 7365 2077 696c 6c20 6265 2061 6464  oise will be add
-000034b0: 6564 2064 7572 696e 6720 7468 6520 7369  ed during the si
-000034c0: 6d75 6c61 7469 6f6e 2e20 0d0a 2d20 606d  mulation. ..- `m
-000034d0: 6561 6e60 3a20 5468 6520 6d65 616e 206f  ean`: The mean o
-000034e0: 6620 7468 6520 6e6f 726d 616c 2064 6973  f the normal dis
-000034f0: 7472 6962 7574 696f 6e20 6672 6f6d 2077  tribution from w
-00003500: 6869 6368 2074 6865 206e 6f69 7365 2076  hich the noise v
-00003510: 616c 7565 7320 6172 6520 7361 6d70 6c65  alues are sample
-00003520: 642e 2054 6869 7320 7265 7072 6573 656e  d. This represen
-00003530: 7473 2074 6865 2061 7665 7261 6765 2076  ts the average v
-00003540: 616c 7565 206f 6620 7468 6520 6e6f 6973  alue of the nois
-00003550: 6520 7468 6174 2077 696c 6c20 6265 2069  e that will be i
-00003560: 6e74 726f 6475 6365 642e 0d0a 2d20 6076  ntroduced...- `v
-00003570: 6172 6961 6e63 6560 3a20 5468 6520 7661  ariance`: The va
-00003580: 7269 616e 6365 206f 6620 7468 6520 6e6f  riance of the no
-00003590: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-000035a0: 6e20 6672 6f6d 2077 6869 6368 2074 6865  n from which the
-000035b0: 206e 6f69 7365 2076 616c 7565 7320 6172   noise values ar
-000035c0: 6520 7361 6d70 6c65 642e 2054 6869 7320  e sampled. This 
-000035d0: 7061 7261 6d65 7465 7220 696e 6469 6361  parameter indica
-000035e0: 7465 7320 7468 6520 7370 7265 6164 206f  tes the spread o
-000035f0: 7220 6469 7370 6572 7369 6f6e 206f 6620  r dispersion of 
-00003600: 7468 6520 6e6f 6973 6520 6172 6f75 6e64  the noise around
-00003610: 2074 6865 206d 6561 6e2e 0d0a 0d0a 546f   the mean.....To
-00003620: 2072 756e 2074 6865 2066 6561 7475 7265   run the feature
-00003630: 2c20 6e61 7669 6761 7465 2074 6f20 602f  , navigate to `/
-00003640: 6576 616c 7561 7469 6f6e 2f6e 6f69 7365  evaluation/noise
-00003650: 5f65 7661 6c75 6174 696f 6e60 2061 6e64  _evaluation` and
-00003660: 2072 756e 3a0d 0a20 2020 6060 6062 6173   run:..   ```bas
-00003670: 680d 0a20 2020 7079 7468 6f6e 206e 6f69  h..   python noi
-00003680: 7365 5f65 7661 6c75 6174 696f 6e2e 7079  se_evaluation.py
-00003690: 0d0a 2020 2060 6060 0d0a 0d0a 2323 2043  ..   ```....## C
-000036a0: 6f6e 7472 6962 7574 696f 6e0d 0a0d 0a43  ontribution....C
-000036b0: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
-000036c0: 2077 656c 636f 6d65 2e20 506c 6561 7365   welcome. Please
-000036d0: 2063 7265 6174 6520 6120 7075 6c6c 2072   create a pull r
-000036e0: 6571 7565 7374 206f 7220 6973 7375 6520  equest or issue 
-000036f0: 746f 2064 6973 6375 7373 2070 726f 706f  to discuss propo
-00003700: 7365 6420 6368 616e 6765 7320 6f72 2072  sed changes or r
-00003710: 6570 6f72 7420 6275 6773 2e0d 0a0d 0a23  eport bugs.....#
-00003720: 2320 4c69 6365 6e73 650d 0a0d 0a54 6869  # License....Thi
-00003730: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-00003740: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00003750: 4d49 5420 4c69 6365 6e73 6520 2d20 7365  MIT License - se
-00003760: 6520 7468 6520 4c49 4345 4e53 4520 6669  e the LICENSE fi
-00003770: 6c65 2066 6f72 2064 6574 6169 6c73 2e0d  le for details..
-00003780: 0a                                       .
+00000350: 2a2a 436f 6e76 6572 6765 6e63 6520 4576  **Convergence Ev
+00000360: 616c 7561 7469 6f6e 2a2a 3a20 4173 7365  aluation**: Asse
+00000370: 7373 6573 2074 6865 2073 7461 6269 6c69  sses the stabili
+00000380: 7479 2061 6e64 2072 656c 6961 6269 6c69  ty and reliabili
+00000390: 7479 206f 6620 7468 6520 6167 656e 7420  ty of the agent 
+000003a0: 6163 726f 7373 2064 6966 6665 7265 6e74  across different
+000003b0: 2074 7261 696e 696e 6720 7365 7475 7073   training setups
+000003c0: 0d0a 2020 2d20 2a2a 4e6f 6973 6520 4576  ..  - **Noise Ev
+000003d0: 616c 7561 7469 6f6e 2a2a 3a20 4576 616c  aluation**: Eval
+000003e0: 7561 7465 2074 6865 2065 6666 6563 7420  uate the effect 
+000003f0: 6f66 2065 6e76 6972 6f6e 6d65 6e74 616c  of environmental
+00000400: 206e 6f69 7365 206f 6e20 7468 6520 7065   noise on the pe
+00000410: 7266 6f72 6d61 6e63 6520 6f66 2074 6865  rformance of the
+00000420: 2061 6765 6e74 0d0a 2020 2d20 2a2a 5374   agent..  - **St
+00000430: 6172 7475 7020 4576 616c 7561 7469 6f6e  artup Evaluation
+00000440: 2a2a 3a20 4964 656e 7469 6669 6573 2074  **: Identifies t
+00000450: 6865 2062 7572 6e2d 696e 2070 6572 696f  he burn-in perio
+00000460: 6420 6f66 2074 6865 2061 6765 6e74 0d0a  d of the agent..
+00000470: 2020 2d20 2a2a 526f 6275 7374 6e65 7373    - **Robustness
+00000480: 2045 7661 6c75 6174 696f 6e2a 2a3a 2041   Evaluation**: A
+00000490: 7373 6573 7320 726f 6275 7374 6e65 7373  ssess robustness
+000004a0: 206f 6620 6465 6369 7369 6f6e 7320 6163   of decisions ac
+000004b0: 726f 7373 206d 756c 7469 706c 6520 7472  ross multiple tr
+000004c0: 6169 6e65 6420 6167 656e 7473 0d0a 0d0a  ained agents....
+000004d0: 2323 2050 7265 7265 7175 6973 6974 6573  ## Prerequisites
+000004e0: 0d0a 0d0a 4265 666f 7265 2072 756e 6e69  ....Before runni
+000004f0: 6e67 2074 6865 2073 696d 756c 6174 696f  ng the simulatio
+00000500: 6e73 2c20 656e 7375 7265 2079 6f75 2068  ns, ensure you h
+00000510: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
+00000520: 6720 696e 7374 616c 6c65 643a 0d0a 2d20  g installed:..- 
+00000530: 5079 7468 6f6e 203e 3d33 2e31 3020 3c33  Python >=3.10 <3
+00000540: 2e31 320d 0a2d 2074 6f72 6368 203d 2022  .12..- torch = "
+00000550: 322e 322e 3022 0d0a 2d20 6e75 6d70 7920  2.2.0"..- numpy 
+00000560: 3d20 2231 2e32 362e 3422 0d0a 2d20 7061  = "1.26.4"..- pa
+00000570: 6e64 6173 203d 2022 322e 322e 3022 0d0a  ndas = "2.2.0"..
+00000580: 2d20 7175 6575 6569 6e67 5f74 6f6f 6c20  - queueing_tool 
+00000590: 3d20 2231 2e32 2e35 220d 0a2d 206d 6174  = "1.2.5"..- mat
+000005a0: 706c 6f74 6c69 6220 3d20 2233 2e38 2e33  plotlib = "3.8.3
+000005b0: 220d 0a2d 2077 616e 6462 203d 2022 302e  "..- wandb = "0.
+000005c0: 3136 2e33 220d 0a2d 2050 7959 414d 4c20  16.3"..- PyYAML 
+000005d0: 3d20 2236 2e30 2e31 220d 0a2d 2072 6179  = "6.0.1"..- ray
+000005e0: 203d 207b 2076 6572 7369 6f6e 203d 2022   = { version = "
+000005f0: 322e 392e 3222 2c20 6578 7472 6173 203d  2.9.2", extras =
+00000600: 205b 2274 7261 696e 222c 2022 7475 6e65   ["train", "tune
+00000610: 225d 207d 0d0a 2d20 7471 646d 203d 2022  "] }..- tqdm = "
+00000620: 342e 3537 2e30 220d 0a2d 2073 6369 7079  4.57.0"..- scipy
+00000630: 203d 2022 312e 3132 2e30 220d 0a0d 0a23   = "1.12.0"....#
+00000640: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
+00000650: 0d0a 436c 6f6e 6520 7468 6520 7265 706f  ..Clone the repo
+00000660: 7369 746f 7279 2061 6e64 2069 6e73 7461  sitory and insta
+00000670: 6c6c 2074 6865 2072 6571 7569 7265 6420  ll the required 
+00000680: 6465 7065 6e64 656e 6369 6573 3a0d 0a0d  dependencies:...
+00000690: 0a60 6060 6261 7368 0d0a 6769 7420 636c  .```bash..git cl
+000006a0: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+000006b0: 7562 2e63 6f6d 2f61 6f2d 3432 302f 7369  ub.com/ao-420/si
+000006c0: 6d5f 726c 2e67 6974 0d0a 6364 2073 696d  m_rl.git..cd sim
+000006d0: 5f72 6c0d 0a70 6970 2069 6e73 7461 6c6c  _rl..pip install
+000006e0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
+000006f0: 2e74 7874 0d0a 6060 600d 0a0d 0a23 2320  .txt..```....## 
+00000700: 5374 6570 2031 3a20 436f 6e66 6967 7572  Step 1: Configur
+00000710: 6174 696f 6e0d 0a0d 0a23 2323 2045 6e76  ation....### Env
+00000720: 6972 6f6e 6d65 6e74 2053 6574 7570 0d0a  ironment Setup..
+00000730: 0d0a 2323 2323 202a 2a51 7565 7565 696e  ..#### **Queuein
+00000740: 6720 456e 7669 726f 6e6d 656e 7420 436f  g Environment Co
+00000750: 6e66 6967 7572 6174 696f 6e2a 2a0d 0a0d  nfiguration**...
+00000760: 0a54 6865 2073 696d 756c 6174 696f 6e20  .The simulation 
+00000770: 656e 7669 726f 6e6d 656e 7420 7265 7175  environment requ
+00000780: 6972 6573 2074 6865 2066 6f6c 6c6f 7769  ires the followi
+00000790: 6e67 2070 6172 616d 6574 6572 7320 746f  ng parameters to
+000007a0: 2062 6520 6465 6669 6e65 6420 696e 2074   be defined in t
+000007b0: 6865 2060 636f 6e66 6967 7572 6174 696f  he `configuratio
+000007c0: 6e2e 796d 6c60 2e0d 0a0d 0a2d 2060 6164  n.yml`.....- `ad
+000007d0: 6a61 6365 6e74 5f6c 6973 7460 3a20 4120  jacent_list`: A 
+000007e0: 6469 6374 696f 6e61 7279 2064 6566 696e  dictionary defin
+000007f0: 696e 6720 7468 6520 6164 6a61 6365 6e63  ing the adjacenc
+00000800: 7920 6c69 7374 2066 6f72 2074 6865 206e  y list for the n
+00000810: 6574 776f 726b 2074 6f70 6f6c 6f67 792e  etwork topology.
+00000820: 0d0a 2d20 606d 6975 5f64 6963 7460 3a20  ..- `miu_dict`: 
+00000830: 4120 6469 6374 696f 6e61 7279 206f 6620  A dictionary of 
+00000840: 7365 7276 6963 6520 7261 7465 7320 666f  service rates fo
+00000850: 7220 6561 6368 2073 6572 7669 6365 206e  r each service n
+00000860: 6f64 6520 696e 2074 6865 206e 6574 776f  ode in the netwo
+00000870: 726b 2e0d 0a2d 2060 7472 616e 7369 7469  rk...- `transiti
+00000880: 6f6e 5f70 726f 6261 5f61 6c6c 603a 2041  on_proba_all`: A
+00000890: 2064 6963 7469 6f6e 6172 7920 6465 6669   dictionary defi
+000008a0: 6e69 6e67 2074 6865 2074 7261 6e73 6974  ning the transit
+000008b0: 696f 6e20 7072 6f62 6162 696c 6974 6965  ion probabilitie
+000008c0: 7320 6265 7477 6565 6e20 6e6f 6465 732e  s between nodes.
+000008d0: 0d0a 2d20 6061 6374 6976 655f 6361 7060  ..- `active_cap`
+000008e0: 3a20 5468 6520 6163 7469 7665 2063 6170  : The active cap
+000008f0: 6163 6974 7920 6f66 2074 6865 206e 6f64  acity of the nod
+00000900: 6573 2066 726f 6d20 6f75 7473 6964 6520  es from outside 
+00000910: 7468 6520 6e65 7477 6f72 6b2e 0d0a 2d20  the network...- 
+00000920: 6064 6561 6374 6976 655f 7460 3a20 5468  `deactive_t`: Th
+00000930: 6520 6465 6163 7469 7661 7469 6f6e 2074  e deactivation t
+00000940: 6872 6573 686f 6c64 2066 6f72 2074 6865  hreshold for the
+00000950: 206e 6f64 6573 2066 726f 6d20 6f75 7473   nodes from outs
+00000960: 6964 6520 7468 6520 6e65 7477 6f72 6b2e  ide the network.
+00000970: 0d0a 2d20 6062 7566 6665 725f 7369 7a65  ..- `buffer_size
+00000980: 5f66 6f72 5f65 6163 685f 7175 6575 6560  _for_each_queue`
+00000990: 3a20 4120 6469 6374 696f 6e61 7279 2074  : A dictionary t
+000009a0: 6861 7420 6465 6669 6e65 7320 7468 6520  hat defines the 
+000009b0: 6275 6666 6572 2073 697a 6520 666f 7220  buffer size for 
+000009c0: 6561 6368 2071 7565 7565 2e0d 0a2d 2060  each queue...- `
+000009d0: 6172 7269 7661 6c5f 7261 7465 603a 2041  arrival_rate`: A
+000009e0: 206c 6973 7420 7468 6174 2064 6566 696e   list that defin
+000009f0: 6573 2074 6865 2061 7272 6976 616c 2072  es the arrival r
+00000a00: 6174 6573 2066 6f72 2061 6c6c 2070 6f73  ates for all pos
+00000a10: 7369 626c 6520 656e 7472 7920 6e6f 6465  sible entry node
+00000a20: 732e 0d0a 2d20 606d 6178 5f61 6765 6e74  s...- `max_agent
+00000a30: 7360 3a20 4120 7661 6c75 6520 7468 6174  s`: A value that
+00000a40: 2064 6566 696e 6573 2074 6865 206d 6178   defines the max
+00000a50: 696d 756d 206e 756d 6265 7220 6f66 2061  imum number of a
+00000a60: 6765 6e74 7320 6361 6e20 6265 2061 6363  gents can be acc
+00000a70: 7065 7465 6420 6672 6f6d 206f 7574 7369  peted from outsi
+00000a80: 6465 2074 6865 206e 6574 776f 726b 2066  de the network f
+00000a90: 6f72 2074 6865 2065 6e74 7279 206e 6f64  or the entry nod
+00000aa0: 6573 2e0d 0a2d 2060 7369 6d5f 6a6f 6273  es...- `sim_jobs
+00000ab0: 603a 2041 2076 616c 7565 2074 6861 7420  `: A value that 
+00000ac0: 6465 6669 6e65 7320 7468 6520 6e75 6d62  defines the numb
+00000ad0: 6572 206f 6620 6a6f 6273 2062 6569 6e67  er of jobs being
+00000ae0: 2073 696d 756c 6174 6564 2064 7572 696e   simulated durin
+00000af0: 6720 6576 6572 7920 7369 6d75 6c61 7469  g every simulati
+00000b00: 6f6e 2e0d 0a2d 2060 6d61 785f 6172 725f  on...- `max_arr_
+00000b10: 7261 7465 5f6c 6973 7460 3a20 4120 6c69  rate_list`: A li
+00000b20: 7374 2074 6861 7420 6465 6669 6e65 7320  st that defines 
+00000b30: 7468 6520 6d61 7869 6d75 6d20 6172 7269  the maximum arri
+00000b40: 7661 6c20 7261 7465 2066 6f72 2061 6c6c  val rate for all
+00000b50: 2065 6e74 7279 2071 7565 7565 732e 0d0a   entry queues...
+00000b60: 2d20 6065 6e74 7279 5f6e 6f64 6573 603a  - `entry_nodes`:
+00000b70: 2041 206c 6973 7420 7468 6174 2064 6566   A list that def
+00000b80: 696e 6573 2074 6865 2073 6f75 7263 6520  ines the source 
+00000b90: 616e 6420 7461 7267 6574 2076 6572 7469  and target verti
+00000ba0: 6365 7320 6f66 2065 6163 6820 656e 7472  ces of each entr
+00000bb0: 7920 6e6f 6465 2e0d 0a0d 0a20 2020 4578  y node.....   Ex
+00000bc0: 616d 706c 653a 0d0a 2020 2060 6060 7961  ample:..   ```ya
+00000bd0: 6d6c 0d0a 2020 206d 6975 5f6c 6973 743a  ml..   miu_list:
+00000be0: 2020 0d0a 2020 2031 3a20 302e 3235 300d    ..   1: 0.250.
+00000bf0: 0a20 2020 323a 2030 2e32 350d 0a20 2020  .   2: 0.25..   
+00000c00: 333a 2030 2e30 3135 3030 0d0a 2020 2034  3: 0.01500..   4
+00000c10: 3a20 3130 300d 0a20 2020 353a 2031 2e32  : 100..   5: 1.2
+00000c20: 300d 0a20 2020 363a 2030 2e30 3130 3030  0..   6: 0.01000
+00000c30: 0d0a 2020 2037 3a20 3130 0d0a 2020 2038  ..   7: 10..   8
+00000c40: 3a20 302e 3130 3030 0d0a 2020 2039 3a20  : 0.1000..   9: 
+00000c50: 302e 3530 300d 0a0d 0a20 2020 6164 6a61  0.500....   adja
+00000c60: 6365 6e74 5f6c 6973 743a 0d0a 2020 2030  cent_list:..   0
+00000c70: 3a20 5b31 5d0d 0a20 2020 313a 205b 322c  : [1]..   1: [2,
+00000c80: 2033 2c20 345d 0d0a 2020 2032 3a20 5b35   3, 4]..   2: [5
+00000c90: 5d0d 0a20 2020 333a 205b 362c 2037 5d0d  ]..   3: [6, 7].
+00000ca0: 0a20 2020 343a 205b 385d 0d0a 2020 2035  .   4: [8]..   5
+00000cb0: 3a20 5b39 5d0d 0a20 2020 363a 205b 395d  : [9]..   6: [9]
+00000cc0: 0d0a 2020 2037 3a20 5b39 5d0d 0a20 2020  ..   7: [9]..   
+00000cd0: 383a 205b 395d 0d0a 2020 2039 3a20 5b31  8: [9]..   9: [1
+00000ce0: 305d 0d0a 0d0a 2020 2062 7566 6665 725f  0]....   buffer_
+00000cf0: 7369 7a65 5f66 6f72 5f65 6163 685f 7175  size_for_each_qu
+00000d00: 6575 653a 200d 0a20 2020 303a 2035 3030  eue: ..   0: 500
+00000d10: 300d 0a20 2020 313a 2035 3030 300d 0a20  0..   1: 5000.. 
+00000d20: 2020 323a 2035 3030 300d 0a20 2020 333a    2: 5000..   3:
+00000d30: 2035 3030 300d 0a20 2020 343a 2035 3030   5000..   4: 500
+00000d40: 300d 0a20 2020 353a 2035 3030 300d 0a20  0..   5: 5000.. 
+00000d50: 2020 363a 2035 3030 300d 0a20 2020 373a    6: 5000..   7:
+00000d60: 2035 3030 300d 0a20 2020 383a 2035 3030   5000..   8: 500
+00000d70: 300d 0a20 2020 393a 2035 3030 300d 0a20  0..   9: 5000.. 
+00000d80: 2020 3130 3a20 3530 3030 0d0a 2020 2031    10: 5000..   1
+00000d90: 313a 2035 3030 300d 0a20 2020 3132 3a20  1: 5000..   12: 
+00000da0: 3530 3030 0d0a 0d0a 2020 2074 7261 6e73  5000....   trans
+00000db0: 6974 696f 6e5f 7072 6f62 615f 616c 6c3a  ition_proba_all:
+00000dc0: 0d0a 2020 2030 3a20 7b31 3a20 317d 0d0a  ..   0: {1: 1}..
+00000dd0: 2020 2031 3a20 7b32 3a20 302e 3333 2c20     1: {2: 0.33, 
+00000de0: 333a 2030 2e33 332c 2034 3a20 302e 3334  3: 0.33, 4: 0.34
+00000df0: 7d0d 0a20 2020 323a 207b 353a 2031 7d0d  }..   2: {5: 1}.
+00000e00: 0a20 2020 333a 207b 363a 2030 2e35 2c20  .   3: {6: 0.5, 
+00000e10: 373a 2030 2e35 7d0d 0a20 2020 343a 207b  7: 0.5}..   4: {
+00000e20: 383a 2031 7d0d 0a20 2020 353a 207b 393a  8: 1}..   5: {9:
+00000e30: 2031 7d0d 0a20 2020 363a 207b 393a 2031   1}..   6: {9: 1
+00000e40: 7d0d 0a20 2020 373a 207b 393a 2031 7d0d  }..   7: {9: 1}.
+00000e50: 0a20 2020 383a 207b 393a 2031 7d0d 0a20  .   8: {9: 1}.. 
+00000e60: 2020 393a 207b 3130 3a20 317d 0d0a 2020    9: {10: 1}..  
+00000e70: 200d 0a20 2020 6163 7469 7665 5f63 6170   ..   active_cap
+00000e80: 3a20 350d 0a0d 0a20 2020 6465 6163 7469  : 5....   deacti
+00000e90: 7665 5f74 3a20 302e 3132 0d0a 0d0a 2020  ve_t: 0.12....  
+00000ea0: 2061 7272 6976 616c 5f72 6174 653a 205b   arrival_rate: [
+00000eb0: 302e 335d 0d0a 0d0a 2020 206d 6178 5f61  0.3]....   max_a
+00000ec0: 6765 6e74 733a 2069 6e66 0d0a 0d0a 2020  gents: inf....  
+00000ed0: 2073 696d 5f6a 6f62 733a 2031 3030 0d0a   sim_jobs: 100..
+00000ee0: 0d0a 2020 206d 6178 5f61 7272 5f72 6174  ..   max_arr_rat
+00000ef0: 655f 6c69 7374 3a20 5b30 2e33 5d0d 0a0d  e_list: [0.3]...
+00000f00: 0a20 2020 656e 7472 795f 6e6f 6465 733a  .   entry_nodes:
+00000f10: 0d0a 2020 202d 205b 302c 2031 5d20 0d0a  ..   - [0, 1] ..
+00000f20: 2020 2060 6060 0d0a 0d0a 2323 2323 202a     ```....#### *
+00000f30: 2a52 4c20 456e 7669 726f 6e6d 656e 7420  *RL Environment 
+00000f40: 5061 7261 6d65 7465 7273 2a2a 0d0a 0d0a  Parameters**....
+00000f50: 5365 7420 7570 2074 6865 2052 4c20 656e  Set up the RL en
+00000f60: 7669 726f 6e6d 656e 7420 7061 7261 6d65  vironment parame
+00000f70: 7465 7273 2069 6e20 6065 7661 6c5f 6879  ters in `eval_hy
+00000f80: 7065 7270 6172 616d 732e 796d 6c60 3a0d  perparams.yml`:.
+00000f90: 0a0d 0a2d 2060 6e75 6d5f 6570 6973 6f64  ...- `num_episod
+00000fa0: 6573 603a 2054 6865 206e 756d 6265 7220  es`: The number 
+00000fb0: 6f66 2065 7069 736f 6465 7320 746f 2072  of episodes to r
+00000fc0: 756e 2074 6865 2073 696d 756c 6174 696f  un the simulatio
+00000fd0: 6e2e 0d0a 2d20 606e 756d 5f65 706f 6368  n...- `num_epoch
+00000fe0: 7360 3a20 5468 6520 6e75 6d62 6572 206f  s`: The number o
+00000ff0: 6620 6570 6f63 6873 2066 6f72 2074 7261  f epochs for tra
+00001000: 696e 696e 672e 0d0a 2d20 6074 696d 655f  ining...- `time_
+00001010: 7374 6570 7360 3a20 5468 6520 6e75 6d62  steps`: The numb
+00001020: 6572 206f 6620 7469 6d65 2073 7465 7073  er of time steps
+00001030: 2069 6e20 6561 6368 2065 7069 736f 6465   in each episode
+00001040: 2e0d 0a2d 2060 6261 7463 685f 7369 7a65  ...- `batch_size
+00001050: 603a 2053 697a 6520 6f66 2074 6865 2062  `: Size of the b
+00001060: 6174 6368 2075 7365 6420 696e 2074 7261  atch used in tra
+00001070: 696e 696e 672e 2028 4465 6661 756c 7420  ining. (Default 
+00001080: 6973 2065 7175 616c 2074 6f20 7469 6d65  is equal to time
+00001090: 5f73 7465 7073 290d 0a2d 2060 6e75 6d5f  _steps)..- `num_
+000010a0: 7369 6d60 3a20 5468 6520 6e75 6d62 6572  sim`: The number
+000010b0: 206f 6620 7369 6d75 6c61 7469 6f6e 7320   of simulations 
+000010c0: 746f 2072 756e 2064 7572 696e 6720 7472  to run during tr
+000010d0: 6169 6e69 6e67 2e0d 0a2d 2060 7461 7560  aining...- `tau`
+000010e0: 3a20 436f 6566 6669 6369 656e 7420 666f  : Coefficient fo
+000010f0: 7220 736f 6674 2075 7064 6174 6520 6f66  r soft update of
+00001100: 2074 6865 2074 6172 6765 7420 7061 7261   the target para
+00001110: 6d65 7465 7273 2e0d 0a2d 2060 6163 746f  meters...- `acto
+00001120: 725f 6c72 603a 204c 6561 726e 696e 6720  r_lr`: Learning 
+00001130: 7261 7465 2066 6f72 2074 6865 2041 6374  rate for the Act
+00001140: 6f72 206e 6574 776f 726b 206f 7074 696d  or network optim
+00001150: 697a 6572 2e0d 0a2d 2060 6372 6974 6963  izer...- `critic
+00001160: 5f6c 7260 3a20 4c65 6172 6e69 6e67 2072  _lr`: Learning r
+00001170: 6174 6520 666f 7220 7468 6520 4372 6974  ate for the Crit
+00001180: 6963 204e 6574 776f 726b 206f 7074 696d  ic Network optim
+00001190: 697a 6572 2e0d 0a2d 2060 6469 7363 6f75  izer...- `discou
+000011a0: 6e74 603a 2044 6973 636f 756e 7420 6661  nt`: Discount fa
+000011b0: 6374 6f72 2066 6f72 2066 7574 7572 6520  ctor for future 
+000011c0: 7265 7761 7264 732e 0d0a 2d20 6070 6c61  rewards...- `pla
+000011d0: 6e6e 696e 675f 7374 6570 7360 3a20 5468  nning_steps`: Th
+000011e0: 6520 6e75 6d62 6572 206f 6620 7374 6570  e number of step
+000011f0: 7320 6475 7269 6e67 2070 6c61 6e6e 696e  s during plannin
+00001200: 672e 0d0a 2d20 6070 6c61 6e6e 696e 675f  g...- `planning_
+00001210: 7374 6460 3a20 5374 616e 6461 7264 2064  std`: Standard d
+00001220: 6576 6961 7469 6f6e 206f 6620 7468 6520  eviation of the 
+00001230: 6e6f 726d 616c 2064 6973 7475 7262 616e  normal disturban
+00001240: 6365 2064 7572 696e 6720 706c 616e 6e69  ce during planni
+00001250: 6e67 2e0d 0a2d 2060 6163 746f 725f 6e65  ng...- `actor_ne
+00001260: 7477 6f72 6b60 3a20 4e65 7477 6f72 6b20  twork`: Network 
+00001270: 6172 6368 6974 6563 7475 7265 2066 6f72  architecture for
+00001280: 2061 6374 6f72 206e 6574 776f 726b 2e0d   actor network..
+00001290: 0a2d 2060 6372 6974 6963 5f6e 6574 776f  .- `critic_netwo
+000012a0: 726b 603a 204e 6574 776f 726b 2061 7263  rk`: Network arc
+000012b0: 6869 7465 6374 7572 6520 666f 7220 6372  hitecture for cr
+000012c0: 6974 6963 206e 6574 776f 726b 2e0d 0a2d  itic network...-
+000012d0: 2060 7265 7761 7264 5f6d 6f64 656c 603a   `reward_model`:
+000012e0: 204e 6574 776f 726b 2061 7263 6869 7465   Network archite
+000012f0: 6374 7572 6520 666f 7220 7265 7761 7264  cture for reward
+00001300: 206d 6f64 656c 2075 7364 2069 6e20 706c   model usd in pl
+00001310: 616e 6e69 6e67 2e0d 0a60 2060 6e65 7874  anning...` `next
+00001320: 5f73 7461 7465 5f6d 6f64 656c 603a 204e  _state_model`: N
+00001330: 6574 776f 726b 2061 7263 6869 7465 6374  etwork architect
+00001340: 7572 6520 666f 7220 6e65 7874 2073 7461  ure for next sta
+00001350: 7465 206d 6f64 656c 2075 7365 6420 696e  te model used in
+00001360: 2070 6c61 6e6e 696e 672e 200d 0a0d 0a20   planning. .... 
+00001370: 2020 4578 616d 706c 653a 0d0a 2020 2060    Example:..   `
+00001380: 6060 7961 6d6c 0d0a 2020 206e 756d 5f65  ``yaml..   num_e
+00001390: 7069 736f 6465 733a 2035 0d0a 0d0a 2020  pisodes: 5....  
+000013a0: 2074 6872 6573 686f 6c64 3a20 3130 0d0a   threshold: 10..
+000013b0: 0d0a 2020 206e 756d 5f65 706f 6368 733a  ..   num_epochs:
+000013c0: 2031 3030 0d0a 0d0a 2020 2074 696d 655f   100....   time_
+000013d0: 7374 6570 733a 2033 300d 0a0d 0a20 2020  steps: 30....   
+000013e0: 6261 7463 685f 7369 7a65 3a20 3330 0d0a  batch_size: 30..
+000013f0: 2020 200d 0a20 2020 7461 7267 6574 5f75     ..   target_u
+00001400: 7064 6174 655f 6672 6571 7565 6e63 793a  pdate_frequency:
+00001410: 2031 3030 0d0a 2020 200d 0a20 2020 6275   100..   ..   bu
+00001420: 6666 6572 5f73 697a 653a 2031 3030 3030  ffer_size: 10000
+00001430: 0d0a 2020 200d 0a20 2020 6e75 6d5f 7369  ..   ..   num_si
+00001440: 6d3a 2031 300d 0a20 2020 0d0a 2020 2074  m: 10..   ..   t
+00001450: 6175 3a20 302e 350d 0a0d 0a20 2020 6e75  au: 0.5....   nu
+00001460: 6d5f 7472 6169 6e5f 4143 3a20 3130 0d0a  m_train_AC: 10..
+00001470: 2020 200d 0a20 2020 6372 6974 6963 5f6c     ..   critic_l
+00001480: 723a 2030 2e30 310d 0a0d 0a20 2020 6163  r: 0.01....   ac
+00001490: 746f 725f 6c72 3a20 302e 3030 3031 0d0a  tor_lr: 0.0001..
+000014a0: 2020 200d 0a20 2020 6469 7363 6f75 6e74     ..   discount
+000014b0: 3a20 302e 380d 0a20 2020 0d0a 2020 2070  : 0.8..   ..   p
+000014c0: 6c61 6e6e 696e 675f 7374 6570 733a 2031  lanning_steps: 1
+000014d0: 300d 0a20 2020 0d0a 2020 2070 6c61 6e6e  0..   ..   plann
+000014e0: 696e 675f 7374 643a 2030 2e31 0d0a 0d0a  ing_std: 0.1....
+000014f0: 2020 2061 6374 6f72 5f6e 6574 776f 726b     actor_network
+00001500: 3a0d 0a20 2020 2d20 3634 0d0a 2020 202d  :..   - 64..   -
+00001510: 2036 340d 0a20 2020 2d20 3634 0d0a 0d0a   64..   - 64....
+00001520: 2020 2063 7269 7469 633a 0d0a 2020 202d     critic:..   -
+00001530: 2036 340d 0a20 2020 2d20 3634 0d0a 2020   64..   - 64..  
+00001540: 202d 2036 340d 0a0d 0a20 2020 7265 7761   - 64....   rewa
+00001550: 7264 5f6d 6f64 656c 3a0d 0a20 2020 2d20  rd_model:..   - 
+00001560: 3332 0d0a 2020 202d 2036 340d 0a20 2020  32..   - 64..   
+00001570: 2d20 3634 0d0a 2020 202d 2033 320d 0a0d  - 64..   - 32...
+00001580: 0a20 2020 6e65 7874 5f73 7461 7465 5f6d  .   next_state_m
+00001590: 6f64 656c 3a0d 0a20 2020 2d20 3332 0d0a  odel:..   - 32..
+000015a0: 2020 202d 2036 340d 0a20 2020 2d20 3634     - 64..   - 64
+000015b0: 0d0a 2020 202d 2033 320d 0a20 2020 6060  ..   - 32..   ``
+000015c0: 600d 0a0d 0a23 2323 2320 2a2a 5475 6e69  `....#### **Tuni
+000015d0: 6e67 2043 6f6e 6669 6775 7261 7469 6f6e  ng Configuration
+000015e0: 2a2a 0d0a 5365 7420 7570 2074 6865 2068  **..Set up the h
+000015f0: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
+00001600: 6e69 6e67 2072 616e 6765 7320 696e 2060  ning ranges in `
+00001610: 7475 6e69 6e67 5f70 6172 616d 732e 796d  tuning_params.ym
+00001620: 6c60 3a0d 0a0d 0a2d 2060 6c72 5f6d 696e  l`:....- `lr_min
+00001630: 2f6d 6178 603a 204d 696e 2061 6e64 206d  /max`: Min and m
+00001640: 6178 2072 616e 6765 7320 6f66 2074 6865  ax ranges of the
+00001650: 206c 6561 726e 696e 6720 7261 7465 2062   learning rate b
+00001660: 6569 6e67 2074 756e 6564 2e0d 0a2d 2060  eing tuned...- `
+00001670: 6570 6f63 6873 5f6c 6973 7460 3a20 4120  epochs_list`: A 
+00001680: 6c69 7374 2074 6861 7420 6465 6669 6e65  list that define
+00001690: 7320 7468 6520 7261 6e67 6520 6f66 2070  s the range of p
+000016a0: 6f73 7369 626c 6520 6570 6f63 6873 2074  ossible epochs t
+000016b0: 6f20 7472 6169 6e20 7265 7761 7264 206d  o train reward m
+000016c0: 6f64 656c 2061 6e64 206e 6578 7420 7374  odel and next st
+000016d0: 6174 6520 6d6f 6465 6c2e 0d0a 2d20 6062  ate model...- `b
+000016e0: 6174 6368 5f73 697a 6560 3a20 4120 6c69  atch_size`: A li
+000016f0: 7374 2074 6861 7420 6465 6669 6e65 7320  st that defines 
+00001700: 7468 6520 7261 6e67 6520 6f66 2062 6174  the range of bat
+00001710: 6368 2073 697a 6573 2074 6f20 7361 6d70  ch sizes to samp
+00001720: 6c65 2066 726f 6d20 7468 6520 7265 706c  le from the repl
+00001730: 6179 2062 7566 6665 722e 0d0a 2d20 6074  ay buffer...- `t
+00001740: 6175 5f6d 696e 2f6d 6178 603a 204d 696e  au_min/max`: Min
+00001750: 2061 6e64 206d 6178 2072 616e 6765 7320   and max ranges 
+00001760: 6f66 2074 6865 2073 6f66 7420 7570 6461  of the soft upda
+00001770: 7465 2070 6172 616d 6574 6572 732e 0d0a  te parameters...
+00001780: 2d20 6064 6973 636f 756e 7420 6d69 6e2f  - `discount min/
+00001790: 6d61 7860 3a20 4d69 6e20 616e 6420 6d61  max`: Min and ma
+000017a0: 7820 7261 6e67 6573 206f 6620 7468 6520  x ranges of the 
+000017b0: 6469 7363 6f75 6e74 2066 6163 746f 7220  discount factor 
+000017c0: 666f 7220 6675 7475 7265 2072 6577 6172  for future rewar
+000017d0: 6473 2e0d 0a2d 2060 6570 7369 6c6f 6e5f  ds...- `epsilon_
+000017e0: 6d69 6e2f 6d61 7860 3a20 4d69 6e20 616e  min/max`: Min an
+000017f0: 6420 6d61 7820 7261 6e67 6573 206f 6620  d max ranges of 
+00001800: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
+00001810: 6961 7469 6f6e 206f 6620 6e6f 726d 616c  iation of normal
+00001820: 2064 6973 7475 7262 616e 6365 7320 6475   disturbances du
+00001830: 7269 6e67 2070 6c61 6e6e 696e 672e 0d0a  ring planning...
+00001840: 2d20 6070 6c61 6e6e 696e 675f 7374 6570  - `planning_step
+00001850: 7360 3a20 4120 6c69 7374 2074 6861 7420  s`: A list that 
+00001860: 6465 6669 6e65 7320 706f 7373 6962 6c65  defines possible
+00001870: 2073 7465 7073 2066 6f72 2070 6c61 6e6e   steps for plann
+00001880: 696e 672e 0d0a 2d20 6077 312f 7732 603a  ing...- `w1/w2`:
+00001890: 2057 6569 6768 7420 7061 7261 6d65 7465   Weight paramete
+000018a0: 7273 2074 6861 7420 696e 666c 7565 6e63  rs that influenc
+000018b0: 6520 7468 6520 6578 706c 6f72 6174 696f  e the exploratio
+000018c0: 6e20 6265 7477 6565 6e20 6b65 7920 616e  n between key an
+000018d0: 6420 7065 7269 7068 6572 616c 2073 7461  d peripheral sta
+000018e0: 7465 732e 0d0a 2d20 606e 756d 5f65 7069  tes...- `num_epi
+000018f0: 736f 6465 7360 3a20 4120 6c69 7374 2074  sodes`: A list t
+00001900: 6861 7420 6465 6669 6e65 7320 7468 6520  hat defines the 
+00001910: 706f 7373 6962 6c65 206e 756d 6265 7273  possible numbers
+00001920: 206f 6620 6570 6973 6f64 6573 2074 6f20   of episodes to 
+00001930: 7472 6169 6e20 7468 6520 6167 656e 7473  train the agents
+00001940: 2e0d 0a2d 2060 7469 6d65 5f73 7465 7073  ...- `time_steps
+00001950: 603a 2041 206c 6973 7420 7468 6174 2064  `: A list that d
+00001960: 6566 696e 6573 2074 6865 2070 6f73 7369  efines the possi
+00001970: 626c 6520 6e75 6d62 6572 206f 6620 7469  ble number of ti
+00001980: 6d65 2073 7465 7073 2064 7572 696e 6720  me steps during 
+00001990: 6561 6368 2065 7069 736f 6465 0d0a 0d0a  each episode....
+000019a0: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
+000019b0: 6060 6079 616d 6c0d 0a20 2020 6c65 6172  ```yaml..   lear
+000019c0: 6e69 6e67 5f72 6174 655f 6d61 783a 2030  ning_rate_max: 0
+000019d0: 2e31 0d0a 2020 206c 6561 726e 696e 675f  .1..   learning_
+000019e0: 7261 7465 5f6d 696e 3a20 302e 3030 310d  rate_min: 0.001.
+000019f0: 0a0d 0a20 2020 6570 6f63 6873 5f6c 6973  ...   epochs_lis
+00001a00: 743a 0d0a 2020 202d 2031 300d 0a20 2020  t:..   - 10..   
+00001a10: 2d20 3130 0d0a 2020 202d 2031 300d 0a0d  - 10..   - 10...
+00001a20: 0a20 2020 6261 7463 685f 7369 7a65 3a0d  .   batch_size:.
+00001a30: 0a20 2020 2d20 3136 0d0a 2020 202d 2033  .   - 16..   - 3
+00001a40: 320d 0a20 2020 2d20 3634 0d0a 0d0a 2020  2..   - 64....  
+00001a50: 2074 6175 5f6d 696e 3a20 302e 3030 3035   tau_min: 0.0005
+00001a60: 0d0a 2020 2074 6175 5f6d 6178 3a20 302e  ..   tau_max: 0.
+00001a70: 3030 320d 0a0d 0a20 2020 6469 7363 6f75  002....   discou
+00001a80: 6e74 5f6d 696e 3a20 302e 310d 0a20 2020  nt_min: 0.1..   
+00001a90: 6469 7363 6f75 6e74 5f6d 6178 3a20 302e  discount_max: 0.
+00001aa0: 330d 0a0d 0a20 2020 6570 7369 6c6f 6e5f  3....   epsilon_
+00001ab0: 6d69 6e3a 2030 2e31 0d0a 2020 2065 7073  min: 0.1..   eps
+00001ac0: 696c 6f6e 5f6d 6178 3a20 302e 330d 0a0d  ilon_max: 0.3...
+00001ad0: 0a20 2020 706c 616e 6e69 6e67 5f73 7465  .   planning_ste
+00001ae0: 7073 3a20 0d0a 2020 202d 2031 300d 0a0d  ps: ..   - 10...
+00001af0: 0a20 2020 6e75 6d5f 7361 6d70 6c65 3a20  .   num_sample: 
+00001b00: 0d0a 2020 202d 2035 300d 0a0d 0a20 2020  ..   - 50....   
+00001b10: 7731 3a20 0d0a 2020 202d 2030 2e35 0d0a  w1: ..   - 0.5..
+00001b20: 0d0a 2020 2077 323a 200d 0a20 2020 2d20  ..   w2: ..   - 
+00001b30: 302e 350d 0a0d 0a20 2020 6e75 6d5f 6570  0.5....   num_ep
+00001b40: 6973 6f64 6573 3a20 0d0a 2020 202d 2035  isodes: ..   - 5
+00001b50: 0d0a 0d0a 2020 2074 696d 655f 7374 6570  ....   time_step
+00001b60: 733a 200d 0a20 2020 2d20 3130 0d0a 2020  s: ..   - 10..  
+00001b70: 200d 0a20 2020 6e75 6d5f 7472 6169 6e5f   ..   num_train_
+00001b80: 4143 3a20 0d0a 2020 202d 2031 300d 0a0d  AC: ..   - 10...
+00001b90: 0a20 2020 6060 600d 0a0d 0a23 2320 5374  .   ```....## St
+00001ba0: 6570 2032 3a20 5275 6e6e 696e 6720 5369  ep 2: Running Si
+00001bb0: 6d75 6c61 7469 6f6e 730d 0a0d 0a23 2323  mulations....###
+00001bc0: 2054 7261 696e 696e 6720 4167 656e 740d   Training Agent.
+00001bd0: 0a54 6869 7320 636f 6d6d 616e 6420 7374  .This command st
+00001be0: 6172 7473 2074 7261 696e 696e 6720 7468  arts training th
+00001bf0: 6520 6167 656e 7420 7769 7468 696e 2074  e agent within t
+00001c00: 6865 2073 696d 756c 6174 6564 2071 7565  he simulated que
+00001c10: 7565 696e 6720 656e 7669 726f 6e6d 656e  ueing environmen
+00001c20: 742e 2052 6573 756c 7473 2061 7265 2073  t. Results are s
+00001c30: 6176 6564 2069 6e20 602f 666f 756e 6461  aved in `/founda
+00001c40: 7469 6f6e 732f 6f75 7470 7574 5f63 7376  tions/output_csv
+00001c50: 6020 616e 6420 602f 666f 756e 6461 7469  ` and `/foundati
+00001c60: 6f6e 732f 6f75 7470 7574 5f70 6c6f 7473  ons/output_plots
+00001c70: 602e 0d0a 0d0a 6060 6062 6173 680d 0a70  `.....```bash..p
+00001c80: 7974 686f 6e20 6d61 696e 2e70 7920 2d2d  ython main.py --
+00001c90: 6675 6e63 7469 6f6e 2074 7261 696e 202d  function train -
+00001ca0: 2d63 6f6e 6669 675f 6669 6c65 2075 7365  -config_file use
+00001cb0: 725f 636f 6e66 6967 2f63 6f6e 6669 6775  r_config/configu
+00001cc0: 7261 7469 6f6e 2e79 6d6c 202d 2d70 6172  ration.yml --par
+00001cd0: 616d 5f66 696c 6520 7573 6572 5f63 6f6e  am_file user_con
+00001ce0: 6669 672f 6576 616c 5f68 7970 6572 7061  fig/eval_hyperpa
+00001cf0: 7261 6d73 2e79 6d6c 202d 2d64 6174 615f  rams.yml --data_
+00001d00: 6669 6c65 206f 7574 7075 745f 6373 7620  file output_csv 
+00001d10: 2d2d 696d 6167 655f 6669 6c65 206f 7574  --image_file out
+00001d20: 7075 745f 706c 6f74 7320 2d2d 706c 6f74  put_plots --plot
+00001d30: 5f63 7572 7665 7320 5472 7565 202d 2d73  _curves True --s
+00001d40: 6176 655f 6669 6c65 2054 7275 650d 0a60  ave_file True..`
+00001d50: 6060 0d0a 0d0a 2323 2320 4879 7065 7270  ``....### Hyperp
+00001d60: 6172 616d 6574 6572 2054 756e 696e 670d  arameter Tuning.
+00001d70: 0a0d 0a42 656c 6f77 2070 726f 7669 6465  ...Below provide
+00001d80: 7320 7573 6572 7320 7477 6f20 7479 7065  s users two type
+00001d90: 7320 6f66 2074 756e 696e 6720 7374 7261  s of tuning stra
+00001da0: 7465 6769 6573 2074 6861 7420 6665 6174  tegies that feat
+00001db0: 7572 6520 6469 6666 6572 656e 7420 6675  ure different fu
+00001dc0: 6e63 7469 6f6e 616c 6974 6965 732e 0d0a  nctionalities...
+00001dd0: 0d0a 2323 2323 202a 2a57 616e 6462 2054  ..#### **Wandb T
+00001de0: 756e 696e 672a 2a0d 0a0d 0a41 206d 6163  uning**....A mac
+00001df0: 6869 6e65 206c 6561 726e 696e 6720 6465  hine learning de
+00001e00: 7665 6c6f 706d 656e 7420 706c 6174 666f  velopment platfo
+00001e10: 726d 2074 6861 7420 616c 6c6f 7773 2075  rm that allows u
+00001e20: 7365 7273 2074 6f20 7472 6163 6b20 616e  sers to track an
+00001e30: 6420 7669 7375 616c 697a 6520 7661 726f  d visualize varo
+00001e40: 7520 6173 7065 6374 7320 6f66 2074 6865  u aspects of the
+00001e50: 6972 206d 6f64 656c 2074 7261 696e 696e  ir model trainin
+00001e60: 6720 7072 6f63 6573 7320 696e 2072 6561  g process in rea
+00001e70: 6c2d 7469 6d65 2c20 696e 636c 7564 696e  l-time, includin
+00001e80: 6720 6c6f 7373 2061 6e64 2061 6363 7572  g loss and accur
+00001e90: 6163 7920 6368 6172 7473 2c20 7061 7261  acy charts, para
+00001ea0: 6d65 7465 7220 6469 7374 7269 6275 7469  meter distributi
+00001eb0: 6f6e 732c 2067 7261 6469 656e 7420 6869  ons, gradient hi
+00001ec0: 7374 6f67 7261 6d73 2061 6e64 2073 7973  stograms and sys
+00001ed0: 7465 6d20 6d65 7472 6963 732e 2054 6f20  tem metrics. To 
+00001ee0: 7275 6e20 7761 6e64 623a 0d0a 0d0a 6060  run wandb:....``
+00001ef0: 6062 6173 680d 0a70 7974 686f 6e20 6d61  `bash..python ma
+00001f00: 696e 2e70 7920 2d2d 6675 6e63 7469 6f6e  in.py --function
+00001f10: 2074 756e 6520 2d2d 636f 6e66 6967 5f66   tune --config_f
+00001f20: 696c 6520 7573 6572 5f63 6f6e 6669 672f  ile user_config/
+00001f30: 636f 6e66 6967 7572 6174 696f 6e2e 796d  configuration.ym
+00001f40: 6c20 2d2d 7061 7261 6d5f 6669 6c65 2075  l --param_file u
+00001f50: 7365 725f 636f 6e66 6967 2f65 7661 6c5f  ser_config/eval_
+00001f60: 6879 7065 7270 6172 616d 732e 796d 6c20  hyperparams.yml 
+00001f70: 2d2d 6461 7461 5f66 696c 6520 6f75 7470  --data_file outp
+00001f80: 7574 5f63 7376 202d 2d69 6d61 6765 5f66  ut_csv --image_f
+00001f90: 696c 6520 6f75 7470 7574 5f70 6c6f 7473  ile output_plots
+00001fa0: 202d 2d70 6c6f 745f 6375 7276 6573 2054   --plot_curves T
+00001fb0: 7275 6520 2d2d 7361 7665 5f66 696c 6520  rue --save_file 
+00001fc0: 5472 7565 202d 2d74 756e 6572 2077 616e  True --tuner wan
+00001fd0: 6462 200d 0a60 6060 0d0a 0d0a 2323 2323  db ..```....####
+00001fe0: 202a 2a52 6179 2054 756e 696e 672a 2a0d   **Ray Tuning**.
+00001ff0: 0a0d 0a41 6e20 696e 6475 7374 7279 2073  ...An industry s
+00002000: 7461 6e64 6172 6420 746f 6f6c 2066 6f72  tandard tool for
+00002010: 2064 6973 7472 6962 7574 6564 2068 7970   distributed hyp
+00002020: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
+00002030: 6e67 2077 6869 6368 2069 6e74 6567 7261  ng which integra
+00002040: 7465 7320 7769 7468 2054 656e 736f 7242  tes with TensorB
+00002050: 6f61 7264 2061 6e64 2065 7874 656e 7369  oard and extensi
+00002060: 7665 2061 6e61 6c79 7369 7320 6c69 6272  ve analysis libr
+00002070: 6172 6965 732e 2049 7420 616c 736f 2061  aries. It also a
+00002080: 6c6c 6f77 7320 7573 6572 7320 746f 206c  llows users to l
+00002090: 6576 6572 6167 6520 6375 7474 696e 6720  everage cutting 
+000020a0: 6564 6765 206f 7074 696d 697a 6174 696f  edge optimizatio
+000020b0: 6e20 616c 676f 7269 7468 6d73 2061 7420  n algorithms at 
+000020c0: 7363 616c 652c 2069 6e63 6c75 6469 6e67  scale, including
+000020d0: 2042 6179 6573 6961 6e20 4f70 7469 6d69   Bayesian Optimi
+000020e0: 7a61 7469 6f6e 2c20 506f 7075 6c61 7469  zation, Populati
+000020f0: 6f6e 2042 6173 6564 2054 7261 696e 696e  on Based Trainin
+00002100: 6720 616e 6420 4879 7065 7242 616e 642e  g and HyperBand.
+00002110: 2054 6f20 7275 6e20 7261 7920 7475 6e69   To run ray tuni
+00002120: 6e67 3a0d 0a0d 0a60 6060 6261 7368 0d0a  ng:....```bash..
+00002130: 7079 7468 6f6e 206d 6169 6e2e 7079 202d  python main.py -
+00002140: 2d66 756e 6374 696f 6e20 7475 6e65 202d  -function tune -
+00002150: 2d63 6f6e 6669 675f 6669 6c65 2075 7365  -config_file use
+00002160: 725f 636f 6e66 6967 2f63 6f6e 6669 6775  r_config/configu
+00002170: 7261 7469 6f6e 2e79 6d6c 202d 2d70 6172  ration.yml --par
+00002180: 616d 5f66 696c 6520 7573 6572 5f63 6f6e  am_file user_con
+00002190: 6669 672f 6576 616c 5f68 7970 6572 7061  fig/eval_hyperpa
+000021a0: 7261 6d73 2e79 6d6c 202d 2d64 6174 615f  rams.yml --data_
+000021b0: 6669 6c65 206f 7574 7075 745f 6373 7620  file output_csv 
+000021c0: 2d2d 696d 6167 655f 6669 6c65 206f 7574  --image_file out
+000021d0: 7075 745f 706c 6f74 7320 2d2d 706c 6f74  put_plots --plot
+000021e0: 5f63 7572 7665 7320 5472 7565 202d 2d73  _curves True --s
+000021f0: 6176 655f 6669 6c65 2054 7275 6520 2d2d  ave_file True --
+00002200: 7475 6e65 7220 7261 795f 7475 6e65 0d0a  tuner ray_tune..
+00002210: 6060 600d 0a0d 0a23 2320 5374 6570 2033  ```....## Step 3
+00002220: 3a20 4578 706c 6f72 6520 4665 6174 7572  : Explore Featur
+00002230: 6573 0d0a 0d0a 2323 2320 312e 202a 2a45  es....### 1. **E
+00002240: 7870 6c6f 7265 2042 7265 616b 646f 776e  xplore Breakdown
+00002250: 2053 6365 6e61 7269 6f73 2a2a 0d0a 0d0a   Scenarios**....
+00002260: 5468 6973 2066 6561 7475 7265 2061 6c6c  This feature all
+00002270: 6f77 7320 7468 6520 7573 6572 2074 6f20  ows the user to 
+00002280: 7472 6169 6e20 7468 6520 6167 656e 7420  train the agent 
+00002290: 6261 7365 6420 6f6e 2063 7573 746f 6d65  based on custome
+000022a0: 6420 6578 706c 6f72 6174 696f 6e20 7072  d exploration pr
+000022b0: 6566 6572 656e 6365 7320 6265 7477 6565  eferences betwee
+000022c0: 6e20 6b65 7920 7374 6174 6573 2061 6e64  n key states and
+000022d0: 2070 6572 6970 6865 7261 6c20 7374 6174   peripheral stat
+000022e0: 6573 2075 7369 6e67 2077 6569 6768 7420  es using weight 
+000022f0: 7061 7261 6d65 7465 7220 6077 315f 6b65  parameter `w1_ke
+00002300: 7960 2061 6e64 2060 7732 5f70 6572 6970  y` and `w2_perip
+00002310: 6865 7261 6c60 2e20 5468 6520 7075 7270  heral`. The purp
+00002320: 6f73 6520 6f66 2074 6869 7320 6665 6174  ose of this feat
+00002330: 7572 6520 6973 2074 6f20 656e 6162 6c65  ure is to enable
+00002340: 2074 6865 2061 6765 6e74 2074 6f20 6e6f   the agent to no
+00002350: 7420 6f6e 6c79 2067 656e 6572 6174 6520  t only generate 
+00002360: 6869 6768 2072 6577 6172 6473 2066 6f72  high rewards for
+00002370: 206b 6579 2073 7461 7465 7320 6275 7420   key states but 
+00002380: 616c 736f 2076 6973 6974 2061 6c6c 2062  also visit all b
+00002390: 7265 6164 6f77 6e20 7363 656e 6172 696f  readown scenario
+000023a0: 7320 7375 6666 6963 6965 6e74 6c79 2065  s sufficiently e
+000023b0: 6e6f 7567 682e 200d 0a0d 0a53 6574 2075  nough. ....Set u
+000023c0: 7020 7468 6520 7061 7261 6d65 7465 7273  p the parameters
+000023d0: 2069 6e20 6075 7365 725f 636f 6e66 6967   in `user_config
+000023e0: 5c66 6561 7475 7265 735f 7061 7261 6d73  \features_params
+000023f0: 5c62 6c6f 6163 6b61 6765 5f65 7870 6c6f  \bloackage_explo
+00002400: 7265 5f70 6172 616d 732e 796d 6c60 3a0d  re_params.yml`:.
+00002410: 0a0d 0a2d 2060 7731 5f6b 6579 603a 2057  ...- `w1_key`: W
+00002420: 6569 6768 7420 7061 7261 6d65 7465 7220  eight parameter 
+00002430: 746f 2063 6f6e 7472 6f6c 2066 6176 6f72  to control favor
+00002440: 2065 7870 6c6f 7269 6e67 206b 6579 2073   exploring key s
+00002450: 7461 7465 732e 0d0a 2d20 6077 325f 7065  tates...- `w2_pe
+00002460: 7269 7068 6572 616c 603a 2057 6569 6768  ripheral`: Weigh
+00002470: 7420 7061 7261 6d65 7465 7220 746f 2063  t parameter to c
+00002480: 6f6e 7472 6f6c 2066 6176 6f72 2065 7870  ontrol favor exp
+00002490: 6c6f 7269 6e67 2070 6572 6970 6865 7261  loring periphera
+000024a0: 6c20 7374 6174 6573 2e0d 0a2d 2060 7265  l states...- `re
+000024b0: 7365 7460 3a20 4120 626f 6f6c 2076 616c  set`: A bool val
+000024c0: 7565 2074 6861 7420 636f 6e74 726f 6c73  ue that controls
+000024d0: 2077 6865 7468 6572 2074 6f20 7265 7365   whether to rese
+000024e0: 7420 7765 6967 6874 2070 6172 616d 6574  t weight paramet
+000024f0: 6572 7320 6475 7269 6e67 2074 7261 696e  ers during train
+00002500: 696e 672e 0d0a 2d20 6072 6573 6574 5f66  ing...- `reset_f
+00002510: 7265 7175 656e 6379 603a 2041 2076 616c  requency`: A val
+00002520: 7565 2074 6861 7420 6465 6669 6e65 7320  ue that defines 
+00002530: 7468 6520 6e75 6d62 6572 206f 6620 6570  the number of ep
+00002540: 6973 6f64 6573 2066 7265 7175 656e 6379  isodes frequency
+00002550: 2074 6f20 7265 7365 7420 7468 6520 7765   to reset the we
+00002560: 6967 6874 2070 6172 616d 6574 6572 732e  ight parameters.
+00002570: 0d0a 2d20 606e 756d 5f6f 7574 7075 7460  ..- `num_output`
+00002580: 3a20 4120 7661 6c75 6520 7468 6174 2064  : A value that d
+00002590: 6566 696e 6573 2074 6865 206e 756d 6265  efines the numbe
+000025a0: 7220 6f66 2074 6f70 2061 6e64 206c 6561  r of top and lea
+000025b0: 7374 2072 6577 6172 642f 7669 7369 7473  st reward/visits
+000025c0: 2073 7461 7465 7320 746f 2070 6c6f 7420   states to plot 
+000025d0: 696e 2061 2068 6973 746f 6772 616d 0d0a  in a histogram..
+000025e0: 2d20 606f 7574 7075 745f 6a73 6f6e 603a  - `output_json`:
+000025f0: 2041 2062 6f6f 6c20 7661 6c75 6520 7468   A bool value th
+00002600: 6174 2064 6574 6572 6d69 6e65 7320 7768  at determines wh
+00002610: 6574 6865 7220 746f 206f 7574 7075 7420  ether to output 
+00002620: 7468 6520 6a73 6f6e 2066 696c 6520 6f66  the json file of
+00002630: 206b 6579 2073 7461 7465 7320 616e 6420   key states and 
+00002640: 7065 7269 7068 6572 616c 2073 7461 7465  peripheral state
+00002650: 730d 0a2d 2060 6f75 7470 7574 5f68 6973  s..- `output_his
+00002660: 746f 6772 616d 603a 2041 2062 6f6f 6c20  togram`: A bool 
+00002670: 7661 6c75 6520 7468 6174 2064 6574 6572  value that deter
+00002680: 6d69 6e65 7320 7768 6574 6865 7220 746f  mines whether to
+00002690: 206f 7574 7075 7420 7468 6520 6869 7374   output the hist
+000026a0: 6f67 7261 6d20 7468 6174 2073 686f 7773  ogram that shows
+000026b0: 2074 6865 2072 6577 6172 6473 2061 6e64   the rewards and
+000026c0: 2076 6973 6974 7320 6f66 2074 6865 2074   visits of the t
+000026d0: 6f70 2061 6e64 206c 6561 7374 2073 7461  op and least sta
+000026e0: 7465 732e 0d0a 2d20 606f 7574 7075 745f  tes...- `output_
+000026f0: 636f 7665 7261 6765 5f6d 6574 7269 6360  coverage_metric`
+00002700: 3a20 4120 626f 6f6c 2076 616c 7565 2074  : A bool value t
+00002710: 6861 7420 6465 7465 726d 696e 6573 2077  hat determines w
+00002720: 6865 7468 6572 2074 6f20 6f75 7470 7574  hether to output
+00002730: 2074 6865 2063 7572 7265 6e74 2063 6f76   the current cov
+00002740: 6572 6167 6520 6d65 7472 6963 2e0d 0a0d  erage metric....
+00002750: 0a54 6f20 7275 6e20 7468 6973 2066 6561  .To run this fea
+00002760: 7475 7265 2c20 6e61 7669 6761 7465 2074  ture, navigate t
+00002770: 6f20 602f 666f 756e 6461 7469 6f6e 732f  o `/foundations/
+00002780: 6272 6561 6b64 6f77 6e5f 6578 706c 6f72  breakdown_explor
+00002790: 6174 696f 6e60 2061 6e64 2072 756e 3a0d  ation` and run:.
+000027a0: 0a20 2020 6060 6062 6173 680d 0a20 2020  .   ```bash..   
+000027b0: 7079 7468 6f6e 2062 7265 616b 646f 776e  python breakdown
+000027c0: 5f65 7870 6c6f 7261 7469 6f6e 2e70 790d  _exploration.py.
+000027d0: 0a20 2020 6060 600d 0a0d 0a23 2323 2032  .   ```....### 2
+000027e0: 2e20 2a2a 4465 6369 7369 6f6e 2045 7661  . **Decision Eva
+000027f0: 6c75 6174 696f 6e20 2842 6c6f 636b 6167  luation (Blockag
+00002800: 6520 4465 6d6f 6e73 7472 6174 696f 6e73  e Demonstrations
+00002810: 292a 2a0d 0a0d 0a54 6869 7320 6665 6174  )**....This feat
+00002820: 7572 6520 616c 6c6f 7773 2074 6865 2075  ure allows the u
+00002830: 7365 7220 746f 2074 6573 7420 6120 7472  ser to test a tr
+00002840: 6169 6e65 6420 6167 656e 7427 7320 7065  ained agent's pe
+00002850: 7266 6f72 6d61 6e63 6520 6f6e 2061 2073  rformance on a s
+00002860: 696d 756c 6174 6564 2073 6572 7665 7220  imulated server 
+00002870: 626c 6f63 6b61 6765 2071 7565 7565 696e  blockage queuein
+00002880: 6720 656e 7669 726f 6e6d 656e 7420 6279  g environment by
+00002890: 2076 6973 7561 6c69 7a69 6e67 2074 6865   visualizing the
+000028a0: 2063 6861 6e67 6573 2069 6e20 7472 616e   changes in tran
+000028b0: 7369 7469 6f6e 2070 726f 6261 6269 6c69  sition probabili
+000028c0: 7469 6573 2e20 5468 6520 7075 7270 6f73  ties. The purpos
+000028d0: 6520 6f66 2074 6869 7320 6665 6174 7572  e of this featur
+000028e0: 6520 6973 2074 6f20 7368 6f77 2068 6f77  e is to show how
+000028f0: 2065 6666 6563 7469 6365 2074 6865 2074   effectice the t
+00002900: 7261 6e69 6564 2061 6765 6e74 2069 7320  ranied agent is 
+00002910: 6163 7469 6e67 206f 6e20 6272 6561 6b64  acting on breakd
+00002920: 6f77 6e20 6361 7365 732e 200d 0a0d 0a2d  own cases. ....-
+00002930: 2060 6e75 6d5f 7369 6d60 3a20 4465 6669   `num_sim`: Defi
+00002940: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
+00002950: 6620 6a6f 6273 2074 6f20 7369 6d75 6c61  f jobs to simula
+00002960: 7465 2066 6f72 2065 6163 6820 7469 6d65  te for each time
+00002970: 2073 7465 7020 6475 7269 6e67 2074 7261   step during tra
+00002980: 696e 696e 672e 0d0a 2d20 6074 696d 655f  ining...- `time_
+00002990: 7374 6570 7360 3a20 4465 6669 6e65 7320  steps`: Defines 
+000029a0: 7468 6520 6e75 6d62 6572 206f 6620 7469  the number of ti
+000029b0: 6d65 2073 7465 7073 2074 6f20 7065 7266  me steps to perf
+000029c0: 6f72 6d20 666f 7220 6561 6368 2065 7069  orm for each epi
+000029d0: 736f 6465 2e0d 0a2d 2060 7175 6575 655f  sode...- `queue_
+000029e0: 696e 6465 7860 3a20 4465 6669 6e65 7320  index`: Defines 
+000029f0: 7468 6520 7175 6575 6520 696e 6465 7820  the queue index 
+00002a00: 7468 6174 2072 6563 6f72 6420 7468 6520  that record the 
+00002a10: 6d65 7472 6963 7320 666f 722e 0d0a 2d20  metrics for...- 
+00002a20: 606d 6574 7269 6360 3a20 4465 6669 6e65  `metric`: Define
+00002a30: 7320 7468 6520 6d65 7472 6963 2074 6f20  s the metric to 
+00002a40: 6265 2072 6570 6f72 7465 6420 666f 7220  be reported for 
+00002a50: 7468 6520 7365 6c65 6374 6564 2071 7565  the selected que
+00002a60: 7565 2e0d 0a0d 0a54 6f20 7573 6520 7468  ue.....To use th
+00002a70: 6973 2066 6561 7475 7265 2c20 6e61 7669  is feature, navi
+00002a80: 6761 7465 2074 6f20 602f 6576 616c 7561  gate to `/evalua
+00002a90: 7469 6f6e 2f64 6563 6973 696f 6e5f 6576  tion/decision_ev
+00002aa0: 616c 7561 7469 6f6e 6020 616e 6420 7275  aluation` and ru
+00002ab0: 6e3a 0d0a 2020 2060 6060 6261 7368 0d0a  n:..   ```bash..
+00002ac0: 2020 2070 7974 686f 6e20 6465 6369 7369     python decisi
+00002ad0: 6f6e 5f65 7661 6c75 6174 696f 6e2e 7079  on_evaluation.py
+00002ae0: 0d0a 2020 2060 6060 0d0a 0d0a 2323 2320  ..   ```....### 
+00002af0: 332e 202a 2a53 7461 7274 7570 2042 6568  3. **Startup Beh
+00002b00: 6176 696f 7220 4964 656e 7469 6669 6361  avior Identifica
+00002b10: 7469 6f6e 2a2a 0d0a 0d0a 5468 6973 2066  tion**....This f
+00002b20: 6561 7475 7265 2061 6c6c 6f77 7320 7468  eature allows th
+00002b30: 6520 7573 6572 2074 6f20 7669 7375 616c  e user to visual
+00002b40: 697a 6520 7768 656e 2074 6865 2062 7572  ize when the bur
+00002b50: 6e2d 696e 2070 6572 696f 6473 2065 6e64  n-in periods end
+00002b60: 206f 6e20 7468 6520 6c65 6172 6e69 6e67   on the learning
+00002b70: 2063 7572 7665 2e20 0d0a 0d0a 5365 7420   curve. ....Set 
+00002b80: 7570 2074 6865 2070 6172 616d 6574 6572  up the parameter
+00002b90: 7320 696e 2074 6865 2073 6372 6970 743a  s in the script:
+00002ba0: 0d0a 0d0a 2d20 6077 696e 646f 775f 7369  ....- `window_si
+00002bb0: 7a65 603a 2053 7065 6369 6669 6573 2074  ze`: Specifies t
+00002bc0: 6865 206e 756d 6265 7220 6f66 2064 6174  he number of dat
+00002bd0: 6120 706f 696e 7473 2075 7365 6420 746f  a points used to
+00002be0: 2063 6f6d 7075 7465 2074 6865 206d 6f76   compute the mov
+00002bf0: 696e 6720 6176 6572 6167 6520 6f66 2074  ing average of t
+00002c00: 6865 2072 6577 6172 6473 2e0d 0a2d 2060  he rewards...- `
+00002c10: 7468 7265 7368 6f6c 6460 3a20 4465 6669  threshold`: Defi
+00002c20: 6e65 7320 7468 6520 6d61 7869 6d75 6d20  nes the maximum 
+00002c30: 6163 6365 7074 6162 6c65 2061 6273 6f6c  acceptable absol
+00002c40: 7574 6520 7661 6c75 6520 6f66 2074 6865  ute value of the
+00002c50: 2064 6572 6976 6174 6976 6520 6f66 2074   derivative of t
+00002c60: 6865 2073 6d6f 6f74 6865 6420 7265 7761  he smoothed rewa
+00002c70: 7264 7320 6265 6c6f 7720 7768 6963 6820  rds below which 
+00002c80: 6120 7265 7761 7264 2069 7320 636f 6e73  a reward is cons
+00002c90: 6964 6572 6564 2073 7461 626c 652e 200d  idered stable. .
+00002ca0: 0a2d 2060 636f 6e73 6563 7574 6976 655f  .- `consecutive_
+00002cb0: 706f 696e 7473 603a 2054 6865 206e 756d  points`: The num
+00002cc0: 6265 7220 6f66 2063 6f6e 7365 6375 7469  ber of consecuti
+00002cd0: 7665 2064 6174 6120 706f 696e 7473 2074  ve data points t
+00002ce0: 6861 7420 6d75 7374 2061 6c6c 2062 6520  hat must all be 
+00002cf0: 6265 6c6f 7720 7468 6520 7468 7265 7368  below the thresh
+00002d00: 6f6c 6420 666f 7220 7468 6520 7265 7761  old for the rewa
+00002d10: 7264 7320 746f 2062 6520 636f 6e73 6964  rds to be consid
+00002d20: 6572 6564 2061 7320 6861 7669 6e67 2073  ered as having s
+00002d30: 7461 6269 6c69 7a65 642e 200d 0a2d 2060  tabilized. ..- `
+00002d40: 6570 6973 6f64 6560 3a20 5370 6563 6966  episode`: Specif
+00002d50: 7920 7768 6963 6820 6570 6973 6f64 6527  y which episode'
+00002d60: 7320 7265 7761 7264 7320 746f 2061 6e61  s rewards to ana
+00002d70: 6c79 7a65 2066 726f 6d20 6120 6461 7461  lyze from a data
+00002d80: 7365 742e 0d0a 0d0a 546f 2070 6572 666f  set.....To perfo
+00002d90: 726d 2074 6865 2066 6561 7475 7265 2c20  rm the feature, 
+00002da0: 6e61 7669 6761 7465 2074 6f20 602f 6576  navigate to `/ev
+00002db0: 616c 7561 7469 6f6e 2f73 7461 7274 7570  aluation/startup
+00002dc0: 5f65 7661 6c75 6174 696f 6e60 2061 6e64  _evaluation` and
+00002dd0: 2072 756e 3a0d 0a20 2020 6060 6062 6173   run:..   ```bas
+00002de0: 680d 0a20 2020 7079 7468 6f6e 2073 7461  h..   python sta
+00002df0: 7274 7570 5f65 7661 6c75 6174 696f 6e2e  rtup_evaluation.
+00002e00: 7079 0d0a 2020 2060 6060 0d0a 0d0a 2323  py..   ```....##
+00002e10: 2320 342e 202a 2a43 6f6e 7665 7267 656e  # 4. **Convergen
+00002e20: 6365 2045 7661 6c75 6174 696f 6e2a 2a20  ce Evaluation** 
+00002e30: 0d0a 0d0a 5468 6973 2066 6561 7475 7265  ....This feature
+00002e40: 2061 6c6c 6f77 7320 7468 6520 7573 6572   allows the user
+00002e50: 2074 7261 696e 206d 756c 7469 706c 6520   train multiple 
+00002e60: 7665 7273 696f 6e73 206f 6620 7468 6520  versions of the 
+00002e70: 6167 656e 7420 666f 7220 6469 6666 6572  agent for differ
+00002e80: 656e 7420 6e75 6d62 6572 7320 6f66 2074  ent numbers of t
+00002e90: 7261 696e 696e 6720 6570 6973 6f64 6573  raining episodes
+00002ea0: 2061 6e64 2074 6865 6e20 6576 616c 7561   and then evalua
+00002eb0: 7465 2074 6865 2070 6572 666f 726d 616e  te the performan
+00002ec0: 6365 206f 6620 6561 6368 2061 6765 6e74  ce of each agent
+00002ed0: 206f 6e20 7468 6520 7369 6d75 6c61 7469   on the simulati
+00002ee0: 6f6e 2065 6e76 6972 6f6e 6d65 6e74 2e0d  on environment..
+00002ef0: 0a0d 0a53 6574 2075 7020 7468 6520 7061  ...Set up the pa
+00002f00: 7261 6d65 7465 7273 2069 6e20 7468 6520  rameters in the 
+00002f10: 7363 7269 7074 3a0d 0a0d 0a2d 2060 6e75  script:....- `nu
+00002f20: 6d5f 6570 6973 6f64 6573 5f6c 6973 7460  m_episodes_list`
+00002f30: 3a20 4120 6c69 7374 2074 6861 7420 636f  : A list that co
+00002f40: 6e74 6169 6e73 2064 6966 6665 7265 6e74  ntains different
+00002f50: 206e 756d 6265 7273 206f 6620 6570 6973   numbers of epis
+00002f60: 6f64 6573 2074 6f20 7472 6169 6e20 7468  odes to train th
+00002f70: 6520 6167 656e 7473 2e0d 0a2d 2060 7469  e agents...- `ti
+00002f80: 6d65 7374 6570 7360 3a20 4120 7661 6c75  mesteps`: A valu
+00002f90: 6520 7468 6174 2064 6566 696e 6573 2074  e that defines t
+00002fa0: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
+00002fb0: 6573 7465 7073 2074 6f20 7472 6169 6e20  esteps to train 
+00002fc0: 7468 6520 6167 656e 7420 6475 7269 6e67  the agent during
+00002fd0: 2065 6163 6820 6570 6973 6f64 652e 0d0a   each episode...
+00002fe0: 0d0a 546f 2072 756e 2074 6869 7320 6665  ..To run this fe
+00002ff0: 6174 7572 652c 206e 6176 6967 6174 6520  ature, navigate 
+00003000: 746f 2060 2f65 7661 6c75 6174 696f 6e2f  to `/evaluation/
+00003010: 636f 6e76 6572 6765 6e63 655f 6576 616c  convergence_eval
+00003020: 7561 7469 6f6e 6020 616e 6420 7275 6e3a  uation` and run:
+00003030: 0d0a 2020 2060 6060 6261 7368 0d0a 2020  ..   ```bash..  
+00003040: 2070 7974 686f 6e20 636f 6e76 6572 6765   python converge
+00003050: 6e63 655f 6576 616c 7561 7469 6f6e 2e70  nce_evaluation.p
+00003060: 790d 0a20 2020 6060 600d 0a0d 0a23 2323  y..   ```....###
+00003070: 2035 2e20 2a2a 526f 6275 7374 6e65 7373   5. **Robustness
+00003080: 2045 7661 6c75 6174 696f 6e2a 2a20 0d0a   Evaluation** ..
+00003090: 0d0a 5468 6973 2066 6561 7475 7265 2061  ..This feature a
+000030a0: 6c6c 6f77 7320 7468 6520 7573 6572 2074  llows the user t
+000030b0: 6f20 7472 6169 6e20 6d75 6c74 6970 6c65  o train multiple
+000030c0: 2061 6765 6e74 732c 2061 6e61 6c79 7a65   agents, analyze
+000030d0: 2074 6865 6972 2062 6568 6176 696f 722c   their behavior,
+000030e0: 2061 6e64 2063 616c 6375 6c61 7465 2073   and calculate s
+000030f0: 7461 7469 7374 6963 616c 206d 6574 7269  tatistical metri
+00003100: 6373 2062 6173 6564 206f 6e20 7468 6569  cs based on thei
+00003110: 7220 7065 7266 6f72 6d61 6e63 652e 0d0a  r performance...
+00003120: 0d0a 5365 7420 7570 2074 6865 2070 6172  ..Set up the par
+00003130: 616d 6574 6572 7320 696e 2074 6865 2073  ameters in the s
+00003140: 6372 6970 743a 0d0a 0d0a 2d20 6063 6f6e  cript:....- `con
+00003150: 6669 6465 6e63 655f 6c65 7665 6c60 3a20  fidence_level`: 
+00003160: 5468 6520 7374 6174 6973 7469 6361 6c20  The statistical 
+00003170: 636f 6e66 6964 656e 6365 206c 6576 656c  confidence level
+00003180: 2066 6f72 2063 616c 6375 6c61 7469 6f6e   for calculation
+00003190: 732e 0d0a 2d20 6064 6573 6972 6564 5f65  s...- `desired_e
+000031a0: 7272 6f72 603a 2054 6865 2074 6172 6765  rror`: The targe
+000031b0: 7420 6572 726f 7220 6d61 7267 696e 2066  t error margin f
+000031c0: 6f72 2065 7374 696d 6174 696e 6720 7374  or estimating st
+000031d0: 6174 6973 7469 6361 6c20 7265 7175 6972  atistical requir
+000031e0: 656d 656e 7473 2e0d 0a2d 2060 6e75 6d5f  ements...- `num_
+000031f0: 7275 6e73 603a 204e 756d 6265 7220 6f66  runs`: Number of
+00003200: 2074 696d 6573 2074 6f20 7472 6169 6e20   times to train 
+00003210: 6167 656e 7473 2e0d 0a2d 2060 7469 6d65  agents...- `time
+00003220: 5f73 7465 7073 603a 204e 756d 6265 7220  _steps`: Number 
+00003230: 6f66 2074 696d 6520 7374 6570 7320 6561  of time steps ea
+00003240: 6368 2061 6765 6e74 2072 756e 7320 696e  ch agent runs in
+00003250: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
+00003260: 656e 7669 726f 6e6d 656e 742e 0d0a 2d20  environment...- 
+00003270: 606e 756d 5f73 696d 603a 204e 756d 6265  `num_sim`: Numbe
+00003280: 7220 6f66 2073 696d 756c 6174 696f 6e73  r of simulations
+00003290: 2074 6f20 7275 6e20 696e 2074 6865 2065   to run in the e
+000032a0: 6e76 6972 6f6e 6d65 6e74 2e0d 0a0d 0a54  nvironment.....T
+000032b0: 6f20 7275 6e20 7468 6973 2066 6561 7475  o run this featu
+000032c0: 7265 2c20 6e61 7669 6761 7465 2074 6f20  re, navigate to 
+000032d0: 602f 6576 616c 7561 7469 6f6e 2f72 6f62  `/evaluation/rob
+000032e0: 7573 746e 6573 735f 6576 616c 7561 7469  ustness_evaluati
+000032f0: 6f6e 6020 616e 6420 7275 6e3a 0d0a 2020  on` and run:..  
+00003300: 2060 6060 6261 7368 0d0a 2020 2070 7974   ```bash..   pyt
+00003310: 686f 6e20 726f 6275 7374 6e65 7373 5f65  hon robustness_e
+00003320: 7661 6c75 6174 696f 6e2e 7079 0d0a 2020  valuation.py..  
+00003330: 2060 6060 0d0a 0d0a 2323 2320 362e 202a   ```....### 6. *
+00003340: 2a4e 6f69 7365 2045 7661 6c75 6174 696f  *Noise Evaluatio
+00003350: 6e2a 2a20 0d0a 0d0a 5468 6973 2066 6561  n** ....This fea
+00003360: 7475 7265 2061 6c6c 6f77 7320 7468 6520  ture allows the 
+00003370: 7573 6572 2074 6f20 6576 616c 7561 7465  user to evaluate
+00003380: 2074 6865 2065 6666 6563 7420 6f66 2065   the effect of e
+00003390: 6e76 6972 6f6e 6d65 6e74 616c 206e 6f69  nvironmental noi
+000033a0: 7365 206f 6e20 7468 6520 7065 7266 6f72  se on the perfor
+000033b0: 6d61 6e63 6520 6f66 2074 6865 2061 6765  mance of the age
+000033c0: 6e74 2e0d 0a0d 0a53 6574 2075 7020 7468  nt.....Set up th
+000033d0: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
+000033e0: 7468 6520 7363 7269 7074 3a0d 0a0d 0a2d  the script:....-
+000033f0: 2060 6672 6571 7565 6e63 7920 603a 2054   `frequency `: T
+00003400: 6865 206c 696b 656c 6968 6f6f 6420 6f72  he likelihood or
+00003410: 2066 7265 7175 656e 6379 2061 7420 7768   frequency at wh
+00003420: 6963 6820 6e6f 6973 6520 6973 2069 6e74  ich noise is int
+00003430: 726f 6475 6365 6420 746f 2074 6865 2073  roduced to the s
+00003440: 7973 7465 6d2e 2049 7420 6d75 7374 2062  ystem. It must b
+00003450: 6520 6120 7661 6c75 6520 6265 7477 6565  e a value betwee
+00003460: 6e20 3020 616e 6420 312e 2054 6869 7320  n 0 and 1. This 
+00003470: 7061 7261 6d65 7465 7220 6465 7465 726d  parameter determ
+00003480: 696e 6573 2068 6f77 206f 6674 656e 2c20  ines how often, 
+00003490: 7072 6f70 6f72 7469 6f6e 616c 6c79 2c20  proportionally, 
+000034a0: 6e6f 6973 6520 7769 6c6c 2062 6520 6164  noise will be ad
+000034b0: 6465 6420 6475 7269 6e67 2074 6865 2073  ded during the s
+000034c0: 696d 756c 6174 696f 6e2e 200d 0a2d 2060  imulation. ..- `
+000034d0: 6d65 616e 603a 2054 6865 206d 6561 6e20  mean`: The mean 
+000034e0: 6f66 2074 6865 206e 6f72 6d61 6c20 6469  of the normal di
+000034f0: 7374 7269 6275 7469 6f6e 2066 726f 6d20  stribution from 
+00003500: 7768 6963 6820 7468 6520 6e6f 6973 6520  which the noise 
+00003510: 7661 6c75 6573 2061 7265 2073 616d 706c  values are sampl
+00003520: 6564 2e20 5468 6973 2072 6570 7265 7365  ed. This represe
+00003530: 6e74 7320 7468 6520 6176 6572 6167 6520  nts the average 
+00003540: 7661 6c75 6520 6f66 2074 6865 206e 6f69  value of the noi
+00003550: 7365 2074 6861 7420 7769 6c6c 2062 6520  se that will be 
+00003560: 696e 7472 6f64 7563 6564 2e0d 0a2d 2060  introduced...- `
+00003570: 7661 7269 616e 6365 603a 2054 6865 2076  variance`: The v
+00003580: 6172 6961 6e63 6520 6f66 2074 6865 206e  ariance of the n
+00003590: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+000035a0: 6f6e 2066 726f 6d20 7768 6963 6820 7468  on from which th
+000035b0: 6520 6e6f 6973 6520 7661 6c75 6573 2061  e noise values a
+000035c0: 7265 2073 616d 706c 6564 2e20 5468 6973  re sampled. This
+000035d0: 2070 6172 616d 6574 6572 2069 6e64 6963   parameter indic
+000035e0: 6174 6573 2074 6865 2073 7072 6561 6420  ates the spread 
+000035f0: 6f72 2064 6973 7065 7273 696f 6e20 6f66  or dispersion of
+00003600: 2074 6865 206e 6f69 7365 2061 726f 756e   the noise aroun
+00003610: 6420 7468 6520 6d65 616e 2e0d 0a0d 0a54  d the mean.....T
+00003620: 6f20 7275 6e20 7468 6520 6665 6174 7572  o run the featur
+00003630: 652c 206e 6176 6967 6174 6520 746f 2060  e, navigate to `
+00003640: 2f65 7661 6c75 6174 696f 6e2f 6e6f 6973  /evaluation/nois
+00003650: 655f 6576 616c 7561 7469 6f6e 6020 616e  e_evaluation` an
+00003660: 6420 7275 6e3a 0d0a 2020 2060 6060 6261  d run:..   ```ba
+00003670: 7368 0d0a 2020 2070 7974 686f 6e20 6e6f  sh..   python no
+00003680: 6973 655f 6576 616c 7561 7469 6f6e 2e70  ise_evaluation.p
+00003690: 790d 0a20 2020 6060 600d 0a0d 0a23 2320  y..   ```....## 
+000036a0: 436f 6e74 7269 6275 7469 6f6e 0d0a 0d0a  Contribution....
+000036b0: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+000036c0: 6520 7765 6c63 6f6d 652e 2050 6c65 6173  e welcome. Pleas
+000036d0: 6520 6372 6561 7465 2061 2070 756c 6c20  e create a pull 
+000036e0: 7265 7175 6573 7420 6f72 2069 7373 7565  request or issue
+000036f0: 2074 6f20 6469 7363 7573 7320 7072 6f70   to discuss prop
+00003700: 6f73 6564 2063 6861 6e67 6573 206f 7220  osed changes or 
+00003710: 7265 706f 7274 2062 7567 732e 0d0a 0d0a  report bugs.....
+00003720: 2323 204c 6963 656e 7365 0d0a 0d0a 5468  ## License....Th
+00003730: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+00003740: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00003750: 204d 4954 204c 6963 656e 7365 202d 2073   MIT License - s
+00003760: 6565 2074 6865 204c 4943 454e 5345 2066  ee the LICENSE f
+00003770: 696c 6520 666f 7220 6465 7461 696c 732e  ile for details.
+00003780: 0d0a                                     ..
```

### Comparing `sim_rl-0.1.7/sim_rl/.gitlab-ci.yml` & `sim_rl-0.1.8/sim_rl/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/__pycache__/buffer.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/agents/__pycache__/buffer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/__pycache__/model.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/agents/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/buffer.py` & `sim_rl-0.1.8/sim_rl/agents/buffer.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/ddpg_agent.py` & `sim_rl-0.1.8/sim_rl/agents/ddpg_agent.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/model.py` & `sim_rl-0.1.8/sim_rl/agents/model.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/trained_agent.pt` & `sim_rl-0.1.8/sim_rl/agents/trained_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/agents/trained_ddpg_agent.pt` & `sim_rl-0.1.8/sim_rl/agents/trained_ddpg_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/debug.py` & `sim_rl-0.1.8/sim_rl/debug.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py` & `sim_rl-0.1.8/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/convergence_evaluation/reward_plot.png` & `sim_rl-0.1.8/sim_rl/evaluation/convergence_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/decision_evaluation/decision_evaluation.py` & `sim_rl-0.1.8/sim_rl/evaluation/decision_evaluation/decision_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png` & `sim_rl-0.1.8/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/noise_evaluation/noise_evaluation.py` & `sim_rl-0.1.8/sim_rl/evaluation/noise_evaluation/noise_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py` & `sim_rl-0.1.8/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot.png` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_0.png` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_0.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_1.png` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_2.png` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/reward_plot_3.png` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/reward_plot_3.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/evaluation/startup_evaluation/startup_evaluation.py` & `sim_rl-0.1.8/sim_rl/evaluation/startup_evaluation/startup_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc` & `sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py` & `sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json` & `sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png` & `sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png` & `sim_rl-0.1.8/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/core_functions.py` & `sim_rl-0.1.8/sim_rl/foundations/core_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/core_plotting.py` & `sim_rl-0.1.8/sim_rl/foundations/core_plotting.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/action_dict.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/action_dict.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/actor_loss.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/actor_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/critic_loss.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/critic_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/next_state_model_loss.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/next_state_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/reward_dict.json` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/reward_dict.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/reward_model_loss.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/reward_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/foundations/output_csv/transition_proba.csv` & `sim_rl-0.1.8/sim_rl/foundations/output_csv/transition_proba.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/main.py` & `sim_rl-0.1.8/sim_rl/main.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_base_functions.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_base_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.gitignore` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.gitignore`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/.readthedocs.yml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/CHANGELOG.md` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/cliff.toml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/cliff.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/search.html` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/search.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/conf.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/current_state.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/current_state.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/current_state1.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/current_state1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/fig.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/fig.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/graph.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/index.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/installation.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/make.bat` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/Makefile` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/my_network.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/my_network.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/my_network1.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/my_network1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/network.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/network.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/overview.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/queues.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/queues.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/sim.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/sim.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/sim1.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/sim1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/store.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/store.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/docs/store1.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/docs/store1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/LICENSE.txt` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/poetry.lock` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/poetry.lock`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/pyproject.toml` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/README.rst` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/README.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_network.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py` & `sim_rl-0.1.8/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/queue_env/queueing_network.py` & `sim_rl-0.1.8/sim_rl/queue_env/queueing_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/rl_env/RL_Environment.py` & `sim_rl-0.1.8/sim_rl/rl_env/RL_Environment.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc` & `sim_rl-0.1.8/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/tuning/ray_tuning.py` & `sim_rl-0.1.8/sim_rl/tuning/ray_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/tuning/wandb_tuning.py` & `sim_rl-0.1.8/sim_rl/tuning/wandb_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/user_config/configuration.yml` & `sim_rl-0.1.8/sim_rl/user_config/configuration.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/sim_rl/user_config/eval_hyperparams.yml` & `sim_rl-0.1.8/sim_rl/user_config/eval_hyperparams.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.7/PKG-INFO` & `sim_rl-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sim_rl
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulation Driven RL Package Utilized to Optimize Queueing Systems
 Author: Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi
 Author-email: fatima.al-ani23@imperial.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,15 +28,15 @@
 ## Project Structure
 
 - `agents`: Contains the Dyna-DDPG agent implementation and allows the integration of new types of agents for exploring the simulated queueing environment.
 - `queue_env`: Defines the simulated queueing environment, utilizing functionalities from the `queueing-tool` package.
 - `rl_env`: Hosts the RL environment, which is portable and compatible with different agent types.
 - `features`: Includes several utility features:
   - **Decision Evaluation**: Demonstrates how the agent responds to a server outage by adjusting routing probabilities.
-  - **Confidence Evaluation**: Assesses the stability and reliability of the agent across different training setups
+  - **Convergence Evaluation**: Assesses the stability and reliability of the agent across different training setups
   - **Noise Evaluation**: Evaluate the effect of environmental noise on the performance of the agent
   - **Startup Evaluation**: Identifies the burn-in period of the agent
   - **Robustness Evaluation**: Assess robustness of decisions across multiple trained agents
 
 ## Prerequisites
 
 Before running the simulations, ensure you have the following installed:
```

