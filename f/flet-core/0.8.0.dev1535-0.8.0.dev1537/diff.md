# Comparing `tmp/flet_core-0.8.0.dev1535.tar.gz` & `tmp/flet_core-0.8.0.dev1537.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_core-0.8.0.dev1535.tar", max compression
+gzip compressed data, was "flet_core-0.8.0.dev1537.tar", max compression
```

## Comparing `flet_core-0.8.0.dev1535.tar` & `flet_core-0.8.0.dev1537.tar`

### file list

```diff
@@ -1,133 +1,132 @@
--rw-r--r--   0        0        0      189 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/README.md
--rw-r--r--   0        0        0      723 2023-06-17 02:45:33.078577 flet_core-0.8.0.dev1535/pyproject.toml
--rw-r--r--   0        0        0     6546 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/__init__.py
--rw-r--r--   0        0        0     6774 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/alignment.py
--rw-r--r--   0        0        0     7226 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     2806 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/animation.py
--rw-r--r--   0        0        0     5403 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7301 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/audio.py
--rw-r--r--   0        0        0     5446 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     4320 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2202 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/buttons.py
--rw-r--r--   0        0        0     3044 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/callable_control.py
--rw-r--r--   0        0        0      514 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4629 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1639 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1361 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      837 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1862 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1907 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3486 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1772 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2361 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1963 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     5695 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/card.py
--rw-r--r--   0        0        0     9855 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2061 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6837 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1949 2023-06-17 02:45:00.182597 flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2924 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11228 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     8258 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5496 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5888 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3824 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0     7156 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/checkbox.py
--rw-r--r--   0        0        0     6795 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3085 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/client_storage.py
--rw-r--r--   0        0        0     1002 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/clipboard.py
--rw-r--r--   0        0        0    10708 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/colors.py
--rw-r--r--   0        0        0     6924 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/column.py
--rw-r--r--   0        0        0     1132 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/connection.py
--rw-r--r--   0        0        0     7099 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    14684 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/container.py
--rw-r--r--   0        0        0    14139 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/control_event.py
--rw-r--r--   0        0        0    20707 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/datatable.py
--rw-r--r--   0        0        0     2263 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/divider.py
--rw-r--r--   0        0        0     6270 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6063 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/draggable.py
--rw-r--r--   0        0        0     9177 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/dropdown.py
--rw-r--r--   0        0        0     8848 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     1978 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/event.py
--rw-r--r--   0        0        0     1839 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9777 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2694 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     2828 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     3613 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/flet_app.py
--rw-r--r--   0        0        0     7111 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    13981 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    28044 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1531 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/gradients.py
--rw-r--r--   0        0        0     6804 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2134 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3430 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/icon.py
--rw-r--r--   0        0        0     8438 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362652 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/icons.py
--rw-r--r--   0        0        0     7171 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/inline_span.py
--rw-r--r--   0        0        0     8737 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     6401 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/list_view.py
--rw-r--r--   0        0        0     8644 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      223 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/locks.py
--rw-r--r--   0        0        0      583 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/margin.py
--rw-r--r--   0        0        0     6129 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5180 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     8334 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0    11998 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     7489 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/padding.py
--rw-r--r--   0        0        0    57080 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/page.py
--rw-r--r--   0        0        0     2674 2023-06-17 02:45:00.186597 flet_core-0.8.0.dev1535/src/flet_core/painting.py
--rw-r--r--   0        0        0     4410 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0     6811 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     4293 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     4491 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4088 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/protocol.py
--rw-r--r--   0        0        0     3419 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/querystring.py
--rw-r--r--   0        0        0     5765 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/radio.py
--rw-r--r--   0        0        0     2389 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/radio_group.py
--rw-r--r--   0        0        0      291 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/ref.py
--rw-r--r--   0        0        0     6344 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     6908 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/row.py
--rw-r--r--   0        0        0     4486 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/scrollable_control.py
--rw-r--r--   0        0        0     1637 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/semantics.py
--rw-r--r--   0        0        0      576 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5318 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2919 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0     7382 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/slider.py
--rw-r--r--   0        0        0     3971 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     4889 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/stack.py
--rw-r--r--   0        0        0     8104 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/switch.py
--rw-r--r--   0        0        0    10820 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10568 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/text.py
--rw-r--r--   0        0        0     7462 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3092 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1260 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/text_style.py
--rw-r--r--   0        0        0    15444 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/textfield.py
--rw-r--r--   0        0        0     6172 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/theme.py
--rw-r--r--   0        0        0     8362 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/transform.py
--rw-r--r--   0        0        0     2753 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     5550 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/types.py
--rw-r--r--   0        0        0      684 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/user_control.py
--rw-r--r--   0        0        0     4263 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/utils.py
--rw-r--r--   0        0        0      103 2023-06-17 02:45:32.370649 flet_core-0.8.0.dev1535/src/flet_core/version.py
--rw-r--r--   0        0        0     2337 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0     5852 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/view.py
--rw-r--r--   0        0        0     4049 2023-06-17 02:45:00.190597 flet_core-0.8.0.dev1535/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.8.0.dev1535/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/README.md
+-rw-r--r--   0        0        0      723 2023-06-17 03:13:36.537280 flet_core-0.8.0.dev1537/pyproject.toml
+-rw-r--r--   0        0        0     6546 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/__init__.py
+-rw-r--r--   0        0        0     6774 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     7226 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     2806 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/animation.py
+-rw-r--r--   0        0        0     5403 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7468 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/audio.py
+-rw-r--r--   0        0        0     5446 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     4320 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2202 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/buttons.py
+-rw-r--r--   0        0        0      514 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4629 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1639 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1361 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      837 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1862 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1907 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3486 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1772 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2361 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1963 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     5695 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/card.py
+-rw-r--r--   0        0        0     9855 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2061 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6837 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1949 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2924 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11228 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     8258 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5496 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5888 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3824 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0     7156 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0     6795 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3085 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0     1148 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/clipboard.py
+-rw-r--r--   0        0        0    10708 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6924 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/column.py
+-rw-r--r--   0        0        0     1132 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7099 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    14684 2023-06-17 03:13:05.600580 flet_core-0.8.0.dev1537/src/flet_core/container.py
+-rw-r--r--   0        0        0    14139 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/control_event.py
+-rw-r--r--   0        0        0    20707 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/datatable.py
+-rw-r--r--   0        0        0     2263 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/divider.py
+-rw-r--r--   0        0        0     6270 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6063 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/draggable.py
+-rw-r--r--   0        0        0     9177 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0     8848 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/event.py
+-rw-r--r--   0        0        0     1839 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9777 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2694 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     2828 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     3613 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0     7111 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    13981 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    28044 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1531 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     6804 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     1932 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3430 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/icon.py
+-rw-r--r--   0        0        0     8438 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362652 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/icons.py
+-rw-r--r--   0        0        0     7171 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0     8737 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     6401 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/list_view.py
+-rw-r--r--   0        0        0     8713 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      223 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/locks.py
+-rw-r--r--   0        0        0      583 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/margin.py
+-rw-r--r--   0        0        0     6129 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5180 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     8334 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0    11998 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     7489 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/padding.py
+-rw-r--r--   0        0        0    57164 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/page.py
+-rw-r--r--   0        0        0     2674 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4410 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0     6811 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     4293 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     4491 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4107 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/protocol.py
+-rw-r--r--   0        0        0     3419 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     5765 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2389 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0      291 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6344 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     6908 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/row.py
+-rw-r--r--   0        0        0     4486 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0     1637 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/semantics.py
+-rw-r--r--   0        0        0      576 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5318 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2919 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0     7382 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/slider.py
+-rw-r--r--   0        0        0     3971 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     4889 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8104 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/switch.py
+-rw-r--r--   0        0        0    10820 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2023-06-17 03:13:05.604580 flet_core-0.8.0.dev1537/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10568 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/text.py
+-rw-r--r--   0        0        0     7462 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3092 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1260 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    15444 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/textfield.py
+-rw-r--r--   0        0        0     6172 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8362 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2753 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     5550 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/types.py
+-rw-r--r--   0        0        0      684 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/user_control.py
+-rw-r--r--   0        0        0     4263 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/utils.py
+-rw-r--r--   0        0        0      103 2023-06-17 03:13:34.793212 flet_core-0.8.0.dev1537/src/flet_core/version.py
+-rw-r--r--   0        0        0     2337 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0     5852 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/view.py
+-rw-r--r--   0        0        0     4049 2023-06-17 03:13:05.608580 flet_core-0.8.0.dev1537/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.8.0.dev1537/PKG-INFO
```

### Comparing `flet_core-0.8.0.dev1535/pyproject.toml` & `flet_core-0.8.0.dev1537/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-core"
-version = "0.8.0.dev1535"
+version = "0.8.0.dev1537"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/__init__.py` & `flet_core-0.8.0.dev1537/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/alert_dialog.py` & `flet_core-0.8.0.dev1537/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/animated_switcher.py` & `flet_core-0.8.0.dev1537/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/animation.py` & `flet_core-0.8.0.dev1537/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/app_bar.py` & `flet_core-0.8.0.dev1537/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/audio.py` & `flet_core-0.8.0.dev1537/src/flet_core/image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,157 @@
-from enum import Enum
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from flet_core.callable_control import CallableControl
-from flet_core.control import OptionalNumber
+from flet_core.constrained_control import ConstrainedControl
+from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
+from flet_core.types import (
+    AnimationValue,
+    BlendMode,
+    BlendModeString,
+    BorderRadiusValue,
+    ImageFit,
+    ImageFitString,
+    ImageRepeat,
+    ImageRepeatString,
+    OffsetValue,
+    ResponsiveNumber,
+    RotateValue,
+    ScaleValue,
+)
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 
-class ReleaseMode(Enum):
-    RELEASE = "release"
-    LOOP = "loop"
-    STOP = "stop"
-
-
-class Audio(CallableControl):
+class Image(ConstrainedControl):
     """
-    A control to simultaneously play multiple audio files. Works on macOS, Linux, Windows, iOS, Android and web. Based on audioplayers Flutter widget (https://pub.dev/packages/audioplayers).
-
-    Audio control is non-visual and should be added to `page.overlay` list.
+    A control that displays an image.
 
     Example:
     ```
     import flet as ft
 
     def main(page: ft.Page):
-        audio1 = ft.Audio(
-            src="https://luan.xyz/files/audio/ambient_c_motion.mp3", autoplay=True
-        )
-        page.overlay.append(audio1)
-        page.add(
-            ft.Text("This is an app with background audio."),
-            ft.ElevatedButton("Stop playing", on_click=lambda _: audio1.pause()),
+        page.title = "Image Example"
+
+        img = ft.Image(
+            src=f"/icons/icon-512.png",
+            width=100,
+            height=100,
+            fit=ft.ImageFit.CONTAIN,
         )
 
+        page.add(img)
+
     ft.app(target=main)
     ```
 
     -----
 
-    Online docs: https://flet.dev/docs/controls/audio
+    Online docs: https://flet.dev/docs/controls/image
     """
 
     def __init__(
         self,
         src: Optional[str] = None,
         ref: Optional[Ref] = None,
+        key: Optional[str] = None,
+        width: OptionalNumber = None,
+        height: OptionalNumber = None,
+        left: OptionalNumber = None,
+        top: OptionalNumber = None,
+        right: OptionalNumber = None,
+        bottom: OptionalNumber = None,
+        expand: Union[None, bool, int] = None,
+        col: Optional[ResponsiveNumber] = None,
+        opacity: OptionalNumber = None,
+        rotate: RotateValue = None,
+        scale: ScaleValue = None,
+        offset: OffsetValue = None,
+        aspect_ratio: OptionalNumber = None,
+        animate_opacity: AnimationValue = None,
+        animate_size: AnimationValue = None,
+        animate_position: AnimationValue = None,
+        animate_rotation: AnimationValue = None,
+        animate_scale: AnimationValue = None,
+        animate_offset: AnimationValue = None,
+        on_animation_end=None,
+        tooltip: Optional[str] = None,
+        visible: Optional[bool] = None,
+        disabled: Optional[bool] = None,
         data: Any = None,
-        # specific
+        #
+        # Specific
+        #
         src_base64: Optional[str] = None,
-        autoplay: Optional[bool] = None,
-        volume: OptionalNumber = None,
-        balance: OptionalNumber = None,
-        playback_rate: OptionalNumber = None,
-        release_mode: Optional[ReleaseMode] = None,
-        on_loaded=None,
-        on_duration_changed=None,
-        on_state_changed=None,
-        on_position_changed=None,
-        on_seek_complete=None,
+        error_content: Optional[Control] = None,
+        repeat: Optional[ImageRepeat] = None,
+        fit: Optional[ImageFit] = None,
+        border_radius: BorderRadiusValue = None,
+        color: Optional[str] = None,
+        color_blend_mode: BlendMode = BlendMode.NONE,
+        gapless_playback: Optional[bool] = None,
+        semantics_label: Optional[str] = None,
     ):
-
-        CallableControl.__init__(
+        ConstrainedControl.__init__(
             self,
             ref=ref,
+            key=key,
+            width=width,
+            height=height,
+            left=left,
+            top=top,
+            right=right,
+            bottom=bottom,
+            expand=expand,
+            col=col,
+            opacity=opacity,
+            rotate=rotate,
+            scale=scale,
+            offset=offset,
+            aspect_ratio=aspect_ratio,
+            animate_opacity=animate_opacity,
+            animate_size=animate_size,
+            animate_position=animate_position,
+            animate_rotation=animate_rotation,
+            animate_scale=animate_scale,
+            animate_offset=animate_offset,
+            on_animation_end=on_animation_end,
+            tooltip=tooltip,
+            visible=visible,
+            disabled=disabled,
             data=data,
         )
 
         self.src = src
         self.src_base64 = src_base64
-        self.autoplay = autoplay
-        self.volume = volume
-        self.balance = balance
-        self.playback_rate = playback_rate
-        self.release_mode = release_mode
-        self.on_loaded = on_loaded
-        self.on_duration_changed = on_duration_changed
-        self.on_state_changed = on_state_changed
-        self.on_position_changed = on_position_changed
-        self.on_seek_complete = on_seek_complete
+        self.error_content = error_content
+        self.fit = fit
+        self.repeat = repeat
+        self.border_radius = border_radius
+        self.color = color
+        self.color_blend_mode = color_blend_mode
+        self.gapless_playback = gapless_playback
+        self.semantics_label = semantics_label
 
     def _get_control_name(self):
-        return "audio"
-
-    def play(self):
-        self._call_method("play", params=[], wait_for_result=False)
-
-    async def play_async(self):
-        await self._call_method_async("play", params=[], wait_for_result=False)
-
-    def pause(self):
-        self._call_method("pause", params=[], wait_for_result=False)
-
-    async def pause_async(self):
-        await self._call_method_async("pause", params=[], wait_for_result=False)
-
-    def resume(self):
-        self._call_method("resume", params=[], wait_for_result=False)
-
-    async def resume_async(self):
-        await self._call_method_async("resume", params=[], wait_for_result=False)
-
-    def release(self):
-        self._call_method("release", params=[], wait_for_result=False)
+        return "image"
 
-    async def release_async(self):
-        await self._call_method_async("release", params=[], wait_for_result=False)
-
-    def seek(self, position_milliseconds: int):
-        self._call_method(
-            "seek", params=[str(position_milliseconds)], wait_for_result=False
-        )
-
-    async def seek_async(self, position_milliseconds: int):
-        await self._call_method_async(
-            "seek", params=[str(position_milliseconds)], wait_for_result=False
-        )
-
-    def get_duration(self) -> Optional[int]:
-        sr = self._call_method("get_duration", [])
-        return int(sr) if sr else None
-
-    async def get_duration_async(self) -> Optional[int]:
-        sr = await self._call_method_async("get_duration", [])
-        return int(sr) if sr else None
-
-    def get_current_position(self) -> Optional[int]:
-        sr = self._call_method("get_current_position", [])
-        return int(sr) if sr else None
-
-    async def get_current_position_async(self) -> Optional[int]:
-        sr = await self._call_method_async("get_current_position", [])
-        return int(sr) if sr else None
+    def _get_children(self):
+        children = []
+        if self.__error_content is not None:
+            self.__error_content._set_attr_internal("n", "error_content")
+            children.append(self.__error_content)
+        return children
+
+    def _before_build_command(self):
+        super()._before_build_command()
+        self._set_attr_json("borderRadius", self.__border_radius)
 
     # src
     @property
     def src(self):
         return self._get_attr("src")
 
     @src.setter
@@ -145,103 +163,99 @@
     def src_base64(self):
         return self._get_attr("srcBase64")
 
     @src_base64.setter
     def src_base64(self, value):
         self._set_attr("srcBase64", value)
 
-    # autoplay
+    # fit
     @property
-    def autoplay(self) -> Optional[bool]:
-        return self._get_attr("autoplay", data_type="bool", def_value=False)
-
-    @autoplay.setter
-    def autoplay(self, value: Optional[bool]):
-        self._set_attr("autoplay", value)
+    def fit(self) -> Optional[ImageFit]:
+        return self.__fit
 
-    # volume
-    @property
-    def volume(self) -> OptionalNumber:
-        return self._get_attr("volume")
+    @fit.setter
+    def fit(self, value: Optional[ImageFit]):
+        self.__fit = value
+        if isinstance(value, ImageFit):
+            self._set_attr("fit", value.value)
+        else:
+            self.__set_fit(value)
 
-    @volume.setter
-    def volume(self, value: OptionalNumber):
-        if value is None or (value >= 0 and value <= 1):
-            self._set_attr("volume", value)
+    def __set_fit(self, value: ImageFitString):
+        self._set_attr("fit", value)
 
-    # balance
+    # repeat
     @property
-    def balance(self) -> OptionalNumber:
-        return self._get_attr("balance")
-
-    @balance.setter
-    def balance(self, value: OptionalNumber):
-        if value is None or (value >= -1 and value <= 1):
-            self._set_attr("balance", value)
+    def repeat(self) -> Optional[ImageRepeat]:
+        return self.__repeat
 
-    # playback_rate
-    @property
-    def playback_rate(self) -> OptionalNumber:
-        return self._get_attr("playbackRate")
+    @repeat.setter
+    def repeat(self, value: Optional[ImageRepeat]):
+        self.__repeat = value
+        if isinstance(value, ImageRepeat):
+            self._set_attr("repeat", value.value)
+        else:
+            self.__set_repeat(value)
 
-    @playback_rate.setter
-    def playback_rate(self, value: OptionalNumber):
-        if value is None or (value >= 0 and value <= 2):
-            self._set_attr("playbackRate", value)
+    def __set_repeat(self, value: ImageRepeatString):
+        self._set_attr("repeat", value)
 
-    # release_mode
+    # border_radius
     @property
-    def release_mode(self):
-        return self._get_attr("releaseMode")
+    def border_radius(self) -> BorderRadiusValue:
+        return self.__border_radius
 
-    @release_mode.setter
-    def release_mode(self, value: Optional[ReleaseMode]):
-        self._set_attr("releaseMode", value.value if value is not None else None)
+    @border_radius.setter
+    def border_radius(self, value: BorderRadiusValue):
+        self.__border_radius = value
 
-    # on_loaded
+    # color
     @property
-    def on_loaded(self):
-        return self._get_event_handler("loaded")
+    def color(self):
+        return self._get_attr("color")
 
-    @on_loaded.setter
-    def on_loaded(self, handler):
-        self._add_event_handler("loaded", handler)
+    @color.setter
+    def color(self, value):
+        self._set_attr("color", value)
 
-    # on_duration_changed
+    # color_blend_mode
     @property
-    def on_duration_changed(self):
-        return self._get_event_handler("duration_changed")
+    def color_blend_mode(self) -> BlendMode:
+        return self.__blend_mode
 
-    @on_duration_changed.setter
-    def on_duration_changed(self, handler):
-        self._add_event_handler("duration_changed", handler)
+    @color_blend_mode.setter
+    def color_blend_mode(self, value: BlendMode):
+        self.__blend_mode = value
+        if isinstance(value, BlendMode):
+            self._set_attr("colorBlendMode", value.value)
+        else:
+            self.__set_blend_mode(value)
+
+    def __set_blend_mode(self, value: BlendModeString):
+        self._set_attr("colorBlendMode", value)
 
-    # on_state_changed
+    # gapless_playback
     @property
-    def on_state_changed(self):
-        return self._get_event_handler("state_changed")
+    def gapless_playback(self) -> Optional[bool]:
+        return self._get_attr("gaplessPlayback", data_type="bool", def_value=False)
 
-    @on_state_changed.setter
-    def on_state_changed(self, handler):
-        self._add_event_handler("state_changed", handler)
+    @gapless_playback.setter
+    def gapless_playback(self, value: Optional[bool]):
+        self._set_attr("gaplessPlayback", value)
 
-    # on_position_changed
+    # semantics_label
     @property
-    def on_position_changed(self):
-        return self._get_event_handler("position_changed")
+    def semantics_label(self):
+        return self._get_attr("semanticsLabel")
 
-    @on_position_changed.setter
-    def on_position_changed(self, handler):
-        self._add_event_handler("position_changed", handler)
-        if handler is not None:
-            self._set_attr("onPositionChanged", True)
-        else:
-            self._set_attr("onPositionChanged", None)
+    @semantics_label.setter
+    def semantics_label(self, value):
+        self._set_attr("semanticsLabel", value)
 
-    # on_seek_complete
+    # error_content
     @property
-    def on_seek_complete(self):
-        return self._get_event_handler("seek_complete")
+    def error_content(self) -> Optional[Control]:
+        return self.__error_content
 
-    @on_seek_complete.setter
-    def on_seek_complete(self, handler):
-        self._add_event_handler("seek_complete", handler)
+    @error_content.setter
+    def error_content(self, value: Optional[Control]):
+        self.__error_content = value
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/banner.py` & `flet_core-0.8.0.dev1537/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/border.py` & `flet_core-0.8.0.dev1537/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/border_radius.py` & `flet_core-0.8.0.dev1537/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/bottom_sheet.py` & `flet_core-0.8.0.dev1537/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/buttons.py` & `flet_core-0.8.0.dev1537/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/__init__.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/arc.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/canvas.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/circle.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/color.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/fill.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/line.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/oval.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/path.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/points.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/rect.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/shadow.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/canvas/text.py` & `flet_core-0.8.0.dev1537/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/card.py` & `flet_core-0.8.0.dev1537/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_group.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_rod.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/chart_axis.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/chart_axis_label.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/chart_point_shape.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart_data.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/line_chart_data_point.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/pie_chart.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/charts/pie_chart_section.py` & `flet_core-0.8.0.dev1537/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/checkbox.py` & `flet_core-0.8.0.dev1537/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/circle_avatar.py` & `flet_core-0.8.0.dev1537/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/client_storage.py` & `flet_core-0.8.0.dev1537/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/colors.py` & `flet_core-0.8.0.dev1537/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/column.py` & `flet_core-0.8.0.dev1537/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/connection.py` & `flet_core-0.8.0.dev1537/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/constrained_control.py` & `flet_core-0.8.0.dev1537/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/container.py` & `flet_core-0.8.0.dev1537/src/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/control.py` & `flet_core-0.8.0.dev1537/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/datatable.py` & `flet_core-0.8.0.dev1537/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/divider.py` & `flet_core-0.8.0.dev1537/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/drag_target.py` & `flet_core-0.8.0.dev1537/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/draggable.py` & `flet_core-0.8.0.dev1537/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/dropdown.py` & `flet_core-0.8.0.dev1537/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/elevated_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/embed_json_encoder.py` & `flet_core-0.8.0.dev1537/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/event_handler.py` & `flet_core-0.8.0.dev1537/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/file_picker.py` & `flet_core-0.8.0.dev1537/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/filled_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/filled_tonal_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/flet_app.py` & `flet_core-0.8.0.dev1537/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/floating_action_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/form_field_control.py` & `flet_core-0.8.0.dev1537/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/gesture_detector.py` & `flet_core-0.8.0.dev1537/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/gradients.py` & `flet_core-0.8.0.dev1537/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/grid_view.py` & `flet_core-0.8.0.dev1537/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/icon.py` & `flet_core-0.8.0.dev1537/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/icon_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/icons.py` & `flet_core-0.8.0.dev1537/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/image.py` & `flet_core-0.8.0.dev1537/src/flet_core/text_button.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,49 @@
+import time
 from typing import Any, Optional, Union
 
+from flet_core.buttons import ButtonStyle
 from flet_core.constrained_control import ConstrainedControl
 from flet_core.control import Control, OptionalNumber
 from flet_core.ref import Ref
 from flet_core.types import (
     AnimationValue,
-    BlendMode,
-    BlendModeString,
-    BorderRadiusValue,
-    ImageFit,
-    ImageFitString,
-    ImageRepeat,
-    ImageRepeatString,
     OffsetValue,
     ResponsiveNumber,
     RotateValue,
     ScaleValue,
 )
 
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
 
-
-class Image(ConstrainedControl):
+class TextButton(ConstrainedControl):
     """
-    A control that displays an image.
+    Text buttons are used for the lowest priority actions, especially when presenting multiple options. Text buttons can be placed on a variety of backgrounds. Until the button is interacted with, its container isn’t visible.
 
     Example:
     ```
     import flet as ft
 
     def main(page: ft.Page):
-        page.title = "Image Example"
-
-        img = ft.Image(
-            src=f"/icons/icon-512.png",
-            width=100,
-            height=100,
-            fit=ft.ImageFit.CONTAIN,
+        page.title = "Basic text buttons"
+        page.add(
+            ft.TextButton(text="Text button"),
+            ft.TextButton("Disabled button", disabled=True),
         )
 
-        page.add(img)
-
     ft.app(target=main)
     ```
 
     -----
 
-    Online docs: https://flet.dev/docs/controls/image
+    Online docs: https://flet.dev/docs/controls/textbutton
     """
 
     def __init__(
         self,
-        src: Optional[str] = None,
+        text: Optional[str] = None,
         ref: Optional[Ref] = None,
         key: Optional[str] = None,
         width: OptionalNumber = None,
         height: OptionalNumber = None,
         left: OptionalNumber = None,
         top: OptionalNumber = None,
         right: OptionalNumber = None,
@@ -80,23 +65,26 @@
         tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
         # Specific
         #
-        src_base64: Optional[str] = None,
-        error_content: Optional[Control] = None,
-        repeat: Optional[ImageRepeat] = None,
-        fit: Optional[ImageFit] = None,
-        border_radius: BorderRadiusValue = None,
-        color: Optional[str] = None,
-        color_blend_mode: BlendMode = BlendMode.NONE,
-        gapless_playback: Optional[bool] = None,
-        semantics_label: Optional[str] = None,
+        icon: Optional[str] = None,
+        icon_color: Optional[str] = None,
+        style: Optional[ButtonStyle] = None,
+        content: Optional[Control] = None,
+        autofocus: Optional[bool] = None,
+        url: Optional[str] = None,
+        url_target: Optional[str] = None,
+        on_click=None,
+        on_long_press=None,
+        on_hover=None,
+        on_focus=None,
+        on_blur=None,
     ):
         ConstrainedControl.__init__(
             self,
             ref=ref,
             key=key,
             width=width,
             height=height,
@@ -120,142 +108,166 @@
             on_animation_end=on_animation_end,
             tooltip=tooltip,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
-        self.src = src
-        self.src_base64 = src_base64
-        self.error_content = error_content
-        self.fit = fit
-        self.repeat = repeat
-        self.border_radius = border_radius
-        self.color = color
-        self.color_blend_mode = color_blend_mode
-        self.gapless_playback = gapless_playback
-        self.semantics_label = semantics_label
+        self.text = text
+        self.icon = icon
+        self.icon_color = icon_color
+        self.style = style
+        self.content = content
+        self.autofocus = autofocus
+        self.url = url
+        self.url_target = url_target
+        self.on_click = on_click
+        self.on_long_press = on_long_press
+        self.on_hover = on_hover
+        self.on_focus = on_focus
+        self.on_blur = on_blur
 
     def _get_control_name(self):
-        return "image"
-
-    def _get_children(self):
-        children = []
-        if self.__error_content is not None:
-            self.__error_content._set_attr_internal("n", "error_content")
-            children.append(self.__error_content)
-        return children
+        return "textbutton"
 
     def _before_build_command(self):
         super()._before_build_command()
-        self._set_attr_json("borderRadius", self.__border_radius)
+        if self.__style is not None:
+            self.__style.side = self._wrap_attr_dict(self.__style.side)
+            self.__style.shape = self._wrap_attr_dict(self.__style.shape)
+        self._set_attr_json("style", self.__style)
 
-    # src
+    def _get_children(self):
+        if self.__content is None:
+            return []
+        self.__content._set_attr_internal("n", "content")
+        return [self.__content]
+
+    def focus(self):
+        self._set_attr_json("focus", str(time.time()))
+        self.update()
+
+    async def focus_async(self):
+        self._set_attr_json("focus", str(time.time()))
+        await self.update_async()
+
+    # text
     @property
-    def src(self):
-        return self._get_attr("src")
+    def text(self):
+        return self._get_attr("text")
 
-    @src.setter
-    def src(self, value):
-        self._set_attr("src", value)
+    @text.setter
+    def text(self, value):
+        self._set_attr("text", value)
 
-    # src_base64
+    # icon
     @property
-    def src_base64(self):
-        return self._get_attr("srcBase64")
+    def icon(self):
+        return self._get_attr("icon")
 
-    @src_base64.setter
-    def src_base64(self, value):
-        self._set_attr("srcBase64", value)
+    @icon.setter
+    def icon(self, value):
+        self._set_attr("icon", value)
 
-    # fit
+    # icon_color
     @property
-    def fit(self) -> Optional[ImageFit]:
-        return self.__fit
+    def icon_color(self):
+        return self._get_attr("iconColor")
 
-    @fit.setter
-    def fit(self, value: Optional[ImageFit]):
-        self.__fit = value
-        if isinstance(value, ImageFit):
-            self._set_attr("fit", value.value)
-        else:
-            self.__set_fit(value)
+    @icon_color.setter
+    def icon_color(self, value):
+        self._set_attr("iconColor", value)
 
-    def __set_fit(self, value: ImageFitString):
-        self._set_attr("fit", value)
+    # style
+    @property
+    def style(self) -> Optional[ButtonStyle]:
+        return self.__style
 
-    # repeat
+    @style.setter
+    def style(self, value: Optional[ButtonStyle]):
+        self.__style = value
+
+    # url
     @property
-    def repeat(self) -> Optional[ImageRepeat]:
-        return self.__repeat
+    def url(self):
+        return self._get_attr("url")
 
-    @repeat.setter
-    def repeat(self, value: Optional[ImageRepeat]):
-        self.__repeat = value
-        if isinstance(value, ImageRepeat):
-            self._set_attr("repeat", value.value)
-        else:
-            self.__set_repeat(value)
+    @url.setter
+    def url(self, value):
+        self._set_attr("url", value)
+
+    # url_target
+    @property
+    def url_target(self):
+        return self._get_attr("urlTarget")
 
-    def __set_repeat(self, value: ImageRepeatString):
-        self._set_attr("repeat", value)
+    @url_target.setter
+    def url_target(self, value):
+        self._set_attr("urlTarget", value)
 
-    # border_radius
+    # on_click
     @property
-    def border_radius(self) -> BorderRadiusValue:
-        return self.__border_radius
+    def on_click(self):
+        return self._get_event_handler("click")
 
-    @border_radius.setter
-    def border_radius(self, value: BorderRadiusValue):
-        self.__border_radius = value
+    @on_click.setter
+    def on_click(self, handler):
+        self._add_event_handler("click", handler)
 
-    # color
+    # on_long_press
     @property
-    def color(self):
-        return self._get_attr("color")
+    def on_long_press(self):
+        return self._get_event_handler("long_press")
 
-    @color.setter
-    def color(self, value):
-        self._set_attr("color", value)
+    @on_long_press.setter
+    def on_long_press(self, handler):
+        self._add_event_handler("long_press", handler)
+        self._set_attr("onLongPress", True if handler is not None else None)
 
-    # color_blend_mode
+    # content
     @property
-    def color_blend_mode(self) -> BlendMode:
-        return self.__blend_mode
+    def content(self) -> Optional[Control]:
+        return self.__content
 
-    @color_blend_mode.setter
-    def color_blend_mode(self, value: BlendMode):
-        self.__blend_mode = value
-        if isinstance(value, BlendMode):
-            self._set_attr("colorBlendMode", value.value)
-        else:
-            self.__set_blend_mode(value)
+    @content.setter
+    def content(self, value: Optional[Control]):
+        self.__content = value
+
+    # autofocus
+    @property
+    def autofocus(self) -> Optional[bool]:
+        return self._get_attr("autofocus", data_type="bool", def_value=False)
 
-    def __set_blend_mode(self, value: BlendModeString):
-        self._set_attr("colorBlendMode", value)
+    @autofocus.setter
+    def autofocus(self, value: Optional[bool]):
+        self._set_attr("autofocus", value)
 
-    # gapless_playback
+    # on_hover
     @property
-    def gapless_playback(self) -> Optional[bool]:
-        return self._get_attr("gaplessPlayback", data_type="bool", def_value=False)
+    def on_hover(self):
+        return self._get_event_handler("hover")
 
-    @gapless_playback.setter
-    def gapless_playback(self, value: Optional[bool]):
-        self._set_attr("gaplessPlayback", value)
+    @on_hover.setter
+    def on_hover(self, handler):
+        self._add_event_handler("hover", handler)
+        if handler is not None:
+            self._set_attr("onHover", True)
+        else:
+            self._set_attr("onHover", None)
 
-    # semantics_label
+    # on_focus
     @property
-    def semantics_label(self):
-        return self._get_attr("semanticsLabel")
+    def on_focus(self):
+        return self._get_event_handler("focus")
 
-    @semantics_label.setter
-    def semantics_label(self, value):
-        self._set_attr("semanticsLabel", value)
+    @on_focus.setter
+    def on_focus(self, handler):
+        self._add_event_handler("focus", handler)
 
-    # error_content
+    # on_blur
     @property
-    def error_content(self) -> Optional[Control]:
-        return self.__error_content
+    def on_blur(self):
+        return self._get_event_handler("blur")
 
-    @error_content.setter
-    def error_content(self, value: Optional[Control]):
-        self.__error_content = value
+    @on_blur.setter
+    def on_blur(self, handler):
+        self._add_event_handler("blur", handler)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/list_tile.py` & `flet_core-0.8.0.dev1537/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/list_view.py` & `flet_core-0.8.0.dev1537/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/local_connection.py` & `flet_core-0.8.0.dev1537/src/flet_core/local_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         elif command.name == "invokeMethod":
             return self._process_invoke_method_command(command.values, command.attrs)
         elif command.name == "error":
             return self._process_error_command(command.values)
         raise Exception(f"Unsupported command: {command.name}")
 
     def _process_add_command(self, command: Command):
-
         top_parent_id = command.attrs.get("to", "page")
         top_parent_at = int(command.attrs.get("at", "-1"))
 
         batch: List[Command] = []
         if len(command.values) > 0:
             batch.append(command)
 
@@ -189,19 +188,22 @@
         assert len(values) == 1, '"error" command has wrong number of values'
         return "", ClientMessage(
             ClientActions.SESSION_CRASHED, SessionCrashedPayload(message=values[0])
         )
 
     def _process_invoke_method_command(self, values, attrs):
         # "invokeMethod", values=[method_id, method_name], attrs=arguments
-        assert len(values) == 2, '"invokeMethod" command has wrong number of values'
+        assert len(values) == 3, '"invokeMethod" command has wrong number of values'
         return "", ClientMessage(
             ClientActions.INVOKE_METHOD,
             InvokeMethodPayload(
-                methodId=values[0], methodName=values[1], arguments=attrs
+                methodId=values[0],
+                methodName=values[1],
+                controlId=values[2],
+                arguments=attrs,
             ),
         )
 
     def _process_get_command(self, values: List[str]):
         assert len(values) == 2, '"get" command has wrong number of values'
         assert self._client_details
         ctrl_id = values[0]
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/margin.py` & `flet_core-0.8.0.dev1537/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/markdown.py` & `flet_core-0.8.0.dev1537/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/matplotlib_chart.py` & `flet_core-0.8.0.dev1537/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/navigation_bar.py` & `flet_core-0.8.0.dev1537/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/navigation_rail.py` & `flet_core-0.8.0.dev1537/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/outlined_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/padding.py` & `flet_core-0.8.0.dev1537/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/page.py` & `flet_core-0.8.0.dev1537/src/flet_core/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,27 +837,28 @@
             offset=offset, delta=delta, key=key, duration=duration, curve=curve
         )
 
     def invoke_method(
         self,
         method_name: str,
         arguments: Optional[Dict[str, str]] = None,
+        control_id: str = "",
         wait_for_result: bool = False,
     ) -> Optional[str]:
         method_id = uuid.uuid4().hex
 
         # register callback
         evt: Optional[threading.Event] = None
         if wait_for_result:
             evt = threading.Event()
             self.__method_calls[method_id] = evt
 
         # call method
         result = self._send_command(
-            "invokeMethod", values=[method_id, method_name], attrs=arguments
+            "invokeMethod", values=[method_id, method_name, control_id], attrs=arguments
         )
 
         if result.error != "":
             if wait_for_result:
                 del self.__method_calls[method_id]
             raise Exception(result.error)
 
@@ -879,27 +880,28 @@
             return None
         return result
 
     async def invoke_method_async(
         self,
         method_name: str,
         arguments: Optional[Dict[str, str]] = None,
+        control_id: str = "",
         wait_for_result: bool = False,
     ) -> Optional[str]:
         method_id = uuid.uuid4().hex
 
         # register callback
         evt: Optional[asyncio.Event] = None
         if wait_for_result:
             evt = asyncio.Event()
             self.__method_calls[method_id] = evt
 
         # call method
         result = await self._send_command_async(
-            "invokeMethod", values=[method_id, method_name], attrs=arguments
+            "invokeMethod", values=[method_id, method_name, control_id], attrs=arguments
         )
 
         if result.error != "":
             if wait_for_result:
                 del self.__method_calls[method_id]
             raise Exception(result.error)
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/painting.py` & `flet_core-0.8.0.dev1537/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/plotly_chart.py` & `flet_core-0.8.0.dev1537/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/popup_menu_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/progress_bar.py` & `flet_core-0.8.0.dev1537/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/progress_ring.py` & `flet_core-0.8.0.dev1537/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/protocol.py` & `flet_core-0.8.0.dev1537/src/flet_core/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     message: str
 
 
 @dataclass
 class InvokeMethodPayload:
     methodId: str
     methodName: str
+    controlId: str
     arguments: Dict[str, str]
 
 
 @dataclass
 class AddPageControlsPayload:
     controls: List[Dict[str, Any]]
     trimIDs: List[str] = field(default_factory=lambda: [])
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/querystring.py` & `flet_core-0.8.0.dev1537/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/radio.py` & `flet_core-0.8.0.dev1537/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/radio_group.py` & `flet_core-0.8.0.dev1537/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/responsive_row.py` & `flet_core-0.8.0.dev1537/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/row.py` & `flet_core-0.8.0.dev1537/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/scrollable_control.py` & `flet_core-0.8.0.dev1537/src/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/semantics.py` & `flet_core-0.8.0.dev1537/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/session_storage.py` & `flet_core-0.8.0.dev1537/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/shader_mask.py` & `flet_core-0.8.0.dev1537/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/shadow.py` & `flet_core-0.8.0.dev1537/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/shake_detector.py` & `flet_core-0.8.0.dev1537/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/slider.py` & `flet_core-0.8.0.dev1537/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/snack_bar.py` & `flet_core-0.8.0.dev1537/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/stack.py` & `flet_core-0.8.0.dev1537/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/switch.py` & `flet_core-0.8.0.dev1537/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/tabs.py` & `flet_core-0.8.0.dev1537/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/template_route.py` & `flet_core-0.8.0.dev1537/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/text.py` & `flet_core-0.8.0.dev1537/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/text_button.py` & `flet_core-0.8.0.dev1537/src/flet_core/tooltip.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,273 +1,297 @@
-import time
 from typing import Any, Optional, Union
 
-from flet_core.buttons import ButtonStyle
-from flet_core.constrained_control import ConstrainedControl
+from flet_core.border import Border
 from flet_core.control import Control, OptionalNumber
+from flet_core.gradients import Gradient
 from flet_core.ref import Ref
+from flet_core.text_style import TextStyle
 from flet_core.types import (
-    AnimationValue,
-    OffsetValue,
-    ResponsiveNumber,
-    RotateValue,
-    ScaleValue,
+    BorderRadiusValue,
+    BoxShape,
+    MarginValue,
+    PaddingValue,
+    TextAlign,
+    TextAlignString,
 )
 
 
-class TextButton(ConstrainedControl):
+class Tooltip(Control):
     """
-    Text buttons are used for the lowest priority actions, especially when presenting multiple options. Text buttons can be placed on a variety of backgrounds. Until the button is interacted with, its container isn’t visible.
+    Tooltips provide text labels which help explain the function of a button or other user interface action. Wrap the button in a Tooltip control and provide a message which will be shown when the control is long pressed.
 
     Example:
     ```
+    import math
+
     import flet as ft
+    from flet import alignment
 
     def main(page: ft.Page):
-        page.title = "Basic text buttons"
+        page.title = "Tooltip Example"
         page.add(
-            ft.TextButton(text="Text button"),
-            ft.TextButton("Disabled button", disabled=True),
+            ft.Tooltip(
+                message="This is tooltip",
+                content=ft.Text("Hover to see tooltip"),
+                padding=20,
+                border_radius=10,
+                text_style=ft.TextStyle(size=20, color=ft.colors.WHITE),
+                gradient=ft.LinearGradient(
+                    begin=alignment.top_left,
+                    end=alignment.Alignment(0.8, 1),
+                    colors=[
+                        "0xff1f005c",
+                        "0xff5b0060",
+                        "0xff870160",
+                        "0xffac255e",
+                        "0xffca485c",
+                        "0xffe16b5c",
+                        "0xfff39060",
+                        "0xffffb56b",
+                    ],
+                    tile_mode=ft.GradientTileMode.MIRROR,
+                    rotation=math.pi / 3,
+                ),
+            )
         )
 
+
     ft.app(target=main)
     ```
 
     -----
 
-    Online docs: https://flet.dev/docs/controls/textbutton
+    Online docs: https://flet.dev/docs/controls/tooltip
     """
 
     def __init__(
         self,
-        text: Optional[str] = None,
         ref: Optional[Ref] = None,
-        key: Optional[str] = None,
-        width: OptionalNumber = None,
-        height: OptionalNumber = None,
-        left: OptionalNumber = None,
-        top: OptionalNumber = None,
-        right: OptionalNumber = None,
-        bottom: OptionalNumber = None,
-        expand: Union[None, bool, int] = None,
-        col: Optional[ResponsiveNumber] = None,
-        opacity: OptionalNumber = None,
-        rotate: RotateValue = None,
-        scale: ScaleValue = None,
-        offset: OffsetValue = None,
-        aspect_ratio: OptionalNumber = None,
-        animate_opacity: AnimationValue = None,
-        animate_size: AnimationValue = None,
-        animate_position: AnimationValue = None,
-        animate_rotation: AnimationValue = None,
-        animate_scale: AnimationValue = None,
-        animate_offset: AnimationValue = None,
-        on_animation_end=None,
-        tooltip: Optional[str] = None,
         visible: Optional[bool] = None,
         disabled: Optional[bool] = None,
         data: Any = None,
         #
         # Specific
         #
-        icon: Optional[str] = None,
-        icon_color: Optional[str] = None,
-        style: Optional[ButtonStyle] = None,
         content: Optional[Control] = None,
-        autofocus: Optional[bool] = None,
-        url: Optional[str] = None,
-        url_target: Optional[str] = None,
-        on_click=None,
-        on_long_press=None,
-        on_hover=None,
-        on_focus=None,
-        on_blur=None,
+        enable_feedback: Optional[bool] = None,
+        height: OptionalNumber = None,
+        vertical_offset: OptionalNumber = None,
+        margin: MarginValue = None,
+        padding: PaddingValue = None,
+        bgcolor: Optional[str] = None,
+        gradient: Optional[Gradient] = None,
+        border: Optional[Border] = None,
+        border_radius: BorderRadiusValue = None,
+        shape: Optional[BoxShape] = None,
+        message: Optional[str] = None,
+        text_style: Optional[TextStyle] = None,
+        text_align: TextAlign = TextAlign.NONE,
+        prefer_below: Optional[bool] = None,
+        show_duration: Optional[int] = None,
+        wait_duration: Optional[int] = None,
     ):
-        ConstrainedControl.__init__(
+        Control.__init__(
             self,
             ref=ref,
-            key=key,
-            width=width,
-            height=height,
-            left=left,
-            top=top,
-            right=right,
-            bottom=bottom,
-            expand=expand,
-            col=col,
-            opacity=opacity,
-            rotate=rotate,
-            scale=scale,
-            offset=offset,
-            aspect_ratio=aspect_ratio,
-            animate_opacity=animate_opacity,
-            animate_size=animate_size,
-            animate_position=animate_position,
-            animate_rotation=animate_rotation,
-            animate_scale=animate_scale,
-            animate_offset=animate_offset,
-            on_animation_end=on_animation_end,
-            tooltip=tooltip,
             visible=visible,
             disabled=disabled,
             data=data,
         )
 
-        self.text = text
-        self.icon = icon
-        self.icon_color = icon_color
-        self.style = style
         self.content = content
-        self.autofocus = autofocus
-        self.url = url
-        self.url_target = url_target
-        self.on_click = on_click
-        self.on_long_press = on_long_press
-        self.on_hover = on_hover
-        self.on_focus = on_focus
-        self.on_blur = on_blur
+        self.enable_feedback = enable_feedback
+        self.height = height
+        self.vertical_offset = vertical_offset
+        self.margin = margin
+        self.padding = padding
+        self.bgcolor = bgcolor
+        self.gradient = gradient
+        self.border = border
+        self.border_radius = border_radius
+        self.shape = shape
+        self.message = message
+        self.text_style = text_style
+        self.text_align = text_align
+        self.prefer_below = prefer_below
+        self.show_duration = show_duration
+        self.wait_duration = wait_duration
 
     def _get_control_name(self):
-        return "textbutton"
+        return "tooltip"
 
     def _before_build_command(self):
         super()._before_build_command()
-        if self.__style is not None:
-            self.__style.side = self._wrap_attr_dict(self.__style.side)
-            self.__style.shape = self._wrap_attr_dict(self.__style.shape)
-        self._set_attr_json("style", self.__style)
+        self._set_attr_json("margin", self.__margin)
+        self._set_attr_json("padding", self.__padding)
+        self._set_attr_json("textStyle", self.__text_style)
+        self._set_attr_json("borderRadius", self.__border_radius)
+        self._set_attr_json("border", self.__border)
+        self._set_attr_json("gradient", self.__gradient)
 
     def _get_children(self):
-        if self.__content is None:
-            return []
-        self.__content._set_attr_internal("n", "content")
-        return [self.__content]
+        children = []
+        if self.__content is not None:
+            self.__content._set_attr_internal("n", "content")
+            children.append(self.__content)
+        return children
 
-    def focus(self):
-        self._set_attr_json("focus", str(time.time()))
-        self.update()
+    # enable_feedback
+    @property
+    def enable_feedback(self) -> Optional[bool]:
+        return self._get_attr("enableFeedback", data_type="bool", def_value=False)
 
-    async def focus_async(self):
-        self._set_attr_json("focus", str(time.time()))
-        await self.update_async()
+    @enable_feedback.setter
+    def enable_feedback(self, value: Optional[bool]):
+        self._set_attr("enableFeedback", value)
 
-    # text
+    # margin
     @property
-    def text(self):
-        return self._get_attr("text")
+    def margin(self) -> MarginValue:
+        return self.__margin
 
-    @text.setter
-    def text(self, value):
-        self._set_attr("text", value)
+    @margin.setter
+    def margin(self, value: MarginValue):
+        self.__margin = value
 
-    # icon
+    # padding
     @property
-    def icon(self):
-        return self._get_attr("icon")
+    def padding(self) -> PaddingValue:
+        return self.__padding
 
-    @icon.setter
-    def icon(self, value):
-        self._set_attr("icon", value)
+    @padding.setter
+    def padding(self, value: PaddingValue):
+        self.__padding = value
 
-    # icon_color
+    # bgcolor
     @property
-    def icon_color(self):
-        return self._get_attr("iconColor")
+    def bgcolor(self):
+        return self._get_attr("bgColor")
 
-    @icon_color.setter
-    def icon_color(self, value):
-        self._set_attr("iconColor", value)
+    @bgcolor.setter
+    def bgcolor(self, value):
+        self._set_attr("bgColor", value)
 
-    # style
+    # gradient
     @property
-    def style(self) -> Optional[ButtonStyle]:
-        return self.__style
+    def gradient(self) -> Optional[Gradient]:
+        return self.__gradient
 
-    @style.setter
-    def style(self, value: Optional[ButtonStyle]):
-        self.__style = value
+    @gradient.setter
+    def gradient(self, value: Optional[Gradient]):
+        self.__gradient = value
 
-    # url
+    # border
     @property
-    def url(self):
-        return self._get_attr("url")
+    def border(self) -> Optional[Border]:
+        return self.__border
 
-    @url.setter
-    def url(self, value):
-        self._set_attr("url", value)
+    @border.setter
+    def border(self, value: Optional[Border]):
+        self.__border = value
 
-    # url_target
+    # border_radius
     @property
-    def url_target(self):
-        return self._get_attr("urlTarget")
+    def border_radius(self) -> BorderRadiusValue:
+        return self.__border_radius
 
-    @url_target.setter
-    def url_target(self, value):
-        self._set_attr("urlTarget", value)
+    @border_radius.setter
+    def border_radius(self, value: BorderRadiusValue):
+        self.__border_radius = value
 
-    # on_click
+    # shape
     @property
-    def on_click(self):
-        return self._get_event_handler("click")
+    def shape(self):
+        return self.__shape
 
-    @on_click.setter
-    def on_click(self, handler):
-        self._add_event_handler("click", handler)
+    @shape.setter
+    def shape(self, value: Optional[BoxShape]):
+        self.__shape = value
+        self._set_attr("shape", value.value if value is not None else None)
 
-    # on_long_press
+    # message
     @property
-    def on_long_press(self):
-        return self._get_event_handler("long_press")
+    def message(self) -> Optional[str]:
+        return self._get_attr("message")
 
-    @on_long_press.setter
-    def on_long_press(self, handler):
-        self._add_event_handler("long_press", handler)
-        self._set_attr("onLongPress", True if handler is not None else None)
+    @message.setter
+    def message(self, value: Optional[str]):
+        self._set_attr("message", value)
 
-    # content
+    # text_align
     @property
-    def content(self) -> Optional[Control]:
-        return self.__content
+    def text_align(self) -> TextAlign:
+        return self.__text_align
 
-    @content.setter
-    def content(self, value: Optional[Control]):
-        self.__content = value
+    @text_align.setter
+    def text_align(self, value: TextAlign):
+        self.__text_align = value
+        if isinstance(value, TextAlign):
+            self._set_attr("textAlign", value.value)
+        else:
+            self.__set_text_align(value)
 
-    # autofocus
+    def __set_text_align(self, value: TextAlignString):
+        self._set_attr("textAlign", value)
+
+    # text_style
     @property
-    def autofocus(self) -> Optional[bool]:
-        return self._get_attr("autofocus", data_type="bool", def_value=False)
+    def text_style(self):
+        return self.__text_style
 
-    @autofocus.setter
-    def autofocus(self, value: Optional[bool]):
-        self._set_attr("autofocus", value)
+    @text_style.setter
+    def text_style(self, value: Optional[TextStyle]):
+        self.__text_style = value
 
-    # on_hover
+    # prefer_below
     @property
-    def on_hover(self):
-        return self._get_event_handler("hover")
+    def prefer_below(self) -> Optional[bool]:
+        return self._get_attr("preferBelow", data_type="bool", def_value=False)
 
-    @on_hover.setter
-    def on_hover(self, handler):
-        self._add_event_handler("hover", handler)
-        if handler is not None:
-            self._set_attr("onHover", True)
-        else:
-            self._set_attr("onHover", None)
+    @prefer_below.setter
+    def prefer_below(self, value: Optional[bool]):
+        self._set_attr("preferBelow", value)
 
-    # on_focus
+    # height
     @property
-    def on_focus(self):
-        return self._get_event_handler("focus")
+    def height(self) -> OptionalNumber:
+        return self._get_attr("height")
 
-    @on_focus.setter
-    def on_focus(self, handler):
-        self._add_event_handler("focus", handler)
+    @height.setter
+    def height(self, value: OptionalNumber):
+        self._set_attr("height", value)
 
-    # on_blur
+    # vertical_offset
     @property
-    def on_blur(self):
-        return self._get_event_handler("blur")
+    def vertical_offset(self) -> OptionalNumber:
+        return self._get_attr("verticalOffset")
+
+    @vertical_offset.setter
+    def vertical_offset(self, value: OptionalNumber):
+        self._set_attr("verticalOffset", value)
 
-    @on_blur.setter
-    def on_blur(self, handler):
-        self._add_event_handler("blur", handler)
+    # show_duration
+    @property
+    def show_duration(self) -> Optional[int]:
+        return self._get_attr("showDuration")
+
+    @show_duration.setter
+    def show_duration(self, value: Optional[int]):
+        self._set_attr("showDuration", value)
+
+    # wait_duration
+    @property
+    def wait_duration(self) -> Optional[int]:
+        return self._get_attr("waitDuration")
+
+    @wait_duration.setter
+    def wait_duration(self, value: Optional[int]):
+        self._set_attr("waitDuration", value)
+
+    # content
+    @property
+    def content(self) -> Optional[Control]:
+        return self.__content
+
+    @content.setter
+    def content(self, value: Optional[Control]):
+        self.__content = value
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/text_span.py` & `flet_core-0.8.0.dev1537/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/text_style.py` & `flet_core-0.8.0.dev1537/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/textfield.py` & `flet_core-0.8.0.dev1537/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/theme.py` & `flet_core-0.8.0.dev1537/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/transform.py` & `flet_core-0.8.0.dev1537/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/transparent_pointer.py` & `flet_core-0.8.0.dev1537/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/types.py` & `flet_core-0.8.0.dev1537/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/user_control.py` & `flet_core-0.8.0.dev1537/src/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/utils.py` & `flet_core-0.8.0.dev1537/src/flet_core/utils.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/vertical_divider.py` & `flet_core-0.8.0.dev1537/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/view.py` & `flet_core-0.8.0.dev1537/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/src/flet_core/window_drag_area.py` & `flet_core-0.8.0.dev1537/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.8.0.dev1535/PKG-INFO` & `flet_core-0.8.0.dev1537/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-core
-Version: 0.8.0.dev1535
+Version: 0.8.0.dev1537
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

