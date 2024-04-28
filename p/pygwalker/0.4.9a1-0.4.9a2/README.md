# Comparing `tmp/pygwalker-0.4.9a1.tar.gz` & `tmp/pygwalker-0.4.9a2.tar.gz`

## Comparing `pygwalker-0.4.9a1.tar` & `pygwalker-0.4.9a2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/.gitignore
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/components.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/index.html
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/postcss.config.js
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/tailwind.config.js
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/tsconfig.json
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/vite.config.ts
--rw-r--r--   0        0        0   279367 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/yarn.lock
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/index.css
--rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/index.tsx
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/options.tsx
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/codeExportModal/usePythonCode.ts
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/initModal/index.tsx
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/preview/index.tsx
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/badge.tsx
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/button.tsx
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/checkbox.tsx
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/input.tsx
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/label.tsx
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/select.tsx
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/tabs.tsx
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/toggle-group.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/ui/toggle.tsx
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/uploadChartModal/index.tsx
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/components/uploadSpecModal/index.tsx
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/dataSource/index.ts
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/interfaces/index.ts
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/notify/index.tsx
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/store/common.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/store/communication.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/store/context.ts
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/tools/exportDataframe.tsx
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/tools/exportTool.tsx
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/tools/loginTool.tsx
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/tools/saveTool.tsx
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/communication.tsx
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/context.tsx
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/formatSpec.ts
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/save.ts
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/theme.ts
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/bin/pygwalker_command.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/_constants.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/_typing.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/__init__.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/gradio.py
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/html.py
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/jupyter.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/kanaries_cloud.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/pygwalker.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/api/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/communications/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/communications/base.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/communications/gradio_comm.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/communications/hacker_comm.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/communications/streamlit_comm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/__init__.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/base.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/cloud_dataset_parser.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/database_parser.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/modin_parser.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/pandas_parser.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/polars_parser.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/data_parsers/spark_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/check_update.py
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/cloud_service.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/config.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/data_parsers.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/fname_encodings.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/format_invoke_walk_code.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/global_var.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/kaggle.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/kanaries_cli_login.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/preview_image.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/render.py
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/spec.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/streamlit_components.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/tip_tools.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/track.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/services/upload_data.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/index.html
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/preview.html
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/preview_list.html
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/pygwalker_iframe.html
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/pygwalker_main_page.html
--rw-r--r--   0        0        0   336362 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/dsl-to-workflow.umd.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  6847039 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0   333908 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/vega-to-dsl.umd.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/codeExportModal/usePythonCode.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/initModal/index.d.ts
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/preview/index.d.ts
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/badge.d.ts
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/button.d.ts
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/checkbox.d.ts
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/dialog.d.ts
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/input.d.ts
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/label.d.ts
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/select.d.ts
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/tabs.d.ts
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/toggle-group.d.ts
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/toggle.d.ts
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/uploadChartModal/index.d.ts
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/components/uploadSpecModal/index.d.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/lib/dslToWorkflow.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/lib/utils.d.ts
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/lib/vegaToDsl.d.ts
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/notify/index.d.ts
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/store/common.d.ts
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/store/communication.d.ts
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/store/context.d.ts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/tools/exportDataframe.d.ts
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/tools/exportTool.d.ts
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/tools/loginTool.d.ts
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/tools/saveTool.d.ts
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/communication.d.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/context.d.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/formatSpec.d.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/theme.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/check_walker_params.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/custom_sqlglot.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/display.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/dsl_transform.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/encode.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/estimate_tools.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/execute_env_check.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/log.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/payload_to_sql.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker/utils/randoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker_tools/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker_tools/metrics/__init__.py
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker_tools/metrics/api.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pygwalker_tools/metrics/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/scripts/__init__.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/scripts/compile.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/LICENSE
--rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/README.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/pyproject.toml
--rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 pygwalker-0.4.9a1/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/.gitignore
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/components.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/index.html
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/postcss.config.js
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/tailwind.config.js
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/tsconfig.json
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/vite.config.ts
+-rw-r--r--   0        0        0   279367 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/yarn.lock
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/index.css
+-rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/index.tsx
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/options.tsx
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/codeExportModal/usePythonCode.ts
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/initModal/index.tsx
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/preview/index.tsx
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/badge.tsx
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/button.tsx
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/checkbox.tsx
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/input.tsx
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/label.tsx
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/select.tsx
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/tabs.tsx
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/toggle-group.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/toggle.tsx
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/uploadChartModal/index.tsx
+-rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/uploadSpecModal/index.tsx
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/notify/index.tsx
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/common.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/communication.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/context.ts
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/exportDataframe.tsx
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/exportTool.tsx
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/loginTool.tsx
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/saveTool.tsx
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/communication.tsx
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/context.tsx
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/formatSpec.ts
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/save.ts
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/theme.ts
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/bin/pygwalker_command.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/_constants.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/_typing.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/__init__.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/gradio.py
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/html.py
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/jupyter.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/kanaries_cloud.py
+-rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/pygwalker.py
+-rw-r--r--   0        0        0    11657 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/base.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/gradio_comm.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/hacker_comm.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/streamlit_comm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/__init__.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/base.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/cloud_dataset_parser.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/database_parser.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/modin_parser.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/pandas_parser.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/polars_parser.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/spark_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/check_update.py
+-rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/cloud_service.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/config.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/data_parsers.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/fname_encodings.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/format_invoke_walk_code.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/global_var.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/kaggle.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/kanaries_cli_login.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/preview_image.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/render.py
+-rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/spec.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/streamlit_components.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/tip_tools.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/track.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/upload_data.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/preview.html
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/preview_list.html
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/pygwalker_iframe.html
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/pygwalker_main_page.html
+-rw-r--r--   0        0        0   336362 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/dsl-to-workflow.umd.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  6847039 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0   333908 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/vega-to-dsl.umd.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/codeExportModal/usePythonCode.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/initModal/index.d.ts
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/preview/index.d.ts
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/badge.d.ts
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/button.d.ts
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/checkbox.d.ts
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/dialog.d.ts
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/input.d.ts
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/label.d.ts
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/select.d.ts
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/tabs.d.ts
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle-group.d.ts
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle.d.ts
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/uploadChartModal/index.d.ts
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/uploadSpecModal/index.d.ts
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/dslToWorkflow.d.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/utils.d.ts
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/vegaToDsl.d.ts
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/notify/index.d.ts
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/common.d.ts
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/communication.d.ts
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/context.d.ts
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/exportDataframe.d.ts
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/exportTool.d.ts
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/loginTool.d.ts
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/saveTool.d.ts
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/communication.d.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/context.d.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/formatSpec.d.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/theme.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/check_walker_params.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/custom_sqlglot.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/display.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/dsl_transform.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/encode.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/estimate_tools.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/execute_env_check.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/log.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/payload_to_sql.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/randoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/__init__.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/api.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/__init__.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/compile.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/LICENSE
+-rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/README.md
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pyproject.toml
+-rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/PKG-INFO
```

### Comparing `pygwalker-0.4.9a1/app/package.json` & `pygwalker-0.4.9a2/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/tailwind.config.js` & `pygwalker-0.4.9a2/app/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/tsconfig.json` & `pygwalker-0.4.9a2/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/vite.config.ts` & `pygwalker-0.4.9a2/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/yarn.lock` & `pygwalker-0.4.9a2/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/index.css` & `pygwalker-0.4.9a2/app/src/index.css`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/index.tsx` & `pygwalker-0.4.9a2/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/options.tsx` & `pygwalker-0.4.9a2/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.4.9a2/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/codeExportModal/usePythonCode.ts` & `pygwalker-0.4.9a2/app/src/components/codeExportModal/usePythonCode.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/initModal/index.tsx` & `pygwalker-0.4.9a2/app/src/components/initModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/preview/index.tsx` & `pygwalker-0.4.9a2/app/src/components/preview/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/badge.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/badge.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/button.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/checkbox.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/checkbox.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/dialog.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/input.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/input.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/label.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/label.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/select.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/select.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/tabs.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/tabs.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/toggle-group.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/toggle-group.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/ui/toggle.tsx` & `pygwalker-0.4.9a2/app/src/components/ui/toggle.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/uploadChartModal/index.tsx` & `pygwalker-0.4.9a2/app/src/components/uploadChartModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/components/uploadSpecModal/index.tsx` & `pygwalker-0.4.9a2/app/src/components/uploadSpecModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/dataSource/index.ts` & `pygwalker-0.4.9a2/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/interfaces/index.ts` & `pygwalker-0.4.9a2/app/src/interfaces/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/notify/index.tsx` & `pygwalker-0.4.9a2/app/src/notify/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/store/common.ts` & `pygwalker-0.4.9a2/app/src/store/common.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/tools/exportDataframe.tsx` & `pygwalker-0.4.9a2/app/src/tools/exportDataframe.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/tools/exportTool.tsx` & `pygwalker-0.4.9a2/app/src/tools/exportTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/tools/loginTool.tsx` & `pygwalker-0.4.9a2/app/src/tools/loginTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/tools/saveTool.tsx` & `pygwalker-0.4.9a2/app/src/tools/saveTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/utils/communication.tsx` & `pygwalker-0.4.9a2/app/src/utils/communication.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/utils/context.tsx` & `pygwalker-0.4.9a2/app/src/utils/context.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/app/src/utils/save.ts` & `pygwalker-0.4.9a2/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/bin/pygwalker_command.py` & `pygwalker-0.4.9a2/bin/pygwalker_command.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/__init__.py` & `pygwalker-0.4.9a2/pygwalker/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 from pygwalker.utils.randoms import rand_str as __rand_str
 from pygwalker.utils.execute_env_check import check_kaggle as __check_kaggle
 from pygwalker.services.global_var import GlobalVarManager
 from pygwalker.services.kaggle import show_tips_user_kaggle as __show_tips_user_kaggle
 
-__version__ = "0.4.9a1"
+__version__ = "0.4.9a2"
 __hash__ = __rand_str()
 
 from pygwalker.api.jupyter import walk, render, table
 from pygwalker.api.html import to_html
 from pygwalker.data_parsers.base import FieldSpec
 
 if GlobalVarManager.privacy == 'offline':
```

### Comparing `pygwalker-0.4.9a1/pygwalker/_typing.py` & `pygwalker-0.4.9a2/pygwalker/_typing.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/errors.py` & `pygwalker-0.4.9a2/pygwalker/errors.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/gradio.py` & `pygwalker-0.4.9a2/pygwalker/api/gradio.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/html.py` & `pygwalker-0.4.9a2/pygwalker/api/html.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/jupyter.py` & `pygwalker-0.4.9a2/pygwalker/api/jupyter.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/kanaries_cloud.py` & `pygwalker-0.4.9a2/pygwalker/api/kanaries_cloud.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/pygwalker.py` & `pygwalker-0.4.9a2/pygwalker/api/pygwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/api/streamlit.py` & `pygwalker-0.4.9a2/pygwalker/api/streamlit.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,16 +83,14 @@
             - kernel_computation(bool): Whether to use kernel compute for datas, Default to True.
             - use_kernel_calc(bool): Deprecated, use kernel_computation instead.
             - kanaries_api_key (str): kanaries api key, Default to "".
             - default_tab (Literal["data", "vis"]): default tab to show. Default to "vis"
         """
         check_expired_params(kwargs)
 
-        init_streamlit_comm()
-
         self.walker = PygWalker(
             gid=gid,
             dataset=dataset,
             field_specs=field_specs if field_specs is not None else [],
             spec=spec,
             source_invoke_code="",
             theme_key=theme_key,
@@ -293,14 +291,16 @@
         - spec (str): chart config data. config id, json, remote file url
         - kernel_computation(bool): Whether to use kernel compute for datas, Default to None.
         - use_kernel_calc(bool): Deprecated, use kernel_computation instead.
         - spec_io_mode (ISpecIOMode): spec io mode, Default to "r", "r" for read, "rw" for read and write.
         - kanaries_api_key (str): kanaries api key, Default to "".
         - default_tab (Literal["data", "vis"]): default tab to show. Default to "vis"
     """
+    init_streamlit_comm()
+
     if field_specs is None:
         field_specs = []
 
     renderer = StreamlitRenderer(
         gid=gid,
         dataset=dataset,
         field_specs=field_specs,
```

### Comparing `pygwalker-0.4.9a1/pygwalker/communications/base.py` & `pygwalker-0.4.9a2/pygwalker/communications/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/communications/gradio_comm.py` & `pygwalker-0.4.9a2/pygwalker/communications/gradio_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/communications/hacker_comm.py` & `pygwalker-0.4.9a2/pygwalker/communications/hacker_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/communications/streamlit_comm.py` & `pygwalker-0.4.9a2/pygwalker/communications/streamlit_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/base.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/cloud_dataset_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/cloud_dataset_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/database_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/database_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/modin_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/modin_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/pandas_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/pandas_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/polars_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/polars_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/data_parsers/spark_parser.py` & `pygwalker-0.4.9a2/pygwalker/data_parsers/spark_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/check_update.py` & `pygwalker-0.4.9a2/pygwalker/services/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/cloud_service.py` & `pygwalker-0.4.9a2/pygwalker/services/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/config.py` & `pygwalker-0.4.9a2/pygwalker/services/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/data_parsers.py` & `pygwalker-0.4.9a2/pygwalker/services/data_parsers.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/fname_encodings.py` & `pygwalker-0.4.9a2/pygwalker/services/fname_encodings.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/format_invoke_walk_code.py` & `pygwalker-0.4.9a2/pygwalker/services/format_invoke_walk_code.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/global_var.py` & `pygwalker-0.4.9a2/pygwalker/services/global_var.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/kaggle.py` & `pygwalker-0.4.9a2/pygwalker/services/kaggle.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/kanaries_cli_login.py` & `pygwalker-0.4.9a2/pygwalker/services/kanaries_cli_login.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/preview_image.py` & `pygwalker-0.4.9a2/pygwalker/services/preview_image.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/render.py` & `pygwalker-0.4.9a2/pygwalker/services/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/spec.py` & `pygwalker-0.4.9a2/pygwalker/services/spec.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/streamlit_components.py` & `pygwalker-0.4.9a2/pygwalker/services/streamlit_components.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/tip_tools.py` & `pygwalker-0.4.9a2/pygwalker/services/tip_tools.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/track.py` & `pygwalker-0.4.9a2/pygwalker/services/track.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/services/upload_data.py` & `pygwalker-0.4.9a2/pygwalker/services/upload_data.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/preview.html` & `pygwalker-0.4.9a2/pygwalker/templates/preview.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/preview_list.html` & `pygwalker-0.4.9a2/pygwalker/templates/preview_list.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/pygwalker_main_page.html` & `pygwalker-0.4.9a2/pygwalker/templates/pygwalker_main_page.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/dsl-to-workflow.umd.js` & `pygwalker-0.4.9a2/pygwalker/templates/dist/dsl-to-workflow.umd.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/index.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.4.9a2/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/vega-to-dsl.umd.js` & `pygwalker-0.4.9a2/pygwalker/templates/dist/vega-to-dsl.umd.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/preview/index.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/preview/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/badge.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/badge.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/button.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/button.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/dialog.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/dialog.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/select.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/select.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/tabs.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/tabs.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/toggle-group.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle-group.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/components/ui/toggle.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/dataSource/index.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/dataSource/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/interfaces/index.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/interfaces/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/store/common.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/store/common.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/tools/saveTool.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/tools/saveTool.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/templates/dist/utils/communication.d.ts` & `pygwalker-0.4.9a2/pygwalker/templates/dist/utils/communication.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/custom_sqlglot.py` & `pygwalker-0.4.9a2/pygwalker/utils/custom_sqlglot.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/display.py` & `pygwalker-0.4.9a2/pygwalker/utils/display.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/dsl_transform.py` & `pygwalker-0.4.9a2/pygwalker/utils/dsl_transform.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/encode.py` & `pygwalker-0.4.9a2/pygwalker/utils/encode.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/execute_env_check.py` & `pygwalker-0.4.9a2/pygwalker/utils/execute_env_check.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker/utils/payload_to_sql.py` & `pygwalker-0.4.9a2/pygwalker/utils/payload_to_sql.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker_tools/metrics/api.py` & `pygwalker-0.4.9a2/pygwalker_tools/metrics/api.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pygwalker_tools/metrics/core.py` & `pygwalker-0.4.9a2/pygwalker_tools/metrics/core.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/scripts/test-init.py` & `pygwalker-0.4.9a2/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/scripts/test-init.sh` & `pygwalker-0.4.9a2/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/.gitignore` & `pygwalker-0.4.9a2/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/LICENSE` & `pygwalker-0.4.9a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/README.md` & `pygwalker-0.4.9a2/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/pyproject.toml` & `pygwalker-0.4.9a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a1/PKG-INFO` & `pygwalker-0.4.9a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pygwalker
-Version: 0.4.9a1
+Version: 0.4.9a2
 Summary: pygwalker: turn your data into an interactive UI for data exploration and visualization
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: kanaries <support@kanaries.net>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pygwalker Version: 0.4.9a1 Summary: pygwalker: turn
+Metadata-Version: 2.3 Name: pygwalker Version: 0.4.9a2 Summary: pygwalker: turn
 your data into an interactive UI for data exploration and visualization
 Project-URL: homepage, https://github.com/Kanaries/pygwalker Project-URL:
 repository, https://github.com/Kanaries/pygwalker Author-email: kanaries
 kanaries.net> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
```

