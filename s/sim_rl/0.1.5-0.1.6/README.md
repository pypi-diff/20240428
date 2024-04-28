# Comparing `tmp/sim_rl-0.1.5.tar.gz` & `tmp/sim_rl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim_rl-0.1.5.tar", max compression
+gzip compressed data, was "sim_rl-0.1.6.tar", max compression
```

## Comparing `sim_rl-0.1.5.tar` & `sim_rl-0.1.6.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0      754 2024-04-28 17:01:04.076165 sim_rl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    14168 2024-04-27 14:20:33.937868 sim_rl-0.1.5/README.md
--rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.5/sim_rl/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.5/sim_rl/__init__.py
--rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.5/sim_rl/agents/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:57.799129 sim_rl-0.1.5/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3593 2024-04-28 15:25:57.812081 sim_rl-0.1.5/sim_rl/agents/__pycache__/buffer.cpython-310.pyc
--rw-r--r--   0        0        0    13843 2024-04-28 15:25:57.804520 sim_rl-0.1.5/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc
--rw-r--r--   0        0        0     9252 2024-04-28 15:25:57.809029 sim_rl-0.1.5/sim_rl/agents/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.5/sim_rl/agents/buffer.py
--rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.5/sim_rl/agents/ddpg_agent.py
--rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.5/sim_rl/agents/model.py
--rw-r--r--   0        0        0   282094 2024-04-28 15:26:02.560345 sim_rl-0.1.5/sim_rl/agents/trained_agent.pt
--rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.5/sim_rl/agents/trained_ddpg_agent.pt
--rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.5/sim_rl/debug.py
--rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.5/sim_rl/dist/sim_rl-0.1.0.tar.gz
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.5/sim_rl/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.5/sim_rl/evaluation/convergence_evaluation/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.5/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
--rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.5/sim_rl/evaluation/convergence_evaluation/reward_plot.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.5/sim_rl/evaluation/decision_evaluation/__init__.py
--rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.5/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
--rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.5/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.5/sim_rl/evaluation/noise_evaluation/__init__.py
--rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.5/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.5/sim_rl/evaluation/robustness_evaluation/__init__.py
--rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.5/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/__init__.py
--rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot.png
--rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
--rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
--rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
--rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
--rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.5/sim_rl/foundations/__init__.py
--rw-r--r--   0        0        0      162 2024-04-28 15:25:54.662508 sim_rl-0.1.5/sim_rl/foundations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    31515 2024-04-28 15:25:54.670219 sim_rl-0.1.5/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc
--rw-r--r--   0        0        0    10353 2024-04-28 15:25:58.846613 sim_rl-0.1.5/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/__init__.py
--rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
--rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
--rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
--rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
--rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
--rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
--rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
--rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
--rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.5/sim_rl/foundations/core_functions.py
--rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.5/sim_rl/foundations/core_plotting.py
--rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.5/sim_rl/foundations/output_csv/action_dict.csv
--rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.5/sim_rl/foundations/output_csv/actor_loss.csv
--rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.5/sim_rl/foundations/output_csv/critic_loss.csv
--rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.5/sim_rl/foundations/output_csv/next_state_model_loss.csv
--rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.5/sim_rl/foundations/output_csv/reward_dict.json
--rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.5/sim_rl/foundations/output_csv/reward_model_loss.csv
--rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.5/sim_rl/foundations/output_csv/transition_proba.csv
--rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.5/sim_rl/main.py
--rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.5/sim_rl/Makefile
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.5/sim_rl/queue_env/__init__.py
--rw-r--r--   0        0        0      160 2024-04-28 15:25:57.816084 sim_rl-0.1.5/sim_rl/queue_env/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9916 2024-04-28 15:25:58.842612 sim_rl-0.1.5/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc
--rw-r--r--   0        0        0     5432 2024-04-28 15:25:57.819081 sim_rl-0.1.5/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc
--rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.5/sim_rl/queue_env/queue_base_functions.py
--rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
--rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.gitignore
--rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.readthedocs.yml
--rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/CHANGELOG.md
--rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/CITATION.cff
--rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/cliff.toml
--rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
--rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
--rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
--rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
--rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
--rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
--rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
--rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
--rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
--rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
--rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
--rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
--rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/conf.py
--rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/current_state.png
--rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/current_state1.png
--rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
--rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
--rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/fig.png
--rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/graph.rst
--rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/index.rst
--rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/installation.rst
--rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/make.bat
--rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/Makefile
--rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/modules.rst
--rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/my_network.png
--rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/my_network1.png
--rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/network.rst
--rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/overview.rst
--rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/queues.rst
--rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/requirements.txt
--rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/sim.png
--rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/sim1.png
--rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/store.png
--rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/store1.png
--rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
--rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/LICENSE.txt
--rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/MANIFEST.in
--rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/poetry.lock
--rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/pyproject.toml
--rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
--rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
--rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
--rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
--rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
--rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
--rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
--rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
--rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
--rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
--rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
--rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
--rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
--rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
--rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
--rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
--rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
--rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/README.rst
--rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/setup.py
--rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
--rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
--rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
--rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_network.py
--rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
--rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
--rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
--rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.5/sim_rl/queue_env/queueing_network.py
--rw-r--r--   0        0        0      191 2024-04-28 17:02:38.117430 sim_rl-0.1.5/sim_rl/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.5/sim_rl/rl_env/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:58.834087 sim_rl-0.1.5/sim_rl/rl_env/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    14513 2024-04-28 15:25:58.838089 sim_rl-0.1.5/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc
--rw-r--r--   0        0        0    16235 2024-04-28 17:01:26.321399 sim_rl-0.1.5/sim_rl/rl_env/RL_Environment.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.5/sim_rl/tuning/__init__.py
--rw-r--r--   0        0        0      157 2024-04-28 15:25:58.827199 sim_rl-0.1.5/sim_rl/tuning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6466 2024-04-28 15:26:00.355144 sim_rl-0.1.5/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc
--rw-r--r--   0        0        0     5627 2024-04-28 15:25:58.831079 sim_rl-0.1.5/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc
--rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.5/sim_rl/tuning/ray_tuning.py
--rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.5/sim_rl/tuning/wandb_tuning.py
--rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.5/sim_rl/user_config/configuration.yml
--rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.5/sim_rl/user_config/eval_hyperparams.yml
--rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.5/sim_rl/user_config/tuning_hyperparams.yml
--rw-r--r--   0        0        0    14592 1970-01-01 00:00:00.000000 sim_rl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-04-28 20:07:57.596870 sim_rl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14279 2024-04-28 20:07:40.501513 sim_rl-0.1.6/README.md
+-rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.6/sim_rl/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.6/sim_rl/__init__.py
+-rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.6/sim_rl/agents/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:57.799129 sim_rl-0.1.6/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3593 2024-04-28 15:25:57.812081 sim_rl-0.1.6/sim_rl/agents/__pycache__/buffer.cpython-310.pyc
+-rw-r--r--   0        0        0    13843 2024-04-28 15:25:57.804520 sim_rl-0.1.6/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc
+-rw-r--r--   0        0        0     9252 2024-04-28 15:25:57.809029 sim_rl-0.1.6/sim_rl/agents/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.6/sim_rl/agents/buffer.py
+-rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.6/sim_rl/agents/ddpg_agent.py
+-rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.6/sim_rl/agents/model.py
+-rw-r--r--   0        0        0   282094 2024-04-28 15:26:02.560345 sim_rl-0.1.6/sim_rl/agents/trained_agent.pt
+-rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.6/sim_rl/agents/trained_ddpg_agent.pt
+-rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.6/sim_rl/debug.py
+-rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.6/sim_rl/dist/sim_rl-0.1.0.tar.gz
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.6/sim_rl/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.6/sim_rl/evaluation/convergence_evaluation/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.6/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
+-rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.6/sim_rl/evaluation/convergence_evaluation/reward_plot.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.6/sim_rl/evaluation/decision_evaluation/__init__.py
+-rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.6/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
+-rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.6/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.6/sim_rl/evaluation/noise_evaluation/__init__.py
+-rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.6/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.6/sim_rl/evaluation/robustness_evaluation/__init__.py
+-rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.6/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/__init__.py
+-rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot.png
+-rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
+-rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
+-rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
+-rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
+-rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.6/sim_rl/foundations/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-28 15:25:54.662508 sim_rl-0.1.6/sim_rl/foundations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    31515 2024-04-28 15:25:54.670219 sim_rl-0.1.6/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc
+-rw-r--r--   0        0        0    10353 2024-04-28 15:25:58.846613 sim_rl-0.1.6/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/__init__.py
+-rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
+-rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
+-rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
+-rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
+-rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
+-rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
+-rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
+-rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
+-rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.6/sim_rl/foundations/core_functions.py
+-rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.6/sim_rl/foundations/core_plotting.py
+-rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.6/sim_rl/foundations/output_csv/action_dict.csv
+-rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.6/sim_rl/foundations/output_csv/actor_loss.csv
+-rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.6/sim_rl/foundations/output_csv/critic_loss.csv
+-rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.6/sim_rl/foundations/output_csv/next_state_model_loss.csv
+-rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.6/sim_rl/foundations/output_csv/reward_dict.json
+-rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.6/sim_rl/foundations/output_csv/reward_model_loss.csv
+-rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.6/sim_rl/foundations/output_csv/transition_proba.csv
+-rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.6/sim_rl/main.py
+-rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.6/sim_rl/Makefile
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.6/sim_rl/queue_env/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-28 15:25:57.816084 sim_rl-0.1.6/sim_rl/queue_env/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9916 2024-04-28 15:25:58.842612 sim_rl-0.1.6/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     5432 2024-04-28 15:25:57.819081 sim_rl-0.1.6/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc
+-rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.6/sim_rl/queue_env/queue_base_functions.py
+-rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
+-rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.gitignore
+-rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.readthedocs.yml
+-rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/CHANGELOG.md
+-rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/CITATION.cff
+-rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/cliff.toml
+-rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
+-rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
+-rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
+-rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
+-rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
+-rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
+-rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
+-rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
+-rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
+-rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
+-rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
+-rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
+-rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/conf.py
+-rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/current_state.png
+-rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/current_state1.png
+-rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
+-rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
+-rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/fig.png
+-rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/graph.rst
+-rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/index.rst
+-rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/installation.rst
+-rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/make.bat
+-rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/Makefile
+-rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/modules.rst
+-rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/my_network.png
+-rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/my_network1.png
+-rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/network.rst
+-rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/overview.rst
+-rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/queues.rst
+-rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/requirements.txt
+-rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/sim.png
+-rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/sim1.png
+-rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/store.png
+-rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/store1.png
+-rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
+-rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/LICENSE.txt
+-rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/MANIFEST.in
+-rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/poetry.lock
+-rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
+-rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
+-rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
+-rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
+-rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
+-rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
+-rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
+-rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
+-rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
+-rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
+-rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
+-rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
+-rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
+-rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
+-rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
+-rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
+-rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/README.rst
+-rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/setup.py
+-rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
+-rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
+-rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
+-rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_network.py
+-rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
+-rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
+-rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
+-rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.6/sim_rl/queue_env/queueing_network.py
+-rw-r--r--   0        0        0      191 2024-04-28 17:02:38.117430 sim_rl-0.1.6/sim_rl/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.6/sim_rl/rl_env/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:58.834087 sim_rl-0.1.6/sim_rl/rl_env/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    14513 2024-04-28 15:25:58.838089 sim_rl-0.1.6/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc
+-rw-r--r--   0        0        0    16235 2024-04-28 17:01:26.321399 sim_rl-0.1.6/sim_rl/rl_env/RL_Environment.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.6/sim_rl/tuning/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-28 15:25:58.827199 sim_rl-0.1.6/sim_rl/tuning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6466 2024-04-28 15:26:00.355144 sim_rl-0.1.6/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc
+-rw-r--r--   0        0        0     5627 2024-04-28 15:25:58.831079 sim_rl-0.1.6/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc
+-rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.6/sim_rl/tuning/ray_tuning.py
+-rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.6/sim_rl/tuning/wandb_tuning.py
+-rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.6/sim_rl/user_config/configuration.yml
+-rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.6/sim_rl/user_config/eval_hyperparams.yml
+-rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.6/sim_rl/user_config/tuning_hyperparams.yml
+-rw-r--r--   0        0        0    14697 1970-01-01 00:00:00.000000 sim_rl-0.1.6/PKG-INFO
```

### Comparing `sim_rl-0.1.5/pyproject.toml` & `sim_rl-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sim_rl"
-version = "0.1.5"
+version = "0.1.6"
 description = "Simulation Driven RL Package Utilized to Optimize Queueing Systems"
 authors = ["Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi <fatima.al-ani23@imperial.ac.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 torch = "2.2.0"
```

### Comparing `sim_rl-0.1.5/README.md` & `sim_rl-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,848 +39,855 @@
 00000260: 742c 2077 6869 6368 2069 7320 706f 7274  t, which is port
 00000270: 6162 6c65 2061 6e64 2063 6f6d 7061 7469  able and compati
 00000280: 626c 6520 7769 7468 2064 6966 6665 7265  ble with differe
 00000290: 6e74 2061 6765 6e74 2074 7970 6573 2e0d  nt agent types..
 000002a0: 0a2d 2060 6665 6174 7572 6573 603a 2049  .- `features`: I
 000002b0: 6e63 6c75 6465 7320 7365 7665 7261 6c20  ncludes several 
 000002c0: 7574 696c 6974 7920 6665 6174 7572 6573  utility features
-000002d0: 3a0d 0a20 202d 202a 2a42 7265 616b 646f  :..  - **Breakdo
-000002e0: 776e 2045 7870 6c6f 7261 7469 6f6e 2a2a  wn Exploration**
-000002f0: 3a20 4578 706c 6f72 6573 206b 6579 2073  : Explores key s
-00000300: 7461 7465 7320 7665 7273 7573 2070 6572  tates versus per
-00000310: 6970 6865 7261 6c20 7374 6174 6573 0d0a  ipheral states..
-00000320: 2020 2d20 2a2a 426c 6f63 6b61 6765 2044    - **Blockage D
-00000330: 656d 6f6e 7374 7261 7469 6f6e 2a2a 3a20  emonstration**: 
-00000340: 4465 6d6f 6e73 7472 6174 6573 2068 6f77  Demonstrates how
-00000350: 2074 6865 2061 6765 6e74 2072 6573 706f   the agent respo
-00000360: 6e64 7320 746f 2061 2073 6572 7665 7220  nds to a server 
-00000370: 6f75 7461 6765 2062 7920 6164 6a75 7374  outage by adjust
-00000380: 696e 6720 726f 7574 696e 6720 7072 6f62  ing routing prob
-00000390: 6162 696c 6974 6965 732e 0d0a 2020 2d20  abilities...  - 
-000003a0: 2a2a 436f 6e66 6964 656e 6365 2045 7661  **Confidence Eva
-000003b0: 6c75 6174 696f 6e2a 2a3a 2041 7373 6573  luation**: Asses
-000003c0: 7365 7320 7468 6520 7374 6162 696c 6974  ses the stabilit
-000003d0: 7920 616e 6420 7265 6c69 6162 696c 6974  y and reliabilit
-000003e0: 7920 6f66 2074 6865 2061 6765 6e74 2061  y of the agent a
-000003f0: 6372 6f73 7320 6469 6666 6572 656e 7420  cross different 
-00000400: 7472 6169 6e69 6e67 2073 6574 7570 730d  training setups.
-00000410: 0a20 202d 202a 2a4e 6f69 7365 2045 7661  .  - **Noise Eva
-00000420: 6c75 6174 696f 6e2a 2a3a 2045 7661 6c75  luation**: Evalu
-00000430: 6174 6520 7468 6520 6566 6665 6374 206f  ate the effect o
-00000440: 6620 656e 7669 726f 6e6d 656e 7461 6c20  f environmental 
-00000450: 6e6f 6973 6520 6f6e 2074 6865 2070 6572  noise on the per
-00000460: 666f 726d 616e 6365 206f 6620 7468 6520  formance of the 
-00000470: 6167 656e 740d 0a20 202d 202a 2a53 7461  agent..  - **Sta
-00000480: 7274 7570 2042 6568 6176 696f 7220 5669  rtup Behavior Vi
-00000490: 7375 616c 697a 6174 696f 6e2a 2a3a 2049  sualization**: I
-000004a0: 6465 6e74 6966 6965 7320 7468 6520 6275  dentifies the bu
-000004b0: 726e 2d69 6e20 7065 7269 6f64 206f 6620  rn-in period of 
-000004c0: 7468 6520 6167 656e 740d 0a20 202d 202a  the agent..  - *
-000004d0: 2a52 6f62 7573 746e 6573 7320 4576 616c  *Robustness Eval
-000004e0: 7561 7469 6f6e 2a2a 3a20 4173 7365 7373  uation**: Assess
-000004f0: 2072 6f62 7573 746e 6573 7320 6f66 2064   robustness of d
-00000500: 6563 6973 696f 6e73 2061 6372 6f73 7320  ecisions across 
-00000510: 6d75 6c74 6970 6c65 2074 7261 696e 6564  multiple trained
-00000520: 2061 6765 6e74 730d 0a0d 0a23 2320 5072   agents....## Pr
-00000530: 6572 6571 7569 7369 7465 730d 0a0d 0a42  erequisites....B
-00000540: 6566 6f72 6520 7275 6e6e 696e 6720 7468  efore running th
-00000550: 6520 7369 6d75 6c61 7469 6f6e 732c 2065  e simulations, e
-00000560: 6e73 7572 6520 796f 7520 6861 7665 2074  nsure you have t
-00000570: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e73  he following ins
-00000580: 7461 6c6c 6564 3a0d 0a2d 2050 7974 686f  talled:..- Pytho
-00000590: 6e20 3e3d 332e 3130 203c 332e 3131 0d0a  n >=3.10 <3.11..
-000005a0: 2d20 5079 546f 7263 6820 312e 372b 0d0a  - PyTorch 1.7+..
-000005b0: 2d20 4e75 6d50 790d 0a2d 2050 616e 6461  - NumPy..- Panda
-000005c0: 730d 0a2d 204d 6174 706c 6f74 6c69 620d  s..- Matplotlib.
-000005d0: 0a2d 2071 7565 7565 696e 672d 746f 6f6c  .- queueing-tool
-000005e0: 0d0a 2d20 7761 6e64 620d 0a2d 2052 6179  ..- wandb..- Ray
-000005f0: 0d0a 0d0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
-00000600: 696f 6e0d 0a0d 0a43 6c6f 6e65 2074 6865  ion....Clone the
-00000610: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-00000620: 696e 7374 616c 6c20 7468 6520 7265 7175  install the requ
-00000630: 6972 6564 2064 6570 656e 6465 6e63 6965  ired dependencie
-00000640: 733a 0d0a 0d0a 6060 6062 6173 680d 0a67  s:....```bash..g
-00000650: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00000660: 2f67 6974 6c61 622e 646f 632e 6963 2e61  /gitlab.doc.ic.a
-00000670: 632e 756b 2f6a 7739 3233 2f4d 5363 4461  c.uk/jw923/MScDa
-00000680: 7461 5370 6172 7150 726f 6a65 6374 2e67  taSparqProject.g
-00000690: 6974 0d0a 6364 204d 5363 4461 7461 5370  it..cd MScDataSp
-000006a0: 6172 7150 726f 6a65 6374 0d0a 7069 7020  arqProject..pip 
-000006b0: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-000006c0: 7265 6d65 6e74 732e 7478 740d 0a60 6060  rements.txt..```
-000006d0: 0d0a 0d0a 2323 2053 7465 7020 313a 2043  ....## Step 1: C
-000006e0: 6f6e 6669 6775 7261 7469 6f6e 0d0a 0d0a  onfiguration....
-000006f0: 2323 2320 456e 7669 726f 6e6d 656e 7420  ### Environment 
-00000700: 5365 7475 700d 0a0d 0a23 2323 2320 2a2a  Setup....#### **
-00000710: 5175 6575 6569 6e67 2045 6e76 6972 6f6e  Queueing Environ
-00000720: 6d65 6e74 2043 6f6e 6669 6775 7261 7469  ment Configurati
-00000730: 6f6e 2a2a 0d0a 0d0a 5468 6520 7369 6d75  on**....The simu
-00000740: 6c61 7469 6f6e 2065 6e76 6972 6f6e 6d65  lation environme
-00000750: 6e74 2072 6571 7569 7265 7320 7468 6520  nt requires the 
-00000760: 666f 6c6c 6f77 696e 6720 7061 7261 6d65  following parame
-00000770: 7465 7273 2074 6f20 6265 2064 6566 696e  ters to be defin
-00000780: 6564 2069 6e20 7468 6520 6063 6f6e 6669  ed in the `confi
-00000790: 6775 7261 7469 6f6e 2e79 6d6c 602e 0d0a  guration.yml`...
-000007a0: 0d0a 2d20 6061 646a 6163 656e 745f 6c69  ..- `adjacent_li
-000007b0: 7374 603a 2041 2064 6963 7469 6f6e 6172  st`: A dictionar
-000007c0: 7920 6465 6669 6e69 6e67 2074 6865 2061  y defining the a
-000007d0: 646a 6163 656e 6379 206c 6973 7420 666f  djacency list fo
-000007e0: 7220 7468 6520 6e65 7477 6f72 6b20 746f  r the network to
-000007f0: 706f 6c6f 6779 2e0d 0a2d 2060 6d69 755f  pology...- `miu_
-00000800: 6469 6374 603a 2041 2064 6963 7469 6f6e  dict`: A diction
-00000810: 6172 7920 6f66 2073 6572 7669 6365 2072  ary of service r
-00000820: 6174 6573 2066 6f72 2065 6163 6820 7365  ates for each se
-00000830: 7276 6963 6520 6e6f 6465 2069 6e20 7468  rvice node in th
-00000840: 6520 6e65 7477 6f72 6b2e 0d0a 2d20 6074  e network...- `t
-00000850: 7261 6e73 6974 696f 6e5f 7072 6f62 615f  ransition_proba_
-00000860: 616c 6c60 3a20 4120 6469 6374 696f 6e61  all`: A dictiona
-00000870: 7279 2064 6566 696e 696e 6720 7468 6520  ry defining the 
-00000880: 7472 616e 7369 7469 6f6e 2070 726f 6261  transition proba
-00000890: 6269 6c69 7469 6573 2062 6574 7765 656e  bilities between
-000008a0: 206e 6f64 6573 2e0d 0a2d 2060 6163 7469   nodes...- `acti
-000008b0: 7665 5f63 6170 603a 2054 6865 2061 6374  ve_cap`: The act
-000008c0: 6976 6520 6361 7061 6369 7479 206f 6620  ive capacity of 
-000008d0: 7468 6520 6e6f 6465 7320 6672 6f6d 206f  the nodes from o
-000008e0: 7574 7369 6465 2074 6865 206e 6574 776f  utside the netwo
-000008f0: 726b 2e0d 0a2d 2060 6465 6163 7469 7665  rk...- `deactive
-00000900: 5f74 603a 2054 6865 2064 6561 6374 6976  _t`: The deactiv
-00000910: 6174 696f 6e20 7468 7265 7368 6f6c 6420  ation threshold 
-00000920: 666f 7220 7468 6520 6e6f 6465 7320 6672  for the nodes fr
-00000930: 6f6d 206f 7574 7369 6465 2074 6865 206e  om outside the n
-00000940: 6574 776f 726b 2e0d 0a2d 2060 6275 6666  etwork...- `buff
-00000950: 6572 5f73 697a 655f 666f 725f 6561 6368  er_size_for_each
-00000960: 5f71 7565 7565 603a 2041 2064 6963 7469  _queue`: A dicti
-00000970: 6f6e 6172 7920 7468 6174 2064 6566 696e  onary that defin
-00000980: 6573 2074 6865 2062 7566 6665 7220 7369  es the buffer si
-00000990: 7a65 2066 6f72 2065 6163 6820 7175 6575  ze for each queu
-000009a0: 652e 0d0a 2d20 6061 7272 6976 616c 5f72  e...- `arrival_r
-000009b0: 6174 6560 3a20 4120 6c69 7374 2074 6861  ate`: A list tha
-000009c0: 7420 6465 6669 6e65 7320 7468 6520 6172  t defines the ar
-000009d0: 7269 7661 6c20 7261 7465 7320 666f 7220  rival rates for 
-000009e0: 616c 6c20 706f 7373 6962 6c65 2065 6e74  all possible ent
-000009f0: 7279 206e 6f64 6573 2e0d 0a2d 2060 6d61  ry nodes...- `ma
-00000a00: 785f 6167 656e 7473 603a 2041 2076 616c  x_agents`: A val
-00000a10: 7565 2074 6861 7420 6465 6669 6e65 7320  ue that defines 
-00000a20: 7468 6520 6d61 7869 6d75 6d20 6e75 6d62  the maximum numb
-00000a30: 6572 206f 6620 6167 656e 7473 2063 616e  er of agents can
-00000a40: 2062 6520 6163 6370 6574 6564 2066 726f   be accpeted fro
-00000a50: 6d20 6f75 7473 6964 6520 7468 6520 6e65  m outside the ne
-00000a60: 7477 6f72 6b20 666f 7220 7468 6520 656e  twork for the en
-00000a70: 7472 7920 6e6f 6465 732e 0d0a 2d20 6073  try nodes...- `s
-00000a80: 696d 5f6a 6f62 7360 3a20 4120 7661 6c75  im_jobs`: A valu
-00000a90: 6520 7468 6174 2064 6566 696e 6573 2074  e that defines t
-00000aa0: 6865 206e 756d 6265 7220 6f66 206a 6f62  he number of job
-00000ab0: 7320 6265 696e 6720 7369 6d75 6c61 7465  s being simulate
-00000ac0: 6420 6475 7269 6e67 2065 7665 7279 2073  d during every s
-00000ad0: 696d 756c 6174 696f 6e2e 0d0a 2d20 606d  imulation...- `m
-00000ae0: 6178 5f61 7272 5f72 6174 655f 6c69 7374  ax_arr_rate_list
-00000af0: 603a 2041 206c 6973 7420 7468 6174 2064  `: A list that d
-00000b00: 6566 696e 6573 2074 6865 206d 6178 696d  efines the maxim
-00000b10: 756d 2061 7272 6976 616c 2072 6174 6520  um arrival rate 
-00000b20: 666f 7220 616c 6c20 656e 7472 7920 7175  for all entry qu
-00000b30: 6575 6573 2e0d 0a2d 2060 656e 7472 795f  eues...- `entry_
-00000b40: 6e6f 6465 7360 3a20 4120 6c69 7374 2074  nodes`: A list t
-00000b50: 6861 7420 6465 6669 6e65 7320 7468 6520  hat defines the 
-00000b60: 736f 7572 6365 2061 6e64 2074 6172 6765  source and targe
-00000b70: 7420 7665 7274 6963 6573 206f 6620 6561  t vertices of ea
-00000b80: 6368 2065 6e74 7279 206e 6f64 652e 0d0a  ch entry node...
-00000b90: 0d0a 2020 2045 7861 6d70 6c65 3a0d 0a20  ..   Example:.. 
-00000ba0: 2020 6060 6079 616d 6c0d 0a20 2020 6d69    ```yaml..   mi
-00000bb0: 755f 6c69 7374 3a20 200d 0a20 2020 313a  u_list:  ..   1:
-00000bc0: 2030 2e32 3530 0d0a 2020 2032 3a20 302e   0.250..   2: 0.
-00000bd0: 3235 0d0a 2020 2033 3a20 302e 3031 3530  25..   3: 0.0150
-00000be0: 300d 0a20 2020 343a 2031 3030 0d0a 2020  0..   4: 100..  
-00000bf0: 2035 3a20 312e 3230 0d0a 2020 2036 3a20   5: 1.20..   6: 
-00000c00: 302e 3031 3030 300d 0a20 2020 373a 2031  0.01000..   7: 1
-00000c10: 300d 0a20 2020 383a 2030 2e31 3030 300d  0..   8: 0.1000.
-00000c20: 0a20 2020 393a 2030 2e35 3030 0d0a 0d0a  .   9: 0.500....
-00000c30: 2020 2061 646a 6163 656e 745f 6c69 7374     adjacent_list
-00000c40: 3a0d 0a20 2020 303a 205b 315d 0d0a 2020  :..   0: [1]..  
-00000c50: 2031 3a20 5b32 2c20 332c 2034 5d0d 0a20   1: [2, 3, 4].. 
-00000c60: 2020 323a 205b 355d 0d0a 2020 2033 3a20    2: [5]..   3: 
-00000c70: 5b36 2c20 375d 0d0a 2020 2034 3a20 5b38  [6, 7]..   4: [8
-00000c80: 5d0d 0a20 2020 353a 205b 395d 0d0a 2020  ]..   5: [9]..  
-00000c90: 2036 3a20 5b39 5d0d 0a20 2020 373a 205b   6: [9]..   7: [
-00000ca0: 395d 0d0a 2020 2038 3a20 5b39 5d0d 0a20  9]..   8: [9].. 
-00000cb0: 2020 393a 205b 3130 5d0d 0a0d 0a20 2020    9: [10]....   
-00000cc0: 6275 6666 6572 5f73 697a 655f 666f 725f  buffer_size_for_
-00000cd0: 6561 6368 5f71 7565 7565 3a20 0d0a 2020  each_queue: ..  
-00000ce0: 2030 3a20 3530 3030 0d0a 2020 2031 3a20   0: 5000..   1: 
-00000cf0: 3530 3030 0d0a 2020 2032 3a20 3530 3030  5000..   2: 5000
-00000d00: 0d0a 2020 2033 3a20 3530 3030 0d0a 2020  ..   3: 5000..  
-00000d10: 2034 3a20 3530 3030 0d0a 2020 2035 3a20   4: 5000..   5: 
-00000d20: 3530 3030 0d0a 2020 2036 3a20 3530 3030  5000..   6: 5000
-00000d30: 0d0a 2020 2037 3a20 3530 3030 0d0a 2020  ..   7: 5000..  
-00000d40: 2038 3a20 3530 3030 0d0a 2020 2039 3a20   8: 5000..   9: 
-00000d50: 3530 3030 0d0a 2020 2031 303a 2035 3030  5000..   10: 500
-00000d60: 300d 0a20 2020 3131 3a20 3530 3030 0d0a  0..   11: 5000..
-00000d70: 2020 2031 323a 2035 3030 300d 0a0d 0a20     12: 5000.... 
-00000d80: 2020 7472 616e 7369 7469 6f6e 5f70 726f    transition_pro
-00000d90: 6261 5f61 6c6c 3a0d 0a20 2020 303a 207b  ba_all:..   0: {
-00000da0: 313a 2031 7d0d 0a20 2020 313a 207b 323a  1: 1}..   1: {2:
-00000db0: 2030 2e33 332c 2033 3a20 302e 3333 2c20   0.33, 3: 0.33, 
-00000dc0: 343a 2030 2e33 347d 0d0a 2020 2032 3a20  4: 0.34}..   2: 
-00000dd0: 7b35 3a20 317d 0d0a 2020 2033 3a20 7b36  {5: 1}..   3: {6
-00000de0: 3a20 302e 352c 2037 3a20 302e 357d 0d0a  : 0.5, 7: 0.5}..
-00000df0: 2020 2034 3a20 7b38 3a20 317d 0d0a 2020     4: {8: 1}..  
-00000e00: 2035 3a20 7b39 3a20 317d 0d0a 2020 2036   5: {9: 1}..   6
-00000e10: 3a20 7b39 3a20 317d 0d0a 2020 2037 3a20  : {9: 1}..   7: 
-00000e20: 7b39 3a20 317d 0d0a 2020 2038 3a20 7b39  {9: 1}..   8: {9
-00000e30: 3a20 317d 0d0a 2020 2039 3a20 7b31 303a  : 1}..   9: {10:
-00000e40: 2031 7d0d 0a20 2020 0d0a 2020 2061 6374   1}..   ..   act
-00000e50: 6976 655f 6361 703a 2035 0d0a 0d0a 2020  ive_cap: 5....  
-00000e60: 2064 6561 6374 6976 655f 743a 2030 2e31   deactive_t: 0.1
-00000e70: 320d 0a0d 0a20 2020 6172 7269 7661 6c5f  2....   arrival_
-00000e80: 7261 7465 3a20 5b30 2e33 5d0d 0a0d 0a20  rate: [0.3].... 
-00000e90: 2020 6d61 785f 6167 656e 7473 3a20 696e    max_agents: in
-00000ea0: 660d 0a0d 0a20 2020 7369 6d5f 6a6f 6273  f....   sim_jobs
-00000eb0: 3a20 3130 300d 0a0d 0a20 2020 6d61 785f  : 100....   max_
-00000ec0: 6172 725f 7261 7465 5f6c 6973 743a 205b  arr_rate_list: [
-00000ed0: 3337 352c 2033 3735 2c20 3337 355d 0d0a  375, 375, 375]..
-00000ee0: 0d0a 2020 2065 6e74 7279 5f6e 6f64 6573  ..   entry_nodes
-00000ef0: 3a0d 0a20 2020 2d20 5b30 2c20 315d 200d  :..   - [0, 1] .
-00000f00: 0a20 2020 6060 600d 0a0d 0a23 2323 2320  .   ```....#### 
-00000f10: 2a2a 524c 2045 6e76 6972 6f6e 6d65 6e74  **RL Environment
-00000f20: 2050 6172 616d 6574 6572 732a 2a0d 0a0d   Parameters**...
-00000f30: 0a53 6574 2075 7020 7468 6520 524c 2065  .Set up the RL e
-00000f40: 6e76 6972 6f6e 6d65 6e74 2070 6172 616d  nvironment param
-00000f50: 6574 6572 7320 696e 2060 6576 616c 5f68  eters in `eval_h
-00000f60: 7970 6572 7061 7261 6d73 2e79 6d6c 603a  yperparams.yml`:
-00000f70: 0d0a 0d0a 2d20 606e 756d 5f65 7069 736f  ....- `num_episo
-00000f80: 6465 7360 3a20 5468 6520 6e75 6d62 6572  des`: The number
-00000f90: 206f 6620 6570 6973 6f64 6573 2074 6f20   of episodes to 
-00000fa0: 7275 6e20 7468 6520 7369 6d75 6c61 7469  run the simulati
-00000fb0: 6f6e 2e0d 0a2d 2060 6e75 6d5f 6570 6f63  on...- `num_epoc
-00000fc0: 6873 603a 2054 6865 206e 756d 6265 7220  hs`: The number 
-00000fd0: 6f66 2065 706f 6368 7320 666f 7220 7472  of epochs for tr
-00000fe0: 6169 6e69 6e67 2e0d 0a2d 2060 7469 6d65  aining...- `time
-00000ff0: 5f73 7465 7073 603a 2054 6865 206e 756d  _steps`: The num
-00001000: 6265 7220 6f66 2074 696d 6520 7374 6570  ber of time step
-00001010: 7320 696e 2065 6163 6820 6570 6973 6f64  s in each episod
-00001020: 652e 0d0a 2d20 6062 6174 6368 5f73 697a  e...- `batch_siz
-00001030: 6560 3a20 5369 7a65 206f 6620 7468 6520  e`: Size of the 
-00001040: 6261 7463 6820 7573 6564 2069 6e20 7472  batch used in tr
-00001050: 6169 6e69 6e67 2e20 2844 6566 6175 6c74  aining. (Default
-00001060: 2069 7320 6571 7561 6c20 746f 2074 696d   is equal to tim
-00001070: 655f 7374 6570 7329 0d0a 2d20 606e 756d  e_steps)..- `num
-00001080: 5f73 696d 603a 2054 6865 206e 756d 6265  _sim`: The numbe
-00001090: 7220 6f66 2073 696d 756c 6174 696f 6e73  r of simulations
-000010a0: 2074 6f20 7275 6e20 6475 7269 6e67 2074   to run during t
-000010b0: 7261 696e 696e 672e 0d0a 2d20 6074 6175  raining...- `tau
-000010c0: 603a 2043 6f65 6666 6963 6965 6e74 2066  `: Coefficient f
-000010d0: 6f72 2073 6f66 7420 7570 6461 7465 206f  or soft update o
-000010e0: 6620 7468 6520 7461 7267 6574 2070 6172  f the target par
-000010f0: 616d 6574 6572 732e 0d0a 2d20 6061 6374  ameters...- `act
-00001100: 6f72 5f6c 7260 3a20 4c65 6172 6e69 6e67  or_lr`: Learning
-00001110: 2072 6174 6520 666f 7220 7468 6520 4163   rate for the Ac
-00001120: 746f 7220 6e65 7477 6f72 6b20 6f70 7469  tor network opti
-00001130: 6d69 7a65 722e 0d0a 2d20 6063 7269 7469  mizer...- `criti
-00001140: 635f 6c72 603a 204c 6561 726e 696e 6720  c_lr`: Learning 
-00001150: 7261 7465 2066 6f72 2074 6865 2043 7269  rate for the Cri
-00001160: 7469 6320 4e65 7477 6f72 6b20 6f70 7469  tic Network opti
-00001170: 6d69 7a65 722e 0d0a 2d20 6064 6973 636f  mizer...- `disco
-00001180: 756e 7460 3a20 4469 7363 6f75 6e74 2066  unt`: Discount f
-00001190: 6163 746f 7220 666f 7220 6675 7475 7265  actor for future
-000011a0: 2072 6577 6172 6473 2e0d 0a2d 2060 706c   rewards...- `pl
-000011b0: 616e 6e69 6e67 5f73 7465 7073 603a 2054  anning_steps`: T
-000011c0: 6865 206e 756d 6265 7220 6f66 2073 7465  he number of ste
-000011d0: 7073 2064 7572 696e 6720 706c 616e 6e69  ps during planni
-000011e0: 6e67 2e0d 0a2d 2060 706c 616e 6e69 6e67  ng...- `planning
-000011f0: 5f73 7464 603a 2053 7461 6e64 6172 6420  _std`: Standard 
-00001200: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
-00001210: 206e 6f72 6d61 6c20 6469 7374 7572 6261   normal disturba
-00001220: 6e63 6520 6475 7269 6e67 2070 6c61 6e6e  nce during plann
-00001230: 696e 672e 0d0a 2d20 6061 6374 6f72 5f6e  ing...- `actor_n
-00001240: 6574 776f 726b 603a 204e 6574 776f 726b  etwork`: Network
-00001250: 2061 7263 6869 7465 6374 7572 6520 666f   architecture fo
-00001260: 7220 6163 746f 7220 6e65 7477 6f72 6b2e  r actor network.
-00001270: 0d0a 2d20 6063 7269 7469 635f 6e65 7477  ..- `critic_netw
-00001280: 6f72 6b60 3a20 4e65 7477 6f72 6b20 6172  ork`: Network ar
-00001290: 6368 6974 6563 7475 7265 2066 6f72 2063  chitecture for c
-000012a0: 7269 7469 6320 6e65 7477 6f72 6b2e 0d0a  ritic network...
-000012b0: 2d20 6072 6577 6172 645f 6d6f 6465 6c60  - `reward_model`
-000012c0: 3a20 4e65 7477 6f72 6b20 6172 6368 6974  : Network archit
-000012d0: 6563 7475 7265 2066 6f72 2072 6577 6172  ecture for rewar
-000012e0: 6420 6d6f 6465 6c20 7573 6420 696e 2070  d model usd in p
-000012f0: 6c61 6e6e 696e 672e 0d0a 6020 606e 6578  lanning...` `nex
-00001300: 745f 7374 6174 655f 6d6f 6465 6c60 3a20  t_state_model`: 
-00001310: 4e65 7477 6f72 6b20 6172 6368 6974 6563  Network architec
-00001320: 7475 7265 2066 6f72 206e 6578 7420 7374  ture for next st
-00001330: 6174 6520 6d6f 6465 6c20 7573 6564 2069  ate model used i
-00001340: 6e20 706c 616e 6e69 6e67 2e20 0d0a 0d0a  n planning. ....
-00001350: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
-00001360: 6060 6079 616d 6c0d 0a20 2020 6e75 6d5f  ```yaml..   num_
-00001370: 6570 6973 6f64 6573 3a20 350d 0a0d 0a20  episodes: 5.... 
-00001380: 2020 7468 7265 7368 6f6c 643a 2031 300d    threshold: 10.
-00001390: 0a0d 0a20 2020 6e75 6d5f 6570 6f63 6873  ...   num_epochs
-000013a0: 3a20 3130 300d 0a0d 0a20 2020 7469 6d65  : 100....   time
-000013b0: 5f73 7465 7073 3a20 3330 0d0a 0d0a 2020  _steps: 30....  
-000013c0: 2062 6174 6368 5f73 697a 653a 2033 300d   batch_size: 30.
-000013d0: 0a20 2020 0d0a 2020 2074 6172 6765 745f  .   ..   target_
-000013e0: 7570 6461 7465 5f66 7265 7175 656e 6379  update_frequency
-000013f0: 3a20 3130 300d 0a20 2020 0d0a 2020 2062  : 100..   ..   b
-00001400: 7566 6665 725f 7369 7a65 3a20 3130 3030  uffer_size: 1000
-00001410: 300d 0a20 2020 0d0a 2020 206e 756d 5f73  0..   ..   num_s
-00001420: 696d 3a20 3130 0d0a 2020 200d 0a20 2020  im: 10..   ..   
-00001430: 7461 753a 2030 2e35 0d0a 0d0a 2020 206e  tau: 0.5....   n
-00001440: 756d 5f74 7261 696e 5f41 433a 2031 300d  um_train_AC: 10.
-00001450: 0a20 2020 0d0a 2020 2063 7269 7469 635f  .   ..   critic_
-00001460: 6c72 3a20 302e 3031 0d0a 0d0a 2020 2061  lr: 0.01....   a
-00001470: 6374 6f72 5f6c 723a 2030 2e30 3030 310d  ctor_lr: 0.0001.
-00001480: 0a20 2020 0d0a 2020 2064 6973 636f 756e  .   ..   discoun
-00001490: 743a 2030 2e38 0d0a 2020 200d 0a20 2020  t: 0.8..   ..   
-000014a0: 706c 616e 6e69 6e67 5f73 7465 7073 3a20  planning_steps: 
-000014b0: 3130 0d0a 2020 200d 0a20 2020 706c 616e  10..   ..   plan
-000014c0: 6e69 6e67 5f73 7464 3a20 302e 310d 0a0d  ning_std: 0.1...
-000014d0: 0a20 2020 6163 746f 725f 6e65 7477 6f72  .   actor_networ
-000014e0: 6b3a 0d0a 2020 202d 2036 340d 0a20 2020  k:..   - 64..   
-000014f0: 2d20 3634 0d0a 2020 202d 2036 340d 0a0d  - 64..   - 64...
-00001500: 0a20 2020 6372 6974 6963 3a0d 0a20 2020  .   critic:..   
-00001510: 2d20 3634 0d0a 2020 202d 2036 340d 0a20  - 64..   - 64.. 
-00001520: 2020 2d20 3634 0d0a 0d0a 2020 2072 6577    - 64....   rew
-00001530: 6172 645f 6d6f 6465 6c3a 0d0a 2020 202d  ard_model:..   -
-00001540: 2033 320d 0a20 2020 2d20 3634 0d0a 2020   32..   - 64..  
-00001550: 202d 2036 340d 0a20 2020 2d20 3332 0d0a   - 64..   - 32..
-00001560: 0d0a 2020 206e 6578 745f 7374 6174 655f  ..   next_state_
-00001570: 6d6f 6465 6c3a 0d0a 2020 202d 2033 320d  model:..   - 32.
-00001580: 0a20 2020 2d20 3634 0d0a 2020 202d 2036  .   - 64..   - 6
-00001590: 340d 0a20 2020 2d20 3332 0d0a 2020 2060  4..   - 32..   `
-000015a0: 6060 0d0a 0d0a 2323 2323 202a 2a54 756e  ``....#### **Tun
-000015b0: 696e 6720 436f 6e66 6967 7572 6174 696f  ing Configuratio
-000015c0: 6e2a 2a0d 0a53 6574 2075 7020 7468 6520  n**..Set up the 
-000015d0: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
-000015e0: 756e 696e 6720 7261 6e67 6573 2069 6e20  uning ranges in 
-000015f0: 6074 756e 696e 675f 7061 7261 6d73 2e79  `tuning_params.y
-00001600: 6d6c 603a 0d0a 0d0a 2d20 606c 725f 6d69  ml`:....- `lr_mi
-00001610: 6e2f 6d61 7860 3a20 4d69 6e20 616e 6420  n/max`: Min and 
-00001620: 6d61 7820 7261 6e67 6573 206f 6620 7468  max ranges of th
-00001630: 6520 6c65 6172 6e69 6e67 2072 6174 6520  e learning rate 
-00001640: 6265 696e 6720 7475 6e65 642e 0d0a 2d20  being tuned...- 
-00001650: 6065 706f 6368 735f 6c69 7374 603a 2041  `epochs_list`: A
-00001660: 206c 6973 7420 7468 6174 2064 6566 696e   list that defin
-00001670: 6573 2074 6865 2072 616e 6765 206f 6620  es the range of 
-00001680: 706f 7373 6962 6c65 2065 706f 6368 7320  possible epochs 
-00001690: 746f 2074 7261 696e 2072 6577 6172 6420  to train reward 
-000016a0: 6d6f 6465 6c20 616e 6420 6e65 7874 2073  model and next s
-000016b0: 7461 7465 206d 6f64 656c 2e0d 0a2d 2060  tate model...- `
-000016c0: 6261 7463 685f 7369 7a65 603a 2041 206c  batch_size`: A l
-000016d0: 6973 7420 7468 6174 2064 6566 696e 6573  ist that defines
-000016e0: 2074 6865 2072 616e 6765 206f 6620 6261   the range of ba
-000016f0: 7463 6820 7369 7a65 7320 746f 2073 616d  tch sizes to sam
-00001700: 706c 6520 6672 6f6d 2074 6865 2072 6570  ple from the rep
-00001710: 6c61 7920 6275 6666 6572 2e0d 0a2d 2060  lay buffer...- `
-00001720: 7461 755f 6d69 6e2f 6d61 7860 3a20 4d69  tau_min/max`: Mi
-00001730: 6e20 616e 6420 6d61 7820 7261 6e67 6573  n and max ranges
-00001740: 206f 6620 7468 6520 736f 6674 2075 7064   of the soft upd
-00001750: 6174 6520 7061 7261 6d65 7465 7273 2e0d  ate parameters..
-00001760: 0a2d 2060 6469 7363 6f75 6e74 206d 696e  .- `discount min
-00001770: 2f6d 6178 603a 204d 696e 2061 6e64 206d  /max`: Min and m
-00001780: 6178 2072 616e 6765 7320 6f66 2074 6865  ax ranges of the
-00001790: 2064 6973 636f 756e 7420 6661 6374 6f72   discount factor
-000017a0: 2066 6f72 2066 7574 7572 6520 7265 7761   for future rewa
-000017b0: 7264 732e 0d0a 2d20 6065 7073 696c 6f6e  rds...- `epsilon
-000017c0: 5f6d 696e 2f6d 6178 603a 204d 696e 2061  _min/max`: Min a
-000017d0: 6e64 206d 6178 2072 616e 6765 7320 6f66  nd max ranges of
-000017e0: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-000017f0: 7669 6174 696f 6e20 6f66 206e 6f72 6d61  viation of norma
-00001800: 6c20 6469 7374 7572 6261 6e63 6573 2064  l disturbances d
-00001810: 7572 696e 6720 706c 616e 6e69 6e67 2e0d  uring planning..
-00001820: 0a2d 2060 706c 616e 6e69 6e67 5f73 7465  .- `planning_ste
-00001830: 7073 603a 2041 206c 6973 7420 7468 6174  ps`: A list that
-00001840: 2064 6566 696e 6573 2070 6f73 7369 626c   defines possibl
-00001850: 6520 7374 6570 7320 666f 7220 706c 616e  e steps for plan
-00001860: 6e69 6e67 2e0d 0a2d 2060 7731 2f77 3260  ning...- `w1/w2`
-00001870: 3a20 5765 6967 6874 2070 6172 616d 6574  : Weight paramet
-00001880: 6572 7320 7468 6174 2069 6e66 6c75 656e  ers that influen
-00001890: 6365 2074 6865 2065 7870 6c6f 7261 7469  ce the explorati
-000018a0: 6f6e 2062 6574 7765 656e 206b 6579 2061  on between key a
-000018b0: 6e64 2070 6572 6970 6865 7261 6c20 7374  nd peripheral st
-000018c0: 6174 6573 2e0d 0a2d 2060 6e75 6d5f 6570  ates...- `num_ep
-000018d0: 6973 6f64 6573 603a 2041 206c 6973 7420  isodes`: A list 
-000018e0: 7468 6174 2064 6566 696e 6573 2074 6865  that defines the
-000018f0: 2070 6f73 7369 626c 6520 6e75 6d62 6572   possible number
-00001900: 7320 6f66 2065 7069 736f 6465 7320 746f  s of episodes to
-00001910: 2074 7261 696e 2074 6865 2061 6765 6e74   train the agent
-00001920: 732e 0d0a 2d20 6074 696d 655f 7374 6570  s...- `time_step
-00001930: 7360 3a20 4120 6c69 7374 2074 6861 7420  s`: A list that 
-00001940: 6465 6669 6e65 7320 7468 6520 706f 7373  defines the poss
-00001950: 6962 6c65 206e 756d 6265 7220 6f66 2074  ible number of t
-00001960: 696d 6520 7374 6570 7320 6475 7269 6e67  ime steps during
-00001970: 2065 6163 6820 6570 6973 6f64 650d 0a0d   each episode...
-00001980: 0a20 2020 4578 616d 706c 653a 0d0a 2020  .   Example:..  
-00001990: 2060 6060 7961 6d6c 0d0a 2020 206c 6561   ```yaml..   lea
-000019a0: 726e 696e 675f 7261 7465 5f6d 6178 3a20  rning_rate_max: 
-000019b0: 302e 310d 0a20 2020 6c65 6172 6e69 6e67  0.1..   learning
-000019c0: 5f72 6174 655f 6d69 6e3a 2030 2e30 3031  _rate_min: 0.001
-000019d0: 0d0a 0d0a 2020 2065 706f 6368 735f 6c69  ....   epochs_li
-000019e0: 7374 3a0d 0a20 2020 2d20 3130 0d0a 2020  st:..   - 10..  
-000019f0: 202d 2031 300d 0a20 2020 2d20 3130 0d0a   - 10..   - 10..
-00001a00: 0d0a 2020 2062 6174 6368 5f73 697a 653a  ..   batch_size:
-00001a10: 0d0a 2020 202d 2031 360d 0a20 2020 2d20  ..   - 16..   - 
-00001a20: 3332 0d0a 2020 202d 2036 340d 0a0d 0a20  32..   - 64.... 
-00001a30: 2020 7461 755f 6d69 6e3a 2030 2e30 3030    tau_min: 0.000
-00001a40: 350d 0a20 2020 7461 755f 6d61 783a 2030  5..   tau_max: 0
-00001a50: 2e30 3032 0d0a 0d0a 2020 2064 6973 636f  .002....   disco
-00001a60: 756e 745f 6d69 6e3a 2030 2e31 0d0a 2020  unt_min: 0.1..  
-00001a70: 2064 6973 636f 756e 745f 6d61 783a 2030   discount_max: 0
-00001a80: 2e33 0d0a 0d0a 2020 2065 7073 696c 6f6e  .3....   epsilon
-00001a90: 5f6d 696e 3a20 302e 310d 0a20 2020 6570  _min: 0.1..   ep
-00001aa0: 7369 6c6f 6e5f 6d61 783a 2030 2e33 0d0a  silon_max: 0.3..
-00001ab0: 0d0a 2020 2070 6c61 6e6e 696e 675f 7374  ..   planning_st
-00001ac0: 6570 733a 200d 0a20 2020 2d20 3130 0d0a  eps: ..   - 10..
-00001ad0: 0d0a 2020 206e 756d 5f73 616d 706c 653a  ..   num_sample:
-00001ae0: 200d 0a20 2020 2d20 3530 0d0a 0d0a 2020   ..   - 50....  
-00001af0: 2077 313a 200d 0a20 2020 2d20 302e 350d   w1: ..   - 0.5.
-00001b00: 0a0d 0a20 2020 7732 3a20 0d0a 2020 202d  ...   w2: ..   -
-00001b10: 2030 2e35 0d0a 0d0a 2020 206e 756d 5f65   0.5....   num_e
-00001b20: 7069 736f 6465 733a 200d 0a20 2020 2d20  pisodes: ..   - 
-00001b30: 350d 0a0d 0a20 2020 7469 6d65 5f73 7465  5....   time_ste
-00001b40: 7073 3a20 0d0a 2020 202d 2031 300d 0a20  ps: ..   - 10.. 
-00001b50: 2020 6060 600d 0a0d 0a23 2320 5374 6570    ```....## Step
-00001b60: 2032 3a20 5275 6e6e 696e 6720 5369 6d75   2: Running Simu
-00001b70: 6c61 7469 6f6e 730d 0a0d 0a23 2323 2054  lations....### T
-00001b80: 7261 696e 696e 6720 4167 656e 740d 0a54  raining Agent..T
-00001b90: 6869 7320 636f 6d6d 616e 6420 7374 6172  his command star
-00001ba0: 7473 2074 7261 696e 696e 6720 7468 6520  ts training the 
-00001bb0: 6167 656e 7420 7769 7468 696e 2074 6865  agent within the
-00001bc0: 2073 696d 756c 6174 6564 2071 7565 7565   simulated queue
-00001bd0: 696e 6720 656e 7669 726f 6e6d 656e 742e  ing environment.
-00001be0: 2052 6573 756c 7473 2061 7265 2073 6176   Results are sav
-00001bf0: 6564 2069 6e20 602f 666f 756e 6461 7469  ed in `/foundati
-00001c00: 6f6e 732f 6f75 7470 7574 5f63 7376 6020  ons/output_csv` 
-00001c10: 616e 6420 602f 666f 756e 6461 7469 6f6e  and `/foundation
-00001c20: 732f 6f75 7470 7574 5f70 6c6f 7473 602e  s/output_plots`.
-00001c30: 0d0a 0d0a 6060 6062 6173 680d 0a70 7974  ....```bash..pyt
-00001c40: 686f 6e20 6d61 696e 2e70 7920 2d2d 6675  hon main.py --fu
-00001c50: 6e63 7469 6f6e 2074 7261 696e 202d 2d63  nction train --c
-00001c60: 6f6e 6669 675f 6669 6c65 2075 7365 725f  onfig_file user_
-00001c70: 636f 6e66 6967 2f63 6f6e 6669 6775 7261  config/configura
-00001c80: 7469 6f6e 2e79 6d6c 202d 2d70 6172 616d  tion.yml --param
-00001c90: 5f66 696c 6520 7573 6572 5f63 6f6e 6669  _file user_confi
-00001ca0: 672f 6576 616c 5f68 7970 6572 7061 7261  g/eval_hyperpara
-00001cb0: 6d73 2e79 6d6c 202d 2d64 6174 615f 6669  ms.yml --data_fi
-00001cc0: 6c65 206f 7574 7075 745f 6373 7620 2d2d  le output_csv --
-00001cd0: 696d 6167 655f 6669 6c65 206f 7574 7075  image_file outpu
-00001ce0: 745f 706c 6f74 7320 2d2d 706c 6f74 5f63  t_plots --plot_c
-00001cf0: 7572 7665 7320 5472 7565 202d 2d73 6176  urves True --sav
-00001d00: 655f 6669 6c65 2054 7275 650d 0a60 6060  e_file True..```
-00001d10: 0d0a 0d0a 2323 2320 4879 7065 7270 6172  ....### Hyperpar
-00001d20: 616d 6574 6572 2054 756e 696e 670d 0a0d  ameter Tuning...
-00001d30: 0a42 656c 6f77 2070 726f 7669 6465 7320  .Below provides 
-00001d40: 7573 6572 7320 7477 6f20 7479 7065 7320  users two types 
-00001d50: 6f66 2074 756e 696e 6720 7374 7261 7465  of tuning strate
-00001d60: 6769 6573 2074 6861 7420 6665 6174 7572  gies that featur
-00001d70: 6520 6469 6666 6572 656e 7420 6675 6e63  e different func
-00001d80: 7469 6f6e 616c 6974 6965 732e 0d0a 0d0a  tionalities.....
-00001d90: 2323 2323 202a 2a57 616e 6462 2054 756e  #### **Wandb Tun
-00001da0: 696e 672a 2a0d 0a0d 0a41 206d 6163 6869  ing**....A machi
-00001db0: 6e65 206c 6561 726e 696e 6720 6465 7665  ne learning deve
-00001dc0: 6c6f 706d 656e 7420 706c 6174 666f 726d  lopment platform
-00001dd0: 2074 6861 7420 616c 6c6f 7773 2075 7365   that allows use
-00001de0: 7273 2074 6f20 7472 6163 6b20 616e 6420  rs to track and 
-00001df0: 7669 7375 616c 697a 6520 7661 726f 7520  visualize varou 
-00001e00: 6173 7065 6374 7320 6f66 2074 6865 6972  aspects of their
-00001e10: 206d 6f64 656c 2074 7261 696e 696e 6720   model training 
-00001e20: 7072 6f63 6573 7320 696e 2072 6561 6c2d  process in real-
-00001e30: 7469 6d65 2c20 696e 636c 7564 696e 6720  time, including 
-00001e40: 6c6f 7373 2061 6e64 2061 6363 7572 6163  loss and accurac
-00001e50: 7920 6368 6172 7473 2c20 7061 7261 6d65  y charts, parame
-00001e60: 7465 7220 6469 7374 7269 6275 7469 6f6e  ter distribution
-00001e70: 732c 2067 7261 6469 656e 7420 6869 7374  s, gradient hist
-00001e80: 6f67 7261 6d73 2061 6e64 2073 7973 7465  ograms and syste
-00001e90: 6d20 6d65 7472 6963 732e 2054 6f20 7275  m metrics. To ru
-00001ea0: 6e20 7761 6e64 623a 0d0a 0d0a 6060 6062  n wandb:....```b
-00001eb0: 6173 680d 0a70 7974 686f 6e20 6d61 696e  ash..python main
-00001ec0: 2e70 7920 2d2d 6675 6e63 7469 6f6e 2074  .py --function t
-00001ed0: 756e 6520 2d2d 636f 6e66 6967 5f66 696c  une --config_fil
-00001ee0: 6520 7573 6572 5f63 6f6e 6669 672f 636f  e user_config/co
-00001ef0: 6e66 6967 7572 6174 696f 6e2e 796d 6c20  nfiguration.yml 
-00001f00: 2d2d 7061 7261 6d5f 6669 6c65 2075 7365  --param_file use
-00001f10: 725f 636f 6e66 6967 2f65 7661 6c5f 6879  r_config/eval_hy
-00001f20: 7065 7270 6172 616d 732e 796d 6c20 2d2d  perparams.yml --
-00001f30: 6461 7461 5f66 696c 6520 6f75 7470 7574  data_file output
-00001f40: 5f63 7376 202d 2d69 6d61 6765 5f66 696c  _csv --image_fil
-00001f50: 6520 6f75 7470 7574 5f70 6c6f 7473 202d  e output_plots -
-00001f60: 2d70 6c6f 745f 6375 7276 6573 2054 7275  -plot_curves Tru
-00001f70: 6520 2d2d 7361 7665 5f66 696c 6520 5472  e --save_file Tr
-00001f80: 7565 202d 2d74 756e 6572 2077 616e 6462  ue --tuner wandb
-00001f90: 200d 0a60 6060 0d0a 0d0a 2323 2323 202a   ..```....#### *
-00001fa0: 2a52 6179 2054 756e 696e 672a 2a0d 0a0d  *Ray Tuning**...
-00001fb0: 0a41 6e20 696e 6475 7374 7279 2073 7461  .An industry sta
-00001fc0: 6e64 6172 6420 746f 6f6c 2066 6f72 2064  ndard tool for d
-00001fd0: 6973 7472 6962 7574 6564 2068 7970 6572  istributed hyper
-00001fe0: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
-00001ff0: 2077 6869 6368 2069 6e74 6567 7261 7465   which integrate
-00002000: 7320 7769 7468 2054 656e 736f 7242 6f61  s with TensorBoa
-00002010: 7264 2061 6e64 2065 7874 656e 7369 7665  rd and extensive
-00002020: 2061 6e61 6c79 7369 7320 6c69 6272 6172   analysis librar
-00002030: 6965 732e 2049 7420 616c 736f 2061 6c6c  ies. It also all
-00002040: 6f77 7320 7573 6572 7320 746f 206c 6576  ows users to lev
-00002050: 6572 6167 6520 6375 7474 696e 6720 6564  erage cutting ed
-00002060: 6765 206f 7074 696d 697a 6174 696f 6e20  ge optimization 
-00002070: 616c 676f 7269 7468 6d73 2061 7420 7363  algorithms at sc
-00002080: 616c 652c 2069 6e63 6c75 6469 6e67 2042  ale, including B
-00002090: 6179 6573 6961 6e20 4f70 7469 6d69 7a61  ayesian Optimiza
-000020a0: 7469 6f6e 2c20 506f 7075 6c61 7469 6f6e  tion, Population
-000020b0: 2042 6173 6564 2054 7261 696e 696e 6720   Based Training 
-000020c0: 616e 6420 4879 7065 7242 616e 642e 2054  and HyperBand. T
-000020d0: 6f20 7275 6e20 7261 7920 7475 6e69 6e67  o run ray tuning
-000020e0: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7079  :....```bash..py
-000020f0: 7468 6f6e 206d 6169 6e2e 7079 202d 2d66  thon main.py --f
-00002100: 756e 6374 696f 6e20 7475 6e65 202d 2d63  unction tune --c
-00002110: 6f6e 6669 675f 6669 6c65 2075 7365 725f  onfig_file user_
-00002120: 636f 6e66 6967 2f63 6f6e 6669 6775 7261  config/configura
-00002130: 7469 6f6e 2e79 6d6c 202d 2d70 6172 616d  tion.yml --param
-00002140: 5f66 696c 6520 7573 6572 5f63 6f6e 6669  _file user_confi
-00002150: 672f 6576 616c 5f68 7970 6572 7061 7261  g/eval_hyperpara
-00002160: 6d73 2e79 6d6c 202d 2d64 6174 615f 6669  ms.yml --data_fi
-00002170: 6c65 206f 7574 7075 745f 6373 7620 2d2d  le output_csv --
-00002180: 696d 6167 655f 6669 6c65 206f 7574 7075  image_file outpu
-00002190: 745f 706c 6f74 7320 2d2d 706c 6f74 5f63  t_plots --plot_c
-000021a0: 7572 7665 7320 5472 7565 202d 2d73 6176  urves True --sav
-000021b0: 655f 6669 6c65 2054 7275 6520 2d2d 7475  e_file True --tu
-000021c0: 6e65 7220 7261 795f 7475 6e65 0d0a 6060  ner ray_tune..``
-000021d0: 600d 0a0d 0a23 2320 5374 6570 2033 3a20  `....## Step 3: 
-000021e0: 4578 706c 6f72 6520 4665 6174 7572 6573  Explore Features
-000021f0: 0d0a 0d0a 2323 2320 312e 202a 2a45 7870  ....### 1. **Exp
-00002200: 6c6f 7265 2042 7265 616b 646f 776e 2053  lore Breakdown S
-00002210: 6365 6e61 7269 6f73 2a2a 0d0a 0d0a 5468  cenarios**....Th
-00002220: 6973 2066 6561 7475 7265 2061 6c6c 6f77  is feature allow
-00002230: 7320 7468 6520 7573 6572 2074 6f20 7472  s the user to tr
-00002240: 6169 6e20 7468 6520 6167 656e 7420 6261  ain the agent ba
-00002250: 7365 6420 6f6e 2063 7573 746f 6d65 6420  sed on customed 
-00002260: 6578 706c 6f72 6174 696f 6e20 7072 6566  exploration pref
-00002270: 6572 656e 6365 7320 6265 7477 6565 6e20  erences between 
-00002280: 6b65 7920 7374 6174 6573 2061 6e64 2070  key states and p
-00002290: 6572 6970 6865 7261 6c20 7374 6174 6573  eripheral states
-000022a0: 2075 7369 6e67 2077 6569 6768 7420 7061   using weight pa
-000022b0: 7261 6d65 7465 7220 6077 315f 6b65 7960  rameter `w1_key`
-000022c0: 2061 6e64 2060 7732 5f70 6572 6970 6865   and `w2_periphe
-000022d0: 7261 6c60 2e20 5468 6520 7075 7270 6f73  ral`. The purpos
-000022e0: 6520 6f66 2074 6869 7320 6665 6174 7572  e of this featur
-000022f0: 6520 6973 2074 6f20 656e 6162 6c65 2074  e is to enable t
-00002300: 6865 2061 6765 6e74 2074 6f20 6e6f 7420  he agent to not 
-00002310: 6f6e 6c79 2067 656e 6572 6174 6520 6869  only generate hi
-00002320: 6768 2072 6577 6172 6473 2066 6f72 206b  gh rewards for k
-00002330: 6579 2073 7461 7465 7320 6275 7420 616c  ey states but al
-00002340: 736f 2076 6973 6974 2061 6c6c 2062 7265  so visit all bre
-00002350: 6164 6f77 6e20 7363 656e 6172 696f 7320  adown scenarios 
-00002360: 7375 6666 6963 6965 6e74 6c79 2065 6e6f  sufficiently eno
-00002370: 7567 682e 200d 0a0d 0a53 6574 2075 7020  ugh. ....Set up 
-00002380: 7468 6520 7061 7261 6d65 7465 7273 2069  the parameters i
-00002390: 6e20 6075 7365 725f 636f 6e66 6967 5c66  n `user_config\f
-000023a0: 6561 7475 7265 735f 7061 7261 6d73 5c62  eatures_params\b
-000023b0: 6c6f 6163 6b61 6765 5f65 7870 6c6f 7265  loackage_explore
-000023c0: 5f70 6172 616d 732e 796d 6c60 3a0d 0a0d  _params.yml`:...
-000023d0: 0a2d 2060 7731 5f6b 6579 603a 2057 6569  .- `w1_key`: Wei
-000023e0: 6768 7420 7061 7261 6d65 7465 7220 746f  ght parameter to
-000023f0: 2063 6f6e 7472 6f6c 2066 6176 6f72 2065   control favor e
-00002400: 7870 6c6f 7269 6e67 206b 6579 2073 7461  xploring key sta
-00002410: 7465 732e 0d0a 2d20 6077 325f 7065 7269  tes...- `w2_peri
-00002420: 7068 6572 616c 603a 2057 6569 6768 7420  pheral`: Weight 
-00002430: 7061 7261 6d65 7465 7220 746f 2063 6f6e  parameter to con
-00002440: 7472 6f6c 2066 6176 6f72 2065 7870 6c6f  trol favor explo
-00002450: 7269 6e67 2070 6572 6970 6865 7261 6c20  ring peripheral 
-00002460: 7374 6174 6573 2e0d 0a2d 2060 7265 7365  states...- `rese
-00002470: 7460 3a20 4120 626f 6f6c 2076 616c 7565  t`: A bool value
-00002480: 2074 6861 7420 636f 6e74 726f 6c73 2077   that controls w
-00002490: 6865 7468 6572 2074 6f20 7265 7365 7420  hether to reset 
-000024a0: 7765 6967 6874 2070 6172 616d 6574 6572  weight parameter
-000024b0: 7320 6475 7269 6e67 2074 7261 696e 696e  s during trainin
-000024c0: 672e 0d0a 2d20 6072 6573 6574 5f66 7265  g...- `reset_fre
-000024d0: 7175 656e 6379 603a 2041 2076 616c 7565  quency`: A value
-000024e0: 2074 6861 7420 6465 6669 6e65 7320 7468   that defines th
-000024f0: 6520 6e75 6d62 6572 206f 6620 6570 6973  e number of epis
-00002500: 6f64 6573 2066 7265 7175 656e 6379 2074  odes frequency t
-00002510: 6f20 7265 7365 7420 7468 6520 7765 6967  o reset the weig
-00002520: 6874 2070 6172 616d 6574 6572 732e 0d0a  ht parameters...
-00002530: 2d20 606e 756d 5f6f 7574 7075 7460 3a20  - `num_output`: 
-00002540: 4120 7661 6c75 6520 7468 6174 2064 6566  A value that def
-00002550: 696e 6573 2074 6865 206e 756d 6265 7220  ines the number 
-00002560: 6f66 2074 6f70 2061 6e64 206c 6561 7374  of top and least
-00002570: 2072 6577 6172 642f 7669 7369 7473 2073   reward/visits s
-00002580: 7461 7465 7320 746f 2070 6c6f 7420 696e  tates to plot in
-00002590: 2061 2068 6973 746f 6772 616d 0d0a 2d20   a histogram..- 
-000025a0: 606f 7574 7075 745f 6a73 6f6e 603a 2041  `output_json`: A
-000025b0: 2062 6f6f 6c20 7661 6c75 6520 7468 6174   bool value that
-000025c0: 2064 6574 6572 6d69 6e65 7320 7768 6574   determines whet
-000025d0: 6865 7220 746f 206f 7574 7075 7420 7468  her to output th
-000025e0: 6520 6a73 6f6e 2066 696c 6520 6f66 206b  e json file of k
-000025f0: 6579 2073 7461 7465 7320 616e 6420 7065  ey states and pe
-00002600: 7269 7068 6572 616c 2073 7461 7465 730d  ripheral states.
-00002610: 0a2d 2060 6f75 7470 7574 5f68 6973 746f  .- `output_histo
-00002620: 6772 616d 603a 2041 2062 6f6f 6c20 7661  gram`: A bool va
-00002630: 6c75 6520 7468 6174 2064 6574 6572 6d69  lue that determi
-00002640: 6e65 7320 7768 6574 6865 7220 746f 206f  nes whether to o
-00002650: 7574 7075 7420 7468 6520 6869 7374 6f67  utput the histog
-00002660: 7261 6d20 7468 6174 2073 686f 7773 2074  ram that shows t
-00002670: 6865 2072 6577 6172 6473 2061 6e64 2076  he rewards and v
-00002680: 6973 6974 7320 6f66 2074 6865 2074 6f70  isits of the top
-00002690: 2061 6e64 206c 6561 7374 2073 7461 7465   and least state
-000026a0: 732e 0d0a 2d20 606f 7574 7075 745f 636f  s...- `output_co
-000026b0: 7665 7261 6765 5f6d 6574 7269 6360 3a20  verage_metric`: 
-000026c0: 4120 626f 6f6c 2076 616c 7565 2074 6861  A bool value tha
-000026d0: 7420 6465 7465 726d 696e 6573 2077 6865  t determines whe
-000026e0: 7468 6572 2074 6f20 6f75 7470 7574 2074  ther to output t
-000026f0: 6865 2063 7572 7265 6e74 2063 6f76 6572  he current cover
-00002700: 6167 6520 6d65 7472 6963 2e0d 0a0d 0a54  age metric.....T
-00002710: 6f20 7275 6e20 7468 6973 2066 6561 7475  o run this featu
-00002720: 7265 2c20 6e61 7669 6761 7465 2074 6f20  re, navigate to 
-00002730: 602f 6576 616c 7561 7469 6f6e 2f62 7265  `/evaluation/bre
-00002740: 616b 646f 776e 5f65 7870 6c6f 7261 7469  akdown_explorati
-00002750: 6f6e 6020 616e 6420 7275 6e3a 0d0a 2020  on` and run:..  
-00002760: 2060 6060 6261 7368 0d0a 2020 2070 7974   ```bash..   pyt
-00002770: 686f 6e20 6272 6561 6b64 6f77 6e5f 6578  hon breakdown_ex
-00002780: 706c 6f72 6174 696f 6e2e 7079 0d0a 2020  ploration.py..  
-00002790: 2060 6060 0d0a 0d0a 2323 2320 322e 202a   ```....### 2. *
-000027a0: 2a42 6c6f 636b 6167 6520 4465 6d6f 6e73  *Blockage Demons
-000027b0: 7472 6174 696f 6e73 2a2a 0d0a 0d0a 5468  trations**....Th
-000027c0: 6973 2066 6561 7475 7265 2061 6c6c 6f77  is feature allow
-000027d0: 7320 7468 6520 7573 6572 2074 6f20 7465  s the user to te
-000027e0: 7374 2061 2074 7261 696e 6564 2061 6765  st a trained age
-000027f0: 6e74 2773 2070 6572 666f 726d 616e 6365  nt's performance
-00002800: 206f 6e20 6120 7369 6d75 6c61 7465 6420   on a simulated 
-00002810: 7365 7276 6572 2062 6c6f 636b 6167 6520  server blockage 
-00002820: 7175 6575 6569 6e67 2065 6e76 6972 6f6e  queueing environ
-00002830: 6d65 6e74 2062 7920 7669 7375 616c 697a  ment by visualiz
-00002840: 696e 6720 7468 6520 6368 616e 6765 7320  ing the changes 
-00002850: 696e 2074 7261 6e73 6974 696f 6e20 7072  in transition pr
-00002860: 6f62 6162 696c 6974 6965 732e 2054 6865  obabilities. The
-00002870: 2070 7572 706f 7365 206f 6620 7468 6973   purpose of this
-00002880: 2066 6561 7475 7265 2069 7320 746f 2073   feature is to s
-00002890: 686f 7720 686f 7720 6566 6665 6374 6963  how how effectic
-000028a0: 6520 7468 6520 7472 616e 6965 6420 6167  e the tranied ag
-000028b0: 656e 7420 6973 2061 6374 696e 6720 6f6e  ent is acting on
-000028c0: 2062 7265 616b 646f 776e 2063 6173 6573   breakdown cases
-000028d0: 2e20 0d0a 0d0a 5365 7420 7570 2074 6865  . ....Set up the
-000028e0: 2070 6172 616d 6574 6572 7320 696e 2060   parameters in `
-000028f0: 7573 6572 5f63 6f6e 6669 675c 6665 6174  user_config\feat
-00002900: 7572 6573 5f70 6172 616d 735c 626c 6f63  ures_params\bloc
-00002910: 6b61 6765 5f64 656d 6f6e 7374 7261 7469  kage_demonstrati
-00002920: 6f6e 5f70 6172 616d 732e 796d 6c60 3a0d  on_params.yml`:.
-00002930: 0a0d 0a2d 2060 6e75 6d5f 7369 6d60 3a20  ...- `num_sim`: 
-00002940: 4465 6669 6e65 7320 7468 6520 6e75 6d62  Defines the numb
-00002950: 6572 206f 6620 6a6f 6273 2074 6f20 7369  er of jobs to si
-00002960: 6d75 6c61 7465 2066 6f72 2065 6163 6820  mulate for each 
-00002970: 7469 6d65 2073 7465 7020 6475 7269 6e67  time step during
-00002980: 2074 7261 696e 696e 672e 0d0a 2d20 6074   training...- `t
-00002990: 696d 655f 7374 6570 7360 3a20 4465 6669  ime_steps`: Defi
-000029a0: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
-000029b0: 6620 7469 6d65 2073 7465 7073 2074 6f20  f time steps to 
-000029c0: 7065 7266 6f72 6d20 666f 7220 6561 6368  perform for each
-000029d0: 2065 7069 736f 6465 2e0d 0a2d 2060 7175   episode...- `qu
-000029e0: 6575 655f 696e 6465 7860 3a20 4465 6669  eue_index`: Defi
-000029f0: 6e65 7320 7468 6520 7175 6575 6520 696e  nes the queue in
-00002a00: 6465 7820 7468 6174 2072 6563 6f72 6420  dex that record 
-00002a10: 7468 6520 6d65 7472 6963 7320 666f 722e  the metrics for.
-00002a20: 0d0a 2d20 606d 6574 7269 6360 3a20 4465  ..- `metric`: De
-00002a30: 6669 6e65 7320 7468 6520 6d65 7472 6963  fines the metric
-00002a40: 2074 6f20 6265 2072 6570 6f72 7465 6420   to be reported 
-00002a50: 666f 7220 7468 6520 7365 6c65 6374 6564  for the selected
-00002a60: 2071 7565 7565 2e0d 0a0d 0a54 6f20 7573   queue.....To us
-00002a70: 6520 7468 6973 2066 6561 7475 7265 2c20  e this feature, 
-00002a80: 6e61 7669 6761 7465 2074 6f20 602f 6576  navigate to `/ev
-00002a90: 616c 7561 7469 6f6e 2f62 6c6f 636b 6167  aluation/blockag
-00002aa0: 655f 6465 6d6f 6e73 7472 6174 696f 6e60  e_demonstration`
-00002ab0: 2061 6e64 2072 756e 3a0d 0a20 2020 6060   and run:..   ``
-00002ac0: 6062 6173 680d 0a20 2020 7079 7468 6f6e  `bash..   python
-00002ad0: 2064 656d 6f6e 7374 7261 7469 6f6e 732e   demonstrations.
-00002ae0: 7079 0d0a 2020 2060 6060 0d0a 0d0a 2323  py..   ```....##
-00002af0: 2320 332e 202a 2a53 7461 7274 7570 2042  # 3. **Startup B
-00002b00: 6568 6176 696f 7220 4964 656e 7469 6669  ehavior Identifi
-00002b10: 6361 7469 6f6e 2a2a 0d0a 0d0a 5468 6973  cation**....This
-00002b20: 2066 6561 7475 7265 2061 6c6c 6f77 7320   feature allows 
-00002b30: 7468 6520 7573 6572 2074 6f20 7669 7375  the user to visu
-00002b40: 616c 697a 6520 7768 656e 2074 6865 2062  alize when the b
-00002b50: 7572 6e2d 696e 2070 6572 696f 6473 2065  urn-in periods e
-00002b60: 6e64 206f 6e20 7468 6520 6c65 6172 6e69  nd on the learni
-00002b70: 6e67 2063 7572 7665 2e20 0d0a 0d0a 5365  ng curve. ....Se
-00002b80: 7420 7570 2074 6865 2070 6172 616d 6574  t up the paramet
-00002b90: 6572 7320 696e 2074 6865 2073 6372 6970  ers in the scrip
-00002ba0: 743a 0d0a 0d0a 2d20 6077 696e 646f 775f  t:....- `window_
-00002bb0: 7369 7a65 603a 2053 7065 6369 6669 6573  size`: Specifies
-00002bc0: 2074 6865 206e 756d 6265 7220 6f66 2064   the number of d
-00002bd0: 6174 6120 706f 696e 7473 2075 7365 6420  ata points used 
-00002be0: 746f 2063 6f6d 7075 7465 2074 6865 206d  to compute the m
-00002bf0: 6f76 696e 6720 6176 6572 6167 6520 6f66  oving average of
-00002c00: 2074 6865 2072 6577 6172 6473 2e0d 0a2d   the rewards...-
-00002c10: 2060 7468 7265 7368 6f6c 6460 3a20 4465   `threshold`: De
-00002c20: 6669 6e65 7320 7468 6520 6d61 7869 6d75  fines the maximu
-00002c30: 6d20 6163 6365 7074 6162 6c65 2061 6273  m acceptable abs
-00002c40: 6f6c 7574 6520 7661 6c75 6520 6f66 2074  olute value of t
-00002c50: 6865 2064 6572 6976 6174 6976 6520 6f66  he derivative of
-00002c60: 2074 6865 2073 6d6f 6f74 6865 6420 7265   the smoothed re
-00002c70: 7761 7264 7320 6265 6c6f 7720 7768 6963  wards below whic
-00002c80: 6820 6120 7265 7761 7264 2069 7320 636f  h a reward is co
-00002c90: 6e73 6964 6572 6564 2073 7461 626c 652e  nsidered stable.
-00002ca0: 200d 0a2d 2060 636f 6e73 6563 7574 6976   ..- `consecutiv
-00002cb0: 655f 706f 696e 7473 603a 2054 6865 206e  e_points`: The n
-00002cc0: 756d 6265 7220 6f66 2063 6f6e 7365 6375  umber of consecu
-00002cd0: 7469 7665 2064 6174 6120 706f 696e 7473  tive data points
-00002ce0: 2074 6861 7420 6d75 7374 2061 6c6c 2062   that must all b
-00002cf0: 6520 6265 6c6f 7720 7468 6520 7468 7265  e below the thre
-00002d00: 7368 6f6c 6420 666f 7220 7468 6520 7265  shold for the re
-00002d10: 7761 7264 7320 746f 2062 6520 636f 6e73  wards to be cons
-00002d20: 6964 6572 6564 2061 7320 6861 7669 6e67  idered as having
-00002d30: 2073 7461 6269 6c69 7a65 642e 200d 0a2d   stabilized. ..-
-00002d40: 2060 6570 6973 6f64 6560 3a20 5370 6563   `episode`: Spec
-00002d50: 6966 7920 7768 6963 6820 6570 6973 6f64  ify which episod
-00002d60: 6527 7320 7265 7761 7264 7320 746f 2061  e's rewards to a
-00002d70: 6e61 6c79 7a65 2066 726f 6d20 6120 6461  nalyze from a da
-00002d80: 7461 7365 742e 0d0a 0d0a 546f 2070 6572  taset.....To per
-00002d90: 666f 726d 2074 6865 2066 6561 7475 7265  form the feature
-00002da0: 2c20 6e61 7669 6761 7465 2074 6f20 602f  , navigate to `/
-00002db0: 6576 616c 7561 7469 6f6e 2f73 7461 7274  evaluation/start
-00002dc0: 7570 5f62 6568 6176 696f 7260 2061 6e64  up_behavior` and
-00002dd0: 2072 756e 3a0d 0a20 2020 6060 6062 6173   run:..   ```bas
-00002de0: 680d 0a20 2020 7079 7468 6f6e 2073 7461  h..   python sta
-00002df0: 7274 7570 2e70 790d 0a20 2020 6060 600d  rtup.py..   ```.
-00002e00: 0a0d 0a23 2323 2034 2e20 2a2a 436f 6e66  ...### 4. **Conf
-00002e10: 6964 656e 6365 2045 7661 6c75 6174 696f  idence Evaluatio
-00002e20: 6e2a 2a20 0d0a 0d0a 5468 6973 2066 6561  n** ....This fea
-00002e30: 7475 7265 2061 6c6c 6f77 7320 7468 6520  ture allows the 
-00002e40: 7573 6572 2074 7261 696e 206d 756c 7469  user train multi
-00002e50: 706c 6520 7665 7273 696f 6e73 206f 6620  ple versions of 
-00002e60: 7468 6520 6167 656e 7420 666f 7220 6469  the agent for di
-00002e70: 6666 6572 656e 7420 6e75 6d62 6572 7320  fferent numbers 
-00002e80: 6f66 2074 7261 696e 696e 6720 6570 6973  of training epis
-00002e90: 6f64 6573 2061 6e64 2074 6865 6e20 6576  odes and then ev
-00002ea0: 616c 7561 7465 2074 6865 2070 6572 666f  aluate the perfo
-00002eb0: 726d 616e 6365 206f 6620 6561 6368 2061  rmance of each a
-00002ec0: 6765 6e74 206f 6e20 7468 6520 7369 6d75  gent on the simu
-00002ed0: 6c61 7469 6f6e 2065 6e76 6972 6f6e 6d65  lation environme
-00002ee0: 6e74 2e0d 0a0d 0a53 6574 2075 7020 7468  nt.....Set up th
-00002ef0: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
-00002f00: 7468 6520 7363 7269 7074 3a0d 0a0d 0a2d  the script:....-
-00002f10: 2060 6e75 6d5f 6570 6973 6f64 6573 5f6c   `num_episodes_l
-00002f20: 6973 7460 3a20 4120 6c69 7374 2074 6861  ist`: A list tha
-00002f30: 7420 636f 6e74 6169 6e73 2064 6966 6665  t contains diffe
-00002f40: 7265 6e74 206e 756d 6265 7273 206f 6620  rent numbers of 
-00002f50: 6570 6973 6f64 6573 2074 6f20 7472 6169  episodes to trai
-00002f60: 6e20 7468 6520 6167 656e 7473 2e0d 0a2d  n the agents...-
-00002f70: 2060 7469 6d65 7374 6570 7360 3a20 4120   `timesteps`: A 
-00002f80: 7661 6c75 6520 7468 6174 2064 6566 696e  value that defin
-00002f90: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-00002fa0: 2074 696d 6573 7465 7073 2074 6f20 7472   timesteps to tr
-00002fb0: 6169 6e20 7468 6520 6167 656e 7420 6475  ain the agent du
-00002fc0: 7269 6e67 2065 6163 6820 6570 6973 6f64  ring each episod
-00002fd0: 652e 0d0a 0d0a 546f 2072 756e 2074 6869  e.....To run thi
-00002fe0: 7320 6665 6174 7572 652c 206e 6176 6967  s feature, navig
-00002ff0: 6174 6520 746f 2060 2f65 7661 6c75 6174  ate to `/evaluat
-00003000: 696f 6e2f 636f 6e66 6964 656e 6365 5f65  ion/confidence_e
-00003010: 7661 6c75 6174 696f 6e60 2061 6e64 2072  valuation` and r
-00003020: 756e 3a0d 0a20 2020 6060 6062 6173 680d  un:..   ```bash.
-00003030: 0a20 2020 7079 7468 6f6e 2063 6f6e 6669  .   python confi
-00003040: 6465 6e63 652e 7079 0d0a 2020 2060 6060  dence.py..   ```
-00003050: 0d0a 0d0a 2323 2320 352e 202a 2a52 6f62  ....### 5. **Rob
-00003060: 7573 746e 6573 7320 4576 616c 7561 7469  ustness Evaluati
-00003070: 6f6e 2a2a 200d 0a0d 0a54 6869 7320 6665  on** ....This fe
-00003080: 6174 7572 6520 616c 6c6f 7773 2074 6865  ature allows the
-00003090: 2075 7365 7220 746f 2074 7261 696e 206d   user to train m
-000030a0: 756c 7469 706c 6520 6167 656e 7473 2c20  ultiple agents, 
-000030b0: 616e 616c 797a 6520 7468 6569 7220 6265  analyze their be
-000030c0: 6861 7669 6f72 2c20 616e 6420 6361 6c63  havior, and calc
-000030d0: 756c 6174 6520 7374 6174 6973 7469 6361  ulate statistica
-000030e0: 6c20 6d65 7472 6963 7320 6261 7365 6420  l metrics based 
-000030f0: 6f6e 2074 6865 6972 2070 6572 666f 726d  on their perform
-00003100: 616e 6365 2e0d 0a0d 0a53 6574 2075 7020  ance.....Set up 
-00003110: 7468 6520 7061 7261 6d65 7465 7273 2069  the parameters i
-00003120: 6e20 7468 6520 7363 7269 7074 3a0d 0a0d  n the script:...
-00003130: 0a2d 2060 636f 6e66 6964 656e 6365 5f6c  .- `confidence_l
-00003140: 6576 656c 603a 2054 6865 2073 7461 7469  evel`: The stati
-00003150: 7374 6963 616c 2063 6f6e 6669 6465 6e63  stical confidenc
-00003160: 6520 6c65 7665 6c20 666f 7220 6361 6c63  e level for calc
-00003170: 756c 6174 696f 6e73 2e0d 0a2d 2060 6465  ulations...- `de
-00003180: 7369 7265 645f 6572 726f 7260 3a20 5468  sired_error`: Th
-00003190: 6520 7461 7267 6574 2065 7272 6f72 206d  e target error m
-000031a0: 6172 6769 6e20 666f 7220 6573 7469 6d61  argin for estima
-000031b0: 7469 6e67 2073 7461 7469 7374 6963 616c  ting statistical
-000031c0: 2072 6571 7569 7265 6d65 6e74 732e 0d0a   requirements...
-000031d0: 2d20 606e 756d 5f72 756e 7360 3a20 4e75  - `num_runs`: Nu
-000031e0: 6d62 6572 206f 6620 7469 6d65 7320 746f  mber of times to
-000031f0: 2074 7261 696e 2061 6765 6e74 732e 0d0a   train agents...
-00003200: 2d20 6074 696d 655f 7374 6570 7360 3a20  - `time_steps`: 
-00003210: 4e75 6d62 6572 206f 6620 7469 6d65 2073  Number of time s
-00003220: 7465 7073 2065 6163 6820 6167 656e 7420  teps each agent 
-00003230: 7275 6e73 2069 6e20 7468 6520 7369 6d75  runs in the simu
-00003240: 6c61 7469 6f6e 2065 6e76 6972 6f6e 6d65  lation environme
-00003250: 6e74 2e0d 0a2d 2060 6e75 6d5f 7369 6d60  nt...- `num_sim`
-00003260: 3a20 4e75 6d62 6572 206f 6620 7369 6d75  : Number of simu
-00003270: 6c61 7469 6f6e 7320 746f 2072 756e 2069  lations to run i
-00003280: 6e20 7468 6520 656e 7669 726f 6e6d 656e  n the environmen
-00003290: 742e 0d0a 0d0a 546f 2072 756e 2074 6869  t.....To run thi
-000032a0: 7320 6665 6174 7572 652c 206e 6176 6967  s feature, navig
-000032b0: 6174 6520 746f 2060 2f65 7661 6c75 6174  ate to `/evaluat
-000032c0: 696f 6e2f 726f 6275 7374 6e65 7373 5f65  ion/robustness_e
-000032d0: 7661 6c75 6174 696f 6e60 2061 6e64 2072  valuation` and r
-000032e0: 756e 3a0d 0a20 2020 6060 6062 6173 680d  un:..   ```bash.
-000032f0: 0a20 2020 7079 7468 6f6e 2072 756e 732e  .   python runs.
-00003300: 7079 0d0a 2020 2060 6060 0d0a 0d0a 2323  py..   ```....##
-00003310: 2320 362e 202a 2a4e 6f69 7365 2045 7661  # 6. **Noise Eva
-00003320: 6c75 6174 696f 6e2a 2a20 0d0a 0d0a 5468  luation** ....Th
-00003330: 6973 2066 6561 7475 7265 2061 6c6c 6f77  is feature allow
-00003340: 7320 7468 6520 7573 6572 2074 6f20 6576  s the user to ev
-00003350: 616c 7561 7465 2074 6865 2065 6666 6563  aluate the effec
-00003360: 7420 6f66 2065 6e76 6972 6f6e 6d65 6e74  t of environment
-00003370: 616c 206e 6f69 7365 206f 6e20 7468 6520  al noise on the 
-00003380: 7065 7266 6f72 6d61 6e63 6520 6f66 2074  performance of t
-00003390: 6865 2061 6765 6e74 2e0d 0a0d 0a53 6574  he agent.....Set
-000033a0: 2075 7020 7468 6520 7061 7261 6d65 7465   up the paramete
-000033b0: 7273 2069 6e20 7468 6520 7363 7269 7074  rs in the script
-000033c0: 3a0d 0a0d 0a2d 2060 6672 6571 7565 6e63  :....- `frequenc
-000033d0: 7920 603a 2054 6865 206c 696b 656c 6968  y `: The likelih
-000033e0: 6f6f 6420 6f72 2066 7265 7175 656e 6379  ood or frequency
-000033f0: 2061 7420 7768 6963 6820 6e6f 6973 6520   at which noise 
-00003400: 6973 2069 6e74 726f 6475 6365 6420 746f  is introduced to
-00003410: 2074 6865 2073 7973 7465 6d2e 2049 7420   the system. It 
-00003420: 6d75 7374 2062 6520 6120 7661 6c75 6520  must be a value 
-00003430: 6265 7477 6565 6e20 3020 616e 6420 312e  between 0 and 1.
-00003440: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-00003450: 6465 7465 726d 696e 6573 2068 6f77 206f  determines how o
-00003460: 6674 656e 2c20 7072 6f70 6f72 7469 6f6e  ften, proportion
-00003470: 616c 6c79 2c20 6e6f 6973 6520 7769 6c6c  ally, noise will
-00003480: 2062 6520 6164 6465 6420 6475 7269 6e67   be added during
-00003490: 2074 6865 2073 696d 756c 6174 696f 6e2e   the simulation.
-000034a0: 200d 0a2d 2060 6d65 616e 603a 2054 6865   ..- `mean`: The
-000034b0: 206d 6561 6e20 6f66 2074 6865 206e 6f72   mean of the nor
-000034c0: 6d61 6c20 6469 7374 7269 6275 7469 6f6e  mal distribution
-000034d0: 2066 726f 6d20 7768 6963 6820 7468 6520   from which the 
-000034e0: 6e6f 6973 6520 7661 6c75 6573 2061 7265  noise values are
-000034f0: 2073 616d 706c 6564 2e20 5468 6973 2072   sampled. This r
-00003500: 6570 7265 7365 6e74 7320 7468 6520 6176  epresents the av
-00003510: 6572 6167 6520 7661 6c75 6520 6f66 2074  erage value of t
-00003520: 6865 206e 6f69 7365 2074 6861 7420 7769  he noise that wi
-00003530: 6c6c 2062 6520 696e 7472 6f64 7563 6564  ll be introduced
-00003540: 2e0d 0a2d 2060 7661 7269 616e 6365 603a  ...- `variance`:
-00003550: 2054 6865 2076 6172 6961 6e63 6520 6f66   The variance of
-00003560: 2074 6865 206e 6f72 6d61 6c20 6469 7374   the normal dist
-00003570: 7269 6275 7469 6f6e 2066 726f 6d20 7768  ribution from wh
-00003580: 6963 6820 7468 6520 6e6f 6973 6520 7661  ich the noise va
-00003590: 6c75 6573 2061 7265 2073 616d 706c 6564  lues are sampled
-000035a0: 2e20 5468 6973 2070 6172 616d 6574 6572  . This parameter
-000035b0: 2069 6e64 6963 6174 6573 2074 6865 2073   indicates the s
-000035c0: 7072 6561 6420 6f72 2064 6973 7065 7273  pread or dispers
-000035d0: 696f 6e20 6f66 2074 6865 206e 6f69 7365  ion of the noise
-000035e0: 2061 726f 756e 6420 7468 6520 6d65 616e   around the mean
-000035f0: 2e0d 0a0d 0a54 6f20 7275 6e20 7468 6520  .....To run the 
-00003600: 6665 6174 7572 652c 206e 6176 6967 6174  feature, navigat
-00003610: 6520 746f 2060 2f65 7661 6c75 6174 696f  e to `/evaluatio
-00003620: 6e2f 6e6f 6973 655f 6576 616c 7561 7469  n/noise_evaluati
-00003630: 6f6e 6020 616e 6420 7275 6e3a 0d0a 2020  on` and run:..  
-00003640: 2060 6060 6261 7368 0d0a 2020 2070 7974   ```bash..   pyt
-00003650: 686f 6e20 6e6f 6973 655f 6576 616c 7561  hon noise_evalua
-00003660: 7469 6f6e 2e70 790d 0a20 2020 6060 600d  tion.py..   ```.
-00003670: 0a0d 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-00003680: 6f6e 0d0a 0d0a 436f 6e74 7269 6275 7469  on....Contributi
-00003690: 6f6e 7320 6172 6520 7765 6c63 6f6d 652e  ons are welcome.
-000036a0: 2050 6c65 6173 6520 6372 6561 7465 2061   Please create a
-000036b0: 2070 756c 6c20 7265 7175 6573 7420 6f72   pull request or
-000036c0: 2069 7373 7565 2074 6f20 6469 7363 7573   issue to discus
-000036d0: 7320 7072 6f70 6f73 6564 2063 6861 6e67  s proposed chang
-000036e0: 6573 206f 7220 7265 706f 7274 2062 7567  es or report bug
-000036f0: 732e 0d0a 0d0a 2323 204c 6963 656e 7365  s.....## License
-00003700: 0d0a 0d0a 5468 6973 2070 726f 6a65 6374  ....This project
-00003710: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00003720: 6572 2074 6865 204d 4954 204c 6963 656e  er the MIT Licen
-00003730: 7365 202d 2073 6565 2074 6865 204c 4943  se - see the LIC
-00003740: 454e 5345 2066 696c 6520 666f 7220 6465  ENSE file for de
-00003750: 7461 696c 732e 0d0a                      tails...
+000002d0: 3a0d 0a20 202d 202a 2a44 6563 6973 696f  :..  - **Decisio
+000002e0: 6e20 4576 616c 7561 7469 6f6e 2a2a 3a20  n Evaluation**: 
+000002f0: 4465 6d6f 6e73 7472 6174 6573 2068 6f77  Demonstrates how
+00000300: 2074 6865 2061 6765 6e74 2072 6573 706f   the agent respo
+00000310: 6e64 7320 746f 2061 2073 6572 7665 7220  nds to a server 
+00000320: 6f75 7461 6765 2062 7920 6164 6a75 7374  outage by adjust
+00000330: 696e 6720 726f 7574 696e 6720 7072 6f62  ing routing prob
+00000340: 6162 696c 6974 6965 732e 0d0a 2020 2d20  abilities...  - 
+00000350: 2a2a 436f 6e66 6964 656e 6365 2045 7661  **Confidence Eva
+00000360: 6c75 6174 696f 6e2a 2a3a 2041 7373 6573  luation**: Asses
+00000370: 7365 7320 7468 6520 7374 6162 696c 6974  ses the stabilit
+00000380: 7920 616e 6420 7265 6c69 6162 696c 6974  y and reliabilit
+00000390: 7920 6f66 2074 6865 2061 6765 6e74 2061  y of the agent a
+000003a0: 6372 6f73 7320 6469 6666 6572 656e 7420  cross different 
+000003b0: 7472 6169 6e69 6e67 2073 6574 7570 730d  training setups.
+000003c0: 0a20 202d 202a 2a4e 6f69 7365 2045 7661  .  - **Noise Eva
+000003d0: 6c75 6174 696f 6e2a 2a3a 2045 7661 6c75  luation**: Evalu
+000003e0: 6174 6520 7468 6520 6566 6665 6374 206f  ate the effect o
+000003f0: 6620 656e 7669 726f 6e6d 656e 7461 6c20  f environmental 
+00000400: 6e6f 6973 6520 6f6e 2074 6865 2070 6572  noise on the per
+00000410: 666f 726d 616e 6365 206f 6620 7468 6520  formance of the 
+00000420: 6167 656e 740d 0a20 202d 202a 2a53 7461  agent..  - **Sta
+00000430: 7274 7570 2045 7661 6c75 6174 696f 6e2a  rtup Evaluation*
+00000440: 2a3a 2049 6465 6e74 6966 6965 7320 7468  *: Identifies th
+00000450: 6520 6275 726e 2d69 6e20 7065 7269 6f64  e burn-in period
+00000460: 206f 6620 7468 6520 6167 656e 740d 0a20   of the agent.. 
+00000470: 202d 202a 2a52 6f62 7573 746e 6573 7320   - **Robustness 
+00000480: 4576 616c 7561 7469 6f6e 2a2a 3a20 4173  Evaluation**: As
+00000490: 7365 7373 2072 6f62 7573 746e 6573 7320  sess robustness 
+000004a0: 6f66 2064 6563 6973 696f 6e73 2061 6372  of decisions acr
+000004b0: 6f73 7320 6d75 6c74 6970 6c65 2074 7261  oss multiple tra
+000004c0: 696e 6564 2061 6765 6e74 730d 0a0d 0a23  ined agents....#
+000004d0: 2320 5072 6572 6571 7569 7369 7465 730d  # Prerequisites.
+000004e0: 0a0d 0a42 6566 6f72 6520 7275 6e6e 696e  ...Before runnin
+000004f0: 6720 7468 6520 7369 6d75 6c61 7469 6f6e  g the simulation
+00000500: 732c 2065 6e73 7572 6520 796f 7520 6861  s, ensure you ha
+00000510: 7665 2074 6865 2066 6f6c 6c6f 7769 6e67  ve the following
+00000520: 2069 6e73 7461 6c6c 6564 3a0d 0a2d 2050   installed:..- P
+00000530: 7974 686f 6e20 3e3d 332e 3130 203c 332e  ython >=3.10 <3.
+00000540: 3132 0d0a 2d20 746f 7263 6820 3d20 2232  12..- torch = "2
+00000550: 2e32 2e30 220d 0a2d 206e 756d 7079 203d  .2.0"..- numpy =
+00000560: 2022 312e 3236 2e34 220d 0a2d 2070 616e   "1.26.4"..- pan
+00000570: 6461 7320 3d20 2232 2e32 2e30 220d 0a2d  das = "2.2.0"..-
+00000580: 2071 7565 7565 696e 675f 746f 6f6c 203d   queueing_tool =
+00000590: 2022 312e 322e 3522 0d0a 2d20 6d61 7470   "1.2.5"..- matp
+000005a0: 6c6f 746c 6962 203d 2022 332e 382e 3322  lotlib = "3.8.3"
+000005b0: 0d0a 2d20 7761 6e64 6220 3d20 2230 2e31  ..- wandb = "0.1
+000005c0: 362e 3322 0d0a 2d20 5079 5941 4d4c 203d  6.3"..- PyYAML =
+000005d0: 2022 362e 302e 3122 0d0a 2d20 7261 7920   "6.0.1"..- ray 
+000005e0: 3d20 7b20 7665 7273 696f 6e20 3d20 2232  = { version = "2
+000005f0: 2e39 2e32 222c 2065 7874 7261 7320 3d20  .9.2", extras = 
+00000600: 5b22 7472 6169 6e22 2c20 2274 756e 6522  ["train", "tune"
+00000610: 5d20 7d0d 0a2d 2074 7164 6d20 3d20 2234  ] }..- tqdm = "4
+00000620: 2e35 372e 3022 0d0a 2d20 7363 6970 7920  .57.0"..- scipy 
+00000630: 3d20 2231 2e31 322e 3022 0d0a 0d0a 2323  = "1.12.0"....##
+00000640: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
+00000650: 0a43 6c6f 6e65 2074 6865 2072 6570 6f73  .Clone the repos
+00000660: 6974 6f72 7920 616e 6420 696e 7374 616c  itory and instal
+00000670: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
+00000680: 6570 656e 6465 6e63 6965 733a 0d0a 0d0a  ependencies:....
+00000690: 6060 6062 6173 680d 0a67 6974 2063 6c6f  ```bash..git clo
+000006a0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+000006b0: 622e 636f 6d2f 616f 2d34 3230 2f73 696d  b.com/ao-420/sim
+000006c0: 5f72 6c2e 6769 740d 0a63 6420 7369 6d5f  _rl.git..cd sim_
+000006d0: 726c 0d0a 7069 7020 696e 7374 616c 6c20  rl..pip install 
+000006e0: 2d72 2072 6571 7569 7265 6d65 6e74 732e  -r requirements.
+000006f0: 7478 740d 0a60 6060 0d0a 0d0a 2323 2053  txt..```....## S
+00000700: 7465 7020 313a 2043 6f6e 6669 6775 7261  tep 1: Configura
+00000710: 7469 6f6e 0d0a 0d0a 2323 2320 456e 7669  tion....### Envi
+00000720: 726f 6e6d 656e 7420 5365 7475 700d 0a0d  ronment Setup...
+00000730: 0a23 2323 2320 2a2a 5175 6575 6569 6e67  .#### **Queueing
+00000740: 2045 6e76 6972 6f6e 6d65 6e74 2043 6f6e   Environment Con
+00000750: 6669 6775 7261 7469 6f6e 2a2a 0d0a 0d0a  figuration**....
+00000760: 5468 6520 7369 6d75 6c61 7469 6f6e 2065  The simulation e
+00000770: 6e76 6972 6f6e 6d65 6e74 2072 6571 7569  nvironment requi
+00000780: 7265 7320 7468 6520 666f 6c6c 6f77 696e  res the followin
+00000790: 6720 7061 7261 6d65 7465 7273 2074 6f20  g parameters to 
+000007a0: 6265 2064 6566 696e 6564 2069 6e20 7468  be defined in th
+000007b0: 6520 6063 6f6e 6669 6775 7261 7469 6f6e  e `configuration
+000007c0: 2e79 6d6c 602e 0d0a 0d0a 2d20 6061 646a  .yml`.....- `adj
+000007d0: 6163 656e 745f 6c69 7374 603a 2041 2064  acent_list`: A d
+000007e0: 6963 7469 6f6e 6172 7920 6465 6669 6e69  ictionary defini
+000007f0: 6e67 2074 6865 2061 646a 6163 656e 6379  ng the adjacency
+00000800: 206c 6973 7420 666f 7220 7468 6520 6e65   list for the ne
+00000810: 7477 6f72 6b20 746f 706f 6c6f 6779 2e0d  twork topology..
+00000820: 0a2d 2060 6d69 755f 6469 6374 603a 2041  .- `miu_dict`: A
+00000830: 2064 6963 7469 6f6e 6172 7920 6f66 2073   dictionary of s
+00000840: 6572 7669 6365 2072 6174 6573 2066 6f72  ervice rates for
+00000850: 2065 6163 6820 7365 7276 6963 6520 6e6f   each service no
+00000860: 6465 2069 6e20 7468 6520 6e65 7477 6f72  de in the networ
+00000870: 6b2e 0d0a 2d20 6074 7261 6e73 6974 696f  k...- `transitio
+00000880: 6e5f 7072 6f62 615f 616c 6c60 3a20 4120  n_proba_all`: A 
+00000890: 6469 6374 696f 6e61 7279 2064 6566 696e  dictionary defin
+000008a0: 696e 6720 7468 6520 7472 616e 7369 7469  ing the transiti
+000008b0: 6f6e 2070 726f 6261 6269 6c69 7469 6573  on probabilities
+000008c0: 2062 6574 7765 656e 206e 6f64 6573 2e0d   between nodes..
+000008d0: 0a2d 2060 6163 7469 7665 5f63 6170 603a  .- `active_cap`:
+000008e0: 2054 6865 2061 6374 6976 6520 6361 7061   The active capa
+000008f0: 6369 7479 206f 6620 7468 6520 6e6f 6465  city of the node
+00000900: 7320 6672 6f6d 206f 7574 7369 6465 2074  s from outside t
+00000910: 6865 206e 6574 776f 726b 2e0d 0a2d 2060  he network...- `
+00000920: 6465 6163 7469 7665 5f74 603a 2054 6865  deactive_t`: The
+00000930: 2064 6561 6374 6976 6174 696f 6e20 7468   deactivation th
+00000940: 7265 7368 6f6c 6420 666f 7220 7468 6520  reshold for the 
+00000950: 6e6f 6465 7320 6672 6f6d 206f 7574 7369  nodes from outsi
+00000960: 6465 2074 6865 206e 6574 776f 726b 2e0d  de the network..
+00000970: 0a2d 2060 6275 6666 6572 5f73 697a 655f  .- `buffer_size_
+00000980: 666f 725f 6561 6368 5f71 7565 7565 603a  for_each_queue`:
+00000990: 2041 2064 6963 7469 6f6e 6172 7920 7468   A dictionary th
+000009a0: 6174 2064 6566 696e 6573 2074 6865 2062  at defines the b
+000009b0: 7566 6665 7220 7369 7a65 2066 6f72 2065  uffer size for e
+000009c0: 6163 6820 7175 6575 652e 0d0a 2d20 6061  ach queue...- `a
+000009d0: 7272 6976 616c 5f72 6174 6560 3a20 4120  rrival_rate`: A 
+000009e0: 6c69 7374 2074 6861 7420 6465 6669 6e65  list that define
+000009f0: 7320 7468 6520 6172 7269 7661 6c20 7261  s the arrival ra
+00000a00: 7465 7320 666f 7220 616c 6c20 706f 7373  tes for all poss
+00000a10: 6962 6c65 2065 6e74 7279 206e 6f64 6573  ible entry nodes
+00000a20: 2e0d 0a2d 2060 6d61 785f 6167 656e 7473  ...- `max_agents
+00000a30: 603a 2041 2076 616c 7565 2074 6861 7420  `: A value that 
+00000a40: 6465 6669 6e65 7320 7468 6520 6d61 7869  defines the maxi
+00000a50: 6d75 6d20 6e75 6d62 6572 206f 6620 6167  mum number of ag
+00000a60: 656e 7473 2063 616e 2062 6520 6163 6370  ents can be accp
+00000a70: 6574 6564 2066 726f 6d20 6f75 7473 6964  eted from outsid
+00000a80: 6520 7468 6520 6e65 7477 6f72 6b20 666f  e the network fo
+00000a90: 7220 7468 6520 656e 7472 7920 6e6f 6465  r the entry node
+00000aa0: 732e 0d0a 2d20 6073 696d 5f6a 6f62 7360  s...- `sim_jobs`
+00000ab0: 3a20 4120 7661 6c75 6520 7468 6174 2064  : A value that d
+00000ac0: 6566 696e 6573 2074 6865 206e 756d 6265  efines the numbe
+00000ad0: 7220 6f66 206a 6f62 7320 6265 696e 6720  r of jobs being 
+00000ae0: 7369 6d75 6c61 7465 6420 6475 7269 6e67  simulated during
+00000af0: 2065 7665 7279 2073 696d 756c 6174 696f   every simulatio
+00000b00: 6e2e 0d0a 2d20 606d 6178 5f61 7272 5f72  n...- `max_arr_r
+00000b10: 6174 655f 6c69 7374 603a 2041 206c 6973  ate_list`: A lis
+00000b20: 7420 7468 6174 2064 6566 696e 6573 2074  t that defines t
+00000b30: 6865 206d 6178 696d 756d 2061 7272 6976  he maximum arriv
+00000b40: 616c 2072 6174 6520 666f 7220 616c 6c20  al rate for all 
+00000b50: 656e 7472 7920 7175 6575 6573 2e0d 0a2d  entry queues...-
+00000b60: 2060 656e 7472 795f 6e6f 6465 7360 3a20   `entry_nodes`: 
+00000b70: 4120 6c69 7374 2074 6861 7420 6465 6669  A list that defi
+00000b80: 6e65 7320 7468 6520 736f 7572 6365 2061  nes the source a
+00000b90: 6e64 2074 6172 6765 7420 7665 7274 6963  nd target vertic
+00000ba0: 6573 206f 6620 6561 6368 2065 6e74 7279  es of each entry
+00000bb0: 206e 6f64 652e 0d0a 0d0a 2020 2045 7861   node.....   Exa
+00000bc0: 6d70 6c65 3a0d 0a20 2020 6060 6079 616d  mple:..   ```yam
+00000bd0: 6c0d 0a20 2020 6d69 755f 6c69 7374 3a20  l..   miu_list: 
+00000be0: 200d 0a20 2020 313a 2030 2e32 3530 0d0a   ..   1: 0.250..
+00000bf0: 2020 2032 3a20 302e 3235 0d0a 2020 2033     2: 0.25..   3
+00000c00: 3a20 302e 3031 3530 300d 0a20 2020 343a  : 0.01500..   4:
+00000c10: 2031 3030 0d0a 2020 2035 3a20 312e 3230   100..   5: 1.20
+00000c20: 0d0a 2020 2036 3a20 302e 3031 3030 300d  ..   6: 0.01000.
+00000c30: 0a20 2020 373a 2031 300d 0a20 2020 383a  .   7: 10..   8:
+00000c40: 2030 2e31 3030 300d 0a20 2020 393a 2030   0.1000..   9: 0
+00000c50: 2e35 3030 0d0a 0d0a 2020 2061 646a 6163  .500....   adjac
+00000c60: 656e 745f 6c69 7374 3a0d 0a20 2020 303a  ent_list:..   0:
+00000c70: 205b 315d 0d0a 2020 2031 3a20 5b32 2c20   [1]..   1: [2, 
+00000c80: 332c 2034 5d0d 0a20 2020 323a 205b 355d  3, 4]..   2: [5]
+00000c90: 0d0a 2020 2033 3a20 5b36 2c20 375d 0d0a  ..   3: [6, 7]..
+00000ca0: 2020 2034 3a20 5b38 5d0d 0a20 2020 353a     4: [8]..   5:
+00000cb0: 205b 395d 0d0a 2020 2036 3a20 5b39 5d0d   [9]..   6: [9].
+00000cc0: 0a20 2020 373a 205b 395d 0d0a 2020 2038  .   7: [9]..   8
+00000cd0: 3a20 5b39 5d0d 0a20 2020 393a 205b 3130  : [9]..   9: [10
+00000ce0: 5d0d 0a0d 0a20 2020 6275 6666 6572 5f73  ]....   buffer_s
+00000cf0: 697a 655f 666f 725f 6561 6368 5f71 7565  ize_for_each_que
+00000d00: 7565 3a20 0d0a 2020 2030 3a20 3530 3030  ue: ..   0: 5000
+00000d10: 0d0a 2020 2031 3a20 3530 3030 0d0a 2020  ..   1: 5000..  
+00000d20: 2032 3a20 3530 3030 0d0a 2020 2033 3a20   2: 5000..   3: 
+00000d30: 3530 3030 0d0a 2020 2034 3a20 3530 3030  5000..   4: 5000
+00000d40: 0d0a 2020 2035 3a20 3530 3030 0d0a 2020  ..   5: 5000..  
+00000d50: 2036 3a20 3530 3030 0d0a 2020 2037 3a20   6: 5000..   7: 
+00000d60: 3530 3030 0d0a 2020 2038 3a20 3530 3030  5000..   8: 5000
+00000d70: 0d0a 2020 2039 3a20 3530 3030 0d0a 2020  ..   9: 5000..  
+00000d80: 2031 303a 2035 3030 300d 0a20 2020 3131   10: 5000..   11
+00000d90: 3a20 3530 3030 0d0a 2020 2031 323a 2035  : 5000..   12: 5
+00000da0: 3030 300d 0a0d 0a20 2020 7472 616e 7369  000....   transi
+00000db0: 7469 6f6e 5f70 726f 6261 5f61 6c6c 3a0d  tion_proba_all:.
+00000dc0: 0a20 2020 303a 207b 313a 2031 7d0d 0a20  .   0: {1: 1}.. 
+00000dd0: 2020 313a 207b 323a 2030 2e33 332c 2033    1: {2: 0.33, 3
+00000de0: 3a20 302e 3333 2c20 343a 2030 2e33 347d  : 0.33, 4: 0.34}
+00000df0: 0d0a 2020 2032 3a20 7b35 3a20 317d 0d0a  ..   2: {5: 1}..
+00000e00: 2020 2033 3a20 7b36 3a20 302e 352c 2037     3: {6: 0.5, 7
+00000e10: 3a20 302e 357d 0d0a 2020 2034 3a20 7b38  : 0.5}..   4: {8
+00000e20: 3a20 317d 0d0a 2020 2035 3a20 7b39 3a20  : 1}..   5: {9: 
+00000e30: 317d 0d0a 2020 2036 3a20 7b39 3a20 317d  1}..   6: {9: 1}
+00000e40: 0d0a 2020 2037 3a20 7b39 3a20 317d 0d0a  ..   7: {9: 1}..
+00000e50: 2020 2038 3a20 7b39 3a20 317d 0d0a 2020     8: {9: 1}..  
+00000e60: 2039 3a20 7b31 303a 2031 7d0d 0a20 2020   9: {10: 1}..   
+00000e70: 0d0a 2020 2061 6374 6976 655f 6361 703a  ..   active_cap:
+00000e80: 2035 0d0a 0d0a 2020 2064 6561 6374 6976   5....   deactiv
+00000e90: 655f 743a 2030 2e31 320d 0a0d 0a20 2020  e_t: 0.12....   
+00000ea0: 6172 7269 7661 6c5f 7261 7465 3a20 5b30  arrival_rate: [0
+00000eb0: 2e33 5d0d 0a0d 0a20 2020 6d61 785f 6167  .3]....   max_ag
+00000ec0: 656e 7473 3a20 696e 660d 0a0d 0a20 2020  ents: inf....   
+00000ed0: 7369 6d5f 6a6f 6273 3a20 3130 300d 0a0d  sim_jobs: 100...
+00000ee0: 0a20 2020 6d61 785f 6172 725f 7261 7465  .   max_arr_rate
+00000ef0: 5f6c 6973 743a 205b 302e 335d 0d0a 0d0a  _list: [0.3]....
+00000f00: 2020 2065 6e74 7279 5f6e 6f64 6573 3a0d     entry_nodes:.
+00000f10: 0a20 2020 2d20 5b30 2c20 315d 200d 0a20  .   - [0, 1] .. 
+00000f20: 2020 6060 600d 0a0d 0a23 2323 2320 2a2a    ```....#### **
+00000f30: 524c 2045 6e76 6972 6f6e 6d65 6e74 2050  RL Environment P
+00000f40: 6172 616d 6574 6572 732a 2a0d 0a0d 0a53  arameters**....S
+00000f50: 6574 2075 7020 7468 6520 524c 2065 6e76  et up the RL env
+00000f60: 6972 6f6e 6d65 6e74 2070 6172 616d 6574  ironment paramet
+00000f70: 6572 7320 696e 2060 6576 616c 5f68 7970  ers in `eval_hyp
+00000f80: 6572 7061 7261 6d73 2e79 6d6c 603a 0d0a  erparams.yml`:..
+00000f90: 0d0a 2d20 606e 756d 5f65 7069 736f 6465  ..- `num_episode
+00000fa0: 7360 3a20 5468 6520 6e75 6d62 6572 206f  s`: The number o
+00000fb0: 6620 6570 6973 6f64 6573 2074 6f20 7275  f episodes to ru
+00000fc0: 6e20 7468 6520 7369 6d75 6c61 7469 6f6e  n the simulation
+00000fd0: 2e0d 0a2d 2060 6e75 6d5f 6570 6f63 6873  ...- `num_epochs
+00000fe0: 603a 2054 6865 206e 756d 6265 7220 6f66  `: The number of
+00000ff0: 2065 706f 6368 7320 666f 7220 7472 6169   epochs for trai
+00001000: 6e69 6e67 2e0d 0a2d 2060 7469 6d65 5f73  ning...- `time_s
+00001010: 7465 7073 603a 2054 6865 206e 756d 6265  teps`: The numbe
+00001020: 7220 6f66 2074 696d 6520 7374 6570 7320  r of time steps 
+00001030: 696e 2065 6163 6820 6570 6973 6f64 652e  in each episode.
+00001040: 0d0a 2d20 6062 6174 6368 5f73 697a 6560  ..- `batch_size`
+00001050: 3a20 5369 7a65 206f 6620 7468 6520 6261  : Size of the ba
+00001060: 7463 6820 7573 6564 2069 6e20 7472 6169  tch used in trai
+00001070: 6e69 6e67 2e20 2844 6566 6175 6c74 2069  ning. (Default i
+00001080: 7320 6571 7561 6c20 746f 2074 696d 655f  s equal to time_
+00001090: 7374 6570 7329 0d0a 2d20 606e 756d 5f73  steps)..- `num_s
+000010a0: 696d 603a 2054 6865 206e 756d 6265 7220  im`: The number 
+000010b0: 6f66 2073 696d 756c 6174 696f 6e73 2074  of simulations t
+000010c0: 6f20 7275 6e20 6475 7269 6e67 2074 7261  o run during tra
+000010d0: 696e 696e 672e 0d0a 2d20 6074 6175 603a  ining...- `tau`:
+000010e0: 2043 6f65 6666 6963 6965 6e74 2066 6f72   Coefficient for
+000010f0: 2073 6f66 7420 7570 6461 7465 206f 6620   soft update of 
+00001100: 7468 6520 7461 7267 6574 2070 6172 616d  the target param
+00001110: 6574 6572 732e 0d0a 2d20 6061 6374 6f72  eters...- `actor
+00001120: 5f6c 7260 3a20 4c65 6172 6e69 6e67 2072  _lr`: Learning r
+00001130: 6174 6520 666f 7220 7468 6520 4163 746f  ate for the Acto
+00001140: 7220 6e65 7477 6f72 6b20 6f70 7469 6d69  r network optimi
+00001150: 7a65 722e 0d0a 2d20 6063 7269 7469 635f  zer...- `critic_
+00001160: 6c72 603a 204c 6561 726e 696e 6720 7261  lr`: Learning ra
+00001170: 7465 2066 6f72 2074 6865 2043 7269 7469  te for the Criti
+00001180: 6320 4e65 7477 6f72 6b20 6f70 7469 6d69  c Network optimi
+00001190: 7a65 722e 0d0a 2d20 6064 6973 636f 756e  zer...- `discoun
+000011a0: 7460 3a20 4469 7363 6f75 6e74 2066 6163  t`: Discount fac
+000011b0: 746f 7220 666f 7220 6675 7475 7265 2072  tor for future r
+000011c0: 6577 6172 6473 2e0d 0a2d 2060 706c 616e  ewards...- `plan
+000011d0: 6e69 6e67 5f73 7465 7073 603a 2054 6865  ning_steps`: The
+000011e0: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
+000011f0: 2064 7572 696e 6720 706c 616e 6e69 6e67   during planning
+00001200: 2e0d 0a2d 2060 706c 616e 6e69 6e67 5f73  ...- `planning_s
+00001210: 7464 603a 2053 7461 6e64 6172 6420 6465  td`: Standard de
+00001220: 7669 6174 696f 6e20 6f66 2074 6865 206e  viation of the n
+00001230: 6f72 6d61 6c20 6469 7374 7572 6261 6e63  ormal disturbanc
+00001240: 6520 6475 7269 6e67 2070 6c61 6e6e 696e  e during plannin
+00001250: 672e 0d0a 2d20 6061 6374 6f72 5f6e 6574  g...- `actor_net
+00001260: 776f 726b 603a 204e 6574 776f 726b 2061  work`: Network a
+00001270: 7263 6869 7465 6374 7572 6520 666f 7220  rchitecture for 
+00001280: 6163 746f 7220 6e65 7477 6f72 6b2e 0d0a  actor network...
+00001290: 2d20 6063 7269 7469 635f 6e65 7477 6f72  - `critic_networ
+000012a0: 6b60 3a20 4e65 7477 6f72 6b20 6172 6368  k`: Network arch
+000012b0: 6974 6563 7475 7265 2066 6f72 2063 7269  itecture for cri
+000012c0: 7469 6320 6e65 7477 6f72 6b2e 0d0a 2d20  tic network...- 
+000012d0: 6072 6577 6172 645f 6d6f 6465 6c60 3a20  `reward_model`: 
+000012e0: 4e65 7477 6f72 6b20 6172 6368 6974 6563  Network architec
+000012f0: 7475 7265 2066 6f72 2072 6577 6172 6420  ture for reward 
+00001300: 6d6f 6465 6c20 7573 6420 696e 2070 6c61  model usd in pla
+00001310: 6e6e 696e 672e 0d0a 6020 606e 6578 745f  nning...` `next_
+00001320: 7374 6174 655f 6d6f 6465 6c60 3a20 4e65  state_model`: Ne
+00001330: 7477 6f72 6b20 6172 6368 6974 6563 7475  twork architectu
+00001340: 7265 2066 6f72 206e 6578 7420 7374 6174  re for next stat
+00001350: 6520 6d6f 6465 6c20 7573 6564 2069 6e20  e model used in 
+00001360: 706c 616e 6e69 6e67 2e20 0d0a 0d0a 2020  planning. ....  
+00001370: 2045 7861 6d70 6c65 3a0d 0a20 2020 6060   Example:..   ``
+00001380: 6079 616d 6c0d 0a20 2020 6e75 6d5f 6570  `yaml..   num_ep
+00001390: 6973 6f64 6573 3a20 350d 0a0d 0a20 2020  isodes: 5....   
+000013a0: 7468 7265 7368 6f6c 643a 2031 300d 0a0d  threshold: 10...
+000013b0: 0a20 2020 6e75 6d5f 6570 6f63 6873 3a20  .   num_epochs: 
+000013c0: 3130 300d 0a0d 0a20 2020 7469 6d65 5f73  100....   time_s
+000013d0: 7465 7073 3a20 3330 0d0a 0d0a 2020 2062  teps: 30....   b
+000013e0: 6174 6368 5f73 697a 653a 2033 300d 0a20  atch_size: 30.. 
+000013f0: 2020 0d0a 2020 2074 6172 6765 745f 7570    ..   target_up
+00001400: 6461 7465 5f66 7265 7175 656e 6379 3a20  date_frequency: 
+00001410: 3130 300d 0a20 2020 0d0a 2020 2062 7566  100..   ..   buf
+00001420: 6665 725f 7369 7a65 3a20 3130 3030 300d  fer_size: 10000.
+00001430: 0a20 2020 0d0a 2020 206e 756d 5f73 696d  .   ..   num_sim
+00001440: 3a20 3130 0d0a 2020 200d 0a20 2020 7461  : 10..   ..   ta
+00001450: 753a 2030 2e35 0d0a 0d0a 2020 206e 756d  u: 0.5....   num
+00001460: 5f74 7261 696e 5f41 433a 2031 300d 0a20  _train_AC: 10.. 
+00001470: 2020 0d0a 2020 2063 7269 7469 635f 6c72    ..   critic_lr
+00001480: 3a20 302e 3031 0d0a 0d0a 2020 2061 6374  : 0.01....   act
+00001490: 6f72 5f6c 723a 2030 2e30 3030 310d 0a20  or_lr: 0.0001.. 
+000014a0: 2020 0d0a 2020 2064 6973 636f 756e 743a    ..   discount:
+000014b0: 2030 2e38 0d0a 2020 200d 0a20 2020 706c   0.8..   ..   pl
+000014c0: 616e 6e69 6e67 5f73 7465 7073 3a20 3130  anning_steps: 10
+000014d0: 0d0a 2020 200d 0a20 2020 706c 616e 6e69  ..   ..   planni
+000014e0: 6e67 5f73 7464 3a20 302e 310d 0a0d 0a20  ng_std: 0.1.... 
+000014f0: 2020 6163 746f 725f 6e65 7477 6f72 6b3a    actor_network:
+00001500: 0d0a 2020 202d 2036 340d 0a20 2020 2d20  ..   - 64..   - 
+00001510: 3634 0d0a 2020 202d 2036 340d 0a0d 0a20  64..   - 64.... 
+00001520: 2020 6372 6974 6963 3a0d 0a20 2020 2d20    critic:..   - 
+00001530: 3634 0d0a 2020 202d 2036 340d 0a20 2020  64..   - 64..   
+00001540: 2d20 3634 0d0a 0d0a 2020 2072 6577 6172  - 64....   rewar
+00001550: 645f 6d6f 6465 6c3a 0d0a 2020 202d 2033  d_model:..   - 3
+00001560: 320d 0a20 2020 2d20 3634 0d0a 2020 202d  2..   - 64..   -
+00001570: 2036 340d 0a20 2020 2d20 3332 0d0a 0d0a   64..   - 32....
+00001580: 2020 206e 6578 745f 7374 6174 655f 6d6f     next_state_mo
+00001590: 6465 6c3a 0d0a 2020 202d 2033 320d 0a20  del:..   - 32.. 
+000015a0: 2020 2d20 3634 0d0a 2020 202d 2036 340d    - 64..   - 64.
+000015b0: 0a20 2020 2d20 3332 0d0a 2020 2060 6060  .   - 32..   ```
+000015c0: 0d0a 0d0a 2323 2323 202a 2a54 756e 696e  ....#### **Tunin
+000015d0: 6720 436f 6e66 6967 7572 6174 696f 6e2a  g Configuration*
+000015e0: 2a0d 0a53 6574 2075 7020 7468 6520 6879  *..Set up the hy
+000015f0: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
+00001600: 696e 6720 7261 6e67 6573 2069 6e20 6074  ing ranges in `t
+00001610: 756e 696e 675f 7061 7261 6d73 2e79 6d6c  uning_params.yml
+00001620: 603a 0d0a 0d0a 2d20 606c 725f 6d69 6e2f  `:....- `lr_min/
+00001630: 6d61 7860 3a20 4d69 6e20 616e 6420 6d61  max`: Min and ma
+00001640: 7820 7261 6e67 6573 206f 6620 7468 6520  x ranges of the 
+00001650: 6c65 6172 6e69 6e67 2072 6174 6520 6265  learning rate be
+00001660: 696e 6720 7475 6e65 642e 0d0a 2d20 6065  ing tuned...- `e
+00001670: 706f 6368 735f 6c69 7374 603a 2041 206c  pochs_list`: A l
+00001680: 6973 7420 7468 6174 2064 6566 696e 6573  ist that defines
+00001690: 2074 6865 2072 616e 6765 206f 6620 706f   the range of po
+000016a0: 7373 6962 6c65 2065 706f 6368 7320 746f  ssible epochs to
+000016b0: 2074 7261 696e 2072 6577 6172 6420 6d6f   train reward mo
+000016c0: 6465 6c20 616e 6420 6e65 7874 2073 7461  del and next sta
+000016d0: 7465 206d 6f64 656c 2e0d 0a2d 2060 6261  te model...- `ba
+000016e0: 7463 685f 7369 7a65 603a 2041 206c 6973  tch_size`: A lis
+000016f0: 7420 7468 6174 2064 6566 696e 6573 2074  t that defines t
+00001700: 6865 2072 616e 6765 206f 6620 6261 7463  he range of batc
+00001710: 6820 7369 7a65 7320 746f 2073 616d 706c  h sizes to sampl
+00001720: 6520 6672 6f6d 2074 6865 2072 6570 6c61  e from the repla
+00001730: 7920 6275 6666 6572 2e0d 0a2d 2060 7461  y buffer...- `ta
+00001740: 755f 6d69 6e2f 6d61 7860 3a20 4d69 6e20  u_min/max`: Min 
+00001750: 616e 6420 6d61 7820 7261 6e67 6573 206f  and max ranges o
+00001760: 6620 7468 6520 736f 6674 2075 7064 6174  f the soft updat
+00001770: 6520 7061 7261 6d65 7465 7273 2e0d 0a2d  e parameters...-
+00001780: 2060 6469 7363 6f75 6e74 206d 696e 2f6d   `discount min/m
+00001790: 6178 603a 204d 696e 2061 6e64 206d 6178  ax`: Min and max
+000017a0: 2072 616e 6765 7320 6f66 2074 6865 2064   ranges of the d
+000017b0: 6973 636f 756e 7420 6661 6374 6f72 2066  iscount factor f
+000017c0: 6f72 2066 7574 7572 6520 7265 7761 7264  or future reward
+000017d0: 732e 0d0a 2d20 6065 7073 696c 6f6e 5f6d  s...- `epsilon_m
+000017e0: 696e 2f6d 6178 603a 204d 696e 2061 6e64  in/max`: Min and
+000017f0: 206d 6178 2072 616e 6765 7320 6f66 2074   max ranges of t
+00001800: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
+00001810: 6174 696f 6e20 6f66 206e 6f72 6d61 6c20  ation of normal 
+00001820: 6469 7374 7572 6261 6e63 6573 2064 7572  disturbances dur
+00001830: 696e 6720 706c 616e 6e69 6e67 2e0d 0a2d  ing planning...-
+00001840: 2060 706c 616e 6e69 6e67 5f73 7465 7073   `planning_steps
+00001850: 603a 2041 206c 6973 7420 7468 6174 2064  `: A list that d
+00001860: 6566 696e 6573 2070 6f73 7369 626c 6520  efines possible 
+00001870: 7374 6570 7320 666f 7220 706c 616e 6e69  steps for planni
+00001880: 6e67 2e0d 0a2d 2060 7731 2f77 3260 3a20  ng...- `w1/w2`: 
+00001890: 5765 6967 6874 2070 6172 616d 6574 6572  Weight parameter
+000018a0: 7320 7468 6174 2069 6e66 6c75 656e 6365  s that influence
+000018b0: 2074 6865 2065 7870 6c6f 7261 7469 6f6e   the exploration
+000018c0: 2062 6574 7765 656e 206b 6579 2061 6e64   between key and
+000018d0: 2070 6572 6970 6865 7261 6c20 7374 6174   peripheral stat
+000018e0: 6573 2e0d 0a2d 2060 6e75 6d5f 6570 6973  es...- `num_epis
+000018f0: 6f64 6573 603a 2041 206c 6973 7420 7468  odes`: A list th
+00001900: 6174 2064 6566 696e 6573 2074 6865 2070  at defines the p
+00001910: 6f73 7369 626c 6520 6e75 6d62 6572 7320  ossible numbers 
+00001920: 6f66 2065 7069 736f 6465 7320 746f 2074  of episodes to t
+00001930: 7261 696e 2074 6865 2061 6765 6e74 732e  rain the agents.
+00001940: 0d0a 2d20 6074 696d 655f 7374 6570 7360  ..- `time_steps`
+00001950: 3a20 4120 6c69 7374 2074 6861 7420 6465  : A list that de
+00001960: 6669 6e65 7320 7468 6520 706f 7373 6962  fines the possib
+00001970: 6c65 206e 756d 6265 7220 6f66 2074 696d  le number of tim
+00001980: 6520 7374 6570 7320 6475 7269 6e67 2065  e steps during e
+00001990: 6163 6820 6570 6973 6f64 650d 0a0d 0a20  ach episode.... 
+000019a0: 2020 4578 616d 706c 653a 0d0a 2020 2060    Example:..   `
+000019b0: 6060 7961 6d6c 0d0a 2020 206c 6561 726e  ``yaml..   learn
+000019c0: 696e 675f 7261 7465 5f6d 6178 3a20 302e  ing_rate_max: 0.
+000019d0: 310d 0a20 2020 6c65 6172 6e69 6e67 5f72  1..   learning_r
+000019e0: 6174 655f 6d69 6e3a 2030 2e30 3031 0d0a  ate_min: 0.001..
+000019f0: 0d0a 2020 2065 706f 6368 735f 6c69 7374  ..   epochs_list
+00001a00: 3a0d 0a20 2020 2d20 3130 0d0a 2020 202d  :..   - 10..   -
+00001a10: 2031 300d 0a20 2020 2d20 3130 0d0a 0d0a   10..   - 10....
+00001a20: 2020 2062 6174 6368 5f73 697a 653a 0d0a     batch_size:..
+00001a30: 2020 202d 2031 360d 0a20 2020 2d20 3332     - 16..   - 32
+00001a40: 0d0a 2020 202d 2036 340d 0a0d 0a20 2020  ..   - 64....   
+00001a50: 7461 755f 6d69 6e3a 2030 2e30 3030 350d  tau_min: 0.0005.
+00001a60: 0a20 2020 7461 755f 6d61 783a 2030 2e30  .   tau_max: 0.0
+00001a70: 3032 0d0a 0d0a 2020 2064 6973 636f 756e  02....   discoun
+00001a80: 745f 6d69 6e3a 2030 2e31 0d0a 2020 2064  t_min: 0.1..   d
+00001a90: 6973 636f 756e 745f 6d61 783a 2030 2e33  iscount_max: 0.3
+00001aa0: 0d0a 0d0a 2020 2065 7073 696c 6f6e 5f6d  ....   epsilon_m
+00001ab0: 696e 3a20 302e 310d 0a20 2020 6570 7369  in: 0.1..   epsi
+00001ac0: 6c6f 6e5f 6d61 783a 2030 2e33 0d0a 0d0a  lon_max: 0.3....
+00001ad0: 2020 2070 6c61 6e6e 696e 675f 7374 6570     planning_step
+00001ae0: 733a 200d 0a20 2020 2d20 3130 0d0a 0d0a  s: ..   - 10....
+00001af0: 2020 206e 756d 5f73 616d 706c 653a 200d     num_sample: .
+00001b00: 0a20 2020 2d20 3530 0d0a 0d0a 2020 2077  .   - 50....   w
+00001b10: 313a 200d 0a20 2020 2d20 302e 350d 0a0d  1: ..   - 0.5...
+00001b20: 0a20 2020 7732 3a20 0d0a 2020 202d 2030  .   w2: ..   - 0
+00001b30: 2e35 0d0a 0d0a 2020 206e 756d 5f65 7069  .5....   num_epi
+00001b40: 736f 6465 733a 200d 0a20 2020 2d20 350d  sodes: ..   - 5.
+00001b50: 0a0d 0a20 2020 7469 6d65 5f73 7465 7073  ...   time_steps
+00001b60: 3a20 0d0a 2020 202d 2031 300d 0a20 2020  : ..   - 10..   
+00001b70: 0d0a 2020 206e 756d 5f74 7261 696e 5f41  ..   num_train_A
+00001b80: 433a 200d 0a20 2020 2d20 3130 0d0a 0d0a  C: ..   - 10....
+00001b90: 2020 2060 6060 0d0a 0d0a 2323 2053 7465     ```....## Ste
+00001ba0: 7020 323a 2052 756e 6e69 6e67 2053 696d  p 2: Running Sim
+00001bb0: 756c 6174 696f 6e73 0d0a 0d0a 2323 2320  ulations....### 
+00001bc0: 5472 6169 6e69 6e67 2041 6765 6e74 0d0a  Training Agent..
+00001bd0: 5468 6973 2063 6f6d 6d61 6e64 2073 7461  This command sta
+00001be0: 7274 7320 7472 6169 6e69 6e67 2074 6865  rts training the
+00001bf0: 2061 6765 6e74 2077 6974 6869 6e20 7468   agent within th
+00001c00: 6520 7369 6d75 6c61 7465 6420 7175 6575  e simulated queu
+00001c10: 6569 6e67 2065 6e76 6972 6f6e 6d65 6e74  eing environment
+00001c20: 2e20 5265 7375 6c74 7320 6172 6520 7361  . Results are sa
+00001c30: 7665 6420 696e 2060 2f66 6f75 6e64 6174  ved in `/foundat
+00001c40: 696f 6e73 2f6f 7574 7075 745f 6373 7660  ions/output_csv`
+00001c50: 2061 6e64 2060 2f66 6f75 6e64 6174 696f   and `/foundatio
+00001c60: 6e73 2f6f 7574 7075 745f 706c 6f74 7360  ns/output_plots`
+00001c70: 2e0d 0a0d 0a60 6060 6261 7368 0d0a 7079  .....```bash..py
+00001c80: 7468 6f6e 206d 6169 6e2e 7079 202d 2d66  thon main.py --f
+00001c90: 756e 6374 696f 6e20 7472 6169 6e20 2d2d  unction train --
+00001ca0: 636f 6e66 6967 5f66 696c 6520 7573 6572  config_file user
+00001cb0: 5f63 6f6e 6669 672f 636f 6e66 6967 7572  _config/configur
+00001cc0: 6174 696f 6e2e 796d 6c20 2d2d 7061 7261  ation.yml --para
+00001cd0: 6d5f 6669 6c65 2075 7365 725f 636f 6e66  m_file user_conf
+00001ce0: 6967 2f65 7661 6c5f 6879 7065 7270 6172  ig/eval_hyperpar
+00001cf0: 616d 732e 796d 6c20 2d2d 6461 7461 5f66  ams.yml --data_f
+00001d00: 696c 6520 6f75 7470 7574 5f63 7376 202d  ile output_csv -
+00001d10: 2d69 6d61 6765 5f66 696c 6520 6f75 7470  -image_file outp
+00001d20: 7574 5f70 6c6f 7473 202d 2d70 6c6f 745f  ut_plots --plot_
+00001d30: 6375 7276 6573 2054 7275 6520 2d2d 7361  curves True --sa
+00001d40: 7665 5f66 696c 6520 5472 7565 0d0a 6060  ve_file True..``
+00001d50: 600d 0a0d 0a23 2323 2048 7970 6572 7061  `....### Hyperpa
+00001d60: 7261 6d65 7465 7220 5475 6e69 6e67 0d0a  rameter Tuning..
+00001d70: 0d0a 4265 6c6f 7720 7072 6f76 6964 6573  ..Below provides
+00001d80: 2075 7365 7273 2074 776f 2074 7970 6573   users two types
+00001d90: 206f 6620 7475 6e69 6e67 2073 7472 6174   of tuning strat
+00001da0: 6567 6965 7320 7468 6174 2066 6561 7475  egies that featu
+00001db0: 7265 2064 6966 6665 7265 6e74 2066 756e  re different fun
+00001dc0: 6374 696f 6e61 6c69 7469 6573 2e0d 0a0d  ctionalities....
+00001dd0: 0a23 2323 2320 2a2a 5761 6e64 6220 5475  .#### **Wandb Tu
+00001de0: 6e69 6e67 2a2a 0d0a 0d0a 4120 6d61 6368  ning**....A mach
+00001df0: 696e 6520 6c65 6172 6e69 6e67 2064 6576  ine learning dev
+00001e00: 656c 6f70 6d65 6e74 2070 6c61 7466 6f72  elopment platfor
+00001e10: 6d20 7468 6174 2061 6c6c 6f77 7320 7573  m that allows us
+00001e20: 6572 7320 746f 2074 7261 636b 2061 6e64  ers to track and
+00001e30: 2076 6973 7561 6c69 7a65 2076 6172 6f75   visualize varou
+00001e40: 2061 7370 6563 7473 206f 6620 7468 6569   aspects of thei
+00001e50: 7220 6d6f 6465 6c20 7472 6169 6e69 6e67  r model training
+00001e60: 2070 726f 6365 7373 2069 6e20 7265 616c   process in real
+00001e70: 2d74 696d 652c 2069 6e63 6c75 6469 6e67  -time, including
+00001e80: 206c 6f73 7320 616e 6420 6163 6375 7261   loss and accura
+00001e90: 6379 2063 6861 7274 732c 2070 6172 616d  cy charts, param
+00001ea0: 6574 6572 2064 6973 7472 6962 7574 696f  eter distributio
+00001eb0: 6e73 2c20 6772 6164 6965 6e74 2068 6973  ns, gradient his
+00001ec0: 746f 6772 616d 7320 616e 6420 7379 7374  tograms and syst
+00001ed0: 656d 206d 6574 7269 6373 2e20 546f 2072  em metrics. To r
+00001ee0: 756e 2077 616e 6462 3a0d 0a0d 0a60 6060  un wandb:....```
+00001ef0: 6261 7368 0d0a 7079 7468 6f6e 206d 6169  bash..python mai
+00001f00: 6e2e 7079 202d 2d66 756e 6374 696f 6e20  n.py --function 
+00001f10: 7475 6e65 202d 2d63 6f6e 6669 675f 6669  tune --config_fi
+00001f20: 6c65 2075 7365 725f 636f 6e66 6967 2f63  le user_config/c
+00001f30: 6f6e 6669 6775 7261 7469 6f6e 2e79 6d6c  onfiguration.yml
+00001f40: 202d 2d70 6172 616d 5f66 696c 6520 7573   --param_file us
+00001f50: 6572 5f63 6f6e 6669 672f 6576 616c 5f68  er_config/eval_h
+00001f60: 7970 6572 7061 7261 6d73 2e79 6d6c 202d  yperparams.yml -
+00001f70: 2d64 6174 615f 6669 6c65 206f 7574 7075  -data_file outpu
+00001f80: 745f 6373 7620 2d2d 696d 6167 655f 6669  t_csv --image_fi
+00001f90: 6c65 206f 7574 7075 745f 706c 6f74 7320  le output_plots 
+00001fa0: 2d2d 706c 6f74 5f63 7572 7665 7320 5472  --plot_curves Tr
+00001fb0: 7565 202d 2d73 6176 655f 6669 6c65 2054  ue --save_file T
+00001fc0: 7275 6520 2d2d 7475 6e65 7220 7761 6e64  rue --tuner wand
+00001fd0: 6220 0d0a 6060 600d 0a0d 0a23 2323 2320  b ..```....#### 
+00001fe0: 2a2a 5261 7920 5475 6e69 6e67 2a2a 0d0a  **Ray Tuning**..
+00001ff0: 0d0a 416e 2069 6e64 7573 7472 7920 7374  ..An industry st
+00002000: 616e 6461 7264 2074 6f6f 6c20 666f 7220  andard tool for 
+00002010: 6469 7374 7269 6275 7465 6420 6879 7065  distributed hype
+00002020: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
+00002030: 6720 7768 6963 6820 696e 7465 6772 6174  g which integrat
+00002040: 6573 2077 6974 6820 5465 6e73 6f72 426f  es with TensorBo
+00002050: 6172 6420 616e 6420 6578 7465 6e73 6976  ard and extensiv
+00002060: 6520 616e 616c 7973 6973 206c 6962 7261  e analysis libra
+00002070: 7269 6573 2e20 4974 2061 6c73 6f20 616c  ries. It also al
+00002080: 6c6f 7773 2075 7365 7273 2074 6f20 6c65  lows users to le
+00002090: 7665 7261 6765 2063 7574 7469 6e67 2065  verage cutting e
+000020a0: 6467 6520 6f70 7469 6d69 7a61 7469 6f6e  dge optimization
+000020b0: 2061 6c67 6f72 6974 686d 7320 6174 2073   algorithms at s
+000020c0: 6361 6c65 2c20 696e 636c 7564 696e 6720  cale, including 
+000020d0: 4261 7965 7369 616e 204f 7074 696d 697a  Bayesian Optimiz
+000020e0: 6174 696f 6e2c 2050 6f70 756c 6174 696f  ation, Populatio
+000020f0: 6e20 4261 7365 6420 5472 6169 6e69 6e67  n Based Training
+00002100: 2061 6e64 2048 7970 6572 4261 6e64 2e20   and HyperBand. 
+00002110: 546f 2072 756e 2072 6179 2074 756e 696e  To run ray tunin
+00002120: 673a 0d0a 0d0a 6060 6062 6173 680d 0a70  g:....```bash..p
+00002130: 7974 686f 6e20 6d61 696e 2e70 7920 2d2d  ython main.py --
+00002140: 6675 6e63 7469 6f6e 2074 756e 6520 2d2d  function tune --
+00002150: 636f 6e66 6967 5f66 696c 6520 7573 6572  config_file user
+00002160: 5f63 6f6e 6669 672f 636f 6e66 6967 7572  _config/configur
+00002170: 6174 696f 6e2e 796d 6c20 2d2d 7061 7261  ation.yml --para
+00002180: 6d5f 6669 6c65 2075 7365 725f 636f 6e66  m_file user_conf
+00002190: 6967 2f65 7661 6c5f 6879 7065 7270 6172  ig/eval_hyperpar
+000021a0: 616d 732e 796d 6c20 2d2d 6461 7461 5f66  ams.yml --data_f
+000021b0: 696c 6520 6f75 7470 7574 5f63 7376 202d  ile output_csv -
+000021c0: 2d69 6d61 6765 5f66 696c 6520 6f75 7470  -image_file outp
+000021d0: 7574 5f70 6c6f 7473 202d 2d70 6c6f 745f  ut_plots --plot_
+000021e0: 6375 7276 6573 2054 7275 6520 2d2d 7361  curves True --sa
+000021f0: 7665 5f66 696c 6520 5472 7565 202d 2d74  ve_file True --t
+00002200: 756e 6572 2072 6179 5f74 756e 650d 0a60  uner ray_tune..`
+00002210: 6060 0d0a 0d0a 2323 2053 7465 7020 333a  ``....## Step 3:
+00002220: 2045 7870 6c6f 7265 2046 6561 7475 7265   Explore Feature
+00002230: 730d 0a0d 0a23 2323 2031 2e20 2a2a 4578  s....### 1. **Ex
+00002240: 706c 6f72 6520 4272 6561 6b64 6f77 6e20  plore Breakdown 
+00002250: 5363 656e 6172 696f 732a 2a0d 0a0d 0a54  Scenarios**....T
+00002260: 6869 7320 6665 6174 7572 6520 616c 6c6f  his feature allo
+00002270: 7773 2074 6865 2075 7365 7220 746f 2074  ws the user to t
+00002280: 7261 696e 2074 6865 2061 6765 6e74 2062  rain the agent b
+00002290: 6173 6564 206f 6e20 6375 7374 6f6d 6564  ased on customed
+000022a0: 2065 7870 6c6f 7261 7469 6f6e 2070 7265   exploration pre
+000022b0: 6665 7265 6e63 6573 2062 6574 7765 656e  ferences between
+000022c0: 206b 6579 2073 7461 7465 7320 616e 6420   key states and 
+000022d0: 7065 7269 7068 6572 616c 2073 7461 7465  peripheral state
+000022e0: 7320 7573 696e 6720 7765 6967 6874 2070  s using weight p
+000022f0: 6172 616d 6574 6572 2060 7731 5f6b 6579  arameter `w1_key
+00002300: 6020 616e 6420 6077 325f 7065 7269 7068  ` and `w2_periph
+00002310: 6572 616c 602e 2054 6865 2070 7572 706f  eral`. The purpo
+00002320: 7365 206f 6620 7468 6973 2066 6561 7475  se of this featu
+00002330: 7265 2069 7320 746f 2065 6e61 626c 6520  re is to enable 
+00002340: 7468 6520 6167 656e 7420 746f 206e 6f74  the agent to not
+00002350: 206f 6e6c 7920 6765 6e65 7261 7465 2068   only generate h
+00002360: 6967 6820 7265 7761 7264 7320 666f 7220  igh rewards for 
+00002370: 6b65 7920 7374 6174 6573 2062 7574 2061  key states but a
+00002380: 6c73 6f20 7669 7369 7420 616c 6c20 6272  lso visit all br
+00002390: 6561 646f 776e 2073 6365 6e61 7269 6f73  eadown scenarios
+000023a0: 2073 7566 6669 6369 656e 746c 7920 656e   sufficiently en
+000023b0: 6f75 6768 2e20 0d0a 0d0a 5365 7420 7570  ough. ....Set up
+000023c0: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+000023d0: 696e 2060 7573 6572 5f63 6f6e 6669 675c  in `user_config\
+000023e0: 6665 6174 7572 6573 5f70 6172 616d 735c  features_params\
+000023f0: 626c 6f61 636b 6167 655f 6578 706c 6f72  bloackage_explor
+00002400: 655f 7061 7261 6d73 2e79 6d6c 603a 0d0a  e_params.yml`:..
+00002410: 0d0a 2d20 6077 315f 6b65 7960 3a20 5765  ..- `w1_key`: We
+00002420: 6967 6874 2070 6172 616d 6574 6572 2074  ight parameter t
+00002430: 6f20 636f 6e74 726f 6c20 6661 766f 7220  o control favor 
+00002440: 6578 706c 6f72 696e 6720 6b65 7920 7374  exploring key st
+00002450: 6174 6573 2e0d 0a2d 2060 7732 5f70 6572  ates...- `w2_per
+00002460: 6970 6865 7261 6c60 3a20 5765 6967 6874  ipheral`: Weight
+00002470: 2070 6172 616d 6574 6572 2074 6f20 636f   parameter to co
+00002480: 6e74 726f 6c20 6661 766f 7220 6578 706c  ntrol favor expl
+00002490: 6f72 696e 6720 7065 7269 7068 6572 616c  oring peripheral
+000024a0: 2073 7461 7465 732e 0d0a 2d20 6072 6573   states...- `res
+000024b0: 6574 603a 2041 2062 6f6f 6c20 7661 6c75  et`: A bool valu
+000024c0: 6520 7468 6174 2063 6f6e 7472 6f6c 7320  e that controls 
+000024d0: 7768 6574 6865 7220 746f 2072 6573 6574  whether to reset
+000024e0: 2077 6569 6768 7420 7061 7261 6d65 7465   weight paramete
+000024f0: 7273 2064 7572 696e 6720 7472 6169 6e69  rs during traini
+00002500: 6e67 2e0d 0a2d 2060 7265 7365 745f 6672  ng...- `reset_fr
+00002510: 6571 7565 6e63 7960 3a20 4120 7661 6c75  equency`: A valu
+00002520: 6520 7468 6174 2064 6566 696e 6573 2074  e that defines t
+00002530: 6865 206e 756d 6265 7220 6f66 2065 7069  he number of epi
+00002540: 736f 6465 7320 6672 6571 7565 6e63 7920  sodes frequency 
+00002550: 746f 2072 6573 6574 2074 6865 2077 6569  to reset the wei
+00002560: 6768 7420 7061 7261 6d65 7465 7273 2e0d  ght parameters..
+00002570: 0a2d 2060 6e75 6d5f 6f75 7470 7574 603a  .- `num_output`:
+00002580: 2041 2076 616c 7565 2074 6861 7420 6465   A value that de
+00002590: 6669 6e65 7320 7468 6520 6e75 6d62 6572  fines the number
+000025a0: 206f 6620 746f 7020 616e 6420 6c65 6173   of top and leas
+000025b0: 7420 7265 7761 7264 2f76 6973 6974 7320  t reward/visits 
+000025c0: 7374 6174 6573 2074 6f20 706c 6f74 2069  states to plot i
+000025d0: 6e20 6120 6869 7374 6f67 7261 6d0d 0a2d  n a histogram..-
+000025e0: 2060 6f75 7470 7574 5f6a 736f 6e60 3a20   `output_json`: 
+000025f0: 4120 626f 6f6c 2076 616c 7565 2074 6861  A bool value tha
+00002600: 7420 6465 7465 726d 696e 6573 2077 6865  t determines whe
+00002610: 7468 6572 2074 6f20 6f75 7470 7574 2074  ther to output t
+00002620: 6865 206a 736f 6e20 6669 6c65 206f 6620  he json file of 
+00002630: 6b65 7920 7374 6174 6573 2061 6e64 2070  key states and p
+00002640: 6572 6970 6865 7261 6c20 7374 6174 6573  eripheral states
+00002650: 0d0a 2d20 606f 7574 7075 745f 6869 7374  ..- `output_hist
+00002660: 6f67 7261 6d60 3a20 4120 626f 6f6c 2076  ogram`: A bool v
+00002670: 616c 7565 2074 6861 7420 6465 7465 726d  alue that determ
+00002680: 696e 6573 2077 6865 7468 6572 2074 6f20  ines whether to 
+00002690: 6f75 7470 7574 2074 6865 2068 6973 746f  output the histo
+000026a0: 6772 616d 2074 6861 7420 7368 6f77 7320  gram that shows 
+000026b0: 7468 6520 7265 7761 7264 7320 616e 6420  the rewards and 
+000026c0: 7669 7369 7473 206f 6620 7468 6520 746f  visits of the to
+000026d0: 7020 616e 6420 6c65 6173 7420 7374 6174  p and least stat
+000026e0: 6573 2e0d 0a2d 2060 6f75 7470 7574 5f63  es...- `output_c
+000026f0: 6f76 6572 6167 655f 6d65 7472 6963 603a  overage_metric`:
+00002700: 2041 2062 6f6f 6c20 7661 6c75 6520 7468   A bool value th
+00002710: 6174 2064 6574 6572 6d69 6e65 7320 7768  at determines wh
+00002720: 6574 6865 7220 746f 206f 7574 7075 7420  ether to output 
+00002730: 7468 6520 6375 7272 656e 7420 636f 7665  the current cove
+00002740: 7261 6765 206d 6574 7269 632e 0d0a 0d0a  rage metric.....
+00002750: 546f 2072 756e 2074 6869 7320 6665 6174  To run this feat
+00002760: 7572 652c 206e 6176 6967 6174 6520 746f  ure, navigate to
+00002770: 2060 2f66 6f75 6e64 6174 696f 6e73 2f62   `/foundations/b
+00002780: 7265 616b 646f 776e 5f65 7870 6c6f 7261  reakdown_explora
+00002790: 7469 6f6e 6020 616e 6420 7275 6e3a 0d0a  tion` and run:..
+000027a0: 2020 2060 6060 6261 7368 0d0a 2020 2070     ```bash..   p
+000027b0: 7974 686f 6e20 6272 6561 6b64 6f77 6e5f  ython breakdown_
+000027c0: 6578 706c 6f72 6174 696f 6e2e 7079 0d0a  exploration.py..
+000027d0: 2020 2060 6060 0d0a 0d0a 2323 2320 322e     ```....### 2.
+000027e0: 202a 2a42 6c6f 636b 6167 6520 4465 6d6f   **Blockage Demo
+000027f0: 6e73 7472 6174 696f 6e73 2a2a 0d0a 0d0a  nstrations**....
+00002800: 5468 6973 2066 6561 7475 7265 2061 6c6c  This feature all
+00002810: 6f77 7320 7468 6520 7573 6572 2074 6f20  ows the user to 
+00002820: 7465 7374 2061 2074 7261 696e 6564 2061  test a trained a
+00002830: 6765 6e74 2773 2070 6572 666f 726d 616e  gent's performan
+00002840: 6365 206f 6e20 6120 7369 6d75 6c61 7465  ce on a simulate
+00002850: 6420 7365 7276 6572 2062 6c6f 636b 6167  d server blockag
+00002860: 6520 7175 6575 6569 6e67 2065 6e76 6972  e queueing envir
+00002870: 6f6e 6d65 6e74 2062 7920 7669 7375 616c  onment by visual
+00002880: 697a 696e 6720 7468 6520 6368 616e 6765  izing the change
+00002890: 7320 696e 2074 7261 6e73 6974 696f 6e20  s in transition 
+000028a0: 7072 6f62 6162 696c 6974 6965 732e 2054  probabilities. T
+000028b0: 6865 2070 7572 706f 7365 206f 6620 7468  he purpose of th
+000028c0: 6973 2066 6561 7475 7265 2069 7320 746f  is feature is to
+000028d0: 2073 686f 7720 686f 7720 6566 6665 6374   show how effect
+000028e0: 6963 6520 7468 6520 7472 616e 6965 6420  ice the tranied 
+000028f0: 6167 656e 7420 6973 2061 6374 696e 6720  agent is acting 
+00002900: 6f6e 2062 7265 616b 646f 776e 2063 6173  on breakdown cas
+00002910: 6573 2e20 0d0a 0d0a 5365 7420 7570 2074  es. ....Set up t
+00002920: 6865 2070 6172 616d 6574 6572 7320 696e  he parameters in
+00002930: 2060 7573 6572 5f63 6f6e 6669 675c 6665   `user_config\fe
+00002940: 6174 7572 6573 5f70 6172 616d 735c 626c  atures_params\bl
+00002950: 6f63 6b61 6765 5f64 656d 6f6e 7374 7261  ockage_demonstra
+00002960: 7469 6f6e 5f70 6172 616d 732e 796d 6c60  tion_params.yml`
+00002970: 3a0d 0a0d 0a2d 2060 6e75 6d5f 7369 6d60  :....- `num_sim`
+00002980: 3a20 4465 6669 6e65 7320 7468 6520 6e75  : Defines the nu
+00002990: 6d62 6572 206f 6620 6a6f 6273 2074 6f20  mber of jobs to 
+000029a0: 7369 6d75 6c61 7465 2066 6f72 2065 6163  simulate for eac
+000029b0: 6820 7469 6d65 2073 7465 7020 6475 7269  h time step duri
+000029c0: 6e67 2074 7261 696e 696e 672e 0d0a 2d20  ng training...- 
+000029d0: 6074 696d 655f 7374 6570 7360 3a20 4465  `time_steps`: De
+000029e0: 6669 6e65 7320 7468 6520 6e75 6d62 6572  fines the number
+000029f0: 206f 6620 7469 6d65 2073 7465 7073 2074   of time steps t
+00002a00: 6f20 7065 7266 6f72 6d20 666f 7220 6561  o perform for ea
+00002a10: 6368 2065 7069 736f 6465 2e0d 0a2d 2060  ch episode...- `
+00002a20: 7175 6575 655f 696e 6465 7860 3a20 4465  queue_index`: De
+00002a30: 6669 6e65 7320 7468 6520 7175 6575 6520  fines the queue 
+00002a40: 696e 6465 7820 7468 6174 2072 6563 6f72  index that recor
+00002a50: 6420 7468 6520 6d65 7472 6963 7320 666f  d the metrics fo
+00002a60: 722e 0d0a 2d20 606d 6574 7269 6360 3a20  r...- `metric`: 
+00002a70: 4465 6669 6e65 7320 7468 6520 6d65 7472  Defines the metr
+00002a80: 6963 2074 6f20 6265 2072 6570 6f72 7465  ic to be reporte
+00002a90: 6420 666f 7220 7468 6520 7365 6c65 6374  d for the select
+00002aa0: 6564 2071 7565 7565 2e0d 0a0d 0a54 6f20  ed queue.....To 
+00002ab0: 7573 6520 7468 6973 2066 6561 7475 7265  use this feature
+00002ac0: 2c20 6e61 7669 6761 7465 2074 6f20 602f  , navigate to `/
+00002ad0: 6576 616c 7561 7469 6f6e 2f64 6563 6973  evaluation/decis
+00002ae0: 696f 6e5f 6576 616c 7561 7469 6f6e 6020  ion_evaluation` 
+00002af0: 616e 6420 7275 6e3a 0d0a 2020 2060 6060  and run:..   ```
+00002b00: 6261 7368 0d0a 2020 2070 7974 686f 6e20  bash..   python 
+00002b10: 6465 6369 7369 6f6e 5f65 7661 6c75 6174  decision_evaluat
+00002b20: 696f 6e2e 7079 0d0a 2020 2060 6060 0d0a  ion.py..   ```..
+00002b30: 0d0a 2323 2320 332e 202a 2a53 7461 7274  ..### 3. **Start
+00002b40: 7570 2042 6568 6176 696f 7220 4964 656e  up Behavior Iden
+00002b50: 7469 6669 6361 7469 6f6e 2a2a 0d0a 0d0a  tification**....
+00002b60: 5468 6973 2066 6561 7475 7265 2061 6c6c  This feature all
+00002b70: 6f77 7320 7468 6520 7573 6572 2074 6f20  ows the user to 
+00002b80: 7669 7375 616c 697a 6520 7768 656e 2074  visualize when t
+00002b90: 6865 2062 7572 6e2d 696e 2070 6572 696f  he burn-in perio
+00002ba0: 6473 2065 6e64 206f 6e20 7468 6520 6c65  ds end on the le
+00002bb0: 6172 6e69 6e67 2063 7572 7665 2e20 0d0a  arning curve. ..
+00002bc0: 0d0a 5365 7420 7570 2074 6865 2070 6172  ..Set up the par
+00002bd0: 616d 6574 6572 7320 696e 2074 6865 2073  ameters in the s
+00002be0: 6372 6970 743a 0d0a 0d0a 2d20 6077 696e  cript:....- `win
+00002bf0: 646f 775f 7369 7a65 603a 2053 7065 6369  dow_size`: Speci
+00002c00: 6669 6573 2074 6865 206e 756d 6265 7220  fies the number 
+00002c10: 6f66 2064 6174 6120 706f 696e 7473 2075  of data points u
+00002c20: 7365 6420 746f 2063 6f6d 7075 7465 2074  sed to compute t
+00002c30: 6865 206d 6f76 696e 6720 6176 6572 6167  he moving averag
+00002c40: 6520 6f66 2074 6865 2072 6577 6172 6473  e of the rewards
+00002c50: 2e0d 0a2d 2060 7468 7265 7368 6f6c 6460  ...- `threshold`
+00002c60: 3a20 4465 6669 6e65 7320 7468 6520 6d61  : Defines the ma
+00002c70: 7869 6d75 6d20 6163 6365 7074 6162 6c65  ximum acceptable
+00002c80: 2061 6273 6f6c 7574 6520 7661 6c75 6520   absolute value 
+00002c90: 6f66 2074 6865 2064 6572 6976 6174 6976  of the derivativ
+00002ca0: 6520 6f66 2074 6865 2073 6d6f 6f74 6865  e of the smoothe
+00002cb0: 6420 7265 7761 7264 7320 6265 6c6f 7720  d rewards below 
+00002cc0: 7768 6963 6820 6120 7265 7761 7264 2069  which a reward i
+00002cd0: 7320 636f 6e73 6964 6572 6564 2073 7461  s considered sta
+00002ce0: 626c 652e 200d 0a2d 2060 636f 6e73 6563  ble. ..- `consec
+00002cf0: 7574 6976 655f 706f 696e 7473 603a 2054  utive_points`: T
+00002d00: 6865 206e 756d 6265 7220 6f66 2063 6f6e  he number of con
+00002d10: 7365 6375 7469 7665 2064 6174 6120 706f  secutive data po
+00002d20: 696e 7473 2074 6861 7420 6d75 7374 2061  ints that must a
+00002d30: 6c6c 2062 6520 6265 6c6f 7720 7468 6520  ll be below the 
+00002d40: 7468 7265 7368 6f6c 6420 666f 7220 7468  threshold for th
+00002d50: 6520 7265 7761 7264 7320 746f 2062 6520  e rewards to be 
+00002d60: 636f 6e73 6964 6572 6564 2061 7320 6861  considered as ha
+00002d70: 7669 6e67 2073 7461 6269 6c69 7a65 642e  ving stabilized.
+00002d80: 200d 0a2d 2060 6570 6973 6f64 6560 3a20   ..- `episode`: 
+00002d90: 5370 6563 6966 7920 7768 6963 6820 6570  Specify which ep
+00002da0: 6973 6f64 6527 7320 7265 7761 7264 7320  isode's rewards 
+00002db0: 746f 2061 6e61 6c79 7a65 2066 726f 6d20  to analyze from 
+00002dc0: 6120 6461 7461 7365 742e 0d0a 0d0a 546f  a dataset.....To
+00002dd0: 2070 6572 666f 726d 2074 6865 2066 6561   perform the fea
+00002de0: 7475 7265 2c20 6e61 7669 6761 7465 2074  ture, navigate t
+00002df0: 6f20 602f 6576 616c 7561 7469 6f6e 2f73  o `/evaluation/s
+00002e00: 7461 7274 7570 5f65 7661 6c75 6174 696f  tartup_evaluatio
+00002e10: 6e60 2061 6e64 2072 756e 3a0d 0a20 2020  n` and run:..   
+00002e20: 6060 6062 6173 680d 0a20 2020 7079 7468  ```bash..   pyth
+00002e30: 6f6e 2073 7461 7274 7570 5f65 7661 6c75  on startup_evalu
+00002e40: 6174 696f 6e2e 7079 0d0a 2020 2060 6060  ation.py..   ```
+00002e50: 0d0a 0d0a 2323 2320 342e 202a 2a43 6f6e  ....### 4. **Con
+00002e60: 6669 6465 6e63 6520 4576 616c 7561 7469  fidence Evaluati
+00002e70: 6f6e 2a2a 200d 0a0d 0a54 6869 7320 6665  on** ....This fe
+00002e80: 6174 7572 6520 616c 6c6f 7773 2074 6865  ature allows the
+00002e90: 2075 7365 7220 7472 6169 6e20 6d75 6c74   user train mult
+00002ea0: 6970 6c65 2076 6572 7369 6f6e 7320 6f66  iple versions of
+00002eb0: 2074 6865 2061 6765 6e74 2066 6f72 2064   the agent for d
+00002ec0: 6966 6665 7265 6e74 206e 756d 6265 7273  ifferent numbers
+00002ed0: 206f 6620 7472 6169 6e69 6e67 2065 7069   of training epi
+00002ee0: 736f 6465 7320 616e 6420 7468 656e 2065  sodes and then e
+00002ef0: 7661 6c75 6174 6520 7468 6520 7065 7266  valuate the perf
+00002f00: 6f72 6d61 6e63 6520 6f66 2065 6163 6820  ormance of each 
+00002f10: 6167 656e 7420 6f6e 2074 6865 2073 696d  agent on the sim
+00002f20: 756c 6174 696f 6e20 656e 7669 726f 6e6d  ulation environm
+00002f30: 656e 742e 0d0a 0d0a 5365 7420 7570 2074  ent.....Set up t
+00002f40: 6865 2070 6172 616d 6574 6572 7320 696e  he parameters in
+00002f50: 2074 6865 2073 6372 6970 743a 0d0a 0d0a   the script:....
+00002f60: 2d20 606e 756d 5f65 7069 736f 6465 735f  - `num_episodes_
+00002f70: 6c69 7374 603a 2041 206c 6973 7420 7468  list`: A list th
+00002f80: 6174 2063 6f6e 7461 696e 7320 6469 6666  at contains diff
+00002f90: 6572 656e 7420 6e75 6d62 6572 7320 6f66  erent numbers of
+00002fa0: 2065 7069 736f 6465 7320 746f 2074 7261   episodes to tra
+00002fb0: 696e 2074 6865 2061 6765 6e74 732e 0d0a  in the agents...
+00002fc0: 2d20 6074 696d 6573 7465 7073 603a 2041  - `timesteps`: A
+00002fd0: 2076 616c 7565 2074 6861 7420 6465 6669   value that defi
+00002fe0: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
+00002ff0: 6620 7469 6d65 7374 6570 7320 746f 2074  f timesteps to t
+00003000: 7261 696e 2074 6865 2061 6765 6e74 2064  rain the agent d
+00003010: 7572 696e 6720 6561 6368 2065 7069 736f  uring each episo
+00003020: 6465 2e0d 0a0d 0a54 6f20 7275 6e20 7468  de.....To run th
+00003030: 6973 2066 6561 7475 7265 2c20 6e61 7669  is feature, navi
+00003040: 6761 7465 2074 6f20 602f 6576 616c 7561  gate to `/evalua
+00003050: 7469 6f6e 2f63 6f6e 7665 7267 656e 6365  tion/convergence
+00003060: 5f65 7661 6c75 6174 696f 6e60 2061 6e64  _evaluation` and
+00003070: 2072 756e 3a0d 0a20 2020 6060 6062 6173   run:..   ```bas
+00003080: 680d 0a20 2020 7079 7468 6f6e 2063 6f6e  h..   python con
+00003090: 7665 7267 656e 6365 5f65 7661 6c75 6174  vergence_evaluat
+000030a0: 696f 6e2e 7079 0d0a 2020 2060 6060 0d0a  ion.py..   ```..
+000030b0: 0d0a 2323 2320 352e 202a 2a52 6f62 7573  ..### 5. **Robus
+000030c0: 746e 6573 7320 4576 616c 7561 7469 6f6e  tness Evaluation
+000030d0: 2a2a 200d 0a0d 0a54 6869 7320 6665 6174  ** ....This feat
+000030e0: 7572 6520 616c 6c6f 7773 2074 6865 2075  ure allows the u
+000030f0: 7365 7220 746f 2074 7261 696e 206d 756c  ser to train mul
+00003100: 7469 706c 6520 6167 656e 7473 2c20 616e  tiple agents, an
+00003110: 616c 797a 6520 7468 6569 7220 6265 6861  alyze their beha
+00003120: 7669 6f72 2c20 616e 6420 6361 6c63 756c  vior, and calcul
+00003130: 6174 6520 7374 6174 6973 7469 6361 6c20  ate statistical 
+00003140: 6d65 7472 6963 7320 6261 7365 6420 6f6e  metrics based on
+00003150: 2074 6865 6972 2070 6572 666f 726d 616e   their performan
+00003160: 6365 2e0d 0a0d 0a53 6574 2075 7020 7468  ce.....Set up th
+00003170: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
+00003180: 7468 6520 7363 7269 7074 3a0d 0a0d 0a2d  the script:....-
+00003190: 2060 636f 6e66 6964 656e 6365 5f6c 6576   `confidence_lev
+000031a0: 656c 603a 2054 6865 2073 7461 7469 7374  el`: The statist
+000031b0: 6963 616c 2063 6f6e 6669 6465 6e63 6520  ical confidence 
+000031c0: 6c65 7665 6c20 666f 7220 6361 6c63 756c  level for calcul
+000031d0: 6174 696f 6e73 2e0d 0a2d 2060 6465 7369  ations...- `desi
+000031e0: 7265 645f 6572 726f 7260 3a20 5468 6520  red_error`: The 
+000031f0: 7461 7267 6574 2065 7272 6f72 206d 6172  target error mar
+00003200: 6769 6e20 666f 7220 6573 7469 6d61 7469  gin for estimati
+00003210: 6e67 2073 7461 7469 7374 6963 616c 2072  ng statistical r
+00003220: 6571 7569 7265 6d65 6e74 732e 0d0a 2d20  equirements...- 
+00003230: 606e 756d 5f72 756e 7360 3a20 4e75 6d62  `num_runs`: Numb
+00003240: 6572 206f 6620 7469 6d65 7320 746f 2074  er of times to t
+00003250: 7261 696e 2061 6765 6e74 732e 0d0a 2d20  rain agents...- 
+00003260: 6074 696d 655f 7374 6570 7360 3a20 4e75  `time_steps`: Nu
+00003270: 6d62 6572 206f 6620 7469 6d65 2073 7465  mber of time ste
+00003280: 7073 2065 6163 6820 6167 656e 7420 7275  ps each agent ru
+00003290: 6e73 2069 6e20 7468 6520 7369 6d75 6c61  ns in the simula
+000032a0: 7469 6f6e 2065 6e76 6972 6f6e 6d65 6e74  tion environment
+000032b0: 2e0d 0a2d 2060 6e75 6d5f 7369 6d60 3a20  ...- `num_sim`: 
+000032c0: 4e75 6d62 6572 206f 6620 7369 6d75 6c61  Number of simula
+000032d0: 7469 6f6e 7320 746f 2072 756e 2069 6e20  tions to run in 
+000032e0: 7468 6520 656e 7669 726f 6e6d 656e 742e  the environment.
+000032f0: 0d0a 0d0a 546f 2072 756e 2074 6869 7320  ....To run this 
+00003300: 6665 6174 7572 652c 206e 6176 6967 6174  feature, navigat
+00003310: 6520 746f 2060 2f65 7661 6c75 6174 696f  e to `/evaluatio
+00003320: 6e2f 726f 6275 7374 6e65 7373 5f65 7661  n/robustness_eva
+00003330: 6c75 6174 696f 6e60 2061 6e64 2072 756e  luation` and run
+00003340: 3a0d 0a20 2020 6060 6062 6173 680d 0a20  :..   ```bash.. 
+00003350: 2020 7079 7468 6f6e 2072 6f62 7573 746e    python robustn
+00003360: 6573 735f 6576 616c 7561 7469 6f6e 2e70  ess_evaluation.p
+00003370: 790d 0a20 2020 6060 600d 0a0d 0a23 2323  y..   ```....###
+00003380: 2036 2e20 2a2a 4e6f 6973 6520 4576 616c   6. **Noise Eval
+00003390: 7561 7469 6f6e 2a2a 200d 0a0d 0a54 6869  uation** ....Thi
+000033a0: 7320 6665 6174 7572 6520 616c 6c6f 7773  s feature allows
+000033b0: 2074 6865 2075 7365 7220 746f 2065 7661   the user to eva
+000033c0: 6c75 6174 6520 7468 6520 6566 6665 6374  luate the effect
+000033d0: 206f 6620 656e 7669 726f 6e6d 656e 7461   of environmenta
+000033e0: 6c20 6e6f 6973 6520 6f6e 2074 6865 2070  l noise on the p
+000033f0: 6572 666f 726d 616e 6365 206f 6620 7468  erformance of th
+00003400: 6520 6167 656e 742e 0d0a 0d0a 5365 7420  e agent.....Set 
+00003410: 7570 2074 6865 2070 6172 616d 6574 6572  up the parameter
+00003420: 7320 696e 2074 6865 2073 6372 6970 743a  s in the script:
+00003430: 0d0a 0d0a 2d20 6066 7265 7175 656e 6379  ....- `frequency
+00003440: 2060 3a20 5468 6520 6c69 6b65 6c69 686f   `: The likeliho
+00003450: 6f64 206f 7220 6672 6571 7565 6e63 7920  od or frequency 
+00003460: 6174 2077 6869 6368 206e 6f69 7365 2069  at which noise i
+00003470: 7320 696e 7472 6f64 7563 6564 2074 6f20  s introduced to 
+00003480: 7468 6520 7379 7374 656d 2e20 4974 206d  the system. It m
+00003490: 7573 7420 6265 2061 2076 616c 7565 2062  ust be a value b
+000034a0: 6574 7765 656e 2030 2061 6e64 2031 2e20  etween 0 and 1. 
+000034b0: 5468 6973 2070 6172 616d 6574 6572 2064  This parameter d
+000034c0: 6574 6572 6d69 6e65 7320 686f 7720 6f66  etermines how of
+000034d0: 7465 6e2c 2070 726f 706f 7274 696f 6e61  ten, proportiona
+000034e0: 6c6c 792c 206e 6f69 7365 2077 696c 6c20  lly, noise will 
+000034f0: 6265 2061 6464 6564 2064 7572 696e 6720  be added during 
+00003500: 7468 6520 7369 6d75 6c61 7469 6f6e 2e20  the simulation. 
+00003510: 0d0a 2d20 606d 6561 6e60 3a20 5468 6520  ..- `mean`: The 
+00003520: 6d65 616e 206f 6620 7468 6520 6e6f 726d  mean of the norm
+00003530: 616c 2064 6973 7472 6962 7574 696f 6e20  al distribution 
+00003540: 6672 6f6d 2077 6869 6368 2074 6865 206e  from which the n
+00003550: 6f69 7365 2076 616c 7565 7320 6172 6520  oise values are 
+00003560: 7361 6d70 6c65 642e 2054 6869 7320 7265  sampled. This re
+00003570: 7072 6573 656e 7473 2074 6865 2061 7665  presents the ave
+00003580: 7261 6765 2076 616c 7565 206f 6620 7468  rage value of th
+00003590: 6520 6e6f 6973 6520 7468 6174 2077 696c  e noise that wil
+000035a0: 6c20 6265 2069 6e74 726f 6475 6365 642e  l be introduced.
+000035b0: 0d0a 2d20 6076 6172 6961 6e63 6560 3a20  ..- `variance`: 
+000035c0: 5468 6520 7661 7269 616e 6365 206f 6620  The variance of 
+000035d0: 7468 6520 6e6f 726d 616c 2064 6973 7472  the normal distr
+000035e0: 6962 7574 696f 6e20 6672 6f6d 2077 6869  ibution from whi
+000035f0: 6368 2074 6865 206e 6f69 7365 2076 616c  ch the noise val
+00003600: 7565 7320 6172 6520 7361 6d70 6c65 642e  ues are sampled.
+00003610: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
+00003620: 696e 6469 6361 7465 7320 7468 6520 7370  indicates the sp
+00003630: 7265 6164 206f 7220 6469 7370 6572 7369  read or dispersi
+00003640: 6f6e 206f 6620 7468 6520 6e6f 6973 6520  on of the noise 
+00003650: 6172 6f75 6e64 2074 6865 206d 6561 6e2e  around the mean.
+00003660: 0d0a 0d0a 546f 2072 756e 2074 6865 2066  ....To run the f
+00003670: 6561 7475 7265 2c20 6e61 7669 6761 7465  eature, navigate
+00003680: 2074 6f20 602f 6576 616c 7561 7469 6f6e   to `/evaluation
+00003690: 2f6e 6f69 7365 5f65 7661 6c75 6174 696f  /noise_evaluatio
+000036a0: 6e60 2061 6e64 2072 756e 3a0d 0a20 2020  n` and run:..   
+000036b0: 6060 6062 6173 680d 0a20 2020 7079 7468  ```bash..   pyth
+000036c0: 6f6e 206e 6f69 7365 5f65 7661 6c75 6174  on noise_evaluat
+000036d0: 696f 6e2e 7079 0d0a 2020 2060 6060 0d0a  ion.py..   ```..
+000036e0: 0d0a 2323 2043 6f6e 7472 6962 7574 696f  ..## Contributio
+000036f0: 6e0d 0a0d 0a43 6f6e 7472 6962 7574 696f  n....Contributio
+00003700: 6e73 2061 7265 2077 656c 636f 6d65 2e20  ns are welcome. 
+00003710: 506c 6561 7365 2063 7265 6174 6520 6120  Please create a 
+00003720: 7075 6c6c 2072 6571 7565 7374 206f 7220  pull request or 
+00003730: 6973 7375 6520 746f 2064 6973 6375 7373  issue to discuss
+00003740: 2070 726f 706f 7365 6420 6368 616e 6765   proposed change
+00003750: 7320 6f72 2072 6570 6f72 7420 6275 6773  s or report bugs
+00003760: 2e0d 0a0d 0a23 2320 4c69 6365 6e73 650d  .....## License.
+00003770: 0a0d 0a54 6869 7320 7072 6f6a 6563 7420  ...This project 
+00003780: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
+00003790: 7220 7468 6520 4d49 5420 4c69 6365 6e73  r the MIT Licens
+000037a0: 6520 2d20 7365 6520 7468 6520 4c49 4345  e - see the LICE
+000037b0: 4e53 4520 6669 6c65 2066 6f72 2064 6574  NSE file for det
+000037c0: 6169 6c73 2e0d 0a                        ails...
```

### Comparing `sim_rl-0.1.5/sim_rl/.gitlab-ci.yml` & `sim_rl-0.1.6/sim_rl/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/__pycache__/buffer.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/agents/__pycache__/buffer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/agents/__pycache__/ddpg_agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/__pycache__/model.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/agents/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/buffer.py` & `sim_rl-0.1.6/sim_rl/agents/buffer.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/ddpg_agent.py` & `sim_rl-0.1.6/sim_rl/agents/ddpg_agent.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/model.py` & `sim_rl-0.1.6/sim_rl/agents/model.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/trained_agent.pt` & `sim_rl-0.1.6/sim_rl/agents/trained_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/agents/trained_ddpg_agent.pt` & `sim_rl-0.1.6/sim_rl/agents/trained_ddpg_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/debug.py` & `sim_rl-0.1.6/sim_rl/debug.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py` & `sim_rl-0.1.6/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/convergence_evaluation/reward_plot.png` & `sim_rl-0.1.6/sim_rl/evaluation/convergence_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/decision_evaluation/decision_evaluation.py` & `sim_rl-0.1.6/sim_rl/evaluation/decision_evaluation/decision_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png` & `sim_rl-0.1.6/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/noise_evaluation/noise_evaluation.py` & `sim_rl-0.1.6/sim_rl/evaluation/noise_evaluation/noise_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py` & `sim_rl-0.1.6/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot.png` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_0.png` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_0.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_1.png` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_2.png` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/reward_plot_3.png` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/reward_plot_3.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/evaluation/startup_evaluation/startup_evaluation.py` & `sim_rl-0.1.6/sim_rl/evaluation/startup_evaluation/startup_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/foundations/__pycache__/core_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/foundations/__pycache__/core_plotting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc` & `sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py` & `sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json` & `sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png` & `sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png` & `sim_rl-0.1.6/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/core_functions.py` & `sim_rl-0.1.6/sim_rl/foundations/core_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/core_plotting.py` & `sim_rl-0.1.6/sim_rl/foundations/core_plotting.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/action_dict.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/action_dict.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/actor_loss.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/actor_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/critic_loss.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/critic_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/next_state_model_loss.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/next_state_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/reward_dict.json` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/reward_dict.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/reward_model_loss.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/reward_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/foundations/output_csv/transition_proba.csv` & `sim_rl-0.1.6/sim_rl/foundations/output_csv/transition_proba.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/main.py` & `sim_rl-0.1.6/sim_rl/main.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/queue_env/__pycache__/queue_base_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/queue_env/__pycache__/queueing_network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_base_functions.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_base_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.gitignore` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.gitignore`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/.readthedocs.yml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/CHANGELOG.md` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/cliff.toml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/cliff.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/search.html` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/search.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/conf.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/current_state.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/current_state.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/current_state1.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/current_state1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/fig.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/fig.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/graph.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/index.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/installation.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/make.bat` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/Makefile` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/my_network.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/my_network.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/my_network1.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/my_network1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/network.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/network.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/overview.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/queues.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/queues.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/sim.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/sim.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/sim1.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/sim1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/store.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/store.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/docs/store1.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/docs/store1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/LICENSE.txt` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/poetry.lock` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/poetry.lock`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/pyproject.toml` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/README.rst` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/README.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_network.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py` & `sim_rl-0.1.6/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/queue_env/queueing_network.py` & `sim_rl-0.1.6/sim_rl/queue_env/queueing_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/rl_env/__pycache__/RL_Environment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/rl_env/RL_Environment.py` & `sim_rl-0.1.6/sim_rl/rl_env/RL_Environment.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/tuning/__pycache__/ray_tuning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc` & `sim_rl-0.1.6/sim_rl/tuning/__pycache__/wandb_tuning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/tuning/ray_tuning.py` & `sim_rl-0.1.6/sim_rl/tuning/ray_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/tuning/wandb_tuning.py` & `sim_rl-0.1.6/sim_rl/tuning/wandb_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/user_config/configuration.yml` & `sim_rl-0.1.6/sim_rl/user_config/configuration.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/sim_rl/user_config/eval_hyperparams.yml` & `sim_rl-0.1.6/sim_rl/user_config/eval_hyperparams.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.5/PKG-INFO` & `sim_rl-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sim_rl
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simulation Driven RL Package Utilized to Optimize Queueing Systems
 Author: Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi
 Author-email: fatima.al-ani23@imperial.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,40 +27,42 @@
 
 ## Project Structure
 
 - `agents`: Contains the Dyna-DDPG agent implementation and allows the integration of new types of agents for exploring the simulated queueing environment.
 - `queue_env`: Defines the simulated queueing environment, utilizing functionalities from the `queueing-tool` package.
 - `rl_env`: Hosts the RL environment, which is portable and compatible with different agent types.
 - `features`: Includes several utility features:
-  - **Breakdown Exploration**: Explores key states versus peripheral states
-  - **Blockage Demonstration**: Demonstrates how the agent responds to a server outage by adjusting routing probabilities.
+  - **Decision Evaluation**: Demonstrates how the agent responds to a server outage by adjusting routing probabilities.
   - **Confidence Evaluation**: Assesses the stability and reliability of the agent across different training setups
   - **Noise Evaluation**: Evaluate the effect of environmental noise on the performance of the agent
-  - **Startup Behavior Visualization**: Identifies the burn-in period of the agent
+  - **Startup Evaluation**: Identifies the burn-in period of the agent
   - **Robustness Evaluation**: Assess robustness of decisions across multiple trained agents
 
 ## Prerequisites
 
 Before running the simulations, ensure you have the following installed:
-- Python >=3.10 <3.11
-- PyTorch 1.7+
-- NumPy
-- Pandas
-- Matplotlib
-- queueing-tool
-- wandb
-- Ray
+- Python >=3.10 <3.12
+- torch = "2.2.0"
+- numpy = "1.26.4"
+- pandas = "2.2.0"
+- queueing_tool = "1.2.5"
+- matplotlib = "3.8.3"
+- wandb = "0.16.3"
+- PyYAML = "6.0.1"
+- ray = { version = "2.9.2", extras = ["train", "tune"] }
+- tqdm = "4.57.0"
+- scipy = "1.12.0"
 
 ## Installation
 
 Clone the repository and install the required dependencies:
 
 ```bash
-git clone https://gitlab.doc.ic.ac.uk/jw923/MScDataSparqProject.git
-cd MScDataSparqProject
+git clone https://github.com/ao-420/sim_rl.git
+cd sim_rl
 pip install -r requirements.txt
 ```
 
 ## Step 1: Configuration
 
 ### Environment Setup
 
@@ -138,15 +140,15 @@
 
    arrival_rate: [0.3]
 
    max_agents: inf
 
    sim_jobs: 100
 
-   max_arr_rate_list: [375, 375, 375]
+   max_arr_rate_list: [0.3]
 
    entry_nodes:
    - [0, 1] 
    ```
 
 #### **RL Environment Parameters**
 
@@ -274,14 +276,18 @@
    - 0.5
 
    num_episodes: 
    - 5
 
    time_steps: 
    - 10
+   
+   num_train_AC: 
+   - 10
+
    ```
 
 ## Step 2: Running Simulations
 
 ### Training Agent
 This command starts training the agent within the simulated queueing environment. Results are saved in `/foundations/output_csv` and `/foundations/output_plots`.
 
@@ -322,15 +328,15 @@
 - `reset`: A bool value that controls whether to reset weight parameters during training.
 - `reset_frequency`: A value that defines the number of episodes frequency to reset the weight parameters.
 - `num_output`: A value that defines the number of top and least reward/visits states to plot in a histogram
 - `output_json`: A bool value that determines whether to output the json file of key states and peripheral states
 - `output_histogram`: A bool value that determines whether to output the histogram that shows the rewards and visits of the top and least states.
 - `output_coverage_metric`: A bool value that determines whether to output the current coverage metric.
 
-To run this feature, navigate to `/evaluation/breakdown_exploration` and run:
+To run this feature, navigate to `/foundations/breakdown_exploration` and run:
    ```bash
    python breakdown_exploration.py
    ```
 
 ### 2. **Blockage Demonstrations**
 
 This feature allows the user to test a trained agent's performance on a simulated server blockage queueing environment by visualizing the changes in transition probabilities. The purpose of this feature is to show how effectice the tranied agent is acting on breakdown cases. 
@@ -338,47 +344,47 @@
 Set up the parameters in `user_config\features_params\blockage_demonstration_params.yml`:
 
 - `num_sim`: Defines the number of jobs to simulate for each time step during training.
 - `time_steps`: Defines the number of time steps to perform for each episode.
 - `queue_index`: Defines the queue index that record the metrics for.
 - `metric`: Defines the metric to be reported for the selected queue.
 
-To use this feature, navigate to `/evaluation/blockage_demonstration` and run:
+To use this feature, navigate to `/evaluation/decision_evaluation` and run:
    ```bash
-   python demonstrations.py
+   python decision_evaluation.py
    ```
 
 ### 3. **Startup Behavior Identification**
 
 This feature allows the user to visualize when the burn-in periods end on the learning curve. 
 
 Set up the parameters in the script:
 
 - `window_size`: Specifies the number of data points used to compute the moving average of the rewards.
 - `threshold`: Defines the maximum acceptable absolute value of the derivative of the smoothed rewards below which a reward is considered stable. 
 - `consecutive_points`: The number of consecutive data points that must all be below the threshold for the rewards to be considered as having stabilized. 
 - `episode`: Specify which episode's rewards to analyze from a dataset.
 
-To perform the feature, navigate to `/evaluation/startup_behavior` and run:
+To perform the feature, navigate to `/evaluation/startup_evaluation` and run:
    ```bash
-   python startup.py
+   python startup_evaluation.py
    ```
 
 ### 4. **Confidence Evaluation** 
 
 This feature allows the user train multiple versions of the agent for different numbers of training episodes and then evaluate the performance of each agent on the simulation environment.
 
 Set up the parameters in the script:
 
 - `num_episodes_list`: A list that contains different numbers of episodes to train the agents.
 - `timesteps`: A value that defines the number of timesteps to train the agent during each episode.
 
-To run this feature, navigate to `/evaluation/confidence_evaluation` and run:
+To run this feature, navigate to `/evaluation/convergence_evaluation` and run:
    ```bash
-   python confidence.py
+   python convergence_evaluation.py
    ```
 
 ### 5. **Robustness Evaluation** 
 
 This feature allows the user to train multiple agents, analyze their behavior, and calculate statistical metrics based on their performance.
 
 Set up the parameters in the script:
@@ -387,15 +393,15 @@
 - `desired_error`: The target error margin for estimating statistical requirements.
 - `num_runs`: Number of times to train agents.
 - `time_steps`: Number of time steps each agent runs in the simulation environment.
 - `num_sim`: Number of simulations to run in the environment.
 
 To run this feature, navigate to `/evaluation/robustness_evaluation` and run:
    ```bash
-   python runs.py
+   python robustness_evaluation.py
    ```
 
 ### 6. **Noise Evaluation** 
 
 This feature allows the user to evaluate the effect of environmental noise on the performance of the agent.
 
 Set up the parameters in the script:
```

