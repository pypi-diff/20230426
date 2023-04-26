# Comparing `tmp/flet_core-0.6.0.dev1352.tar.gz` & `tmp/flet_core-0.6.0.dev1355.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_core-0.6.0.dev1352.tar", max compression
+gzip compressed data, was "flet_core-0.6.0.dev1355.tar", max compression
```

## Comparing `flet_core-0.6.0.dev1352.tar` & `flet_core-0.6.0.dev1355.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0      189 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/README.md
--rw-r--r--   0        0        0      723 2023-04-24 23:27:59.249248 flet_core-0.6.0.dev1352/pyproject.toml
--rw-r--r--   0        0        0     6335 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/__init__.py
--rw-r--r--   0        0        0     6774 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/alignment.py
--rw-r--r--   0        0        0     7226 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     2806 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/animation.py
--rw-r--r--   0        0        0     5403 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7301 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/audio.py
--rw-r--r--   0        0        0     5446 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     2826 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2202 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/buttons.py
--rw-r--r--   0        0        0     3044 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/callable_control.py
--rw-r--r--   0        0        0      514 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0     2903 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4629 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1639 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1361 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      837 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1862 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1907 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3486 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1772 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2361 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1963 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     5639 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/card.py
--rw-r--r--   0        0        0     9855 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2061 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6837 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1949 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2924 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11228 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     8258 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5496 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5888 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3824 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0     7122 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/checkbox.py
--rw-r--r--   0        0        0     6739 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3085 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/client_storage.py
--rw-r--r--   0        0        0     1002 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/clipboard.py
--rw-r--r--   0        0        0    10627 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/colors.py
--rw-r--r--   0        0        0     7305 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/column.py
--rw-r--r--   0        0        0     1132 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/connection.py
--rw-r--r--   0        0        0     6848 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    13384 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/container.py
--rw-r--r--   0        0        0    14162 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/control_event.py
--rw-r--r--   0        0        0    20740 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/datatable.py
--rw-r--r--   0        0        0     2263 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/divider.py
--rw-r--r--   0        0        0     6270 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6063 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/draggable.py
--rw-r--r--   0        0        0     9121 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/dropdown.py
--rw-r--r--   0        0        0     8066 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     2170 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/event.py
--rw-r--r--   0        0        0     1839 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9777 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2505 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     2639 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     2542 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/flet_app.py
--rw-r--r--   0        0        0     6556 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    13925 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27988 2023-04-24 23:27:23.777017 flet_core-0.6.0.dev1352/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1531 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/gradients.py
--rw-r--r--   0        0        0     6301 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2134 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3375 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/icon.py
--rw-r--r--   0        0        0     7700 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362652 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/icons.py
--rw-r--r--   0        0        0     6530 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/inline_span.py
--rw-r--r--   0        0        0     7805 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     6206 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/list_view.py
--rw-r--r--   0        0        0     8644 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      223 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/locks.py
--rw-r--r--   0        0        0      583 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/margin.py
--rw-r--r--   0        0        0     5165 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5125 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     8322 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0    11986 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     6751 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/padding.py
--rw-r--r--   0        0        0    52427 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/page.py
--rw-r--r--   0        0        0     2674 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/painting.py
--rw-r--r--   0        0        0     4355 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0     6756 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     4237 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     4435 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4088 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/protocol.py
--rw-r--r--   0        0        0     3419 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/querystring.py
--rw-r--r--   0        0        0     5731 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/radio.py
--rw-r--r--   0        0        0     2389 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/radio_group.py
--rw-r--r--   0        0        0      291 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/ref.py
--rw-r--r--   0        0        0     6354 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     7289 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/row.py
--rw-r--r--   0        0        0     1637 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/semantics.py
--rw-r--r--   0        0        0      576 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5318 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2919 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0     7326 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/slider.py
--rw-r--r--   0        0        0     3971 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     4833 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/stack.py
--rw-r--r--   0        0        0     8092 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/switch.py
--rw-r--r--   0        0        0     6776 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10512 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/text.py
--rw-r--r--   0        0        0     6724 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/text_button.py
--rw-r--r--   0        0        0     2593 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1260 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/text_style.py
--rw-r--r--   0        0        0    15388 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/textfield.py
--rw-r--r--   0        0        0     1482 2023-04-24 23:27:23.781017 flet_core-0.6.0.dev1352/src/flet_core/theme.py
--rw-r--r--   0        0        0     8362 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/transform.py
--rw-r--r--   0        0        0     2753 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     5186 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/types.py
--rw-r--r--   0        0        0      684 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/user_control.py
--rw-r--r--   0        0        0      409 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/utils.py
--rw-r--r--   0        0        0     2337 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0     6225 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/view.py
--rw-r--r--   0        0        0     4049 2023-04-24 23:27:23.785017 flet_core-0.6.0.dev1352/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.6.0.dev1352/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/README.md
+-rw-r--r--   0        0        0      723 2023-04-25 18:17:21.144500 flet_core-0.6.0.dev1355/pyproject.toml
+-rw-r--r--   0        0        0     6335 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/__init__.py
+-rw-r--r--   0        0        0     6774 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     7226 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     2806 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/animation.py
+-rw-r--r--   0        0        0     5403 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7301 2023-04-25 18:16:44.298373 flet_core-0.6.0.dev1355/src/flet_core/audio.py
+-rw-r--r--   0        0        0     5446 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     2826 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2202 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/buttons.py
+-rw-r--r--   0        0        0     3044 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/callable_control.py
+-rw-r--r--   0        0        0      514 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0     2903 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4629 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1639 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1361 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      837 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1862 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1907 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3486 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1772 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2361 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1963 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     5639 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/card.py
+-rw-r--r--   0        0        0     9855 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2061 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6837 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1949 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2924 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11228 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     8258 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5496 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5888 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3824 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0     7122 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0     6739 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3085 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0     1002 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/clipboard.py
+-rw-r--r--   0        0        0    10627 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/colors.py
+-rw-r--r--   0        0        0     7305 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/column.py
+-rw-r--r--   0        0        0     1132 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/connection.py
+-rw-r--r--   0        0        0     6848 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    13883 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/container.py
+-rw-r--r--   0        0        0    14162 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/control_event.py
+-rw-r--r--   0        0        0    20740 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/datatable.py
+-rw-r--r--   0        0        0     2263 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/divider.py
+-rw-r--r--   0        0        0     6270 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6063 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/draggable.py
+-rw-r--r--   0        0        0     9121 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0     8565 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     2170 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/event.py
+-rw-r--r--   0        0        0     1839 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9777 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2638 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     2772 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     2542 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0     7055 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    13925 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    27988 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1531 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     6301 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2134 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3375 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/icon.py
+-rw-r--r--   0        0        0     8199 2023-04-25 18:16:44.302373 flet_core-0.6.0.dev1355/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362652 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/icons.py
+-rw-r--r--   0        0        0     6530 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0     8304 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     6206 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/list_view.py
+-rw-r--r--   0        0        0     8644 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      223 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/locks.py
+-rw-r--r--   0        0        0      583 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/margin.py
+-rw-r--r--   0        0        0     6073 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5125 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     8322 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0    11986 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     7250 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/padding.py
+-rw-r--r--   0        0        0    52427 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/page.py
+-rw-r--r--   0        0        0     2674 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4355 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0     6756 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     4237 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     4435 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4088 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/protocol.py
+-rw-r--r--   0        0        0     3419 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     5731 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2389 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0      291 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6354 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     7289 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/row.py
+-rw-r--r--   0        0        0     1637 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/semantics.py
+-rw-r--r--   0        0        0      576 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5318 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2919 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0     7326 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/slider.py
+-rw-r--r--   0        0        0     3971 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     4833 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8092 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/switch.py
+-rw-r--r--   0        0        0     6776 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10512 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/text.py
+-rw-r--r--   0        0        0     7223 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3092 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1260 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    15388 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/textfield.py
+-rw-r--r--   0        0        0     1482 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8362 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2753 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     5186 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/types.py
+-rw-r--r--   0        0        0      684 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      409 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/utils.py
+-rw-r--r--   0        0        0     2337 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0     6225 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/view.py
+-rw-r--r--   0        0        0     4049 2023-04-25 18:16:44.306373 flet_core-0.6.0.dev1355/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.6.0.dev1355/PKG-INFO
```

### Comparing `flet_core-0.6.0.dev1352/pyproject.toml` & `flet_core-0.6.0.dev1355/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-core"
-version = "0.6.0.dev1352"
+version = "0.6.0.dev1355"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/__init__.py` & `flet_core-0.6.0.dev1355/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/alert_dialog.py` & `flet_core-0.6.0.dev1355/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/animated_switcher.py` & `flet_core-0.6.0.dev1355/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/animation.py` & `flet_core-0.6.0.dev1355/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/app_bar.py` & `flet_core-0.6.0.dev1355/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/audio.py` & `flet_core-0.6.0.dev1355/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/banner.py` & `flet_core-0.6.0.dev1355/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/border.py` & `flet_core-0.6.0.dev1355/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/border_radius.py` & `flet_core-0.6.0.dev1355/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/bottom_sheet.py` & `flet_core-0.6.0.dev1355/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/buttons.py` & `flet_core-0.6.0.dev1355/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/callable_control.py` & `flet_core-0.6.0.dev1355/src/flet_core/callable_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/__init__.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/arc.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/canvas.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/circle.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/color.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/fill.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/line.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/oval.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/path.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/points.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/rect.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/shadow.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/canvas/text.py` & `flet_core-0.6.0.dev1355/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/card.py` & `flet_core-0.6.0.dev1355/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_group.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_rod.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/chart_axis.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/chart_axis_label.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/chart_point_shape.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart_data.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/line_chart_data_point.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/pie_chart.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/charts/pie_chart_section.py` & `flet_core-0.6.0.dev1355/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/checkbox.py` & `flet_core-0.6.0.dev1355/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/circle_avatar.py` & `flet_core-0.6.0.dev1355/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/client_storage.py` & `flet_core-0.6.0.dev1355/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/clipboard.py` & `flet_core-0.6.0.dev1355/src/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/colors.py` & `flet_core-0.6.0.dev1355/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/column.py` & `flet_core-0.6.0.dev1355/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/connection.py` & `flet_core-0.6.0.dev1355/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/constrained_control.py` & `flet_core-0.6.0.dev1355/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/container.py` & `flet_core-0.6.0.dev1355/src/flet_core/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,16 @@
         clip_behavior: Optional[ClipBehavior] = None,
         ink: Optional[bool] = None,
         animate: AnimationValue = None,
         blur: Union[
             None, float, int, Tuple[Union[float, int], Union[float, int]], Blur
         ] = None,
         shadow: Union[None, BoxShadow, List[BoxShadow]] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
@@ -172,14 +174,16 @@
         self.image_opacity = image_opacity
         self.shape = shape
         self.clip_behavior = clip_behavior
         self.ink = ink
         self.animate = animate
         self.blur = blur
         self.shadow = shadow
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_long_press = on_long_press
         self.on_hover = on_hover
 
     def _get_control_name(self):
         return "container"
 
@@ -417,14 +421,32 @@
     def animate(self) -> AnimationValue:
         return self.__animate
 
     @animate.setter
     def animate(self, value: AnimationValue):
         self.__animate = value
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self.__on_click
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/control.py` & `flet_core-0.6.0.dev1355/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/datatable.py` & `flet_core-0.6.0.dev1355/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/divider.py` & `flet_core-0.6.0.dev1355/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/drag_target.py` & `flet_core-0.6.0.dev1355/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/draggable.py` & `flet_core-0.6.0.dev1355/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/dropdown.py` & `flet_core-0.6.0.dev1355/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/elevated_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/elevated_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         bgcolor: Optional[str] = None,
         elevation: OptionalNumber = None,
         style: Optional[ButtonStyle] = None,
         icon: Optional[str] = None,
         icon_color: Optional[str] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
@@ -120,14 +122,16 @@
         self.bgcolor = bgcolor
         self.elevation = elevation
         self.style = style
         self.icon = icon
         self.icon_color = icon_color
         self.content = content
         self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_long_press = on_long_press
         self.on_hover = on_hover
         self.on_focus = on_focus
         self.on_blur = on_blur
 
     def _get_control_name(self):
@@ -223,14 +227,32 @@
     def icon_color(self):
         return self._get_attr("iconColor")
 
     @icon_color.setter
     def icon_color(self, value):
         self._set_attr("iconColor", value)
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/embed_json_encoder.py` & `flet_core-0.6.0.dev1355/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/event_handler.py` & `flet_core-0.6.0.dev1355/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/file_picker.py` & `flet_core-0.6.0.dev1355/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/filled_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/filled_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         # Specific
         #
         icon: Optional[str] = None,
         icon_color: Optional[str] = None,
         style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ElevatedButton.__init__(
             self,
             ref=ref,
@@ -77,11 +79,13 @@
             elevation=0,
             style=style,
             text=text,
             icon=icon,
             icon_color=icon_color,
             content=content,
             autofocus=autofocus,
+            url=url,
+            url_target=url_target,
             on_click=on_click,
             on_long_press=on_long_press,
             on_hover=on_hover,
         )
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/filled_tonal_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/filled_tonal_button.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         # Specific
         #
         icon: Optional[str] = None,
         icon_color: Optional[str] = None,
         style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
     ):
         ElevatedButton.__init__(
             self,
             ref=ref,
@@ -77,11 +79,13 @@
             elevation=0,
             style=style,
             text=text,
             icon=icon,
             icon_color=icon_color,
             content=content,
             autofocus=autofocus,
+            url=url,
+            url_target=url_target,
             on_click=on_click,
             on_long_press=on_long_press,
             on_hover=on_hover,
         )
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/flet_app.py` & `flet_core-0.6.0.dev1355/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/floating_action_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/floating_action_button.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,14 +95,16 @@
         #
         icon: Optional[str] = None,
         bgcolor: Optional[str] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
         shape: Optional[OutlinedBorder] = None,
         mini: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
             width=width,
             height=height,
@@ -133,14 +135,16 @@
         self.text = text
         self.icon = icon
         self.bgcolor = bgcolor
         self.content = content
         self.autofocus = autofocus
         self.shape = shape
         self.mini = mini
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
 
     def _get_control_name(self):
         return "floatingactionbutton"
 
     def _before_build_command(self):
         super()._before_build_command()
@@ -175,14 +179,32 @@
     def bgcolor(self):
         return self._get_attr("bgcolor")
 
     @bgcolor.setter
     def bgcolor(self, value):
         self._set_attr("bgcolor", value)
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/form_field_control.py` & `flet_core-0.6.0.dev1355/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/gesture_detector.py` & `flet_core-0.6.0.dev1355/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/gradients.py` & `flet_core-0.6.0.dev1355/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/grid_view.py` & `flet_core-0.6.0.dev1355/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/haptic_feedback.py` & `flet_core-0.6.0.dev1355/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/icon.py` & `flet_core-0.6.0.dev1355/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/icon_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/icon_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         selected_icon: Optional[str] = None,
         selected_icon_color: Optional[str] = None,
         selected: Optional[bool] = None,
         bgcolor: Optional[str] = None,
         style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
@@ -132,14 +134,16 @@
         self.selected_icon = selected_icon
         self.selected_icon_color = selected_icon_color
         self.selected = selected
         self.bgcolor = bgcolor
         self.style = style
         self.content = content
         self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_focus = on_focus
         self.on_blur = on_blur
 
     def _get_control_name(self):
         return "iconbutton"
 
@@ -229,14 +233,32 @@
     def style(self) -> Optional[ButtonStyle]:
         return self.__style
 
     @style.setter
     def style(self, value: Optional[ButtonStyle]):
         self.__style = value
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/icons.py` & `flet_core-0.6.0.dev1355/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/image.py` & `flet_core-0.6.0.dev1355/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/list_tile.py` & `flet_core-0.6.0.dev1355/src/flet_core/list_tile.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         title: Optional[Control] = None,
         subtitle: Optional[Control] = None,
         trailing: Optional[Control] = None,
         is_three_line: Optional[bool] = None,
         selected: Optional[bool] = None,
         dense: Optional[bool] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
             width=width,
@@ -130,14 +132,16 @@
         self.title = title
         self.subtitle = subtitle
         self.trailing = trailing
         self.is_three_line = is_three_line
         self.selected = selected
         self.dense = dense
         self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_long_press = on_long_press
 
     def _get_control_name(self):
         return "listtile"
 
     def _before_build_command(self):
@@ -237,14 +241,32 @@
     def autofocus(self) -> Optional[bool]:
         return self._get_attr("autofocus", data_type="bool", def_value=False)
 
     @autofocus.setter
     def autofocus(self, value: Optional[bool]):
         self._set_attr("autofocus", value)
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/list_view.py` & `flet_core-0.6.0.dev1355/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/local_connection.py` & `flet_core-0.6.0.dev1355/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/margin.py` & `flet_core-0.6.0.dev1355/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/markdown.py` & `flet_core-0.6.0.dev1355/src/flet_core/markdown.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, cast
 
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import OptionalNumber
 from flet_core.ref import Ref
 from flet_core.text_style import TextStyle
 from flet_core.types import (
     AnimationValue,
@@ -70,14 +70,16 @@
         #
         # Specific
         #
         selectable: Optional[bool] = None,
         extension_set: Optional[MarkdownExtensionSet] = None,
         code_theme: Optional[str] = None,
         code_style: Optional[TextStyle] = None,
+        auto_follow_links: Optional[bool] = None,
+        auto_follow_links_target: Optional[str] = None,
         on_tap_link=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
             width=width,
             height=height,
@@ -106,14 +108,16 @@
         )
 
         self.value = value
         self.selectable = selectable
         self.extension_set = extension_set
         self.code_theme = code_theme
         self.code_style = code_style
+        self.auto_follow_links = auto_follow_links
+        self.auto_follow_links_target = auto_follow_links_target
         self.on_tap_link = on_tap_link
 
     def _get_control_name(self):
         return "markdown"
 
     def _before_build_command(self):
         super()._before_build_command()
@@ -167,14 +171,35 @@
     def code_style(self):
         return self.__code_style
 
     @code_style.setter
     def code_style(self, value: Optional[TextStyle]):
         self.__code_style = value
 
+    # auto_follow_links
+    @property
+    def auto_follow_links(self) -> Optional[bool]:
+        return cast(
+            Optional[bool],
+            self._get_attr("autoFollowLinks", data_type="bool", def_value=False),
+        )
+
+    @auto_follow_links.setter
+    def auto_follow_links(self, value: Optional[bool]):
+        self._set_attr("autoFollowLinks", value)
+
+    # auto_follow_links_target
+    @property
+    def auto_follow_links_target(self) -> Optional[str]:
+        return self._get_attr("autoFollowLinksTarget")
+
+    @auto_follow_links_target.setter
+    def auto_follow_links_target(self, value: Optional[str]):
+        self._set_attr("autoFollowLinksTarget", value)
+
     # on_tap_link
     @property
     def on_tap_link(self):
         return self._get_event_handler("tap_link")
 
     @on_tap_link.setter
     def on_tap_link(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/matplotlib_chart.py` & `flet_core-0.6.0.dev1355/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/navigation_bar.py` & `flet_core-0.6.0.dev1355/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/navigation_rail.py` & `flet_core-0.6.0.dev1355/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/outlined_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/outlined_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         # Specific
         #
         icon: Optional[str] = None,
         icon_color: Optional[str] = None,
         style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
@@ -110,14 +112,16 @@
 
         self.text = text
         self.icon = icon
         self.icon_color = icon_color
         self.style = style
         self.content = content
         self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_long_press = on_long_press
         self.on_hover = on_hover
         self.on_focus = on_focus
         self.on_blur = on_blur
 
     def _get_control_name(self):
@@ -173,14 +177,32 @@
     def style(self) -> Optional[ButtonStyle]:
         return self.__style
 
     @style.setter
     def style(self, value: Optional[ButtonStyle]):
         self.__style = value
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/padding.py` & `flet_core-0.6.0.dev1355/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/page.py` & `flet_core-0.6.0.dev1355/src/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/painting.py` & `flet_core-0.6.0.dev1355/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/plotly_chart.py` & `flet_core-0.6.0.dev1355/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/popup_menu_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/progress_bar.py` & `flet_core-0.6.0.dev1355/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/progress_ring.py` & `flet_core-0.6.0.dev1355/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/protocol.py` & `flet_core-0.6.0.dev1355/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/querystring.py` & `flet_core-0.6.0.dev1355/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/radio.py` & `flet_core-0.6.0.dev1355/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/radio_group.py` & `flet_core-0.6.0.dev1355/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/responsive_row.py` & `flet_core-0.6.0.dev1355/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/row.py` & `flet_core-0.6.0.dev1355/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/semantics.py` & `flet_core-0.6.0.dev1355/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/session_storage.py` & `flet_core-0.6.0.dev1355/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/shader_mask.py` & `flet_core-0.6.0.dev1355/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/shadow.py` & `flet_core-0.6.0.dev1355/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/shake_detector.py` & `flet_core-0.6.0.dev1355/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/slider.py` & `flet_core-0.6.0.dev1355/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/snack_bar.py` & `flet_core-0.6.0.dev1355/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/stack.py` & `flet_core-0.6.0.dev1355/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/switch.py` & `flet_core-0.6.0.dev1355/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/tabs.py` & `flet_core-0.6.0.dev1355/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/template_route.py` & `flet_core-0.6.0.dev1355/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/text.py` & `flet_core-0.6.0.dev1355/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/text_button.py` & `flet_core-0.6.0.dev1355/src/flet_core/text_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         # Specific
         #
         icon: Optional[str] = None,
         icon_color: Optional[str] = None,
         style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
         autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_long_press=None,
         on_hover=None,
         on_focus=None,
         on_blur=None,
     ):
         ConstrainedControl.__init__(
@@ -110,14 +112,16 @@
 
         self.text = text
         self.icon = icon
         self.icon_color = icon_color
         self.style = style
         self.content = content
         self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_long_press = on_long_press
         self.on_hover = on_hover
         self.on_focus = on_focus
         self.on_blur = on_blur
 
     def _get_control_name(self):
@@ -173,14 +177,32 @@
     def style(self) -> Optional[ButtonStyle]:
         return self.__style
 
     @style.setter
     def style(self, value: Optional[ButtonStyle]):
         self.__style = value
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/text_span.py` & `flet_core-0.6.0.dev1355/src/flet_core/text_span.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 class TextSpan(InlineSpan):
     def __init__(
         self,
         text: Optional[str] = None,
         style: Optional[TextStyle] = None,
         spans: Optional[List[InlineSpan]] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
         on_click=None,
         on_enter=None,
         on_exit=None,
         # base
         ref=None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
@@ -22,14 +24,16 @@
         InlineSpan.__init__(
             self, ref=ref, visible=visible, disabled=disabled, data=data
         )
 
         self.text = text
         self.style = style
         self.spans = spans
+        self.url = url
+        self.url_target = url_target
         self.on_click = on_click
         self.on_enter = on_enter
         self.on_exit = on_exit
 
     def _get_control_name(self):
         return "textspan"
 
@@ -65,14 +69,32 @@
     def spans(self) -> Optional[List[InlineSpan]]:
         return self.__spans
 
     @spans.setter
     def spans(self, value: Optional[List[InlineSpan]]):
         self.__spans = value if value is not None else []
 
+    # url
+    @property
+    def url(self):
+        return self._get_attr("url")
+
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
+
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
+
     # on_click
     @property
     def on_click(self):
         return self._get_event_handler("click")
 
     @on_click.setter
     def on_click(self, handler):
```

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/text_style.py` & `flet_core-0.6.0.dev1355/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/textfield.py` & `flet_core-0.6.0.dev1355/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/theme.py` & `flet_core-0.6.0.dev1355/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/tooltip.py` & `flet_core-0.6.0.dev1355/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/transform.py` & `flet_core-0.6.0.dev1355/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/transparent_pointer.py` & `flet_core-0.6.0.dev1355/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/types.py` & `flet_core-0.6.0.dev1355/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/user_control.py` & `flet_core-0.6.0.dev1355/src/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/vertical_divider.py` & `flet_core-0.6.0.dev1355/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/view.py` & `flet_core-0.6.0.dev1355/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/src/flet_core/window_drag_area.py` & `flet_core-0.6.0.dev1355/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.6.0.dev1352/PKG-INFO` & `flet_core-0.6.0.dev1355/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-core
-Version: 0.6.0.dev1352
+Version: 0.6.0.dev1355
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

