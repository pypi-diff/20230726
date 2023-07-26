# Comparing `tmp/PySide2-Material-Widgets-0.0.10.tar.gz` & `tmp/PySide2-Material-Widgets-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Material-Widgets-0.0.10.tar", last modified: Wed Jul 26 04:48:17 2023, max compression
+gzip compressed data, was "dist\PySide2-Material-Widgets-0.0.11.tar", last modified: Wed Jul 26 04:50:53 2023, max compression
```

## Comparing `PySide2-Material-Widgets-0.0.10.tar` & `PySide2-Material-Widgets-0.0.11.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.402633 PySide2-Material-Widgets-0.0.10/
--rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide2-Material-Widgets-0.0.10/LICENSE
--rw-rw-rw-   0        0        0     4405 2023-07-26 04:48:17.401635 PySide2-Material-Widgets-0.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.199754 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4405 2023-07-26 04:48:17.000000 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3899 2023-07-26 04:48:17.000000 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 04:48:17.000000 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-26 04:48:17.000000 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 04:48:17.000000 PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3601 2023-07-26 00:28:05.000000 PySide2-Material-Widgets-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.202755 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/
--rw-rw-rw-   0        0        0      710 2023-07-26 04:47:11.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.207122 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5933542 2023-07-26 03:47:15.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.258348 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/
--rw-rw-rw-   0        0        0      552 2023-07-22 14:31:29.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     7944 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1189 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/color.py
--rw-rw-rw-   0        0        0    10647 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     1306 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/font.py
--rw-rw-rw-   0        0        0    12716 2023-07-26 03:51:09.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/icon.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.261405 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.264797 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/blend/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/blend/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/blend/blend.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.275415 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/cam16.py
--rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/hct.py
--rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.282477 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/__init__.py
--rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/core_palette.py
--rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.298734 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
--rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
--rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
--rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.302444 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/scheme/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/scheme/__init__.py
--rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.307026 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/score/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/score/__init__.py
--rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/score/score.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.322379 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/__init__.py
--rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/color_utils.py
--rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/image_utils.py
--rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/math_utils.py
--rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/string_utils.py
--rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/theme_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/router.py
--rw-rw-rw-   0        0        0     4874 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    12748 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      460 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.324699 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/
--rw-rw-rw-   0        0        0       72 2023-07-26 04:29:03.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.331538 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0     3194 2023-07-26 04:17:47.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     4660 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/message_box.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.339438 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/
--rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/flow_layout.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:48:17.398625 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2050 2023-07-26 04:33:30.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0    16812 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     4932 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     2437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0     5717 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/floating_action_button.py
--rw-rw-rw-   0        0        0    16139 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2049 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1355 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16646 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    21236 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     9136 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    35532 2023-07-26 03:51:47.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0      711 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/overlay_widget.py
--rw-rw-rw-   0        0        0     8210 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     5562 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     1346 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/radio_button.py
--rw-rw-rw-   0        0        0     5707 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/ripple.py
--rw-rw-rw-   0        0        0     2598 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18195 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     6356 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0    10489 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    22383 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10242 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0       42 2023-07-26 04:48:17.402633 PySide2-Material-Widgets-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-07-26 04:47:08.000000 PySide2-Material-Widgets-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.363751 PySide2-Material-Widgets-0.0.11/
+-rw-rw-rw-   0        0        0    35823 2023-07-24 00:28:48.000000 PySide2-Material-Widgets-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0     4405 2023-07-26 04:50:53.362333 PySide2-Material-Widgets-0.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.160305 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4405 2023-07-26 04:50:52.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3899 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 04:50:52.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 04:50:53.000000 PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3601 2023-07-26 04:49:23.000000 PySide2-Material-Widgets-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.162789 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/
+-rw-rw-rw-   0        0        0      710 2023-07-26 04:50:02.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.167342 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5933542 2023-07-26 03:47:15.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.210538 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/
+-rw-rw-rw-   0        0        0      552 2023-07-22 14:31:29.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     7944 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1189 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/color.py
+-rw-rw-rw-   0        0        0    10647 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0     1306 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/font.py
+-rw-rw-rw-   0        0        0    12716 2023-07-26 03:51:09.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/icon.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.212625 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.217533 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/__init__.py
+-rw-rw-rw-   0        0        0     4816 2023-07-17 01:35:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/blend.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.228572 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-07-17 01:35:19.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/cam16.py
+-rw-rw-rw-   0        0        0     8397 2023-07-17 01:35:26.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/hct.py
+-rw-rw-rw-   0        0        0     5391 2023-07-17 01:35:30.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/viewing_conditions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.236201 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-07-17 01:35:03.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/core_palette.py
+-rw-rw-rw-   0        0        0     1985 2023-07-17 01:35:12.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/tonal_palette.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.254774 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/__init__.py
+-rw-rw-rw-   0        0        0     1929 2023-07-17 01:34:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py
+-rw-rw-rw-   0        0        0     2158 2023-07-17 01:34:38.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py
+-rw-rw-rw-   0        0        0     1723 2023-07-17 01:34:42.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_map.py
+-rw-rw-rw-   0        0        0     8297 2023-07-17 01:34:46.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py
+-rw-rw-rw-   0        0        0    14347 2023-07-17 01:34:55.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.260477 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/__init__.py
+-rw-rw-rw-   0        0        0     7792 2023-07-21 13:40:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.265841 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/__init__.py
+-rw-rw-rw-   0        0        0     6017 2023-07-17 01:34:16.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/score.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.282364 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:52:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/__init__.py
+-rw-rw-rw-   0        0        0     7656 2023-07-17 01:33:35.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/color_utils.py
+-rw-rw-rw-   0        0        0     2850 2023-07-17 01:35:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/image_utils.py
+-rw-rw-rw-   0        0        0     2854 2023-07-16 13:31:20.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/math_utils.py
+-rw-rw-rw-   0        0        0     2325 2023-07-17 01:33:56.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/string_utils.py
+-rw-rw-rw-   0        0        0     3857 2023-07-17 01:34:05.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/theme_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4874 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    12748 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      460 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.284371 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/
+-rw-rw-rw-   0        0        0       72 2023-07-26 04:29:03.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.292140 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0       35 2023-07-22 09:35:54.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0     3194 2023-07-26 04:17:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     4660 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/message_box.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.300077 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/
+-rw-rw-rw-   0        0        0       76 2023-07-18 06:23:37.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/flow_layout.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:50:53.359671 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2050 2023-07-26 04:33:30.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0    16812 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     4932 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     2437 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0     5717 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/floating_action_button.py
+-rw-rw-rw-   0        0        0    16139 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2049 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1355 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16646 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    21236 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     9136 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    35532 2023-07-26 03:51:47.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0      711 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/overlay_widget.py
+-rw-rw-rw-   0        0        0     8210 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     5562 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     1346 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/radio_button.py
+-rw-rw-rw-   0        0        0     5707 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/ripple.py
+-rw-rw-rw-   0        0        0     2598 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    18195 2023-07-26 03:47:14.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     6356 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0    10489 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    22383 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10242 2023-07-26 03:47:13.000000 PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 04:50:53.363751 PySide2-Material-Widgets-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-07-26 04:50:09.000000 PySide2-Material-Widgets-0.0.11/setup.py
```

### Comparing `PySide2-Material-Widgets-0.0.10/LICENSE` & `PySide2-Material-Widgets-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/PKG-INFO` & `PySide2-Material-Widgets-0.0.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Material-Widgets
-Version: 0.0.10
+Version: 0.0.11
 Summary: A material design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -17,27 +17,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img width="18%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/logo.png" alt="logo">
 </p>
   <h1 align="center">
-  PySide6-Material-Widgets
+  PySide2-Material-Widgets
 </h1>
 <p align="center">
-  A material design widgets library based on PySide6
+  A material design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
-    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  <a href="https://pypi.org/project/PySide2-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pySide2-material-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
+    <img src="https://static.pepy.tech/personalized-badge/PySide2-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
@@ -50,49 +50,49 @@
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/Interface.jpg)
 
 ## Install
 To install Community version:
 ```shell
-pip install PySide6-Material-Widgets -i https://pypi.org/simple/
+pip install PySide2-Material-Widgets -i https://pypi.org/simple/
 ```
 
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
-> Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
+> Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
-After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
+After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
+Want to know more about PySide2-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide2-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
-You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
+You can use PySide2-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide2-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## Reference
 * [**Figma/Material 3 Design Kit**: Provides an introduction to the material design system](https://www.figma.com/community/file/1035203688168086460/Material-3-Design-Kit)
 * [**Google/Material Design**: A website demonstrates the controls available in Material Design 3 System](https://m3.material.io/get-started)
 
 
 ## License
-PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
+PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 
 Copyright © 2021 by zhiyiYo.
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.10 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.11 Summary: A
 material design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside2 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [logo]
-                    ****** PySide6-Material-Widgets ******
-              A material design widgets library based on PySide6
+                    ****** PySide2-Material-Widgets ******
+              A material design widgets library based on PySide2
          [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
-```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
+```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
-zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
+zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
+`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
 package using pip, you can run the demo in examples directory, for example:
 ```python cd examples/button python demo.py ``` If you encounter `ImportError:
 cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
 imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
+Want to know more about PySide2-Material-Widgets? Please read the [help
 document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
 Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
+that shows off what PySide2-Material-Widgets are capable of ð ## Work with
+QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
 running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
+should be able to see the PySide2-Material-Widgets in the sidebar of
 QtDesigner. ## Support If this project helps you a lot and you want to support
 the development and maintenance of this project, feel free to sponsor me via
 [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
 zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
 Material 3 Design Kit**: Provides an introduction to the material design
 system](https://www.figma.com/community/file/1035203688168086460/Material-3-
 Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
 available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
+License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
 licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
 [ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
 of this project. Copyright Â© 2021 by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/PKG-INFO` & `PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Material-Widgets
-Version: 0.0.10
+Version: 0.0.11
 Summary: A material design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/QMaterialWidgets/tree/master
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qmaterialwidgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/QMaterialWidgets/tree/master
@@ -17,27 +17,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img width="18%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/logo.png" alt="logo">
 </p>
   <h1 align="center">
-  PySide6-Material-Widgets
+  PySide2-Material-Widgets
 </h1>
 <p align="center">
-  A material design widgets library based on PySide6
+  A material design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
-    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  <a href="https://pypi.org/project/PySide2-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pySide2-material-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
+    <img src="https://static.pepy.tech/personalized-badge/PySide2-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
@@ -50,49 +50,49 @@
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/Interface.jpg)
 
 ## Install
 To install Community version:
 ```shell
-pip install PySide6-Material-Widgets -i https://pypi.org/simple/
+pip install PySide2-Material-Widgets -i https://pypi.org/simple/
 ```
 
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
-> Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
+> Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
-After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
+After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
+Want to know more about PySide2-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide2-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
-You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
+You can use PySide2-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide2-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## Reference
 * [**Figma/Material 3 Design Kit**: Provides an introduction to the material design system](https://www.figma.com/community/file/1035203688168086460/Material-3-Design-Kit)
 * [**Google/Material Design**: A website demonstrates the controls available in Material Design 3 System](https://m3.material.io/get-started)
 
 
 ## License
-PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
+PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 
 Copyright © 2021 by zhiyiYo.
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.10 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Material-Widgets Version: 0.0.11 Summary: A
 material design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 qmaterialwidgets.readthedocs.io/ Project-URL: Source Code, https://github.com/
 zhiyiYo/QMaterialWidgets/tree/master Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/QMaterialWidgets/issues Keywords: pyside2 material widgets
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [logo]
-                    ****** PySide6-Material-Widgets ******
-              A material design widgets library based on PySide6
+                    ****** PySide2-Material-Widgets ******
+              A material design widgets library based on PySide2
          [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
-```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
+```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
-zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
+zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
+`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
 package using pip, you can run the demo in examples directory, for example:
 ```python cd examples/button python demo.py ``` If you encounter `ImportError:
 cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
 imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
+Want to know more about PySide2-Material-Widgets? Please read the [help
 document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
 Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
+that shows off what PySide2-Material-Widgets are capable of ð ## Work with
+QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
 running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
+should be able to see the PySide2-Material-Widgets in the sidebar of
 QtDesigner. ## Support If this project helps you a lot and you want to support
 the development and maintenance of this project, feel free to sponsor me via
 [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
 zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
 Material 3 Design Kit**: Provides an introduction to the material design
 system](https://www.figma.com/community/file/1035203688168086460/Material-3-
 Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
 available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
+License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
 licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
 [ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
 of this project. Copyright Â© 2021 by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.10/PySide2_Material_Widgets.egg-info/SOURCES.txt` & `PySide2-Material-Widgets-0.0.11/PySide2_Material_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/README.md` & `PySide2-Material-Widgets-0.0.11/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <p align="center">
   <img width="18%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/logo.png" alt="logo">
 </p>
   <h1 align="center">
-  PySide6-Material-Widgets
+  PySide2-Material-Widgets
 </h1>
 <p align="center">
-  A material design widgets library based on PySide6
+  A material design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a href="https://pypi.org/project/PySide6-Material-Widgets" target="_blank">
-    <img src="https://img.shields.io/pypi/v/pyside6-material-widgets?color=%2334D058&label=Version" alt="Version">
+  <a href="https://pypi.org/project/PySide2-Material-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pySide2-material-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://static.pepy.tech/personalized-badge/pyside6-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
+    <img src="https://static.pepy.tech/personalized-badge/PySide2-material-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 
   <a style="text-decoration:none">
@@ -31,47 +31,47 @@
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/docs/source/_static/Interface.jpg)
 
 ## Install
 To install Community version:
 ```shell
-pip install PySide6-Material-Widgets -i https://pypi.org/simple/
+pip install PySide2-Material-Widgets -i https://pypi.org/simple/
 ```
 
 The Community version only provides basic components, while the more advanced ones are available in the [Premium version](https://afdian.net/a/zhiyiYo?tab=shop).
 
 > **Warning**
-> Don't install PySide6-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
+> Don't install PySide2-Material-Widgets and PySide2-Material-Widgets at the same time, because their package names are all `qmaterialwidgets`.
 
 
 ## Run Example
-After installing PySide6-Material-Widgets package using pip, you can run the demo in examples directory, for example:
+After installing PySide2-Material-Widgets package using pip, you can run the demo in examples directory, for example:
 ```python
 cd examples/button
 python demo.py
 ```
 
 If you encounter `ImportError: cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the imported components are only available in the Premium version.
 
 ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
+Want to know more about PySide2-Material-Widgets? Please read the [help document](https://qmaterialwidgets.readthedocs.io/) 👈
 
 ## Video Demonstration
-Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide6-Material-Widgets are capable of 🎉
+Check out this [▶ example video](https://www.bilibili.com/video/BV1k14y1z74o) that shows off what PySide2-Material-Widgets are capable of 🎉
 
 ## Work with QtDesigner
-You can use PySide6-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide6-Material-Widgets in the sidebar of QtDesigner.
+You can use PySide2-Material-Widgets in QtDesigner directly by running `python ./tools/designer.py`. If the operation is successful, you should be able to see the PySide2-Material-Widgets in the sidebar of QtDesigner.
 
 
 ## Support
 If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## Reference
 * [**Figma/Material 3 Design Kit**: Provides an introduction to the material design system](https://www.figma.com/community/file/1035203688168086460/Material-3-Design-Kit)
 * [**Google/Material Design**: A website demonstrates the controls available in Material Design 3 System](https://m3.material.io/get-started)
 
 
 ## License
-PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
+PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 
 Copyright © 2021 by zhiyiYo.
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
                                     [logo]
-                    ****** PySide6-Material-Widgets ******
-              A material design widgets library based on PySide6
+                    ****** PySide2-Material-Widgets ******
+              A material design widgets library based on PySide2
          [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/QMaterialWidgets/master/
 docs/source/_static/Interface.jpg) ## Install To install Community version:
-```shell pip install PySide6-Material-Widgets -i https://pypi.org/simple/ ```
+```shell pip install PySide2-Material-Widgets -i https://pypi.org/simple/ ```
 The Community version only provides basic components, while the more advanced
 ones are available in the [Premium version](https://afdian.net/a/
-zhiyiYo?tab=shop). > **Warning** > Don't install PySide6-Material-Widgets and
+zhiyiYo?tab=shop). > **Warning** > Don't install PySide2-Material-Widgets and
 PySide2-Material-Widgets at the same time, because their package names are all
-`qmaterialwidgets`. ## Run Example After installing PySide6-Material-Widgets
+`qmaterialwidgets`. ## Run Example After installing PySide2-Material-Widgets
 package using pip, you can run the demo in examples directory, for example:
 ```python cd examples/button python demo.py ``` If you encounter `ImportError:
 cannot import name 'XXX' from 'qmaterialwidgets'`, it indicates that the
 imported components are only available in the Premium version. ## Documentation
-Want to know more about PySide6-Material-Widgets? Please read the [help
+Want to know more about PySide2-Material-Widgets? Please read the [help
 document](https://qmaterialwidgets.readthedocs.io/) ð ## Video Demonstration
 Check out this [â¶ example video](https://www.bilibili.com/video/BV1k14y1z74o)
-that shows off what PySide6-Material-Widgets are capable of ð ## Work with
-QtDesigner You can use PySide6-Material-Widgets in QtDesigner directly by
+that shows off what PySide2-Material-Widgets are capable of ð ## Work with
+QtDesigner You can use PySide2-Material-Widgets in QtDesigner directly by
 running `python ./tools/designer.py`. If the operation is successful, you
-should be able to see the PySide6-Material-Widgets in the sidebar of
+should be able to see the PySide2-Material-Widgets in the sidebar of
 QtDesigner. ## Support If this project helps you a lot and you want to support
 the development and maintenance of this project, feel free to sponsor me via
 [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/
 zhiyiYo). Your support is highly appreciated ð¥° ## Reference * [**Figma/
 Material 3 Design Kit**: Provides an introduction to the material design
 system](https://www.figma.com/community/file/1035203688168086460/Material-3-
 Design-Kit) * [**Google/Material Design**: A website demonstrates the controls
 available in Material Design 3 System](https://m3.material.io/get-started) ##
-License PySide6-Material-Widgets adopts dual licenses. Non-commercial usage is
+License PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is
 licensed under [GPLv3](./LICENSE). For commercial purposes, please purchase on
 [ç±åçµ](https://afdian.net/a/zhiyiYo?tab=shop) to support the development
 of this project. Copyright Â© 2021 by zhiyiYo.
```

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/__init__.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 Examples are available at https://github.com/zhiyiYo/QMaterialWidgets/tree/master/examples.
 
 :copyright: (c) 2023 by zhiyiYo.
 :license: PySide2-Material-Widgets adopts dual licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE).
 For commercial purposes, please purchase on [爱发电](https://afdian.net/a/zhiyiYo?tab=shop) to support the development of this project.
 """
 
-__version__ = "0.0.10"
+__version__ = "0.0.11"
 
 from .components import *
 from .common import *
 from ._rc import resource
```

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/_rc/resource.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/__init__.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/animation.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/auto_wrap.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/color.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/config.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/exception_handler.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/font.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/icon.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/blend/blend.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/blend/blend.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/cam16.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/cam16.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/hct.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/hct.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/hct/viewing_conditions.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/hct/viewing_conditions.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/core_palette.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/core_palette.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/palettes/tonal_palette.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/lab_point_provider.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_celebi.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_map.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_map.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wsmeans.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/quantize/quantizer_wu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/scheme/scheme.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/score/score.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/score/score.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/color_utils.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/image_utils.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/math_utils.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/string_utils.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/material_color/utils/theme_utils.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/material_color/utils/theme_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/overload.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/router.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/smooth_scroll.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/common/style_sheet.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/mask_dialog_base.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/dialog_box/message_box.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/dialog_box/message_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/expand_layout.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/layout/flow_layout.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/__init__.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/button.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/card_widget.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/check_box.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/floating_action_button.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/flyout.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/frameless_window.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/icon_widget.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/info_badge.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/info_bar.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/label.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/menu.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/overlay_widget.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/overlay_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/progress_bar.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/progress_ring.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/radio_button.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/ripple.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/ripple.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/scroll_area.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/scroll_bar.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/stacked_widget.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/switch_button.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/teaching_tip.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/qmaterialwidgets/components/widgets/tool_tip.py` & `PySide2-Material-Widgets-0.0.11/qmaterialwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Material-Widgets-0.0.10/setup.py` & `PySide2-Material-Widgets-0.0.11/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Material-Widgets",
-    version="0.0.10",
+    version="0.0.11",
     keywords="pyside2 material widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A material design widgets library based on PySide2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

