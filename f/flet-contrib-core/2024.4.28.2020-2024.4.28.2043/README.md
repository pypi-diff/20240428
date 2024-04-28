# Comparing `tmp/flet_contrib_core-2024.4.28.2020.tar.gz` & `tmp/flet_contrib_core-2024.4.28.2043.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_core-2024.4.28.2020.tar", max compression
+gzip compressed data, was "flet_contrib_core-2024.4.28.2043.tar", max compression
```

## Comparing `flet_contrib_core-2024.4.28.2020.tar` & `flet_contrib_core-2024.4.28.2043.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0      189 2024-04-28 20:19:42.621929 flet_contrib_core-2024.4.28.2020/README.md
--rw-r--r--   0        0        0      673 2024-04-28 20:20:32.149641 flet_contrib_core-2024.4.28.2020/pyproject.toml
--rw-r--r--   0        0        0    10950 2024-04-28 20:19:42.621929 flet_contrib_core-2024.4.28.2020/src/flet_core/__init__.py
--rw-r--r--   0        0        0      434 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/adaptive_control.py
--rw-r--r--   0        0        0    13342 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/alignment.py
--rw-r--r--   0        0        0     6757 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     1955 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/animation.py
--rw-r--r--   0        0        0    11031 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7915 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/audio.py
--rw-r--r--   0        0        0     8439 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/audio_recorder.py
--rw-r--r--   0        0        0     5781 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/badge.py
--rw-r--r--   0        0        0     8099 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     5930 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/bottom_app_bar.py
--rw-r--r--   0        0        0     5830 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2103 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/buttons.py
--rw-r--r--   0        0        0      514 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0      846 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3524 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
--rw-r--r--   0        0        0     4799 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
--rw-r--r--   0        0        0     2352 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
--rw-r--r--   0        0        0     1800 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0     1439 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
--rw-r--r--   0        0        0     2596 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
--rw-r--r--   0        0        0     2606 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
--rw-r--r--   0        0        0     4856 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
--rw-r--r--   0        0        0     2490 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
--rw-r--r--   0        0        0     3005 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
--rw-r--r--   0        0        0     2534 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
--rw-r--r--   0        0        0      704 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
--rw-r--r--   0        0        0     4879 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
--rw-r--r--   0        0        0     2910 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4813 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1646 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1236 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      844 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1869 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1891 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3493 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1813 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2345 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1951 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     8220 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/card.py
--rw-r--r--   0        0        0     9184 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
--rw-r--r--   0        0        0     2642 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
--rw-r--r--   0        0        0     3314 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
--rw-r--r--   0        0        0     1867 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
--rw-r--r--   0        0        0      693 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
--rw-r--r--   0        0        0      654 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
--rw-r--r--   0        0        0     1541 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
--rw-r--r--   0        0        0    10717 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
--rw-r--r--   0        0        0     9157 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
--rw-r--r--   0        0        0     5936 2024-04-28 20:19:42.629929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
--rw-r--r--   0        0        0     5564 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
--rw-r--r--   0        0        0     4511 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
--rw-r--r--   0        0        0     9932 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2044 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6679 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1932 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2923 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11305 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     9357 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5338 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5965 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3807 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0    12179 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/checkbox.py
--rw-r--r--   0        0        0    14830 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/chip.py
--rw-r--r--   0        0        0     9261 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3097 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/client_storage.py
--rw-r--r--   0        0        0    10869 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/colors.py
--rw-r--r--   0        0        0     6968 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/column.py
--rw-r--r--   0        0        0      877 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/connection.py
--rw-r--r--   0        0        0     7224 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    15069 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/container.py
--rw-r--r--   0        0        0    17732 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/control_event.py
--rw-r--r--   0        0        0     4387 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_action_sheet.py
--rw-r--r--   0        0        0     4507 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_action_sheet_action.py
--rw-r--r--   0        0        0     3102 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_activity_indicator.py
--rw-r--r--   0        0        0     3947 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_alert_dialog.py
--rw-r--r--   0        0        0     5453 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_app_bar.py
--rw-r--r--   0        0        0     3108 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_bottom_sheet.py
--rw-r--r--   0        0        0     7697 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_button.py
--rw-r--r--   0        0        0     6851 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_checkbox.py
--rw-r--r--   0        0        0     2260 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_colors.py
--rw-r--r--   0        0        0     2464 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_context_menu.py
--rw-r--r--   0        0        0     3016 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_context_menu_action.py
--rw-r--r--   0        0        0     8126 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_date_picker.py
--rw-r--r--   0        0        0     3667 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_dialog_action.py
--rw-r--r--   0        0        0     2706 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_filled_button.py
--rw-r--r--   0        0        0    61696 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_icons.py
--rw-r--r--   0        0        0     9207 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_list_tile.py
--rw-r--r--   0        0        0     6378 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_navigation_bar.py
--rw-r--r--   0        0        0     6847 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_picker.py
--rw-r--r--   0        0        0     6833 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_radio.py
--rw-r--r--   0        0        0     5590 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_segmented_button.py
--rw-r--r--   0        0        0     6429 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_slider.py
--rw-r--r--   0        0        0     4722 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_sliding_segmented_button.py
--rw-r--r--   0        0        0     7545 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_switch.py
--rw-r--r--   0        0        0    10254 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_textfield.py
--rw-r--r--   0        0        0     5308 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_timer_picker.py
--rw-r--r--   0        0        0    21708 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/datatable.py
--rw-r--r--   0        0        0    11675 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/date_picker.py
--rw-r--r--   0        0        0    10163 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/dismissible.py
--rw-r--r--   0        0        0     3081 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/divider.py
--rw-r--r--   0        0        0     7147 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6701 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/draggable.py
--rw-r--r--   0        0        0    14762 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/dropdown.py
--rw-r--r--   0        0        0    10571 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     1978 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/event.py
--rw-r--r--   0        0        0     1250 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9795 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/expansion_panel.py
--rw-r--r--   0        0        0    13461 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/expansion_tile.py
--rw-r--r--   0        0        0     9659 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2886 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     3020 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     3608 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/flet_app.py
--rw-r--r--   0        0        0    11149 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    15979 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27285 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1432 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/gradients.py
--rw-r--r--   0        0        0     8485 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2315 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3849 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/icon.py
--rw-r--r--   0        0        0    13137 2024-04-28 20:19:42.633929 flet_contrib_core-2024.4.28.2020/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362386 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/icons.py
--rw-r--r--   0        0        0     7812 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/inline_span.py
--rw-r--r--   0        0        0    17916 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     8075 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/list_view.py
--rw-r--r--   0        0        0    10049 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      219 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/locks.py
--rw-r--r--   0        0        0     5591 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/lottie.py
--rw-r--r--   0        0        0      583 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/margin.py
--rw-r--r--   0        0        0     5894 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5015 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     4319 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/menu_bar.py
--rw-r--r--   0        0        0     7484 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/menu_item_button.py
--rw-r--r--   0        0        0     1486 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/merge_semantics.py
--rw-r--r--   0        0        0    11864 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0     9992 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_drawer.py
--rw-r--r--   0        0        0    15476 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     8550 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/padding.py
--rw-r--r--   0        0        0    63608 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/page.py
--rw-r--r--   0        0        0    10503 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pagelet.py
--rw-r--r--   0        0        0     2746 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/painting.py
--rw-r--r--   0        0        0     4235 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0    13789 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     5600 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     5663 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4163 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/protocol.py
--rw-r--r--   0        0        0      106 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__init__.py
--rw-r--r--   0        0        0      310 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4520 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
--rw-r--r--   0        0        0     5620 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
--rw-r--r--   0        0        0     3393 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/pubsub_client.py
--rw-r--r--   0        0        0     5873 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/pubsub_hub.py
--rw-r--r--   0        0        0     3419 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/querystring.py
--rw-r--r--   0        0        0     9309 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/radio.py
--rw-r--r--   0        0        0     2350 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/radio_group.py
--rw-r--r--   0        0        0     8133 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/range_slider.py
--rw-r--r--   0        0        0      291 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/ref.py
--rw-r--r--   0        0        0     6438 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     5326 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/rive.py
--rw-r--r--   0        0        0     6989 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/row.py
--rw-r--r--   0        0        0     5151 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/safe_area.py
--rw-r--r--   0        0        0     4513 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/scrollable_control.py
--rw-r--r--   0        0        0    14078 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/search_bar.py
--rw-r--r--   0        0        0     8430 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/segmented_button.py
--rw-r--r--   0        0        0     1690 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/selection_area.py
--rw-r--r--   0        0        0    16317 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/semantics.py
--rw-r--r--   0        0        0     1186 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/semantics_service.py
--rw-r--r--   0        0        0      576 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5260 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2938 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0    10403 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/slider.py
--rw-r--r--   0        0        0     8473 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     5651 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/stack.py
--rw-r--r--   0        0        0     8403 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/submenu_button.py
--rw-r--r--   0        0        0    11516 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/switch.py
--rw-r--r--   0        0        0    14308 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10900 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/text.py
--rw-r--r--   0        0        0     8065 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3282 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1375 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/text_style.py
--rw-r--r--   0        0        0    18286 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/textfield.py
--rw-r--r--   0        0        0    32507 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/theme.py
--rw-r--r--   0        0        0     8094 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/time_picker.py
--rw-r--r--   0        0        0     9157 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/transform.py
--rw-r--r--   0        0        0     2847 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     3476 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/two_dimensional_scrollables.py
--rw-r--r--   0        0        0     6265 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/types.py
--rw-r--r--   0        0        0      450 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/user_control.py
--rw-r--r--   0        0        0      311 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__init__.py
--rw-r--r--   0        0        0      567 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      823 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
--rw-r--r--   0        0        0      562 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1220 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
--rw-r--r--   0        0        0      692 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
--rw-r--r--   0        0        0      565 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
--rw-r--r--   0        0        0     4687 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
--rw-r--r--   0        0        0      271 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/classproperty.py
--rw-r--r--   0        0        0      243 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/concurrency_utils.py
--rw-r--r--   0        0        0      835 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/deprecated.py
--rw-r--r--   0        0        0      465 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/slugify.py
--rw-r--r--   0        0        0      178 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/strings.py
--rw-r--r--   0        0        0     3207 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/utils/vector.py
--rw-r--r--   0        0        0       90 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/version.py
--rw-r--r--   0        0        0     3123 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0    17853 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/video.py
--rw-r--r--   0        0        0     8864 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/view.py
--rw-r--r--   0        0        0     6042 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/webview.py
--rw-r--r--   0        0        0     4181 2024-04-28 20:19:42.637929 flet_contrib_core-2024.4.28.2020/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 flet_contrib_core-2024.4.28.2020/PKG-INFO
+-rw-r--r--   0        0        0      189 2024-04-28 20:42:33.169003 flet_contrib_core-2024.4.28.2043/README.md
+-rw-r--r--   0        0        0      673 2024-04-28 20:43:17.441388 flet_contrib_core-2024.4.28.2043/pyproject.toml
+-rw-r--r--   0        0        0    10950 2024-04-28 20:42:33.169003 flet_contrib_core-2024.4.28.2043/src/flet_core/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/adaptive_control.py
+-rw-r--r--   0        0        0    13342 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     6757 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     1955 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/animation.py
+-rw-r--r--   0        0        0    11031 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7915 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/audio.py
+-rw-r--r--   0        0        0     8439 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/audio_recorder.py
+-rw-r--r--   0        0        0     5781 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/badge.py
+-rw-r--r--   0        0        0     8099 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     5930 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/bottom_app_bar.py
+-rw-r--r--   0        0        0     5830 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2103 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/buttons.py
+-rw-r--r--   0        0        0      514 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3524 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
+-rw-r--r--   0        0        0     4799 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
+-rw-r--r--   0        0        0     2352 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
+-rw-r--r--   0        0        0     1800 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0     1439 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
+-rw-r--r--   0        0        0     2596 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
+-rw-r--r--   0        0        0     2606 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
+-rw-r--r--   0        0        0     4856 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
+-rw-r--r--   0        0        0     2490 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
+-rw-r--r--   0        0        0     3005 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
+-rw-r--r--   0        0        0     2534 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
+-rw-r--r--   0        0        0      704 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
+-rw-r--r--   0        0        0     4879 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
+-rw-r--r--   0        0        0     2910 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4813 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1646 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1236 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      844 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1869 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1891 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3493 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1813 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2345 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1951 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     8220 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/card.py
+-rw-r--r--   0        0        0     9184 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     2761 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
+-rw-r--r--   0        0        0     7264 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
+-rw-r--r--   0        0        0     2642 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
+-rw-r--r--   0        0        0     3314 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
+-rw-r--r--   0        0        0     1867 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
+-rw-r--r--   0        0        0      693 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
+-rw-r--r--   0        0        0      654 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1541 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
+-rw-r--r--   0        0        0    10717 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     9157 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
+-rw-r--r--   0        0        0     5936 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
+-rw-r--r--   0        0        0     5564 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     4511 2024-04-28 20:42:33.177003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
+-rw-r--r--   0        0        0     9932 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2044 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6679 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1932 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2923 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11305 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     9357 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5338 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5965 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3807 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0    12179 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0    14830 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/chip.py
+-rw-r--r--   0        0        0     9261 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3097 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0    10869 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6968 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/column.py
+-rw-r--r--   0        0        0      877 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7224 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    15069 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/container.py
+-rw-r--r--   0        0        0    17732 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/control_event.py
+-rw-r--r--   0        0        0     4387 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_action_sheet.py
+-rw-r--r--   0        0        0     4507 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_action_sheet_action.py
+-rw-r--r--   0        0        0     3102 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_activity_indicator.py
+-rw-r--r--   0        0        0     3947 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_alert_dialog.py
+-rw-r--r--   0        0        0     5453 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_app_bar.py
+-rw-r--r--   0        0        0     3108 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_bottom_sheet.py
+-rw-r--r--   0        0        0     7697 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_button.py
+-rw-r--r--   0        0        0     6851 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_checkbox.py
+-rw-r--r--   0        0        0     2260 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_colors.py
+-rw-r--r--   0        0        0     2464 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_context_menu.py
+-rw-r--r--   0        0        0     3016 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_context_menu_action.py
+-rw-r--r--   0        0        0     8126 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_date_picker.py
+-rw-r--r--   0        0        0     3667 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_dialog_action.py
+-rw-r--r--   0        0        0     2706 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_filled_button.py
+-rw-r--r--   0        0        0    61696 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_icons.py
+-rw-r--r--   0        0        0     9207 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_list_tile.py
+-rw-r--r--   0        0        0     6378 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_navigation_bar.py
+-rw-r--r--   0        0        0     6847 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_picker.py
+-rw-r--r--   0        0        0     6833 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_radio.py
+-rw-r--r--   0        0        0     5590 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_segmented_button.py
+-rw-r--r--   0        0        0     6429 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_slider.py
+-rw-r--r--   0        0        0     4722 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_sliding_segmented_button.py
+-rw-r--r--   0        0        0     7545 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_switch.py
+-rw-r--r--   0        0        0    10254 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_textfield.py
+-rw-r--r--   0        0        0     5308 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_timer_picker.py
+-rw-r--r--   0        0        0    21708 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/datatable.py
+-rw-r--r--   0        0        0    11675 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/date_picker.py
+-rw-r--r--   0        0        0    10163 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/dismissible.py
+-rw-r--r--   0        0        0     3081 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/divider.py
+-rw-r--r--   0        0        0     7147 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6701 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/draggable.py
+-rw-r--r--   0        0        0    14762 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0    10571 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/event.py
+-rw-r--r--   0        0        0     1250 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9795 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/expansion_panel.py
+-rw-r--r--   0        0        0    13461 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/expansion_tile.py
+-rw-r--r--   0        0        0     9659 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2886 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     3020 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     3608 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0    11149 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    15979 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    27285 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1432 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     8485 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2315 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3849 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/icon.py
+-rw-r--r--   0        0        0    13137 2024-04-28 20:42:33.181003 flet_contrib_core-2024.4.28.2043/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362386 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/icons.py
+-rw-r--r--   0        0        0     7812 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0    17916 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     8075 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/list_view.py
+-rw-r--r--   0        0        0    10049 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      219 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/locks.py
+-rw-r--r--   0        0        0     5591 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/lottie.py
+-rw-r--r--   0        0        0      583 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/margin.py
+-rw-r--r--   0        0        0     5894 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5015 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     4319 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/menu_bar.py
+-rw-r--r--   0        0        0     7484 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/menu_item_button.py
+-rw-r--r--   0        0        0     1486 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/merge_semantics.py
+-rw-r--r--   0        0        0    11864 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0     9992 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_drawer.py
+-rw-r--r--   0        0        0    15476 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     8550 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/padding.py
+-rw-r--r--   0        0        0    63608 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/page.py
+-rw-r--r--   0        0        0    10503 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pagelet.py
+-rw-r--r--   0        0        0     2746 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4235 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0    13789 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     5600 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     5663 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4163 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/protocol.py
+-rw-r--r--   0        0        0      106 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4520 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
+-rw-r--r--   0        0        0     5620 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
+-rw-r--r--   0        0        0     3393 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/pubsub_client.py
+-rw-r--r--   0        0        0     5873 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/pubsub_hub.py
+-rw-r--r--   0        0        0     3419 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     9309 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2350 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0     8133 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/range_slider.py
+-rw-r--r--   0        0        0      291 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6438 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     5326 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/rive.py
+-rw-r--r--   0        0        0     6989 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/row.py
+-rw-r--r--   0        0        0     5151 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/safe_area.py
+-rw-r--r--   0        0        0     4513 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0    14078 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/search_bar.py
+-rw-r--r--   0        0        0     8430 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/segmented_button.py
+-rw-r--r--   0        0        0     1690 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/selection_area.py
+-rw-r--r--   0        0        0    16317 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/semantics.py
+-rw-r--r--   0        0        0     1186 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/semantics_service.py
+-rw-r--r--   0        0        0      576 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5260 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2938 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0    10403 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/slider.py
+-rw-r--r--   0        0        0     8473 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     5651 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8403 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/submenu_button.py
+-rw-r--r--   0        0        0    11516 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/switch.py
+-rw-r--r--   0        0        0    14308 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10900 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/text.py
+-rw-r--r--   0        0        0     8065 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3282 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1375 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    18286 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/textfield.py
+-rw-r--r--   0        0        0    32507 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8094 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/time_picker.py
+-rw-r--r--   0        0        0     9157 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2847 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     3476 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/two_dimensional_scrollables.py
+-rw-r--r--   0        0        0     6265 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/types.py
+-rw-r--r--   0        0        0      450 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      311 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      823 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
+-rw-r--r--   0        0        0      562 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1220 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
+-rw-r--r--   0        0        0      692 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
+-rw-r--r--   0        0        0      565 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
+-rw-r--r--   0        0        0     4687 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
+-rw-r--r--   0        0        0      271 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/classproperty.py
+-rw-r--r--   0        0        0      243 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/concurrency_utils.py
+-rw-r--r--   0        0        0      835 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/deprecated.py
+-rw-r--r--   0        0        0      465 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/slugify.py
+-rw-r--r--   0        0        0      178 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/strings.py
+-rw-r--r--   0        0        0     3207 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/utils/vector.py
+-rw-r--r--   0        0        0       90 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/version.py
+-rw-r--r--   0        0        0     3123 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0    17853 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/video.py
+-rw-r--r--   0        0        0     8864 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/view.py
+-rw-r--r--   0        0        0     6042 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/webview.py
+-rw-r--r--   0        0        0     4181 2024-04-28 20:42:33.185003 flet_contrib_core-2024.4.28.2043/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 flet_contrib_core-2024.4.28.2043/PKG-INFO
```

### Comparing `flet_contrib_core-2024.4.28.2020/pyproject.toml` & `flet_contrib_core-2024.4.28.2043/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-core"
-version = "2024.04.28.2020"
+version = "2024.04.28.2043"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/__init__.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/alert_dialog.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/animated_switcher.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/animation.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/app_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/audio.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/audio_recorder.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/audio_recorder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/badge.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/badge.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/banner.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/border.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/border_radius.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/bottom_app_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/bottom_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/bottom_sheet.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/buttons.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__init__.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/color.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/color.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/line.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/path.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/path.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/points.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/points.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/__pycache__/text.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/__pycache__/text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/arc.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/canvas.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/circle.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/color.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/fill.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/line.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/oval.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/path.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/points.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/rect.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/shadow.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/canvas/text.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/card.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_group.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_rod.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_axis.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_axis_label.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/chart_point_shape.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart_data.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/line_chart_data_point.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/pie_chart.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/charts/pie_chart_section.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/checkbox.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/chip.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/chip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/circle_avatar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/client_storage.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/colors.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/column.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/connection.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/constrained_control.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/container.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/control.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_action_sheet.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_action_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_action_sheet_action.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_action_sheet_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_activity_indicator.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_activity_indicator.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_alert_dialog.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_app_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_bottom_sheet.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_checkbox.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_colors.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_context_menu.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_context_menu.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_context_menu_action.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_context_menu_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_date_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_dialog_action.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_dialog_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_filled_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_icons.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_list_tile.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_navigation_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_radio.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_segmented_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_slider.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_sliding_segmented_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_sliding_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_switch.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_textfield.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/cupertino_timer_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/cupertino_timer_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/datatable.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/date_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/dismissible.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/dismissible.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/divider.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/drag_target.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/draggable.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/dropdown.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/elevated_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/embed_json_encoder.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/event_handler.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/expansion_panel.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/expansion_panel.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/expansion_tile.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/expansion_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/file_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/filled_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/filled_tonal_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/flet_app.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/floating_action_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/form_field_control.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/gesture_detector.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/gradients.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/grid_view.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/haptic_feedback.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/icon.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/icon_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/icons.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/image.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/list_tile.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/list_view.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/local_connection.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/lottie.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/lottie.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/margin.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/markdown.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/matplotlib_chart.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/menu_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/menu_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/menu_item_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/menu_item_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/merge_semantics.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/merge_semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_drawer.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_drawer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/navigation_rail.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/outlined_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/padding.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/page.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/pagelet.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/pagelet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/painting.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/plotly_chart.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/popup_menu_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/progress_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/progress_ring.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/protocol.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/pubsub_client.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/pubsub_client.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/pubsub/pubsub_hub.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/pubsub/pubsub_hub.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/querystring.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/radio.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/radio_group.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/range_slider.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/range_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/responsive_row.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/rive.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/rive.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/row.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/safe_area.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/safe_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/scrollable_control.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/search_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/search_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/segmented_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/selection_area.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/selection_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/semantics.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/semantics_service.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/semantics_service.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/session_storage.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/shader_mask.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/shadow.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/shake_detector.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/slider.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/snack_bar.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/stack.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/submenu_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/submenu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/switch.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/tabs.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/template_route.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/text.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/text_button.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/text_span.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/text_style.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/textfield.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/theme.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/time_picker.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/time_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/tooltip.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/transform.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/transparent_pointer.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/two_dimensional_scrollables.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/two_dimensional_scrollables.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/types.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/strings.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/strings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/__pycache__/vector.cpython-39.pyc` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/__pycache__/vector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/deprecated.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/utils/vector.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/utils/vector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/vertical_divider.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/video.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/video.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/view.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/webview.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/webview.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/src/flet_core/window_drag_area.py` & `flet_contrib_core-2024.4.28.2043/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2020/PKG-INFO` & `flet_contrib_core-2024.4.28.2043/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-contrib-core
-Version: 2024.4.28.2020
+Version: 2024.4.28.2043
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

