# Comparing `tmp/pywayland-0.4.8.tar.gz` & `tmp/pywayland-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayland-0.4.8.tar", last modified: Tue Jan 11 20:29:30 2022, max compression
+gzip compressed data, was "pywayland-0.4.9.tar", last modified: Fri Jan 21 14:10:34 2022, max compression
```

## Comparing `pywayland-0.4.8.tar` & `pywayland-0.4.9.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.911056 pywayland-0.4.8/
--rw-r--r--   0 root         (0) root         (0)    10141 2022-01-11 20:29:26.000000 pywayland-0.4.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2022-01-11 20:29:26.000000 pywayland-0.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4269 2022-01-11 20:29:30.911056 pywayland-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2992 2022-01-11 20:29:26.000000 pywayland-0.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.879056 pywayland-0.4.8/pywayland/
--rw-r--r--   0 root         (0) root         (0)      939 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.879056 pywayland-0.4.8/pywayland/_ffi/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/_ffi/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)     1473 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/_ffi/ffi.pyi
--rw-r--r--   0 root         (0) root         (0)     4237 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/_ffi/lib.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.879056 pywayland-0.4.8/pywayland/client/
--rw-r--r--   0 root         (0) root         (0)      653 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11177 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/client/display.py
--rw-r--r--   0 root         (0) root         (0)     2792 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/client/eventqueue.py
--rw-r--r--   0 root         (0) root         (0)     3671 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)    13707 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/ffi_build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.879056 pywayland-0.4.8/pywayland/protocol/
--rw-r--r--   0 root         (0) root         (0)      572 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/
--rw-r--r--   0 root         (0) root         (0)     1535 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5969 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_connector_v1.py
--rw-r--r--   0 root         (0) root         (0)     8308 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_device_v1.py
--rw-r--r--   0 root         (0) root         (0)     4364 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_request_v1.py
--rw-r--r--   0 root         (0) root         (0)     4257 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1422 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3480 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_mode_feedback_v1.py
--rw-r--r--   0 root         (0) root         (0)    10759 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1349 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3715 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibit_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     2947 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibitor_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1479 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16775 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_method_context_v1.py
--rw-r--r--   0 root         (0) root         (0)     3189 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_method_v1.py
--rw-r--r--   0 root         (0) root         (0)     2921 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_surface_v1.py
--rw-r--r--   0 root         (0) root         (0)     2554 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1348 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6669 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     4103 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1387 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3975 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibit_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     5117 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibitor_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.883056 pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1417 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13495 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_buffer_params_v1.py
--rw-r--r--   0 root         (0) root         (0)    11595 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_feedback_v1.py
--rw-r--r--   0 root         (0) root         (0)    11466 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.887056 pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1447 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5134 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_confined_pointer_v1.py
--rw-r--r--   0 root         (0) root         (0)     6031 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_locked_pointer_v1.py
--rw-r--r--   0 root         (0) root         (0)     9309 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_pointer_constraints_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.887056 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)      946 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4553 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_hold_v1.py
--rw-r--r--   0 root         (0) root         (0)     6073 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_pinch_v1.py
--rw-r--r--   0 root         (0) root         (0)     5218 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_swipe_v1.py
--rw-r--r--   0 root         (0) root         (0)     4799 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gestures_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.887056 pywayland-0.4.8/pywayland/protocol/presentation_time/
--rw-r--r--   0 root         (0) root         (0)     1327 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/presentation_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6331 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/presentation_time/wp_presentation.py
--rw-r--r--   0 root         (0) root         (0)     7598 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/presentation_time/wp_presentation_feedback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.887056 pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1388 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3290 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     5691 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.891056 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1491 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3314 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     3820 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_seat_v1.py
--rw-r--r--   0 root         (0) root         (0)    21800 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_tool_v1.py
--rw-r--r--   0 root         (0) root         (0)     5109 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.891056 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/
--rw-r--r--   0 root         (0) root         (0)     1762 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3314 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_manager_v2.py
--rw-r--r--   0 root         (0) root         (0)     9190 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_group_v2.py
--rw-r--r--   0 root         (0) root         (0)     6975 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_ring_v2.py
--rw-r--r--   0 root         (0) root         (0)     7095 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_strip_v2.py
--rw-r--r--   0 root         (0) root         (0)    10369 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_v2.py
--rw-r--r--   0 root         (0) root         (0)     4785 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_seat_v2.py
--rw-r--r--   0 root         (0) root         (0)    21535 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_tool_v2.py
--rw-r--r--   0 root         (0) root         (0)     5109 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.891056 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1332 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2422 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/zwp_text_input_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)    18843 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/zwp_text_input_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.891056 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/
--rw-r--r--   0 root         (0) root         (0)     1498 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3028 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/zwp_text_input_manager_v3.py
--rw-r--r--   0 root         (0) root         (0)    19674 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/zwp_text_input_v3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.891056 pywayland-0.4.8/pywayland/protocol/viewporter/
--rw-r--r--   0 root         (0) root         (0)     1298 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/viewporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8799 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/viewporter/wp_viewport.py
--rw-r--r--   0 root         (0) root         (0)     3635 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/viewporter/wp_viewporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.895056 pywayland-0.4.8/pywayland/protocol/wayland/
--rw-r--r--   0 root         (0) root         (0)     2396 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3897 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_buffer.py
--rw-r--r--   0 root         (0) root         (0)     2300 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_callback.py
--rw-r--r--   0 root         (0) root         (0)     2860 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_compositor.py
--rw-r--r--   0 root         (0) root         (0)    11884 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_data_device.py
--rw-r--r--   0 root         (0) root         (0)     4127 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_data_device_manager.py
--rw-r--r--   0 root         (0) root         (0)    12745 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_data_offer.py
--rw-r--r--   0 root         (0) root         (0)     9415 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_data_source.py
--rw-r--r--   0 root         (0) root         (0)     5677 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_display.py
--rw-r--r--   0 root         (0) root         (0)     8394 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_keyboard.py
--rw-r--r--   0 root         (0) root         (0)    12578 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_output.py
--rw-r--r--   0 root         (0) root         (0)    18289 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_pointer.py
--rw-r--r--   0 root         (0) root         (0)     3691 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_region.py
--rw-r--r--   0 root         (0) root         (0)     5489 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_registry.py
--rw-r--r--   0 root         (0) root         (0)     8102 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_seat.py
--rw-r--r--   0 root         (0) root         (0)     3302 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_shell.py
--rw-r--r--   0 root         (0) root         (0)    15564 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_shell_surface.py
--rw-r--r--   0 root         (0) root         (0)     6805 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_shm.py
--rw-r--r--   0 root         (0) root         (0)     5078 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_shm_pool.py
--rw-r--r--   0 root         (0) root         (0)     5344 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_subcompositor.py
--rw-r--r--   0 root         (0) root         (0)    11320 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_subsurface.py
--rw-r--r--   0 root         (0) root         (0)    27440 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_surface.py
--rw-r--r--   0 root         (0) root         (0)    10742 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wayland/wl_touch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1548 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3911 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     4808 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_v1.py
--rw-r--r--   0 root         (0) root         (0)     4056 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_offer_v1.py
--rw-r--r--   0 root         (0) root         (0)     3798 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_source_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/
--rw-r--r--   0 root         (0) root         (0)     1400 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6162 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/xdg_activation_token_v1.py
--rw-r--r--   0 root         (0) root         (0)     4201 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/xdg_activation_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1341 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4443 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_decoration_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     5608 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_toplevel_decoration_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1427 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3041 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exported_v1.py
--rw-r--r--   0 root         (0) root         (0)     3359 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exporter_v1.py
--rw-r--r--   0 root         (0) root         (0)     3603 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_imported_v1.py
--rw-r--r--   0 root         (0) root         (0)     3201 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_importer_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/
--rw-r--r--   0 root         (0) root         (0)     1427 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3050 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exported_v2.py
--rw-r--r--   0 root         (0) root         (0)     3524 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exporter_v2.py
--rw-r--r--   0 root         (0) root         (0)     3743 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_imported_v2.py
--rw-r--r--   0 root         (0) root         (0)     3244 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_importer_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.899056 pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1311 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3069 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     9099 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.903056 pywayland-0.4.8/pywayland/protocol/xdg_shell/
--rw-r--r--   0 root         (0) root         (0)     1671 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12297 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_popup.py
--rw-r--r--   0 root         (0) root         (0)    12473 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_positioner.py
--rw-r--r--   0 root         (0) root         (0)    12372 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_surface.py
--rw-r--r--   0 root         (0) root         (0)    24049 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_toplevel.py
--rw-r--r--   0 root         (0) root         (0)     6939 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_wm_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.903056 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5127 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_popup.py
--rw-r--r--   0 root         (0) root         (0)     8343 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_shell.py
--rw-r--r--   0 root         (0) root         (0)    20590 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.903056 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/
--rw-r--r--   0 root         (0) root         (0)     1611 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_popup_v6.py
--rw-r--r--   0 root         (0) root         (0)    10619 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_positioner_v6.py
--rw-r--r--   0 root         (0) root         (0)     7051 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_shell_v6.py
--rw-r--r--   0 root         (0) root         (0)    12100 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_surface_v6.py
--rw-r--r--   0 root         (0) root         (0)    20570 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_toplevel_v6.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.903056 pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1367 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4413 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_manager_v1.py
--rw-r--r--   0 root         (0) root         (0)     2286 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.903056 pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/
--rw-r--r--   0 root         (0) root         (0)     1533 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_buffer_release_v1.py
--rw-r--r--   0 root         (0) root         (0)     5322 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_explicit_synchronization_v1.py
--rw-r--r--   0 root         (0) root         (0)     7889 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_surface_synchronization_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.907056 pywayland-0.4.8/pywayland/protocol_core/
--rw-r--r--   0 root         (0) root         (0)     1113 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2041 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/argument.py
--rw-r--r--   0 root         (0) root         (0)     3448 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/globals.py
--rw-r--r--   0 root         (0) root         (0)     4448 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/interface.py
--rw-r--r--   0 root         (0) root         (0)     8828 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/message.py
--rw-r--r--   0 root         (0) root         (0)     4053 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/proxy.py
--rw-r--r--   0 root         (0) root         (0)     3493 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/protocol_core/resource.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.907056 pywayland-0.4.8/pywayland/scanner/
--rw-r--r--   0 root         (0) root         (0)      618 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3891 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5023 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/argument.py
--rw-r--r--   0 root         (0) root         (0)     1785 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/copyright.py
--rw-r--r--   0 root         (0) root         (0)     1235 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/description.py
--rw-r--r--   0 root         (0) root         (0)     2252 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/element.py
--rw-r--r--   0 root         (0) root         (0)     2209 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/entry.py
--rw-r--r--   0 root         (0) root         (0)     2052 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/enum.py
--rw-r--r--   0 root         (0) root         (0)     2265 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/event.py
--rw-r--r--   0 root         (0) root         (0)     4988 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/interface.py
--rw-r--r--   0 root         (0) root         (0)     4151 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/method.py
--rw-r--r--   0 root         (0) root         (0)     8698 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/printer.py
--rw-r--r--   0 root         (0) root         (0)     3778 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/protocol.py
--rw-r--r--   0 root         (0) root         (0)     4904 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/scanner/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.911056 pywayland-0.4.8/pywayland/server/
--rw-r--r--   0 root         (0) root         (0)      733 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4537 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/server/client.py
--rw-r--r--   0 root         (0) root         (0)     6149 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/server/display.py
--rw-r--r--   0 root         (0) root         (0)     9148 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/server/eventloop.py
--rw-r--r--   0 root         (0) root         (0)     4180 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/server/listener.py
--rw-r--r--   0 root         (0) root         (0)     4137 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/utils.py
--rw-r--r--   0 root         (0) root         (0)      595 2022-01-11 20:29:26.000000 pywayland-0.4.8/pywayland/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.879056 pywayland-0.4.8/pywayland.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4269 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10239 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-01-11 20:29:30.000000 pywayland-0.4.8/pywayland.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-01-11 20:29:26.000000 pywayland-0.4.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-01-11 20:29:26.000000 pywayland-0.4.8/requirements-types.txt
--rw-r--r--   0 root         (0) root         (0)       55 2022-01-11 20:29:26.000000 pywayland-0.4.8/requirements-wheel-build.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-01-11 20:29:26.000000 pywayland-0.4.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1964 2022-01-11 20:29:30.915056 pywayland-0.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6087 2022-01-11 20:29:26.000000 pywayland-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.911056 pywayland-0.4.8/test/
--rw-r--r--   0 root         (0) root         (0)      572 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-11 20:29:30.911056 pywayland-0.4.8/test/scanner_files/
--rw-r--r--   0 root         (0) root         (0)      870 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7724 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/test_scanner_input.xml
--rw-r--r--   0 root         (0) root         (0)     3639 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/wl_core.py
--rw-r--r--   0 root         (0) root         (0)     2433 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/wl_destructor.py
--rw-r--r--   0 root         (0) root         (0)     4066 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/wl_events.py
--rw-r--r--   0 root         (0) root         (0)     5044 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/wl_requests.py
--rw-r--r--   0 root         (0) root         (0)     1211 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/scanner_files/wl_xfail.py
--rw-r--r--   0 root         (0) root         (0)     1344 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_client_destroy.py
--rw-r--r--   0 root         (0) root         (0)     1607 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_event_queue.py
--rw-r--r--   0 root         (0) root         (0)     5297 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_protocol_interface.py
--rw-r--r--   0 root         (0) root         (0)     2526 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_registry_bind.py
--rw-r--r--   0 root         (0) root         (0)     2262 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_registry_query.py
--rw-r--r--   0 root         (0) root         (0)     2888 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_resource.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_scanner.py
--rw-r--r--   0 root         (0) root         (0)     1038 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_server_display.py
--rw-r--r--   0 root         (0) root         (0)     4335 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_server_eventloop.py
--rw-r--r--   0 root         (0) root         (0)      878 2022-01-11 20:29:26.000000 pywayland-0.4.8/test/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.935609 pywayland-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)    10141 2022-01-21 14:10:30.000000 pywayland-0.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2022-01-21 14:10:30.000000 pywayland-0.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4269 2022-01-21 14:10:34.935609 pywayland-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2992 2022-01-21 14:10:30.000000 pywayland-0.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.915608 pywayland-0.4.9/pywayland/
+-rw-r--r--   0 root         (0) root         (0)      939 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.915608 pywayland-0.4.9/pywayland/_ffi/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/_ffi/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/_ffi/ffi.pyi
+-rw-r--r--   0 root         (0) root         (0)     4237 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/_ffi/lib.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/client/
+-rw-r--r--   0 root         (0) root         (0)      653 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11177 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/client/display.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/client/eventqueue.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)    13707 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/ffi_build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/
+-rw-r--r--   0 root         (0) root         (0)      572 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/
+-rw-r--r--   0 root         (0) root         (0)     1535 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_connector_v1.py
+-rw-r--r--   0 root         (0) root         (0)     8308 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_device_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_request_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1422 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_mode_feedback_v1.py
+-rw-r--r--   0 root         (0) root         (0)    10759 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1349 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibit_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibitor_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1479 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16775 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_method_context_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_method_v1.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_surface_v1.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1348 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1387 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3975 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibit_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5117 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibitor_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1417 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_buffer_params_v1.py
+-rw-r--r--   0 root         (0) root         (0)    11595 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_feedback_v1.py
+-rw-r--r--   0 root         (0) root         (0)    11466 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.919608 pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_confined_pointer_v1.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_locked_pointer_v1.py
+-rw-r--r--   0 root         (0) root         (0)     9309 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_pointer_constraints_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)      946 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_hold_v1.py
+-rw-r--r--   0 root         (0) root         (0)     6073 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_pinch_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_swipe_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gestures_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/presentation_time/
+-rw-r--r--   0 root         (0) root         (0)     1327 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/presentation_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/presentation_time/wp_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     7598 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/presentation_time/wp_presentation_feedback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1388 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5691 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_seat_v1.py
+-rw-r--r--   0 root         (0) root         (0)    21800 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_tool_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5109 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/
+-rw-r--r--   0 root         (0) root         (0)     1762 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_manager_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_group_v2.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_ring_v2.py
+-rw-r--r--   0 root         (0) root         (0)     7095 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_strip_v2.py
+-rw-r--r--   0 root         (0) root         (0)    10369 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_seat_v2.py
+-rw-r--r--   0 root         (0) root         (0)    21535 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_tool_v2.py
+-rw-r--r--   0 root         (0) root         (0)     5109 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1332 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/zwp_text_input_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)    18843 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/zwp_text_input_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/
+-rw-r--r--   0 root         (0) root         (0)     1498 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/zwp_text_input_manager_v3.py
+-rw-r--r--   0 root         (0) root         (0)    19674 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/zwp_text_input_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.923608 pywayland-0.4.9/pywayland/protocol/viewporter/
+-rw-r--r--   0 root         (0) root         (0)     1298 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/viewporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8799 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/viewporter/wp_viewport.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/viewporter/wp_viewporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/wayland/
+-rw-r--r--   0 root         (0) root         (0)     2396 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_buffer.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_callback.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_compositor.py
+-rw-r--r--   0 root         (0) root         (0)    11884 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_data_device.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_data_device_manager.py
+-rw-r--r--   0 root         (0) root         (0)    12745 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_data_offer.py
+-rw-r--r--   0 root         (0) root         (0)     9415 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     5677 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_display.py
+-rw-r--r--   0 root         (0) root         (0)     8394 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)    12578 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_output.py
+-rw-r--r--   0 root         (0) root         (0)    18289 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_pointer.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_region.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_registry.py
+-rw-r--r--   0 root         (0) root         (0)     8102 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_seat.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_shell.py
+-rw-r--r--   0 root         (0) root         (0)    15564 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_shell_surface.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_shm.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_shm_pool.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_subcompositor.py
+-rw-r--r--   0 root         (0) root         (0)    11320 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_subsurface.py
+-rw-r--r--   0 root         (0) root         (0)    27440 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_surface.py
+-rw-r--r--   0 root         (0) root         (0)    10742 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wayland/wl_touch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1548 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_offer_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_source_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/
+-rw-r--r--   0 root         (0) root         (0)     1400 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6162 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/xdg_activation_token_v1.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/xdg_activation_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1341 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_decoration_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_toplevel_decoration_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1427 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3041 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exported_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exporter_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_imported_v1.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_importer_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.927608 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/
+-rw-r--r--   0 root         (0) root         (0)     1427 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exported_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exporter_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_imported_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_importer_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1311 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     9099 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/xdg_shell/
+-rw-r--r--   0 root         (0) root         (0)     1671 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12297 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_popup.py
+-rw-r--r--   0 root         (0) root         (0)    12473 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_positioner.py
+-rw-r--r--   0 root         (0) root         (0)    12372 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_surface.py
+-rw-r--r--   0 root         (0) root         (0)    24049 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_toplevel.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_wm_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5127 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_popup.py
+-rw-r--r--   0 root         (0) root         (0)     8343 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_shell.py
+-rw-r--r--   0 root         (0) root         (0)    20590 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/
+-rw-r--r--   0 root         (0) root         (0)     1611 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_popup_v6.py
+-rw-r--r--   0 root         (0) root         (0)    10619 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_positioner_v6.py
+-rw-r--r--   0 root         (0) root         (0)     7051 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_shell_v6.py
+-rw-r--r--   0 root         (0) root         (0)    12100 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_surface_v6.py
+-rw-r--r--   0 root         (0) root         (0)    20570 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_toplevel_v6.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1367 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_manager_v1.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/
+-rw-r--r--   0 root         (0) root         (0)     1533 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_buffer_release_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_explicit_synchronization_v1.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_surface_synchronization_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.931609 pywayland-0.4.9/pywayland/protocol_core/
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/argument.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/globals.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/interface.py
+-rw-r--r--   0 root         (0) root         (0)     8828 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/message.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/protocol_core/resource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.935609 pywayland-0.4.9/pywayland/scanner/
+-rw-r--r--   0 root         (0) root         (0)      618 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/argument.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/copyright.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/description.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/element.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/entry.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/enum.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/event.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/interface.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/method.py
+-rw-r--r--   0 root         (0) root         (0)     8698 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/scanner/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.935609 pywayland-0.4.9/pywayland/server/
+-rw-r--r--   0 root         (0) root         (0)      733 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4537 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/server/client.py
+-rw-r--r--   0 root         (0) root         (0)     6149 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/server/display.py
+-rw-r--r--   0 root         (0) root         (0)     9148 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/server/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/server/listener.py
+-rw-r--r--   0 root         (0) root         (0)     4137 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/utils.py
+-rw-r--r--   0 root         (0) root         (0)      595 2022-01-21 14:10:30.000000 pywayland-0.4.9/pywayland/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.915608 pywayland-0.4.9/pywayland.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4269 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10239 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-01-21 14:10:34.000000 pywayland-0.4.9/pywayland.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2022-01-21 14:10:30.000000 pywayland-0.4.9/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-21 14:10:30.000000 pywayland-0.4.9/requirements-types.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2022-01-21 14:10:30.000000 pywayland-0.4.9/requirements-wheel-build.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2022-01-21 14:10:30.000000 pywayland-0.4.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1974 2022-01-21 14:10:34.935609 pywayland-0.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6075 2022-01-21 14:10:30.000000 pywayland-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.935609 pywayland-0.4.9/test/
+-rw-r--r--   0 root         (0) root         (0)      572 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-21 14:10:34.935609 pywayland-0.4.9/test/scanner_files/
+-rw-r--r--   0 root         (0) root         (0)      870 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7724 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/test_scanner_input.xml
+-rw-r--r--   0 root         (0) root         (0)     3639 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/wl_core.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/wl_destructor.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/wl_events.py
+-rw-r--r--   0 root         (0) root         (0)     5044 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/wl_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/scanner_files/wl_xfail.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_client_destroy.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_event_queue.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_protocol_interface.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_registry_bind.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_registry_query.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_resource.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_server_display.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_server_eventloop.py
+-rw-r--r--   0 root         (0) root         (0)      878 2022-01-21 14:10:30.000000 pywayland-0.4.9/test/test_utils.py
```

### Comparing `pywayland-0.4.8/LICENSE` & `pywayland-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/PKG-INFO` & `pywayland-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayland
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python bindings for the libwayland library written in pure Python
 Home-page: https://github.com/flacjacket/pywayland
 Author: Sean Vig
 Author-email: sean.v.775@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pywayland.readthedocs.io
 Project-URL: Code, https://github.com/flacjacket/pywayland
```

### Comparing `pywayland-0.4.8/README.rst` & `pywayland-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/__init__.py` & `pywayland-0.4.9/pywayland/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/_ffi/ffi.pyi` & `pywayland-0.4.9/pywayland/_ffi/ffi.pyi`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/_ffi/lib.pyi` & `pywayland-0.4.9/pywayland/_ffi/lib.pyi`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/client/__init__.py` & `pywayland-0.4.9/pywayland/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/client/display.py` & `pywayland-0.4.9/pywayland/client/display.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/client/eventqueue.py` & `pywayland-0.4.9/pywayland/client/eventqueue.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/dispatcher.py` & `pywayland-0.4.9/pywayland/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/ffi_build.py` & `pywayland-0.4.9/pywayland/ffi_build.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/__init__.py` & `pywayland-0.4.9/pywayland/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/drm_lease_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/drm_lease_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_connector_v1.py` & `pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_connector_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_device_v1.py` & `pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_device_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_request_v1.py` & `pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_request_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/drm_lease_v1/wp_drm_lease_v1.py` & `pywayland-0.4.9/pywayland/protocol/drm_lease_v1/wp_drm_lease_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_mode_feedback_v1.py` & `pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_mode_feedback_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_v1.py` & `pywayland-0.4.9/pywayland/protocol/fullscreen_shell_unstable_v1/zwp_fullscreen_shell_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibit_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibit_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibitor_v1.py` & `pywayland-0.4.9/pywayland/protocol/idle_inhibit_unstable_v1/zwp_idle_inhibitor_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_method_context_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_method_context_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_method_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_method_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_surface_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_surface_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_method_unstable_v1/zwp_input_panel_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_v1.py` & `pywayland-0.4.9/pywayland/protocol/input_timestamps_unstable_v1/zwp_input_timestamps_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibit_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibit_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibitor_v1.py` & `pywayland-0.4.9/pywayland/protocol/keyboard_shortcuts_inhibit_unstable_v1/zwp_keyboard_shortcuts_inhibitor_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_buffer_params_v1.py` & `pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_buffer_params_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_feedback_v1.py` & `pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_feedback_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_v1.py` & `pywayland-0.4.9/pywayland/protocol/linux_dmabuf_unstable_v1/zwp_linux_dmabuf_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_confined_pointer_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_confined_pointer_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_locked_pointer_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_locked_pointer_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_constraints_unstable_v1/zwp_pointer_constraints_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_constraints_unstable_v1/zwp_pointer_constraints_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_hold_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_hold_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_pinch_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_pinch_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_swipe_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gesture_swipe_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gestures_v1.py` & `pywayland-0.4.9/pywayland/protocol/pointer_gestures_unstable_v1/zwp_pointer_gestures_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/presentation_time/__init__.py` & `pywayland-0.4.9/pywayland/protocol/presentation_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/presentation_time/wp_presentation.py` & `pywayland-0.4.9/pywayland/protocol/presentation_time/wp_presentation.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/presentation_time/wp_presentation_feedback.py` & `pywayland-0.4.9/pywayland/protocol/presentation_time/wp_presentation_feedback.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_v1.py` & `pywayland-0.4.9/pywayland/protocol/relative_pointer_unstable_v1/zwp_relative_pointer_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_seat_v1.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_seat_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_tool_v1.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_tool_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v1/zwp_tablet_v1.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v1/zwp_tablet_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/__init__.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_manager_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_manager_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_group_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_group_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_ring_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_ring_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_strip_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_strip_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_pad_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_seat_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_seat_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_tool_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_tool_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/tablet_unstable_v2/zwp_tablet_v2.py` & `pywayland-0.4.9/pywayland/protocol/tablet_unstable_v2/zwp_tablet_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/zwp_text_input_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/zwp_text_input_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v1/zwp_text_input_v1.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v1/zwp_text_input_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/__init__.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/zwp_text_input_manager_v3.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/zwp_text_input_manager_v3.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/text_input_unstable_v3/zwp_text_input_v3.py` & `pywayland-0.4.9/pywayland/protocol/text_input_unstable_v3/zwp_text_input_v3.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/viewporter/__init__.py` & `pywayland-0.4.9/pywayland/protocol/viewporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/viewporter/wp_viewport.py` & `pywayland-0.4.9/pywayland/protocol/viewporter/wp_viewport.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/viewporter/wp_viewporter.py` & `pywayland-0.4.9/pywayland/protocol/viewporter/wp_viewporter.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/__init__.py` & `pywayland-0.4.9/pywayland/protocol/wayland/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_buffer.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_buffer.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_callback.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_callback.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_compositor.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_compositor.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_data_device.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_data_device.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_data_device_manager.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_data_device_manager.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_data_offer.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_data_offer.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_data_source.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_data_source.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_display.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_display.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_keyboard.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_keyboard.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_output.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_output.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_pointer.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_pointer.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_region.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_region.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_registry.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_registry.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_seat.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_seat.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_shell.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_shell.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_shell_surface.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_shell_surface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_shm.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_shm.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_shm_pool.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_shm_pool.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_subcompositor.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_subcompositor.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_subsurface.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_subsurface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_surface.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_surface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wayland/wl_touch.py` & `pywayland-0.4.9/pywayland/protocol/wayland/wl_touch.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_v1.py` & `pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_device_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_offer_v1.py` & `pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_offer_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_source_v1.py` & `pywayland-0.4.9/pywayland/protocol/wp_primary_selection_unstable_v1/zwp_primary_selection_source_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/xdg_activation_token_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/xdg_activation_token_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_activation_v1/xdg_activation_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_activation_v1/xdg_activation_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_decoration_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_decoration_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_toplevel_decoration_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_decoration_unstable_v1/zxdg_toplevel_decoration_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exported_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exported_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exporter_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_exporter_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_imported_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_imported_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_importer_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v1/zxdg_importer_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exported_v2.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exported_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exporter_v2.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_exporter_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_imported_v2.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_imported_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_importer_v2.py` & `pywayland-0.4.9/pywayland/protocol/xdg_foreign_unstable_v2/zxdg_importer_v2.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_v1.py` & `pywayland-0.4.9/pywayland/protocol/xdg_output_unstable_v1/zxdg_output_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_popup.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_popup.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_positioner.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_positioner.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_surface.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_surface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_toplevel.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_toplevel.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell/xdg_wm_base.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell/xdg_wm_base.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_popup.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_popup.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_shell.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_shell.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v5/xdg_surface.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v5/xdg_surface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_popup_v6.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_popup_v6.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_positioner_v6.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_positioner_v6.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_shell_v6.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_shell_v6.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_surface_v6.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_surface_v6.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xdg_shell_unstable_v6/zxdg_toplevel_v6.py` & `pywayland-0.4.9/pywayland/protocol/xdg_shell_unstable_v6/zxdg_toplevel_v6.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_manager_v1.py` & `pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_manager_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_v1.py` & `pywayland-0.4.9/pywayland/protocol/xwayland_keyboard_grab_unstable_v1/zwp_xwayland_keyboard_grab_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/__init__.py` & `pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_buffer_release_v1.py` & `pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_buffer_release_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_explicit_synchronization_v1.py` & `pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_explicit_synchronization_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_surface_synchronization_v1.py` & `pywayland-0.4.9/pywayland/protocol/zwp_linux_explicit_synchronization_unstable_v1/zwp_linux_surface_synchronization_v1.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/__init__.py` & `pywayland-0.4.9/pywayland/protocol_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/argument.py` & `pywayland-0.4.9/pywayland/protocol_core/argument.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/globals.py` & `pywayland-0.4.9/pywayland/protocol_core/globals.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/interface.py` & `pywayland-0.4.9/pywayland/protocol_core/interface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/message.py` & `pywayland-0.4.9/pywayland/protocol_core/message.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/proxy.py` & `pywayland-0.4.9/pywayland/protocol_core/proxy.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/protocol_core/resource.py` & `pywayland-0.4.9/pywayland/protocol_core/resource.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/__init__.py` & `pywayland-0.4.9/pywayland/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/__main__.py` & `pywayland-0.4.9/pywayland/scanner/__main__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/argument.py` & `pywayland-0.4.9/pywayland/scanner/argument.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/copyright.py` & `pywayland-0.4.9/pywayland/scanner/copyright.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/description.py` & `pywayland-0.4.9/pywayland/scanner/description.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/element.py` & `pywayland-0.4.9/pywayland/scanner/element.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/entry.py` & `pywayland-0.4.9/pywayland/scanner/entry.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/enum.py` & `pywayland-0.4.9/pywayland/scanner/enum.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/event.py` & `pywayland-0.4.9/pywayland/scanner/event.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/interface.py` & `pywayland-0.4.9/pywayland/scanner/interface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/method.py` & `pywayland-0.4.9/pywayland/scanner/method.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/printer.py` & `pywayland-0.4.9/pywayland/scanner/printer.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/protocol.py` & `pywayland-0.4.9/pywayland/scanner/protocol.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/scanner/request.py` & `pywayland-0.4.9/pywayland/scanner/request.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/server/__init__.py` & `pywayland-0.4.9/pywayland/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/server/client.py` & `pywayland-0.4.9/pywayland/server/client.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/server/display.py` & `pywayland-0.4.9/pywayland/server/display.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/server/eventloop.py` & `pywayland-0.4.9/pywayland/server/eventloop.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/server/listener.py` & `pywayland-0.4.9/pywayland/server/listener.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/utils.py` & `pywayland-0.4.9/pywayland/utils.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/pywayland/version.py` & `pywayland-0.4.9/pywayland/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
```

### Comparing `pywayland-0.4.8/pywayland.egg-info/PKG-INFO` & `pywayland-0.4.9/pywayland.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayland
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python bindings for the libwayland library written in pure Python
 Home-page: https://github.com/flacjacket/pywayland
 Author: Sean Vig
 Author-email: sean.v.775@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pywayland.readthedocs.io
 Project-URL: Code, https://github.com/flacjacket/pywayland
```

### Comparing `pywayland-0.4.8/pywayland.egg-info/SOURCES.txt` & `pywayland-0.4.9/pywayland.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/setup.cfg` & `pywayland-0.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pywayland
-version = attr:version.__version__
+version = attr:pywayland.version.__version__
 author = Sean Vig
 author_email = sean.v.775@gmail.com
 license = Apache License 2.0
 license_file = LICENSE
 description = Python bindings for the libwayland library written in pure Python
 url = https://github.com/flacjacket/pywayland
 classifiers =
```

### Comparing `pywayland-0.4.8/setup.py` & `pywayland-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from setuptools.command.sdist import sdist
 
 try:
     from wheel.bdist_wheel import bdist_wheel
 except ImportError:
     bdist_wheel = None
 
-# we need this to import the version and scanner module directly so we can
-# build the protocol before the cffi module has been compiled
+# we need this to import the scanner module directly so we can build the
+# protocol before the cffi module has been compiled
 sys.path.insert(0, "pywayland")
 
 default_xml_file = "/usr/share/wayland/wayland.xml"
 
 
 def get_protocol_command(klass):
     class ProtocolCommand(klass):
```

### Comparing `pywayland-0.4.8/test/__init__.py` & `pywayland-0.4.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/__init__.py` & `pywayland-0.4.9/test/scanner_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/test_scanner_input.xml` & `pywayland-0.4.9/test/scanner_files/test_scanner_input.xml`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/wl_core.py` & `pywayland-0.4.9/test/scanner_files/wl_core.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/wl_destructor.py` & `pywayland-0.4.9/test/scanner_files/wl_destructor.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/wl_events.py` & `pywayland-0.4.9/test/scanner_files/wl_events.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/wl_requests.py` & `pywayland-0.4.9/test/scanner_files/wl_requests.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/scanner_files/wl_xfail.py` & `pywayland-0.4.9/test/scanner_files/wl_xfail.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_client_destroy.py` & `pywayland-0.4.9/test/test_client_destroy.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_event_queue.py` & `pywayland-0.4.9/test/test_event_queue.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_protocol_interface.py` & `pywayland-0.4.9/test/test_protocol_interface.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_registry_bind.py` & `pywayland-0.4.9/test/test_registry_bind.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_registry_query.py` & `pywayland-0.4.9/test/test_registry_query.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_resource.py` & `pywayland-0.4.9/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_scanner.py` & `pywayland-0.4.9/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_server_display.py` & `pywayland-0.4.9/test/test_server_display.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_server_eventloop.py` & `pywayland-0.4.9/test/test_server_eventloop.py`

 * *Files identical despite different names*

### Comparing `pywayland-0.4.8/test/test_utils.py` & `pywayland-0.4.9/test/test_utils.py`

 * *Files identical despite different names*

