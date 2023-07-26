# Comparing `tmp/python-pptx-fix-0.6.21.1.tar.gz` & `tmp/python-pptx-fix-0.6.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pptx-fix-0.6.21.1.tar", last modified: Tue Jul 25 08:35:20 2023, max compression
+gzip compressed data, was "python-pptx-fix-0.6.21.2.tar", last modified: Wed Jul 26 10:14:43 2023, max compression
```

## Comparing `python-pptx-fix-0.6.21.1.tar` & `python-pptx-fix-0.6.21.2.tar`

### file list

```diff
@@ -1,565 +1,565 @@
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.910500 python-pptx-fix-0.6.21.1/
--rw-rw-r--   0 kas       (1000) kas       (1000)    15654 2023-07-25 08:35:16.000000 python-pptx-fix-0.6.21.1/HISTORY.rst
--rw-rw-r--   0 kas       (1000) kas       (1000)     1104 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/LICENSE
--rw-rw-r--   0 kas       (1000) kas       (1000)      177 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/MANIFEST.in
--rw-rw-r--   0 kas       (1000) kas       (1000)    19225 2023-07-25 08:35:20.914500 python-pptx-fix-0.6.21.1/PKG-INFO
--rw-rw-r--   0 kas       (1000) kas       (1000)     1328 2023-07-25 07:29:02.000000 python-pptx-fix-0.6.21.1/README.rst
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.630496 python-pptx-fix-0.6.21.1/features/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.630496 python-pptx-fix-0.6.21.1/features/_scratch/
--rw-rw-r--   0 kas       (1000) kas       (1000)    20086 2023-07-25 07:50:39.000000 python-pptx-fix-0.6.21.1/features/_scratch/test_out.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     3215 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/act-action.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2045 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/act-hyperlink.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     6389 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-axis-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1360 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-axistitle-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2059 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-category-access.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      569 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-category-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4227 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-chart.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1374 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-charttitle-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4641 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-data-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     6935 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-datalabels.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      406 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-gridlines-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1034 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-legend-access.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     3185 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-legend-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-marker-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4323 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-plot-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      945 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-point-access.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-point-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1471 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-replace-data.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4648 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-series.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      972 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/cht-ticklabels-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      687 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/dml-color.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1018 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/dml-effect.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     3098 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/dml-fill.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2163 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/dml-line.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      518 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/environment.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1602 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/ph-inherit-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1391 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/ph-insert-shape.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      815 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/ph-phfmt-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1427 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/ph-placeholder-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      992 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/prs-coreprops.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      466 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/prs-default-template.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1417 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/prs-open-save.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1134 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/prs-presentation-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      761 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-autoshape.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2720 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-connector.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2245 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-freeform.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1622 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-graphicframe.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1353 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-groupshape.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      568 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-movie-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2475 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-picture.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      612 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-placeholder.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)    14081 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-shapes.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     6239 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/shp-shared.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      488 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/sld-background.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4081 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/sld-slide.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2339 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/sld-slides.feature
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.646497 python-pptx-fix-0.6.21.1/features/steps/
--rw-rw-r--   0 kas       (1000) kas       (1000)     3317 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/action.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    11392 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/axis.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1018 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/background.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6013 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/category.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13879 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/chartdata.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2114 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/color.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2756 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/coreprops.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8097 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/datalabel.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1173 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/effect.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5143 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/fill.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4980 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/font.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3371 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/font_color.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1523 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/helpers.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3144 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/legend.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3245 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/line.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2803 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/picture.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    11179 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/placeholder.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4809 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/plot.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6035 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/presentation.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    12340 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/series.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    22389 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/shape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    12099 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/shapes.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7570 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4644 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/slides.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10292 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/table.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.734498 python-pptx-fix-0.6.21.1/features/steps/test_files/
--rw-rw-r--   0 kas       (1000) kas       (1000)     9454 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/72-dpi.tiff
--rw-rw-r--   0 kas       (1000) kas       (1000)     1526 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/CVS_LOGO.WMF
--rw-rw-r--   0 kas       (1000) kas       (1000)   982098 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/act-props.pptm
--rw-rw-r--   0 kas       (1000) kas       (1000)   867288 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/calibriz.ttf
--rw-rw-r--   0 kas       (1000) kas       (1000)   366536 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-axis-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   222711 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-category-access.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   218303 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-chart-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)  1393564 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-chart-type.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    77751 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-charts.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   243765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-datalabels.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    62864 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-gridlines-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   145467 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-legend-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   125134 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-legend.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    78544 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-marker-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   214116 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-plot-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   145108 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-point-access.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   144812 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-point-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   323685 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-replace-data.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   518464 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-series.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   127056 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/cht-ticklabels-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    21620 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/dml-effect.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   778084 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/dml-fill.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    27246 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/dml-line.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    21457 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/ext-rels.pptx
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.734498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/
--rw-rw-r--   0 kas       (1000) kas       (1000)     3332 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/[Content_Types].xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.734498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      751 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/_rels/.rels
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.738498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/
--rw-rw-r--   0 kas       (1000) kas       (1000)     1356 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/app.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)      765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/core.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     8147 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.738498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.738498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)     1160 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      692 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/presProps.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4000 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/presentation.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.742498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/
--rw-rw-r--   0 kas       (1000) kas       (1000)     9395 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.746498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.750498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)     7176 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4616 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4954 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4561 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7312 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7811 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    12024 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     3198 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     2607 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7768 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7325 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.754498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.754498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)     2028 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)    17336 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.754498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slides/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.754498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)     2128 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)      182 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.754498 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/theme/
--rw-rw-r--   0 kas       (1000) kas       (1000)    10013 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     1022 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    25061 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/font-color.pptx
--rwxrwxr-x   0 kas       (1000) kas       (1000)   470987 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/just-two-mice.mp4
--rw-rw-r--   0 kas       (1000) kas       (1000)   179346 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/just-two-mice.png
--rw-rw-r--   0 kas       (1000) kas       (1000)    23202 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/lyt-shapes.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    15802 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/minimal.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    64276 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/monty-truth.png
--rw-rw-r--   0 kas       (1000) kas       (1000)    25251 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/mst-placeholders.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    25539 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/mst-shapes.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    21166 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/mst-slide-layouts.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    23566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/ph-inherit-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   172254 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/ph-populated-placeholders.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    34405 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/ph-unpopulated-placeholders.pptx
--rwxrwxr-x   0 kas       (1000) kas       (1000)    49704 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/pic.emf
--rw-rw-r--   0 kas       (1000) kas       (1000)    19655 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/prs-add-slide.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    86792 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/prs-notes.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    15806 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/prs-properties.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    21528 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/prs-slide-masters.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     3277 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/python-icon.jpeg
--rw-rw-r--   0 kas       (1000) kas       (1000)     6111 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/python-powered.png
--rw-rw-r--   0 kas       (1000) kas       (1000)    45210 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/python.bmp
--rw-rw-r--   0 kas       (1000) kas       (1000)    80038 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-access-chart.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   119022 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-access-ole-object.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    17626 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-autoshape-adjustments.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    22929 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-autoshape-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    81639 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-common-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    22899 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-connector-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    11680 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-docx.docx
--rw-rw-r--   0 kas       (1000) kas       (1000)    29214 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-pptx.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     8250 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-xlsx.xlsx
--rw-rw-r--   0 kas       (1000) kas       (1000)    16704 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-freeform.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    23786 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-groupshape.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   684874 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-movie-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    91730 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-picture.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    94116 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-pos-and-size.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   125205 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/shp-shapes.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    17676 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sld-background.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    16703 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sld-blank.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    22964 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sld-notes.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    18894 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sld-slide.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    18478 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sld-slides.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    33273 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/sonic.gif
--rw-rw-r--   0 kas       (1000) kas       (1000)    28247 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/tbl-cell.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    37859 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/test.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    21337 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-fit-text.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    18874 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-font-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    25817 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-font-typeface.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    24620 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-paragraph-spacing.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    27659 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-text-frame.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    16051 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/test_files/txt-text.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     8264 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/text.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4615 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/steps/text_frame.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3549 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/tbl-cell.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/tbl-column.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1565 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/tbl-table.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      471 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-fit-text.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     1733 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-font-color.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     4945 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-font-props.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     3969 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-paragraph.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)      734 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-text.feature
--rw-rw-r--   0 kas       (1000) kas       (1000)     2371 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/features/txt-textframe.feature
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.758498 python-pptx-fix-0.6.21.1/pptx/
--rw-rw-r--   0 kas       (1000) kas       (1000)     1974 2023-07-25 07:29:02.000000 python-pptx-fix-0.6.21.1/pptx/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8672 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/action.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1593 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/api.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.762498 python-pptx-fix-0.6.21.1/pptx/chart/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    17304 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/axis.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7250 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/category.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9999 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    29740 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/data.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9528 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/datalabel.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/legend.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2130 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/marker.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13213 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/plot.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2797 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/point.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7484 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/series.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10942 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/xlsx.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    67673 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/chart/xmlwriter.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.766498 python-pptx-fix-0.6.21.1/pptx/compat/
--rw-rw-r--   0 kas       (1000) kas       (1000)      727 2023-07-25 06:18:02.000000 python-pptx-fix-0.6.21.1/pptx/compat/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1302 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/compat/python2.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      920 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/compat/python3.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.766498 python-pptx-fix-0.6.21.1/pptx/dml/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1373 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/chtfmt.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9124 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/color.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1592 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/effect.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13237 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/fill.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3108 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/dml/line.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.770498 python-pptx-fix-0.6.21.1/pptx/enum/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1548 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/action.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10697 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/base.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13226 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    11940 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/dml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    22808 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/lang.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    31458 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/shapes.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8215 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/enum/text.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      457 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/exc.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10532 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/media.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.774498 python-pptx-fix-0.6.21.1/pptx/opc/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    19950 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/constants.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4514 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/oxml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    26976 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/package.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3880 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/packuri.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9969 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/serialized.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      692 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/shared.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1012 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/opc/spec.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.778498 python-pptx-fix-0.6.21.1/pptx/oxml/
--rw-rw-r--   0 kas       (1000) kas       (1000)    15446 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1604 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/action.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.786498 python-pptx-fix-0.6.21.1/pptx/oxml/chart/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9428 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/axis.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8190 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/datalabel.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2129 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/legend.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1838 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/marker.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9224 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/plot.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7625 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/series.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6097 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/chart/shared.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9820 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/coreprops.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.790498 python-pptx-fix-0.6.21.1/pptx/oxml/dml/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/dml/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2477 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/dml/color.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5981 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/dml/fill.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      446 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/dml/line.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4670 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/ns.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2795 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/presentation.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.790498 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13400 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/autoshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3518 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/connector.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    12053 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/graphfrm.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9214 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/groupshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8096 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/picture.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    12696 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/shapes/shared.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    19929 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/simpletypes.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10213 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    18277 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/table.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    16439 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/text.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      754 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/theme.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    25027 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/oxml/xmlchemy.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7626 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/package.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.794498 python-pptx-fix-0.6.21.1/pptx/parts/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3000 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4052 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/coreprops.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2815 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/embeddedpackage.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9038 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/image.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      901 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/media.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4477 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/presentation.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10432 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/parts/slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/presentation.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.802498 python-pptx-fix-0.6.21.1/pptx/shapes/
--rw-rw-r--   0 kas       (1000) kas       (1000)      589 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13710 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/autoshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7574 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/base.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10063 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/connector.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10933 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/freeform.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5005 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/graphfrm.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1859 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/group.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6637 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/picture.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    14539 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/placeholder.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    41368 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shapes/shapetree.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2593 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/shared.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    17890 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    23582 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/spec.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    16275 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/table.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.806498 python-pptx-fix-0.6.21.1/pptx/templates/
--rw-rw-r--   0 kas       (1000) kas       (1000)    34030 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/default.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)   127228 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/docx-icon.emf
--rw-rw-r--   0 kas       (1000) kas       (1000)     5396 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/generic-icon.emf
--rw-rw-r--   0 kas       (1000) kas       (1000)      722 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/notes.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    11135 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/notesMaster.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     5492 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/pptx-icon.emf
--rw-rw-r--   0 kas       (1000) kas       (1000)    10964 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/theme.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)   130380 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/templates/xlsx-icon.emf
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.810499 python-pptx-fix-0.6.21.1/pptx/text/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/text/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    12900 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/text/fonts.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9959 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/text/layout.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    25179 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/text/text.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7826 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.1/pptx/util.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.810499 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/
--rw-rw-r--   0 kas       (1000) kas       (1000)    19225 2023-07-25 08:35:20.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/PKG-INFO
--rw-rw-r--   0 kas       (1000) kas       (1000)    18712 2023-07-25 08:35:20.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/SOURCES.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)        1 2023-07-25 08:35:20.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/dependency_links.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)        1 2023-07-25 07:57:07.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/not-zip-safe
--rw-rw-r--   0 kas       (1000) kas       (1000)       44 2023-07-25 08:35:20.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/requires.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)        5 2023-07-25 08:35:20.000000 python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/top_level.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)       38 2023-07-25 08:35:20.914500 python-pptx-fix-0.6.21.1/setup.cfg
--rwxrwxr-x   0 kas       (1000) kas       (1000)     2786 2023-07-25 07:31:00.000000 python-pptx-fix-0.6.21.1/setup.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.822499 python-pptx-fix-0.6.21.1/tests/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/__init__.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.826499 python-pptx-fix-0.6.21.1/tests/chart/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    48371 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_axis.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9346 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_category.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    21201 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    34116 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_data.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    26214 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_datalabel.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6797 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_legend.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4827 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_marker.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    18769 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_plot.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7659 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_point.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    19055 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_series.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    15936 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_xlsx.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    28442 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/chart/test_xmlwriter.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.830499 python-pptx-fix-0.6.21.1/tests/dml/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3235 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/test_chtfmt.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    11638 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/test_color.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1923 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/test_effect.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    25636 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/test_fill.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5963 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/dml/test_line.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.830499 python-pptx-fix-0.6.21.1/tests/opc/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6460 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/test_oxml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    38342 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/test_package.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2976 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/test_packuri.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    14807 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/test_serialized.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.834499 python-pptx-fix-0.6.21.1/tests/opc/unitdata/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/unitdata/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7480 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/opc/unitdata/rels.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.838499 python-pptx-fix-0.6.21.1/tests/oxml/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/__init__.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.842499 python-pptx-fix-0.6.21.1/tests/oxml/shapes/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/shapes/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10011 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_autoshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3383 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_graphfrm.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10820 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_groupshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3591 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_picture.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3204 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test___init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5059 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_dml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2669 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_ns.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1436 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_presentation.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8990 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_simpletypes.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      719 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10125 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_table.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      693 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_theme.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    20871 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/test_xmlchemy.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.846499 python-pptx-fix-0.6.21.1/tests/oxml/unitdata/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/unitdata/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1946 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/unitdata/dml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4060 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/unitdata/shape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1792 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/oxml/unitdata/text.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.850499 python-pptx-fix-0.6.21.1/tests/parts/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     5973 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_chart.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9096 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_coreprops.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3007 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_embeddedpackage.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     7799 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_image.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1185 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_media.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9156 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_presentation.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    22548 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/parts/test_slide.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.854499 python-pptx-fix-0.6.21.1/tests/shapes/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    18645 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_autoshape.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    19691 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_base.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    16235 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_connector.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    20589 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_freeform.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     6651 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_graphfrm.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2360 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_group.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    10621 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_picture.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    22431 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_placeholder.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    87112 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/shapes/test_shapetree.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13970 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_action.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1527 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_api.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3739 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_enum.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.866499 python-pptx-fix-0.6.21.1/tests/test_files/
--rw-rw-r--   0 kas       (1000) kas       (1000)   867288 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/calibriz.ttf
--rwxrwxr-x   0 kas       (1000) kas       (1000)    21818 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/cdw-logo.eps
--rw-rw-r--   0 kas       (1000) kas       (1000)       42 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/dummy.mp4
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.866499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/
--rw-rw-r--   0 kas       (1000) kas       (1000)     3359 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/[Content_Types].xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.866499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      758 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/_rels/.rels
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.866499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/
--rw-rw-r--   0 kas       (1000) kas       (1000)     1354 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/app.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)      750 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/core.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     8147 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.870499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.870499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)     1170 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      327 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/presProps.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4157 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/presentation.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.870499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/printerSettings/
--rw-rw-r--   0 kas       (1000) kas       (1000)     9395 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.874499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.878499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)     7473 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4783 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     5131 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     4786 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7613 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     8154 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    12501 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     3371 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     2757 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     8100 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     7633 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.878499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.882499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)     2093 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)    17871 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.882499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slides/
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.882499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slides/_rels/
--rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
--rw-rw-r--   0 kas       (1000) kas       (1000)     2198 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)      182 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/tableStyles.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.882499 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/theme/
--rw-rw-r--   0 kas       (1000) kas       (1000)    10294 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     1081 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/viewProps.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    15802 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/minimal.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)      477 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/minimal_slide.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)    32944 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/missing_rels_item.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    64276 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/monty-truth.png
--rw-rw-r--   0 kas       (1000) kas       (1000)    34436 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/no-core-props.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    34036 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/no-slides.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     4157 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/presentation.xml
--rw-rw-r--   0 kas       (1000) kas       (1000)     3277 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/python-icon.jpeg
--rw-rw-r--   0 kas       (1000) kas       (1000)     6111 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/python-powered.png
--rw-rw-r--   0 kas       (1000) kas       (1000)    45210 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/python.bmp
--rw-rw-r--   0 kas       (1000) kas       (1000)     8134 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/slideLayout1.xml
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.906500 python-pptx-fix-0.6.21.1/tests/test_files/snippets/
--rw-rw-r--   0 kas       (1000) kas       (1000)     4920 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-date.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4916 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-float.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4816 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-stacked-100.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4809 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-stacked.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4810 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4308 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered-date.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4246 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered-float.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4140 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4176 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-stacked-100.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4169 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-stacked.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4140 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-clustered.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4176 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-stacked-100.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4169 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-stacked.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4745 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-date.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4683 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-float.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4427 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4420 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers-stacked.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4421 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4583 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-stacked-100.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4576 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-stacked.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4577 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     6440 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-bubble-3d.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     6440 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-bubble.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     5082 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4926 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-lines.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     5084 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4928 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-smooth.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     5154 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     6102 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x5-radar.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     2107 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x1-pie-exploded.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     2073 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x1-pie.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4141 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x2-doughnut-exploded.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     4073 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x2-doughnut.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     5336 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/4x2-multi-cat-bar.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     3458 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/adjust-ser-count.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     3636 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/cat-labels.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      517 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/content-types-xml.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      666 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-notes.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)    11062 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-notesMaster.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)    10896 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-theme.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     1087 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/freeform.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      757 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/package-rels-xml.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     1763 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/placeholders.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      600 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/presentation-rels-xml.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      445 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/relationships.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)      622 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/rels-load-from-xml.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)    10545 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/rewrite-ser.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)     2792 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/snippets/timing.txt
--rw-rw-r--   0 kas       (1000) kas       (1000)    37859 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/test.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)    38616 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_files/test_slides.pptx
--rw-rw-r--   0 kas       (1000) kas       (1000)     4604 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_media.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    13510 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_package.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8925 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_presentation.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     2455 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_shared.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    39126 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_slide.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    29166 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_table.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1878 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/test_util.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.910500 python-pptx-fix-0.6.21.1/tests/text/
--rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/text/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    25213 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/text/test_fonts.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     9012 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/text/test_layout.py
--rw-rw-r--   0 kas       (1000) kas       (1000)    45716 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/text/test_text.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     3661 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/unitdata.py
-drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-25 08:35:20.910500 python-pptx-fix-0.6.21.1/tests/unitutil/
--rw-rw-r--   0 kas       (1000) kas       (1000)      247 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/unitutil/__init__.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     8312 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/unitutil/cxml.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     1855 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/unitutil/file.py
--rw-rw-r--   0 kas       (1000) kas       (1000)     4129 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.1/tests/unitutil/mock.py
--rw-rw-r--   0 kas       (1000) kas       (1000)      652 2023-07-25 05:29:49.000000 python-pptx-fix-0.6.21.1/tox.ini
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.883999 python-pptx-fix-0.6.21.2/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15898 2023-07-26 09:30:37.000000 python-pptx-fix-0.6.21.2/HISTORY.rst
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1104 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/LICENSE
+-rw-rw-r--   0 kas       (1000) kas       (1000)      177 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/MANIFEST.in
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19536 2023-07-26 10:14:43.883999 python-pptx-fix-0.6.21.2/PKG-INFO
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1392 2023-07-26 09:15:40.000000 python-pptx-fix-0.6.21.2/README.rst
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.619996 python-pptx-fix-0.6.21.2/features/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.619996 python-pptx-fix-0.6.21.2/features/_scratch/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    20086 2023-07-26 09:56:41.000000 python-pptx-fix-0.6.21.2/features/_scratch/test_out.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3215 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/act-action.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2045 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/act-hyperlink.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6389 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-axis-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1360 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-axistitle-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2059 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-category-access.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      569 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-category-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4227 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-chart.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1374 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-charttitle-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4641 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-data-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6935 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-datalabels.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      406 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-gridlines-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1034 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-legend-access.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3185 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-legend-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-marker-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4323 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-plot-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      945 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-point-access.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-point-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1471 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-replace-data.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4648 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-series.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      972 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/cht-ticklabels-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      687 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/dml-color.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1018 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/dml-effect.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3098 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/dml-fill.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2163 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/dml-line.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      518 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/environment.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1602 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/ph-inherit-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1391 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/ph-insert-shape.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      815 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/ph-phfmt-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1427 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/ph-placeholder-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      992 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/prs-coreprops.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      466 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/prs-default-template.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1417 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/prs-open-save.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1134 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/prs-presentation-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      761 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-autoshape.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2720 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-connector.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2245 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-freeform.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1622 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-graphicframe.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1353 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-groupshape.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      568 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-movie-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2475 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-picture.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      612 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-placeholder.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)    14081 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-shapes.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6239 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/shp-shared.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      488 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/sld-background.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4081 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/sld-slide.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2339 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/sld-slides.feature
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.627996 python-pptx-fix-0.6.21.2/features/steps/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3317 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/action.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11392 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/axis.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1018 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/background.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6013 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/category.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13879 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/chartdata.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2114 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/color.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2756 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/coreprops.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8097 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/datalabel.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1173 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/effect.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5143 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/fill.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4980 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/font.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3371 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/font_color.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1523 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/helpers.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3144 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/legend.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3245 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/line.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2803 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/picture.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11179 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/placeholder.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4809 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/plot.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6035 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/presentation.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12340 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/series.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22389 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/shape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12099 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/shapes.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7570 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4644 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/slides.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10292 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/table.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.699997 python-pptx-fix-0.6.21.2/features/steps/test_files/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9454 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/72-dpi.tiff
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1526 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/CVS_LOGO.WMF
+-rw-rw-r--   0 kas       (1000) kas       (1000)   982098 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/act-props.pptm
+-rw-rw-r--   0 kas       (1000) kas       (1000)   867288 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/calibriz.ttf
+-rw-rw-r--   0 kas       (1000) kas       (1000)   366536 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-axis-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   222711 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-category-access.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   218303 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-chart-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)  1393564 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-chart-type.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    77751 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-charts.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   243765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-datalabels.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    62864 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-gridlines-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   145467 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-legend-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   125134 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-legend.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    78544 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-marker-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   214116 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-plot-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   145108 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-point-access.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   144812 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-point-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   323685 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-replace-data.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   518464 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-series.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   127056 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/cht-ticklabels-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21620 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/dml-effect.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   778084 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/dml-fill.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    27246 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/dml-line.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21457 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/ext-rels.pptx
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.699997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3332 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/[Content_Types].xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.699997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      751 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/_rels/.rels
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.703997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1356 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/app.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)      765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/core.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8147 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.703997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.703997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1160 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      692 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/presProps.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4000 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/presentation.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.707997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9395 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.711997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.715997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7176 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4616 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4954 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4561 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7312 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7811 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12024 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3198 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2607 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7768 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7325 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.715997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.719997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2028 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17336 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.719997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slides/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.719997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2128 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)      182 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.719997 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/theme/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10013 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1022 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25061 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/font-color.pptx
+-rwxrwxr-x   0 kas       (1000) kas       (1000)   470987 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/just-two-mice.mp4
+-rw-rw-r--   0 kas       (1000) kas       (1000)   179346 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/just-two-mice.png
+-rw-rw-r--   0 kas       (1000) kas       (1000)    23202 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/lyt-shapes.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15802 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/minimal.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    64276 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/monty-truth.png
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25251 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/mst-placeholders.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25539 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/mst-shapes.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21166 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/mst-slide-layouts.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    23566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/ph-inherit-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   172254 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/ph-populated-placeholders.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    34405 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/ph-unpopulated-placeholders.pptx
+-rwxrwxr-x   0 kas       (1000) kas       (1000)    49704 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/pic.emf
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19655 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/prs-add-slide.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    86792 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/prs-notes.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15806 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/prs-properties.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21528 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/prs-slide-masters.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3277 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/python-icon.jpeg
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6111 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/python-powered.png
+-rw-rw-r--   0 kas       (1000) kas       (1000)    45210 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/python.bmp
+-rw-rw-r--   0 kas       (1000) kas       (1000)    80038 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-access-chart.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   119022 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-access-ole-object.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17626 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-autoshape-adjustments.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22929 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-autoshape-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    81639 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-common-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22899 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-connector-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11680 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-docx.docx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    29214 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-pptx.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8250 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-xlsx.xlsx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16704 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-freeform.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    23786 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-groupshape.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   684874 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-movie-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    91730 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-picture.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    94116 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-pos-and-size.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   125205 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/shp-shapes.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17676 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sld-background.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16703 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sld-blank.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22964 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sld-notes.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18894 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sld-slide.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18478 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sld-slides.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    33273 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/sonic.gif
+-rw-rw-r--   0 kas       (1000) kas       (1000)    28247 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/tbl-cell.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    37859 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/test.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21337 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-fit-text.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18874 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-font-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25817 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-font-typeface.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    24620 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-paragraph-spacing.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    27659 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-text-frame.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16051 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/test_files/txt-text.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8264 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/text.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4615 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/steps/text_frame.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3549 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/tbl-cell.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/tbl-column.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1565 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/tbl-table.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      471 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-fit-text.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1733 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-font-color.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4945 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-font-props.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3969 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-paragraph.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)      734 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-text.feature
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2371 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/features/txt-textframe.feature
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.723997 python-pptx-fix-0.6.21.2/pptx/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1974 2023-07-26 08:48:03.000000 python-pptx-fix-0.6.21.2/pptx/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8672 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/action.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1593 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/api.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.731997 python-pptx-fix-0.6.21.2/pptx/chart/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17304 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/axis.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7250 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/category.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9999 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    29740 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/data.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9528 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/datalabel.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2566 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/legend.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2130 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/marker.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13213 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/plot.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2797 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/point.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7484 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/series.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10942 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/xlsx.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    67673 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/chart/xmlwriter.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.735997 python-pptx-fix-0.6.21.2/pptx/compat/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      727 2023-07-25 10:30:39.000000 python-pptx-fix-0.6.21.2/pptx/compat/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1302 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/compat/python2.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      920 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/compat/python3.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.739997 python-pptx-fix-0.6.21.2/pptx/dml/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1373 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/chtfmt.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9124 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/color.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1592 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/effect.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13237 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/fill.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3108 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/dml/line.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.743997 python-pptx-fix-0.6.21.2/pptx/enum/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1548 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/action.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10697 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/base.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13226 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11940 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/dml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22808 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/lang.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    31458 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/shapes.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8215 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/enum/text.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      457 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/exc.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10532 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/media.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.747997 python-pptx-fix-0.6.21.2/pptx/opc/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19950 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/constants.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4514 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/oxml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    26976 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/package.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3880 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/packuri.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9969 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/serialized.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      692 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/shared.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1012 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/opc/spec.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.751997 python-pptx-fix-0.6.21.2/pptx/oxml/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15446 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1604 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/action.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.755997 python-pptx-fix-0.6.21.2/pptx/oxml/chart/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9428 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/axis.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8190 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7765 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/datalabel.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2129 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/legend.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1838 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/marker.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9224 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/plot.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7625 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/series.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6097 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/chart/shared.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9820 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/coreprops.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.759997 python-pptx-fix-0.6.21.2/pptx/oxml/dml/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/dml/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2477 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/dml/color.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5981 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/dml/fill.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      446 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/dml/line.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4670 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/ns.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2795 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/presentation.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.759997 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13400 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/autoshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3518 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/connector.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12053 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/graphfrm.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9214 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/groupshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8096 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/picture.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12696 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/shapes/shared.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19929 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/simpletypes.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10213 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18277 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/table.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16439 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/text.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      754 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/theme.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25027 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/oxml/xmlchemy.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7626 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/package.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.763997 python-pptx-fix-0.6.21.2/pptx/parts/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3000 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4052 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/coreprops.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2815 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/embeddedpackage.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9038 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/image.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      901 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/media.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4477 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/presentation.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10432 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/parts/slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3343 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/presentation.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.767998 python-pptx-fix-0.6.21.2/pptx/shapes/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      589 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13710 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/autoshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7574 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/base.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10063 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/connector.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10933 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/freeform.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5005 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/graphfrm.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1859 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/group.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6637 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/picture.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    14539 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/placeholder.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    41368 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shapes/shapetree.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2593 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/shared.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17890 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    23582 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/spec.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16275 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/table.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.771998 python-pptx-fix-0.6.21.2/pptx/templates/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    34030 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/default.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)   127228 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/docx-icon.emf
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5396 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/generic-icon.emf
+-rw-rw-r--   0 kas       (1000) kas       (1000)      722 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/notes.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11135 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/notesMaster.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5492 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/pptx-icon.emf
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10964 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/theme.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)   130380 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/templates/xlsx-icon.emf
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.775998 python-pptx-fix-0.6.21.2/pptx/text/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/text/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12900 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/text/fonts.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10251 2023-07-26 06:14:52.000000 python-pptx-fix-0.6.21.2/pptx/text/layout.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25179 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/text/text.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7826 2023-07-24 07:00:38.000000 python-pptx-fix-0.6.21.2/pptx/util.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.779998 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19536 2023-07-26 10:14:43.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/PKG-INFO
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18712 2023-07-26 10:14:43.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/SOURCES.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)        1 2023-07-26 10:14:43.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/dependency_links.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)        1 2023-07-25 07:57:07.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/not-zip-safe
+-rw-rw-r--   0 kas       (1000) kas       (1000)       44 2023-07-26 10:14:43.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/requires.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)        5 2023-07-26 10:14:43.000000 python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/top_level.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)       38 2023-07-26 10:14:43.883999 python-pptx-fix-0.6.21.2/setup.cfg
+-rwxrwxr-x   0 kas       (1000) kas       (1000)     2789 2023-07-26 08:22:33.000000 python-pptx-fix-0.6.21.2/setup.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.783998 python-pptx-fix-0.6.21.2/tests/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/__init__.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.791998 python-pptx-fix-0.6.21.2/tests/chart/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    48371 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_axis.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9346 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_category.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    21201 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    34116 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_data.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    26214 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_datalabel.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6797 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_legend.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4827 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_marker.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18769 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_plot.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7659 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_point.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19055 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_series.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15936 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_xlsx.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    28442 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/chart/test_xmlwriter.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.795998 python-pptx-fix-0.6.21.2/tests/dml/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3235 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/test_chtfmt.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11638 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/test_color.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1923 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/test_effect.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25636 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/test_fill.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5963 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/dml/test_line.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.795998 python-pptx-fix-0.6.21.2/tests/opc/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6460 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/test_oxml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    38342 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/test_package.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2976 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/test_packuri.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    14807 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/test_serialized.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.795998 python-pptx-fix-0.6.21.2/tests/opc/unitdata/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/unitdata/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7480 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/opc/unitdata/rels.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.803998 python-pptx-fix-0.6.21.2/tests/oxml/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/__init__.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.807998 python-pptx-fix-0.6.21.2/tests/oxml/shapes/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/shapes/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10011 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_autoshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3383 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_graphfrm.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10820 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_groupshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3591 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_picture.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3204 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test___init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5059 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_dml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2669 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_ns.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1436 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_presentation.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8990 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_simpletypes.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      719 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10125 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_table.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      693 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_theme.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    20871 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/test_xmlchemy.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.807998 python-pptx-fix-0.6.21.2/tests/oxml/unitdata/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/unitdata/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1946 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/unitdata/dml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4060 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/unitdata/shape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1792 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/oxml/unitdata/text.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.811998 python-pptx-fix-0.6.21.2/tests/parts/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5973 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_chart.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9096 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_coreprops.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3007 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_embeddedpackage.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7799 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_image.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1185 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_media.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9156 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_presentation.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22548 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/parts/test_slide.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.815998 python-pptx-fix-0.6.21.2/tests/shapes/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    18645 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_autoshape.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    19691 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_base.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    16235 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_connector.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    20589 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_freeform.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6651 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_graphfrm.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2360 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_group.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10621 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_picture.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    22431 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_placeholder.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    87112 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/shapes/test_shapetree.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13970 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_action.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1527 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_api.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3739 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_enum.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.831998 python-pptx-fix-0.6.21.2/tests/test_files/
+-rw-rw-r--   0 kas       (1000) kas       (1000)   867288 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/calibriz.ttf
+-rwxrwxr-x   0 kas       (1000) kas       (1000)    21818 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/cdw-logo.eps
+-rw-rw-r--   0 kas       (1000) kas       (1000)       42 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/dummy.mp4
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.831998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3359 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/[Content_Types].xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.831998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      758 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/_rels/.rels
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.835998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1354 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/app.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)      750 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/core.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8147 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.835998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.835998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1170 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      327 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/presProps.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4157 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/presentation.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.835998 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/printerSettings/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9395 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.843999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.847999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)      319 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7473 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4783 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5131 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4786 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7613 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8154 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    12501 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3371 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2757 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8100 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     7633 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.847999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.847999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2093 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)    17871 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.847999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slides/
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.847999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slides/_rels/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      315 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2198 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)      182 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/tableStyles.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.851999 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/theme/
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10294 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1081 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/viewProps.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    15802 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/minimal.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)      477 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/minimal_slide.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)    32944 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/missing_rels_item.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    64276 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/monty-truth.png
+-rw-rw-r--   0 kas       (1000) kas       (1000)    34436 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/no-core-props.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    34036 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/no-slides.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4157 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/presentation.xml
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3277 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/python-icon.jpeg
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6111 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/python-powered.png
+-rw-rw-r--   0 kas       (1000) kas       (1000)    45210 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/python.bmp
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8134 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/slideLayout1.xml
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.879999 python-pptx-fix-0.6.21.2/tests/test_files/snippets/
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4920 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-date.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4916 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-float.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4816 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-stacked-100.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4809 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-stacked.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4810 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4308 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered-date.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4246 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered-float.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4140 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4176 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-stacked-100.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4169 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-stacked.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4140 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-clustered.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4176 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-stacked-100.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4169 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-stacked.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4745 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-date.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4683 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-float.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4427 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4420 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers-stacked.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4421 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4583 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-stacked-100.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4576 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-stacked.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4577 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6440 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-bubble-3d.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6440 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-bubble.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5082 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4926 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-lines.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5084 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4928 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-smooth.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5154 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     6102 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x5-radar.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2107 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x1-pie-exploded.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2073 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x1-pie.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4141 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x2-doughnut-exploded.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4073 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x2-doughnut.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     5336 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/4x2-multi-cat-bar.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3458 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/adjust-ser-count.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3636 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/cat-labels.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      517 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/content-types-xml.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      666 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-notes.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)    11062 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-notesMaster.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10896 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-theme.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1087 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/freeform.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      757 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/package-rels-xml.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1763 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/placeholders.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      600 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/presentation-rels-xml.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      445 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/relationships.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)      622 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/rels-load-from-xml.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)    10545 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/rewrite-ser.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2792 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/snippets/timing.txt
+-rw-rw-r--   0 kas       (1000) kas       (1000)    37859 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/test.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)    38616 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_files/test_slides.pptx
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4604 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_media.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    13510 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_package.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8925 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_presentation.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     2455 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_shared.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    39126 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_slide.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    29166 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_table.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1878 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/test_util.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.883999 python-pptx-fix-0.6.21.2/tests/text/
+-rw-rw-r--   0 kas       (1000) kas       (1000)        0 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/text/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    25213 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/text/test_fonts.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     9012 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/text/test_layout.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)    45716 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/text/test_text.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     3661 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/unitdata.py
+drwxrwxr-x   0 kas       (1000) kas       (1000)        0 2023-07-26 10:14:43.883999 python-pptx-fix-0.6.21.2/tests/unitutil/
+-rw-rw-r--   0 kas       (1000) kas       (1000)      247 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/unitutil/__init__.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     8312 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/unitutil/cxml.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     1855 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/unitutil/file.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)     4129 2023-07-24 07:00:39.000000 python-pptx-fix-0.6.21.2/tests/unitutil/mock.py
+-rw-rw-r--   0 kas       (1000) kas       (1000)      659 2023-07-26 07:00:30.000000 python-pptx-fix-0.6.21.2/tox.ini
```

### Comparing `python-pptx-fix-0.6.21.1/HISTORY.rst` & `python-pptx-fix-0.6.21.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 .. :changelog:
 
 Release History
 ---------------
 
 
+0.6.21.2 (2023-07-26)
++++++++++++++++++++++
+
+- Fix #3 handled removal of getsize() api in pillow 10
+- setup.py updated for twine upload to pypi
+- requirements.txt updated with sphinx tox virtualenv tox
+- tox.ini update with py310 in envlist
+
+
+
 0.6.21.1 (2023-07-25)
 +++++++++++++++++++++
 
 - Fix #1 Handling errors related to collections.abc
 - Fix #878 #762 #770 #820 #834 of https://github.com/scanny/python-pptx/issues
```

### Comparing `python-pptx-fix-0.6.21.1/LICENSE` & `python-pptx-fix-0.6.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/PKG-INFO` & `python-pptx-fix-0.6.21.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pptx-fix
-Version: 0.6.21.1
+Version: 0.6.21.2
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/kascodeo/python-pptx
 Author: Steve Canny
 Author-email: python-pptx@googlegroups.com
 Maintainer: Karim
 Maintainer-email: kascodeo@gmail.com
 License: The MIT License (MIT)
@@ -33,28 +33,29 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 .. image:: https://travis-ci.org/scanny/python-pptx.svg?branch=master
    :target: https://travis-ci.org/scanny/python-pptx
 
 *python-pptx-fix* is a Python library for creating and updating PowerPoint (.pptx)
 files.
 
-This project is created to fix bugs and add minor features to the original project 
-by Scanny at https://github.com/scanny/python-pptx. Original project is 
+This project `python-pptx-fix <https://github.com/kascodeo/python-pptx>`_ is 
+created to fix bugs and add minor features to the original project 
+by `Scanny <https://github.com/scanny/python-pptx>`_. Original project is 
 unresponsive at the moment so had to create this project as *python-pptx-fix*. 
 Feel free to contribute to this project.
 
 
 A typical use would be generating a customized PowerPoint presentation from
 database content, downloadable by clicking a link in a web application.
 Several developers have used it to automate production of presentation-ready
@@ -77,14 +78,24 @@
 
 .. :changelog:
 
 Release History
 ---------------
 
 
+0.6.21.2 (2023-07-26)
++++++++++++++++++++++
+
+- Fix #3 handled removal of getsize() api in pillow 10
+- setup.py updated for twine upload to pypi
+- requirements.txt updated with sphinx tox virtualenv tox
+- tox.ini update with py310 in envlist
+
+
+
 0.6.21.1 (2023-07-25)
 +++++++++++++++++++++
 
 - Fix #1 Handling errors related to collections.abc
 - Fix #878 #762 #770 #820 #834 of https://github.com/scanny/python-pptx/issues
```

### Comparing `python-pptx-fix-0.6.21.1/README.rst` & `python-pptx-fix-0.6.21.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .. image:: https://travis-ci.org/scanny/python-pptx.svg?branch=master
    :target: https://travis-ci.org/scanny/python-pptx
 
 *python-pptx-fix* is a Python library for creating and updating PowerPoint (.pptx)
 files.
 
-This project is created to fix bugs and add minor features to the original project 
-by Scanny at https://github.com/scanny/python-pptx. Original project is 
+This project `python-pptx-fix <https://github.com/kascodeo/python-pptx>`_ is 
+created to fix bugs and add minor features to the original project 
+by `Scanny <https://github.com/scanny/python-pptx>`_. Original project is 
 unresponsive at the moment so had to create this project as *python-pptx-fix*. 
 Feel free to contribute to this project.
 
 
 A typical use would be generating a customized PowerPoint presentation from
 database content, downloadable by clicking a link in a web application.
 Several developers have used it to automate production of presentation-ready
```

### Comparing `python-pptx-fix-0.6.21.1/features/_scratch/test_out.pptx` & `python-pptx-fix-0.6.21.2/features/_scratch/test_out.pptx`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 936a f956 6531  PK.........j.Ve1
+00000000: 504b 0304 1400 0000 0800 547b fa56 6531  PK........T{.Ve1
 00000010: 0cc8 8e01 0000 f006 0000 1300 0000 5b43  ..............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6cb5 95cb 6ec2 3010 45f7 fd8a 289b 2c2a  l...n.0.E...(.,*
 00000040: 62e8 a2aa 2a02 8b3e 567d 2041 3fc0 2403  b...*..>V} A?.$.
 00000050: b875 6ccb 3350 f8fb 4e42 4088 0201 019b  .ul.3P..NB@.....
 00000060: 44f6 ccdc 7b3c b693 7677 9eeb 6006 1e95  D...{<..vw..`...
 00000070: 3549 d48a 9b51 0026 b599 32e3 24fa 1abc  5I...Q.&..2.$...
@@ -22,15 +22,15 @@
 00000150: 74f3 558f 8aea 231d 9d23 51ec 7a69 7bf6  t.U...#..#Q.zi{.
 00000160: 72ff 9d9f 4af8 1882 55dd 3520 d6da b954  r...J...U.5 ...T
 00000170: a60e 0635 4fbe c985 9d12 6e0e 5a97 26db  ...5O.....n.Z.&.
 00000180: d03e 8ae9 5d22 df46 dc1c 5c87 69a9 7d14  .>..]".F..\.i.}.
 00000190: 5345 731d 8e3a 0292 430d 7d5a 68b8 f8d1  SEs..:..C.}Zh...
 000001a0: dd90 aea5 e0cf 372c 9fe7 b7a1 94a9 739c  ......7,......s.
 000001b0: 29f8 bdca 855d 0baf 0844 f9c3 eafc 0150  )....]...D.....P
-000001c0: 4b03 0414 0000 0008 0093 6af9 56f1 0d37  K.........j.V..7
+000001c0: 4b03 0414 0000 0008 0054 7bfa 56f1 0d37  K........T{.V..7
 000001d0: ec00 0100 00e1 0200 000b 0000 005f 7265  ............._re
 000001e0: 6c73 2f2e 7265 6c73 ad92 cf4e 0321 1087  ls/.rels...N.!..
 000001f0: ef3e 05d9 0ba7 2edb 6a8c 3165 7b31 26bd  .>......j.1e{1&.
 00000200: 1953 1f60 84e9 2e75 8109 4c4d fbf6 a289  .S.`...u..LM....
 00000210: 7f6a b64d 0f3d c2fc f8e6 1b60 bed8 f941  .j.M.=.....`...A
 00000220: bc63 ca2e 062d a775 2305 0613 ad0b 9d96  .c...-.u#.......
 00000230: 2fab c7c9 9d14 9921 5818 6240 2df7 98e5  /......!X.b@-...
@@ -41,15 +41,15 @@
 00000280: 8eeb b533 f810 cdd6 63e0 9116 ff12 850c  ...3....c.......
 00000290: a943 d615 112b 4a98 cbe6 57ba 2ee4 4a8d  .C...+J...W...J.
 000002a0: 0bcd ce17 3a3e acf2 c860 8141 71bf f5af  ....:>...`.Aq...
 000002b0: 01dc f06b 63a3 794a b184 7e6a f586 b03b  ...kc.yJ..~j...;
 000002c0: 2674 7d59 2113 134e a8f4 c7c4 0ef3 88d6  &t}Y!..N........
 000002d0: 67e2 d40d dd5c f2c9 70c7 182c dad3 4a40  g....\..p..,..J@
 000002e0: f46d a40e 7e66 fb01 504b 0304 1400 0000  .m..~f..PK......
-000002f0: 0800 936a f956 76bc 49cc 2c02 0000 9b0c  ...j.Vv.I.,.....
+000002f0: 0800 547b fa56 76bc 49cc 2c02 0000 9b0c  ..T{.Vv.I.,.....
 00000300: 0000 1400 0000 7070 742f 7072 6573 656e  ......ppt/presen
 00000310: 7461 7469 6f6e 2e78 6d6c ed97 db6a e330  tation.xml...j.0
 00000320: 1086 eff7 2984 6e7c b1a4 3ec6 764d 94c2  ....).n|..>.vM..
 00000330: ee12 58e8 4268 d207 50ed 4962 2acb 4652  ..X.Bh..P.Ib*.FR
 00000340: b249 9f7e 2547 3e24 65a1 0fe0 3b49 f3cf  .I.~%G>$e...;I..
 00000350: 3fa3 4f42 d88b a773 c5d0 0984 2c6b 4e1c  ?.OB...s....,kN.
 00000360: ffc1 7310 f0bc 2e4a be27 ceeb 7635 4b1d  ..s....J.'..v5K.
@@ -79,15 +79,15 @@
 000004e0: 2c9a 6040 13cd 13d3 f0c4 a785 62f9 8403  ,.`@........b...
 000004f0: 9f0e c2c4 271c f844 031f 3f4c fc78 02d4  ....'..D..?L.x..
 00000500: 51b1 80e6 2340 6990 a613 a08e 8a05 140f  Q...#@i.........
 00000510: 8082 208d bd09 5047 c502 4a46 8092 289c  .. ...PG..JF..(.
 00000520: dee8 9e8a 0594 0e80 0c9d e991 eea9 5840  ..............X@
 00000530: 8f23 40f1 3c99 1ee9 9e4a fb25 fbf9 13d3  .#@.<....J.%....
 00000540: bdfd a558 fe03 504b 0304 1400 0000 0800  ...X..PK........
-00000550: 936a f956 dd09 adf6 1b01 0000 7104 0000  .j.V........q...
+00000550: 547b fa56 dd09 adf6 1b01 0000 7104 0000  T{.V........q...
 00000560: 1f00 0000 7070 742f 5f72 656c 732f 7072  ....ppt/_rels/pr
 00000570: 6573 656e 7461 7469 6f6e 2e78 6d6c 2e72  esentation.xml.r
 00000580: 656c 73ad 94c1 4ec3 300c 86ef 3c45 944b  els...N.0...<E.K
 00000590: 4e34 ed80 81d0 d25d 10d2 0e48 888d 07c8  N4.....]...H....
 000005a0: 5ab7 8d48 9328 3183 be3d 110c 68ab 5171  Z..H.(1..=..h.Qq
 000005b0: e8d1 bfed 3f5f 1c2b abf5 7bab c901 7c50  ....?_.+..{...|P
 000005c0: d608 9625 2923 600a 5b2a 530b f6bc bb3f  ...%)#`.[*S....?
@@ -100,15 +100,15 @@
 00000630: 107c b495 be06 14b4 270e 2ab2 24fa 537e  .|......'.*.$.S~
 00000640: 1a6b 313b d608 e8a8 4e42 5ccc 09e1 bc32  .k1;....NB\....2
 00000650: f1d6 5b40 8c6f 1f7e 7146 8971 6196 ec95  ..[@.o.~qF.qa...
 00000660: f98b f072 5e42 088f deba 01db 519a 1ad3  ...r^B......Q...
 00000670: d59c 1007 056f 2388 1f69 0a62 3927 04c6  .....o#..i.b9'..
 00000680: dede c27c 865f e2e4 be5c cfca 20f7 1ab6  ...|._...\.. ...
 00000690: d869 e88d a227 7e83 f0c1 4f91 7f00 504b  .i...'~...O...PK
-000006a0: 0304 1400 0000 0800 936a f956 f3f6 6658  .........j.V..fX
+000006a0: 0304 1400 0000 0800 547b fa56 f3f6 6658  ........T{.V..fX
 000006b0: c903 0000 821e 0000 2100 0000 7070 742f  ........!...ppt/
 000006c0: 736c 6964 654d 6173 7465 7273 2f73 6c69  slideMasters/sli
 000006d0: 6465 4d61 7374 6572 312e 786d 6ced 99cd  deMaster1.xml...
 000006e0: 8edb 3610 80ef 7d0a 8117 1f82 8d24 ead7  ..6...}......$..
 000006f0: c66a 8326 edb6 0136 a911 6f1e 80a6 684b  .j.&...6..o...hK
 00000700: 5d8a 1228 dab5 73ca 3be4 0dfa 1abd e551  ]..(..s.;......Q
 00000710: f224 1d51 e24a ebf5 2e72 8881 d8f0 c51a  .$.Q.J...r......
@@ -165,15 +165,15 @@
 00000a40: 7aa3 d37b ea83 d2fa 2078 0731 768f a13a  z..{.... x.1v..:
 00000a50: da5f c9fa 4184 0f93 fec7 169f fdd5 a309  ._..A...........
 00000a60: c239 3e4f 146c 5ee4 1ee8 fc3c b600 ed2f  .9>O.l^....<.../
 00000a70: 92dc 18c7 f139 40cf 5426 fa0f f81c a0a7  .....9@.T&......
 00000a80: ab81 c8f7 ce67 f473 3770 70f7 7c48 3f77  .....g.s7pp.|H?w
 00000a90: eb0d 83e8 7c48 3fbc 690e 2f97 f6f0 4398  ....|H?.i./...C.
 00000aa0: 3df8 787c f53f 504b 0304 1400 0000 0800  =.x|.?PK........
-00000ab0: 936a f956 981a fe61 ce00 0000 bd01 0000  .j.V...a........
+00000ab0: 547b fa56 981a fe61 ce00 0000 bd01 0000  T{.V...a........
 00000ac0: 2c00 0000 7070 742f 736c 6964 654d 6173  ,...ppt/slideMas
 00000ad0: 7465 7273 2f5f 7265 6c73 2f73 6c69 6465  ters/_rels/slide
 00000ae0: 4d61 7374 6572 312e 786d 6c2e 7265 6c73  Master1.xml.rels
 00000af0: ad90 bf6a c330 10c6 f73c 85d0 a2a9 929d  ...j.0...<......
 00000b00: a194 1039 4b08 043a 95f4 010e e96c 8bd8  ...9K..:.....l..
 00000b10: 92d0 5d4a fdf6 152d 9418 3274 e872 707f  ..]J...-..2t.rp.
 00000b20: bedf f771 fbc3 e73c 890f 2c14 52b4 aad5  ...q...<..,.R...
@@ -182,15 +182,15 @@
 00000b50: 8d21 93a8 9048 568e cc79 670c b911 6720  .!...HV..yg...g 
 00000b60: 9d32 c6ba e953 9981 6b5b 0693 c15d 6140  .2...S..k[...]a@
 00000b70: b36d 9a67 53ee 19b2 5b31 c5d9 5b59 cebe  .m.gS...[1..[Y..
 00000b80: 95e2 b264 fc0b 3bf5 7d70 784c ee36 63e4  ...d..;.}pxL.6c.
 00000b90: 0716 86a6 e0f1 1596 74e3 8a85 3220 5ba9  ........t...2 [.
 00000ba0: f5fd 7c75 d4ea 6a21 cde3 64db ff4c c655  ..|u..j!..d..L.U
 00000bb0: 8bab 4cdf 939f fa1b c3ac bede 7d01 504b  ..L.........}.PK
-00000bc0: 0304 1400 0000 0800 936a f956 6cf3 2a37  .........j.Vl.*7
+00000bc0: 0304 1400 0000 0800 547b fa56 6cf3 2a37  ........T{.Vl.*7
 00000bd0: 3501 0000 6f02 0000 2100 0000 7070 742f  5...o...!...ppt/
 00000be0: 736c 6964 654c 6179 6f75 7473 2f73 6c69  slideLayouts/sli
 00000bf0: 6465 4c61 796f 7574 312e 786d 6c8d 52c9  deLayout1.xml.R.
 00000c00: 6ec3 2014 bcf7 2b10 179f 1a9c 1eaa ca8a  n. ...+.........
 00000c10: 13a9 eba5 6d22 25fd 008a 9f17 954d 0fe2  ....m"%......M..
 00000c20: da7f 5f8c 1d25 a972 c805 1ec3 ccbc 0516  .._..%.r........
 00000c30: ab4e 49d2 02ba c6e8 3c99 cfd2 8480 16a6  .NI.....<.......
@@ -205,15 +205,15 @@
 00000cc0: b220 9aab 003c 46c6 003a bb43 8021 d2ed  . ...<F..:.C.!..
 00000cd0: 1bda addd 60e4 7eb6 1b24 4d31 6827 0d65  ....`.~..$M1h'.e
 00000ce0: d3c5 4463 a328 06ec 9fbc 3a84 3ceb 4a54  ..Dc.(....:.<.JT
 00000cf0: c31e 4640 ba9c a694 f4c3 ca06 0c3a 4fc4  ..F@.........:O.
 00000d00: 088a 232a eaf5 05ae a85f 2eb0 d921 013b  ..#*....._...!.;
 00000d10: 49ca 8e6d b1b1 ed58 b9c4 0f6e d76d ac2a  I..m...X...n.m.*
 00000d20: 4cd6 033e 45c8 8697 1d7b 38a1 b093 9fb2  L..>E....{8.....
-00000d30: fc03 504b 0304 1400 0000 0800 936a f956  ..PK.........j.V
+00000d30: fc03 504b 0304 1400 0000 0800 547b fa56  ..PK........T{.V
 00000d40: 8065 e188 b700 0000 3601 0000 2c00 0000  .e......6...,...
 00000d50: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
 00000d60: 2f5f 7265 6c73 2f73 6c69 6465 4c61 796f  /_rels/slideLayo
 00000d70: 7574 312e 786d 6c2e 7265 6c73 8dcf bd0e  ut1.xml.rels....
 00000d80: c220 1007 f0dd a720 2c4c 42eb 608c 29ed  . ..... ,LB.`.).
 00000d90: 624c 1c5c 8c3e c005 ae2d b105 c2a1 d1b7  bL.\.>...-......
 00000da0: 97d1 260e 8ef7 f5fb e79a ee35 4fec 8989  ..&........5O...
@@ -221,15 +221,15 @@
 00000dc0: de09 4619 bc85 2978 d4e2 8d24 ba76 d55c  ..F...)x...$.v.\
 00000dd0: 7082 5c6e 6874 9158 413c 693e e61c f74a  p.\nht.XA<i>...J
 00000de0: 9119 7106 9221 a22f 933e a419 7229 d3a0  ..q..!./.>..r)..
 00000df0: 2298 3b0c a836 55b5 55e9 dbe0 edc2 6427  ".;..6U.U.....d'
 00000e00: ab79 3ad9 9ab3 eb3b e23f 76e8 7b67 f010  .y:....;.?v.{g..
 00000e10: cc63 469f 7f44 289a 9cc5 3350 c654 5848  .cF..D(...3P.TXH
 00000e20: 0366 cda5 fcee 2f96 6a59 22b8 6a1b b578  .f..../.jY".j..x
-00000e30: b7fd 0050 4b03 0414 0000 0008 0093 6af9  ...PK.........j.
+00000e30: b7fd 0050 4b03 0414 0000 0008 0054 7bfa  ...PK........T{.
 00000e40: 56f9 cf09 39b6 0500 005c 1b00 0014 0000  V...9....\......
 00000e50: 0070 7074 2f74 6865 6d65 2f74 6865 6d65  .ppt/theme/theme
 00000e60: 312e 786d 6ced 594d 8fd3 4618 be57 ea7f  1.xml.YM..F..W..
 00000e70: 18f9 0e8e 137b c9ae c8a2 4d36 8102 0bab  .....{....M6....
 00000e80: dd40 c571 624f ec21 638f 3533 d925 b70a  .@.qbO.!c.53.%..
 00000e90: 8e95 2a55 a555 2f95 7aeb a16a 8b04 522f  ..*U.U/.z..j..R/
 00000ea0: f4d7 6c4b d552 89bf d0d7 1f49 c6c9 64c9  ..lK.R.....I..d.
@@ -316,15 +316,15 @@
 000013b0: 8fda 140e 1f28 fb82 c64d 85cf e6f3 6d9f  .....(...M....m.
 000013c0: 1f40 f4d1 6ca2 4490 8817 9a65 f9cd 3607  .@..l.D....e..6.
 000013d0: a073 5333 2e63 f5df 8e51 f310 3457 c4fb  .sS3.c...Q..4W..
 000013e0: 3c87 4fcd d98d 15ce 3e5d dc9b 3bdb 33f8  <.O.....>]..;.3.
 000013f0: da3b ddd5 f672 89da da41 265f 2dfd 03c5  .;...r...A&_-...
 00001400: 07f7 41f6 2e1c 94c6 4cc9 e28d d203 386a  ..A.....L.....8j
 00001410: 76a6 ff1d 001f 7b4e bafd 2f50 4b03 0414  v.....{N../PK...
-00001420: 0000 0008 0093 6af9 56cf 2d86 045e 0300  ......j.V.-..^..
+00001420: 0000 0008 0054 7bfa 56cf 2d86 045e 0300  .....T{.V.-..^..
 00001430: 003d 0f00 0015 0000 0070 7074 2f73 6c69  .=.......ppt/sli
 00001440: 6465 732f 736c 6964 6531 2e78 6d6c ed97  des/slide1.xml..
 00001450: cd6e db38 10c7 effb 1484 80c2 2787 1249  .n.8........'..I
 00001460: 7dd8 a852 c46e 1d2c b0dd 064d fa00 2c45  }..R.n.,...M..,E
 00001470: dbc2 52a4 4032 8e83 62df 7d49 4a8a 1325  ..R.@2..b.}IJ..%
 00001480: 05bc a97b d96d 0e16 3d9c 19ce 3ff3 b3a4  ...{.m..=...?...
 00001490: 79fb 6edf 08b0 e3da d44a 9693 e42c 9e00  y.n......J...,..
@@ -373,30 +373,30 @@
 00001740: 9a92 f7b3 7c7a b1ca d2e9 caf3 b95c 1417  ....|z.......\..
 00001750: 4bfc e16f 3f6f 2564 ce34 0fa3 d8ef c348  K..o?o%d.4.....H
 00001760: e98c cfc6 b8a6 665a 19b5 b667 4c35 fd3c  ......fZ...gL5.<
 00001770: 085b 75c7 75ab ea30 1226 713f 5706 b549  .[u.u..0.&q?W..I
 00001780: e25e 7592 2229 3ad6 436d c335 540b 0fa3  .^u."):.Cm.5T...
 00001790: 1e13 fa23 6d3f ed42 5bdc 61ae 57cb 606a  ...#m?.B[.a.W.`j
 000017a0: ddcc da45 3f72 8161 fa3d ff07 504b 0304  ...E?r.a.=..PK..
-000017b0: 1400 0000 0800 936a f956 36e8 50cd b700  .......j.V6.P...
+000017b0: 1400 0000 0800 547b fa56 36e8 50cd b700  ......T{.V6.P...
 000017c0: 0000 3601 0000 2000 0000 7070 742f 736c  ..6... ...ppt/sl
 000017d0: 6964 6573 2f5f 7265 6c73 2f73 6c69 6465  ides/_rels/slide
 000017e0: 312e 786d 6c2e 7265 6c73 8dcf bd0a c230  1.xml.rels.....0
 000017f0: 1007 f0dd a708 5932 99b4 0e22 d2d4 4504  ......Y2..."..E.
 00001800: c149 f401 8ee4 da06 db24 e4a2 d8b7 37a3  .I.......$....7.
 00001810: 0507 c7fb fafd b9e6 f09e 46f6 c244 2e78  ..........F..D.x
 00001820: 2d6a 5909 86de 04eb 7caf c5fd 765a ef04  -jY.....|...vZ..
 00001830: a30c dec2 183c 6a31 2389 43bb 6aae 3842  .....<j1#.C.j.8B
 00001840: 2e37 34b8 48ac 209e 341f 728e 7ba5 c80c  .74.H. .4.r.{...
 00001850: 3801 c910 d197 4917 d204 b994 a957 11cc  8.....I......W..
 00001860: 037a 549b aada aaf4 6df0 7661 b2b3 d53c  .zT.....m.va...<
 00001870: 9d6d cdd9 6d8e f88f 1dba ce19 3c06 f39c  .m..m.......<...
 00001880: d0e7 1f11 8a46 67f1 0273 78e6 c242 ea31  .....Fg..sx..B.1
 00001890: 6b2e e577 7fb1 54cb 12c1 55db a8c5 bbed  k..w..T...U.....
-000018a0: 0750 4b03 0414 0000 0008 0093 6af9 56e8  .PK.........j.V.
+000018a0: 0750 4b03 0414 0000 0008 0054 7bfa 56e8  .PK........T{.V.
 000018b0: e449 d139 0300 00b3 2400 0028 0000 0070  .I.9....$..(...p
 000018c0: 7074 2f70 7269 6e74 6572 5365 7474 696e  pt/printerSettin
 000018d0: 6773 2f70 7269 6e74 6572 5365 7474 696e  gs/printerSettin
 000018e0: 6773 312e 6269 6eed 59cf 6eda 3018 cf7a  gs1.bin.Y.n.0..z
 000018f0: 2b6f b05b 963b 3150 56d8 9452 3128 1a12  +o.[.;1PV..R1(..
 00001900: 6da3 122a ed54 b989 cbdc 8638 72cc 187b  m..*.T.....8r..{
 00001910: a4bd dfee 7302 0113 3084 1dd6 24ea a155  ....s...0...$..U
@@ -444,15 +444,15 @@
 00001bb0: 2b16 4ec3 ff43 9e48 3896 8093 e810 1fe7  +.N..C.H8.......
 00001bc0: bd78 bd97 92a8 5e86 3ee1 6c63 9e77 88eb  .x....^.>.lc.w..
 00001bd0: f267 16cd 8b24 af70 28a3 5304 b2e6 410f  .g...$.p(.S...A.
 00001be0: d380 8529 bb50 0e6c b1ca c782 18c0 027a  ...).P.l.......z
 00001bf0: 9124 252a 58ab d61b f5e6 d979 bd91 594f  .$%*X......y..YO
 00001c00: a2f3 29f4 0a66 ca16 abe4 494b ba5a d298  ..)..f....IK.Z..
 00001c10: 279e a45e cfc9 ffbf f315 453e b8f9 fd0b  '..^......E>....
-00001c20: 504b 0304 1400 0000 0800 936a f956 0f2d  PK.........j.V.-
+00001c20: 504b 0304 1400 0000 0800 547b fa56 0f2d  PK........T{.V.-
 00001c30: afae 4801 0000 8b02 0000 1100 0000 7070  ..H...........pp
 00001c40: 742f 7072 6573 5072 6f70 732e 786d 6cad  t/presProps.xml.
 00001c50: 92cb 4ec3 3010 45f7 48fc 43e4 bdeb 47d2  ..N.0.E.H.C...G.
 00001c60: b489 9a54 4913 2424 162c e003 acc4 692d  ...TI.$$.,....i-
 00001c70: c50f d9ee 0321 fe9d 1052 a0b0 e982 dd8c  .....!...R......
 00001c80: 46f7 ceb9 a359 ad4f b20f 0edc 3aa1 5506  F....Y.O....:.U.
 00001c90: c80c 8380 ab46 b742 6d33 f0fc 7407 9720  .....F.Bm3..t.. 
@@ -468,15 +468,15 @@
 00001d30: b6c2 35cc b6f7 926d 79dd 0a5f 31cf ce70  ..5....my.._1..p
 00001d40: 24fa 8327 4563 b5d3 9d9f 355a 4e39 91d1  $..'Ec....5ZN9..
 00001d50: 476e 8d16 6354 82a7 7b1d 589f 010c 50be  Gn..cT..{.X...P.
 00001d60: 4223 dc25 6315 9202 c7b4 808b 6459 c028  B#.%c.......dY.(
 00001d70: a409 2cca aa82 6559 2ce7 714c f19c e02f  ..,...eY,.qL.../
 00001d80: 46de b17d ef47 c6ca 887f c4a3 f402 107d  F..}.G.........}
 00001d90: df13 fdfe 9ffc 1d50 4b03 0414 0000 0008  .......PK.......
-00001da0: 0093 6af9 56d7 e8ed 176e 0100 0045 0300  ..j.V....n...E..
+00001da0: 0054 7bfa 56d7 e8ed 176e 0100 0045 0300  .T{.V....n...E..
 00001db0: 0011 0000 0070 7074 2f76 6965 7750 726f  .....ppt/viewPro
 00001dc0: 7073 2e78 6d6c 8d53 4d6f c220 18be 2fd9  ps.xml.SMo. ../.
 00001dd0: 7f20 dc15 ea5c d735 b65e 969d 3c2c d1ed  . ...\.5.^..<,..
 00001de0: 4e28 ad24 1408 a0b6 fefa bd6d fd9c 26f3  N(.$.......m..&.
 00001df0: d4f7 f3e1 799e c26c ded4 0a6d 85f3 d2e8  ....y..l...m....
 00001e00: 0c47 638a 91d0 dc14 5257 19fe 5e7d 8e12  .Gc.....RW..^}..
 00001e10: 8c7c 60ba 60ca 6891 e156 783c cf9f 9f66  .|`.`.h..Vx<...f
@@ -493,29 +493,29 @@
 00001ec0: 8172 7ba7 4c4e 7b36 354e 5652 a326 c3a3  .r{.LN{65NVR.&..
 00001ed0: 284a a618 b55d 44a7 8739 7ea6 506d 80df  (J...]D..9~.Pm..
 00001ee0: c287 538c 6017 5c02 438d db63 648d cff0  ..S.`.\.C..cd...
 00001ef0: 248a 0fd2 8791 a198 24c7 73cf 20e4 5a22  $.......$.s. .Z"
 00001f00: b931 409b 20fc 4a34 e1c6 85bb c2e9 7de1  .1@. .J4......}.
 00001f10: f47f e1b4 174d ff2a 2677 2954 4e16 4bcb  .....M.*&w)TN.K.
 00001f20: 385c 56c4 61f9 0d2e 073c 04de 1ec3 0165  8\V.a....<.....e
-00001f30: 7801 f92f 504b 0304 1400 0000 0800 936a  x../PK.........j
-00001f40: f956 d8fd 8d8f a500 0000 b600 0000 1300  .V..............
+00001f30: 7801 f92f 504b 0304 1400 0000 0800 547b  x../PK........T{
+00001f40: fa56 d8fd 8d8f a500 0000 b600 0000 1300  .V..............
 00001f50: 0000 7070 742f 7461 626c 6553 7479 6c65  ..ppt/tableStyle
 00001f60: 732e 786d 6c0d cc49 0e82 3018 40e1 bd89  s.xml..I..0.@...
 00001f70: 7768 fe7d 2d43 5124 14c2 202b 77ea 012a  wh.}-CQ$.. +w..*
 00001f80: 9421 e940 68a3 12e3 dd65 f9f2 922f cd3f  .!.@h....e.../.?
 00001f90: 4aa2 9758 ec64 3403 ffe0 0112 ba35 dda4  J..X.d4......5..
 00001fa0: 0706 8f7b 8363 40d6 71dd 7169 b460 b00a  ...{.c@.q.qi.`..
 00001fb0: 0b79 b6df a53c 714f 7973 ab14 57eb d0a6  .y...<qOys..W...
 00001fc0: 689b 7006 a373 7342 886d 47a1 b83d 9859  h.p..ssB.mG..=.Y
 00001fd0: e8ed f566 51dc 6db9 0ca4 5bf8 7bd3 9524  ...fQ.m...[.{..$
 00001fe0: 81e7 1d89 e293 06d4 899e c137 aa82 20a2  ...........7.. .
 00001ff0: b4c0 a7cb e588 6948 035c 7a34 c671 54d6  ......iH.\z4.qT.
 00002000: d5b9 a9fd 2a2c 7e40 b23f 504b 0304 1400  ....*,~@.?PK....
-00002010: 0000 0800 936a f956 b00f 588b 3b25 0000  .....j.V..X.;%..
+00002010: 0000 0800 547b fa56 b00f 588b 3b25 0000  ....T{.V..X.;%..
 00002020: 662e 0000 1700 0000 646f 6350 726f 7073  f.......docProps
 00002030: 2f74 6875 6d62 6e61 696c 2e6a 7065 67dd  /thumbnail.jpeg.
 00002040: 7877 5853 59b7 f741 8a4a 558a 34c5 42ef  xwXSY..A.JU.4.B.
 00002050: bd4a 7905 0149 2440 0841 a943 0910 7a49  .Jy..I$@.A.C..zI
 00002060: 3460 c419 4150 9a23 55a9 0a84 1030 02d2  4`..AP.#U....0..
 00002070: 9b0a 0154 1010 48a8 0226 482f 1214 8c0d  ...T..H..&H/....
 00002080: bea0 ce8c f7de b9df 7d9f 7bef 1fef f7ed  ........}.{.....
@@ -1106,15 +1106,15 @@
 00004510: 78fc 5858 f395 93a5 d09b 3445 6796 ad5b  x.XX......4Eg..[
 00004520: ace7 db94 3438 36aa 1479 c408 1e08 282a  ....486..y....(*
 00004530: c3c0 31cf 2217 e7d0 ae51 8e58 59dc e8d2  ..1."....Q.XY...
 00004540: 0ce6 54b6 a1ce 3948 15df 348d 79f0 7aea  ..T...9H..4.y.z.
 00004550: f829 d83c c16f c85a dada baec 6270 c45c  .).<.o.Z....bp.\
 00004560: 7a61 fac4 8768 453d f392 a011 fdca 7f85  za...hE=........
 00004570: efb4 ff8d 6eef ced8 ff01 504b 0304 1400  ....n.....PK....
-00004580: 0000 0800 936a f956 a05e 3bcd 7c01 0000  .....j.V.^;.|...
+00004580: 0000 0800 547b fa56 a05e 3bcd 7c01 0000  ....T{.V.^;.|...
 00004590: dd02 0000 1100 0000 646f 6350 726f 7073  ........docProps
 000045a0: 2f63 6f72 652e 786d 6c7d 92cd 4ec3 3010  /core.xml}..N.0.
 000045b0: 84ef 3c45 d44b 4e89 e314 f113 a541 02c4  ..<E.KN......A..
 000045c0: 894a 955a 04e2 66ec 2535 24b6 656f 9be6  .J.Z..f.%5$.eo..
 000045d0: ed71 dc36 0581 38ae 67f6 f3ec dae5 cdae  .q.6..8.g.......
 000045e0: 6da2 2d58 27b5 9ac5 34cd e208 14d7 42aa  m.-X'...4.....B.
 000045f0: 7a16 3fad 1e92 ab38 72c8 9460 8d56 308b  z.?....8r..`.V0.
@@ -1132,16 +1132,16 @@
 000046b0: 2bdc be43 80e3 569a 014c 82dc 3087 73ff  +..C..V..L..0.s.
 000046c0: 74ef 12c4 6d5f 2d11 b610 dd31 a5fa 92fc  t...m_-....1....
 000046d0: 9687 0e0b 5b39 bc7c 751d 1c63 591e f6b8  ....[9.|u..cY...
 000046e0: bf1d 44e4 e72f f6db 3a2a cfd3 bbfb d5c3  ..D../..:*......
 000046f0: a4ca 339a 2794 26f4 7245 6991 5d16 e7d9  ..3.'.&.rEi.]...
 00004700: eb10 fc47 ff09 d81e 02fc 4f9c 0662 b6ca  ...G......O..b..
 00004710: f340 a4df 8847 40c8 cf3d bcd6 b6f7 f393  .@...G@..=......
-00004720: 5f3f b2fa 0250 4b03 0414 0000 0008 0093  _?...PK.........
-00004730: 6af9 56a2 c411 aa08 0200 00a8 0400 0010  j.V.............
+00004720: 5f3f b2fa 0250 4b03 0414 0000 0008 0054  _?...PK........T
+00004730: 7bfa 56a2 c411 aa08 0200 00a8 0400 0010  {.V.............
 00004740: 0000 0064 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
 00004750: 786d 6ca5 544d 8fda 3010 bd57 ea7f b07c  xml.TM..0..W...|
 00004760: 6a0f 60a0 74b5 42c6 ab96 d58a 4329 4864  j.`.t.B.....C)Hd
 00004770: b7e7 6932 2156 836d d92e 0bfd f59d 249b  ..i2!V.m......$.
 00004780: 10ca aa87 3697 bc37 337a 9e0f 8fe5 dd71  ....6..73z.....q
 00004790: 5fb2 03fa a0ad 99f3 f170 c419 9ad4 66da  _........p....f.
 000047a0: ece6 fc31 7918 dc72 1622 980c 4a6b 70ce  ...1y..r."..Jkp.
@@ -1168,89 +1168,89 @@
 000048f0: a243 e7cb c4fa b7e2 aaa2 36b7 3fb2 5981  .C........6.?.Y.
 00004900: 811d 568e 0e2d ecde 8139 2983 d679 38ea  ..V..-...9)..y8.
 00004910: 7a47 a468 cdf2 8b36 3fc2 a34b ec3d 446c  zG.h...6?..K.=Dl
 00004920: c77f 6994 db02 3c66 b451 ddf5 e80c 7249  ..i...<f.Q....rI
 00004930: 95fa 92e2 3f53 d955 b72e 7947 c3a2 00b3  ....?S.U..yG....
 00004940: c3ac 95b8 7654 9bf6 d43c 3c6a 3c1d 8ee8  ....vT...<<j<...
 00004950: ab37 aab5 558b d2be 08ea 3750 4b01 0214  .7..U.....7PK...
-00004960: 0314 0000 0008 0093 6af9 5665 310c c88e  ........j.Ve1...
+00004960: 0314 0000 0008 0054 7bfa 5665 310c c88e  .......T{.Ve1...
 00004970: 0100 00f0 0600 0013 0000 0000 0000 0000  ................
 00004980: 0000 0080 0100 0000 005b 436f 6e74 656e  .........[Conten
 00004990: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
-000049a0: 1403 1400 0000 0800 936a f956 f10d 37ec  .........j.V..7.
+000049a0: 1403 1400 0000 0800 547b fa56 f10d 37ec  ........T{.V..7.
 000049b0: 0001 0000 e102 0000 0b00 0000 0000 0000  ................
 000049c0: 0000 0000 8001 bf01 0000 5f72 656c 732f  .........._rels/
 000049d0: 2e72 656c 7350 4b01 0214 0314 0000 0008  .relsPK.........
-000049e0: 0093 6af9 5676 bc49 cc2c 0200 009b 0c00  ..j.Vv.I.,......
+000049e0: 0054 7bfa 5676 bc49 cc2c 0200 009b 0c00  .T{.Vv.I.,......
 000049f0: 0014 0000 0000 0000 0000 0000 0080 01e8  ................
 00004a00: 0200 0070 7074 2f70 7265 7365 6e74 6174  ...ppt/presentat
 00004a10: 696f 6e2e 786d 6c50 4b01 0214 0314 0000  ion.xmlPK.......
-00004a20: 0008 0093 6af9 56dd 09ad f61b 0100 0071  ....j.V........q
+00004a20: 0008 0054 7bfa 56dd 09ad f61b 0100 0071  ...T{.V........q
 00004a30: 0400 001f 0000 0000 0000 0000 0000 0080  ................
 00004a40: 0146 0500 0070 7074 2f5f 7265 6c73 2f70  .F...ppt/_rels/p
 00004a50: 7265 7365 6e74 6174 696f 6e2e 786d 6c2e  resentation.xml.
 00004a60: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-00004a70: 936a f956 f3f6 6658 c903 0000 821e 0000  .j.V..fX........
+00004a70: 547b fa56 f3f6 6658 c903 0000 821e 0000  T{.V..fX........
 00004a80: 2100 0000 0000 0000 0000 0000 8001 9e06  !...............
 00004a90: 0000 7070 742f 736c 6964 654d 6173 7465  ..ppt/slideMaste
 00004aa0: 7273 2f73 6c69 6465 4d61 7374 6572 312e  rs/slideMaster1.
-00004ab0: 786d 6c50 4b01 0214 0314 0000 0008 0093  xmlPK...........
-00004ac0: 6af9 5698 1afe 61ce 0000 00bd 0100 002c  j.V...a........,
+00004ab0: 786d 6c50 4b01 0214 0314 0000 0008 0054  xmlPK..........T
+00004ac0: 7bfa 5698 1afe 61ce 0000 00bd 0100 002c  {.V...a........,
 00004ad0: 0000 0000 0000 0000 0000 0080 01a6 0a00  ................
 00004ae0: 0070 7074 2f73 6c69 6465 4d61 7374 6572  .ppt/slideMaster
 00004af0: 732f 5f72 656c 732f 736c 6964 654d 6173  s/_rels/slideMas
 00004b00: 7465 7231 2e78 6d6c 2e72 656c 7350 4b01  ter1.xml.relsPK.
-00004b10: 0214 0314 0000 0008 0093 6af9 566c f32a  ..........j.Vl.*
+00004b10: 0214 0314 0000 0008 0054 7bfa 566c f32a  .........T{.Vl.*
 00004b20: 3735 0100 006f 0200 0021 0000 0000 0000  75...o...!......
 00004b30: 0000 0000 0080 01be 0b00 0070 7074 2f73  ...........ppt/s
 00004b40: 6c69 6465 4c61 796f 7574 732f 736c 6964  lideLayouts/slid
 00004b50: 654c 6179 6f75 7431 2e78 6d6c 504b 0102  eLayout1.xmlPK..
-00004b60: 1403 1400 0000 0800 936a f956 8065 e188  .........j.V.e..
+00004b60: 1403 1400 0000 0800 547b fa56 8065 e188  ........T{.V.e..
 00004b70: b700 0000 3601 0000 2c00 0000 0000 0000  ....6...,.......
 00004b80: 0000 0000 8001 320d 0000 7070 742f 736c  ......2...ppt/sl
 00004b90: 6964 654c 6179 6f75 7473 2f5f 7265 6c73  ideLayouts/_rels
 00004ba0: 2f73 6c69 6465 4c61 796f 7574 312e 786d  /slideLayout1.xm
 00004bb0: 6c2e 7265 6c73 504b 0102 1403 1400 0000  l.relsPK........
-00004bc0: 0800 936a f956 f9cf 0939 b605 0000 5c1b  ...j.V...9....\.
+00004bc0: 0800 547b fa56 f9cf 0939 b605 0000 5c1b  ..T{.V...9....\.
 00004bd0: 0000 1400 0000 0000 0000 0000 0000 8001  ................
 00004be0: 330e 0000 7070 742f 7468 656d 652f 7468  3...ppt/theme/th
 00004bf0: 656d 6531 2e78 6d6c 504b 0102 1403 1400  eme1.xmlPK......
-00004c00: 0000 0800 936a f956 cf2d 8604 5e03 0000  .....j.V.-..^...
+00004c00: 0000 0800 547b fa56 cf2d 8604 5e03 0000  ....T{.V.-..^...
 00004c10: 3d0f 0000 1500 0000 0000 0000 0000 0000  =...............
 00004c20: 8001 1b14 0000 7070 742f 736c 6964 6573  ......ppt/slides
 00004c30: 2f73 6c69 6465 312e 786d 6c50 4b01 0214  /slide1.xmlPK...
-00004c40: 0314 0000 0008 0093 6af9 5636 e850 cdb7  ........j.V6.P..
+00004c40: 0314 0000 0008 0054 7bfa 5636 e850 cdb7  .......T{.V6.P..
 00004c50: 0000 0036 0100 0020 0000 0000 0000 0000  ...6... ........
 00004c60: 0000 0080 01ac 1700 0070 7074 2f73 6c69  .........ppt/sli
 00004c70: 6465 732f 5f72 656c 732f 736c 6964 6531  des/_rels/slide1
 00004c80: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
-00004c90: 0000 0008 0093 6af9 56e8 e449 d139 0300  ......j.V..I.9..
+00004c90: 0000 0008 0054 7bfa 56e8 e449 d139 0300  .....T{.V..I.9..
 00004ca0: 00b3 2400 0028 0000 0000 0000 0000 0000  ..$..(..........
 00004cb0: 0080 01a1 1800 0070 7074 2f70 7269 6e74  .......ppt/print
 00004cc0: 6572 5365 7474 696e 6773 2f70 7269 6e74  erSettings/print
 00004cd0: 6572 5365 7474 696e 6773 312e 6269 6e50  erSettings1.binP
-00004ce0: 4b01 0214 0314 0000 0008 0093 6af9 560f  K...........j.V.
+00004ce0: 4b01 0214 0314 0000 0008 0054 7bfa 560f  K..........T{.V.
 00004cf0: 2daf ae48 0100 008b 0200 0011 0000 0000  -..H............
 00004d00: 0000 0000 0000 0080 0120 1c00 0070 7074  ......... ...ppt
 00004d10: 2f70 7265 7350 726f 7073 2e78 6d6c 504b  /presProps.xmlPK
-00004d20: 0102 1403 1400 0000 0800 936a f956 d7e8  ...........j.V..
+00004d20: 0102 1403 1400 0000 0800 547b fa56 d7e8  ..........T{.V..
 00004d30: ed17 6e01 0000 4503 0000 1100 0000 0000  ..n...E.........
 00004d40: 0000 0000 0000 8001 971d 0000 7070 742f  ............ppt/
 00004d50: 7669 6577 5072 6f70 732e 786d 6c50 4b01  viewProps.xmlPK.
-00004d60: 0214 0314 0000 0008 0093 6af9 56d8 fd8d  ..........j.V...
+00004d60: 0214 0314 0000 0008 0054 7bfa 56d8 fd8d  .........T{.V...
 00004d70: 8fa5 0000 00b6 0000 0013 0000 0000 0000  ................
 00004d80: 0000 0000 0080 0134 1f00 0070 7074 2f74  .......4...ppt/t
 00004d90: 6162 6c65 5374 796c 6573 2e78 6d6c 504b  ableStyles.xmlPK
-00004da0: 0102 1403 1400 0000 0800 936a f956 b00f  ...........j.V..
+00004da0: 0102 1403 1400 0000 0800 547b fa56 b00f  ..........T{.V..
 00004db0: 588b 3b25 0000 662e 0000 1700 0000 0000  X.;%..f.........
 00004dc0: 0000 0000 0000 8001 0a20 0000 646f 6350  ......... ..docP
 00004dd0: 726f 7073 2f74 6875 6d62 6e61 696c 2e6a  rops/thumbnail.j
-00004de0: 7065 6750 4b01 0214 0314 0000 0008 0093  pegPK...........
-00004df0: 6af9 56a0 5e3b cd7c 0100 00dd 0200 0011  j.V.^;.|........
+00004de0: 7065 6750 4b01 0214 0314 0000 0008 0054  pegPK..........T
+00004df0: 7bfa 56a0 5e3b cd7c 0100 00dd 0200 0011  {.V.^;.|........
 00004e00: 0000 0000 0000 0000 0000 0080 017a 4500  .............zE.
 00004e10: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00004e20: 6d6c 504b 0102 1403 1400 0000 0800 936a  mlPK...........j
-00004e30: f956 a2c4 11aa 0802 0000 a804 0000 1000  .V..............
+00004e20: 6d6c 504b 0102 1403 1400 0000 0800 547b  mlPK..........T{
+00004e30: fa56 a2c4 11aa 0802 0000 a804 0000 1000  .V..............
 00004e40: 0000 0000 0000 0000 0000 8001 2547 0000  ............%G..
 00004e50: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
 00004e60: 504b 0506 0000 0000 1200 1200 0505 0000  PK..............
 00004e70: 5b49 0000 0000                           [I....
```

### Comparing `python-pptx-fix-0.6.21.1/features/act-action.feature` & `python-pptx-fix-0.6.21.2/features/act-action.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/act-hyperlink.feature` & `python-pptx-fix-0.6.21.2/features/act-hyperlink.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-axis-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-axis-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-axistitle-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-axistitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-category-access.feature` & `python-pptx-fix-0.6.21.2/features/cht-category-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-category-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-category-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-chart.feature` & `python-pptx-fix-0.6.21.2/features/cht-chart.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-charttitle-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-charttitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-data-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-data-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-datalabels.feature` & `python-pptx-fix-0.6.21.2/features/cht-datalabels.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-legend-access.feature` & `python-pptx-fix-0.6.21.2/features/cht-legend-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-legend-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-legend-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-marker-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-marker-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-plot-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-plot-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-point-access.feature` & `python-pptx-fix-0.6.21.2/features/cht-point-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-point-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-point-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-replace-data.feature` & `python-pptx-fix-0.6.21.2/features/cht-replace-data.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-series.feature` & `python-pptx-fix-0.6.21.2/features/cht-series.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/cht-ticklabels-props.feature` & `python-pptx-fix-0.6.21.2/features/cht-ticklabels-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/dml-color.feature` & `python-pptx-fix-0.6.21.2/features/dml-color.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/dml-effect.feature` & `python-pptx-fix-0.6.21.2/features/dml-effect.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/dml-fill.feature` & `python-pptx-fix-0.6.21.2/features/dml-fill.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/dml-line.feature` & `python-pptx-fix-0.6.21.2/features/dml-line.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/environment.py` & `python-pptx-fix-0.6.21.2/features/environment.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/ph-inherit-props.feature` & `python-pptx-fix-0.6.21.2/features/ph-inherit-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/ph-insert-shape.feature` & `python-pptx-fix-0.6.21.2/features/ph-insert-shape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/ph-phfmt-props.feature` & `python-pptx-fix-0.6.21.2/features/ph-phfmt-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/ph-placeholder-props.feature` & `python-pptx-fix-0.6.21.2/features/ph-placeholder-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/prs-coreprops.feature` & `python-pptx-fix-0.6.21.2/features/prs-coreprops.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/prs-open-save.feature` & `python-pptx-fix-0.6.21.2/features/prs-open-save.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/prs-presentation-props.feature` & `python-pptx-fix-0.6.21.2/features/prs-presentation-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-autoshape.feature` & `python-pptx-fix-0.6.21.2/features/shp-autoshape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-connector.feature` & `python-pptx-fix-0.6.21.2/features/shp-connector.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-freeform.feature` & `python-pptx-fix-0.6.21.2/features/shp-freeform.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-graphicframe.feature` & `python-pptx-fix-0.6.21.2/features/shp-graphicframe.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-groupshape.feature` & `python-pptx-fix-0.6.21.2/features/shp-groupshape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-movie-props.feature` & `python-pptx-fix-0.6.21.2/features/shp-movie-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-picture.feature` & `python-pptx-fix-0.6.21.2/features/shp-picture.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-placeholder.feature` & `python-pptx-fix-0.6.21.2/features/shp-placeholder.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-shapes.feature` & `python-pptx-fix-0.6.21.2/features/shp-shapes.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/shp-shared.feature` & `python-pptx-fix-0.6.21.2/features/shp-shared.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/sld-slide.feature` & `python-pptx-fix-0.6.21.2/features/sld-slide.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/sld-slides.feature` & `python-pptx-fix-0.6.21.2/features/sld-slides.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/action.py` & `python-pptx-fix-0.6.21.2/features/steps/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/axis.py` & `python-pptx-fix-0.6.21.2/features/steps/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/background.py` & `python-pptx-fix-0.6.21.2/features/steps/background.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/category.py` & `python-pptx-fix-0.6.21.2/features/steps/category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/chart.py` & `python-pptx-fix-0.6.21.2/features/steps/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/chartdata.py` & `python-pptx-fix-0.6.21.2/features/steps/chartdata.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/color.py` & `python-pptx-fix-0.6.21.2/features/steps/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/coreprops.py` & `python-pptx-fix-0.6.21.2/features/steps/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/datalabel.py` & `python-pptx-fix-0.6.21.2/features/steps/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/effect.py` & `python-pptx-fix-0.6.21.2/features/steps/effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/fill.py` & `python-pptx-fix-0.6.21.2/features/steps/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/font.py` & `python-pptx-fix-0.6.21.2/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/font_color.py` & `python-pptx-fix-0.6.21.2/features/steps/font_color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/helpers.py` & `python-pptx-fix-0.6.21.2/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/legend.py` & `python-pptx-fix-0.6.21.2/features/steps/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/line.py` & `python-pptx-fix-0.6.21.2/features/steps/line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/picture.py` & `python-pptx-fix-0.6.21.2/features/steps/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/placeholder.py` & `python-pptx-fix-0.6.21.2/features/steps/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/plot.py` & `python-pptx-fix-0.6.21.2/features/steps/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/presentation.py` & `python-pptx-fix-0.6.21.2/features/steps/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/series.py` & `python-pptx-fix-0.6.21.2/features/steps/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/shape.py` & `python-pptx-fix-0.6.21.2/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/shapes.py` & `python-pptx-fix-0.6.21.2/features/steps/shapes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/slide.py` & `python-pptx-fix-0.6.21.2/features/steps/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/slides.py` & `python-pptx-fix-0.6.21.2/features/steps/slides.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/table.py` & `python-pptx-fix-0.6.21.2/features/steps/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/72-dpi.tiff` & `python-pptx-fix-0.6.21.2/features/steps/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/CVS_LOGO.WMF` & `python-pptx-fix-0.6.21.2/features/steps/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/act-props.pptm` & `python-pptx-fix-0.6.21.2/features/steps/test_files/act-props.pptm`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/calibriz.ttf` & `python-pptx-fix-0.6.21.2/features/steps/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-axis-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-axis-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-category-access.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-category-access.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-chart-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-chart-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-chart-type.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-chart-type.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-charts.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-charts.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-datalabels.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-datalabels.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-gridlines-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-gridlines-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-legend-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-legend-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-legend.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-legend.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-marker-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-marker-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-plot-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-plot-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-point-access.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-point-access.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-point-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-point-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-replace-data.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-replace-data.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-series.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-series.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/cht-ticklabels-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/cht-ticklabels-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/dml-effect.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/dml-effect.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/dml-fill.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/dml-fill.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/dml-line.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/dml-line.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/ext-rels.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/ext-rels.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/[Content_Types].xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/_rels/.rels` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/app.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/core.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/presProps.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/presProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/presentation.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/extracted-pptx/ppt/viewProps.xml` & `python-pptx-fix-0.6.21.2/features/steps/test_files/extracted-pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/font-color.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/font-color.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/just-two-mice.mp4` & `python-pptx-fix-0.6.21.2/features/steps/test_files/just-two-mice.mp4`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/just-two-mice.png` & `python-pptx-fix-0.6.21.2/features/steps/test_files/just-two-mice.png`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/lyt-shapes.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/lyt-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/minimal.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/monty-truth.png` & `python-pptx-fix-0.6.21.2/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/mst-placeholders.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/mst-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/mst-shapes.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/mst-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/mst-slide-layouts.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/mst-slide-layouts.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/ph-inherit-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/ph-inherit-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/ph-populated-placeholders.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/ph-populated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/ph-unpopulated-placeholders.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/ph-unpopulated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/pic.emf` & `python-pptx-fix-0.6.21.2/features/steps/test_files/pic.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/prs-add-slide.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/prs-add-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/prs-notes.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/prs-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/prs-properties.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/prs-properties.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/prs-slide-masters.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/prs-slide-masters.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/python-icon.jpeg` & `python-pptx-fix-0.6.21.2/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/python-powered.png` & `python-pptx-fix-0.6.21.2/features/steps/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/python.bmp` & `python-pptx-fix-0.6.21.2/features/steps/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-access-chart.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-access-chart.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-access-ole-object.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-access-ole-object.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-autoshape-adjustments.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-autoshape-adjustments.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-autoshape-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-autoshape-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-common-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-common-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-connector-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-connector-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-docx.docx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-docx.docx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-pptx.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-pptx.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-embedded-xlsx.xlsx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-embedded-xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-freeform.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-freeform.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-groupshape.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-groupshape.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-movie-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-movie-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-picture.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-picture.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-pos-and-size.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-pos-and-size.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/shp-shapes.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/shp-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sld-background.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sld-background.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sld-blank.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sld-blank.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sld-notes.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sld-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sld-slide.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sld-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sld-slides.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sld-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/sonic.gif` & `python-pptx-fix-0.6.21.2/features/steps/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/tbl-cell.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/tbl-cell.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/test.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-fit-text.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-fit-text.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-font-props.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-font-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-font-typeface.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-font-typeface.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-paragraph-spacing.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-paragraph-spacing.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-text-frame.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-text-frame.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/test_files/txt-text.pptx` & `python-pptx-fix-0.6.21.2/features/steps/test_files/txt-text.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/text.py` & `python-pptx-fix-0.6.21.2/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/steps/text_frame.py` & `python-pptx-fix-0.6.21.2/features/steps/text_frame.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/tbl-cell.feature` & `python-pptx-fix-0.6.21.2/features/tbl-cell.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/tbl-table.feature` & `python-pptx-fix-0.6.21.2/features/tbl-table.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/txt-font-color.feature` & `python-pptx-fix-0.6.21.2/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/txt-font-props.feature` & `python-pptx-fix-0.6.21.2/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/txt-paragraph.feature` & `python-pptx-fix-0.6.21.2/features/txt-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/txt-text.feature` & `python-pptx-fix-0.6.21.2/features/txt-text.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/features/txt-textframe.feature` & `python-pptx-fix-0.6.21.2/features/txt-textframe.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/__init__.py` & `python-pptx-fix-0.6.21.2/pptx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 
 """Initialization module for python-pptx package."""
 
-__version__ = "0.6.21.1"
+__version__ = "0.6.21.2"
 
 
 import pptx.exc as exceptions
 import sys
 
 sys.modules["pptx.exceptions"] = exceptions
 del sys
```

### Comparing `python-pptx-fix-0.6.21.1/pptx/action.py` & `python-pptx-fix-0.6.21.2/pptx/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/api.py` & `python-pptx-fix-0.6.21.2/pptx/api.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/axis.py` & `python-pptx-fix-0.6.21.2/pptx/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/category.py` & `python-pptx-fix-0.6.21.2/pptx/chart/category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/chart.py` & `python-pptx-fix-0.6.21.2/pptx/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/data.py` & `python-pptx-fix-0.6.21.2/pptx/chart/data.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/datalabel.py` & `python-pptx-fix-0.6.21.2/pptx/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/legend.py` & `python-pptx-fix-0.6.21.2/pptx/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/marker.py` & `python-pptx-fix-0.6.21.2/pptx/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/plot.py` & `python-pptx-fix-0.6.21.2/pptx/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/point.py` & `python-pptx-fix-0.6.21.2/pptx/chart/point.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/series.py` & `python-pptx-fix-0.6.21.2/pptx/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/xlsx.py` & `python-pptx-fix-0.6.21.2/pptx/chart/xlsx.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/chart/xmlwriter.py` & `python-pptx-fix-0.6.21.2/pptx/chart/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/compat/__init__.py` & `python-pptx-fix-0.6.21.2/pptx/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/compat/python2.py` & `python-pptx-fix-0.6.21.2/pptx/compat/python2.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/compat/python3.py` & `python-pptx-fix-0.6.21.2/pptx/compat/python3.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/dml/chtfmt.py` & `python-pptx-fix-0.6.21.2/pptx/dml/chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/dml/color.py` & `python-pptx-fix-0.6.21.2/pptx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/dml/effect.py` & `python-pptx-fix-0.6.21.2/pptx/dml/effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/dml/fill.py` & `python-pptx-fix-0.6.21.2/pptx/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/dml/line.py` & `python-pptx-fix-0.6.21.2/pptx/dml/line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/action.py` & `python-pptx-fix-0.6.21.2/pptx/enum/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/base.py` & `python-pptx-fix-0.6.21.2/pptx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/chart.py` & `python-pptx-fix-0.6.21.2/pptx/enum/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/dml.py` & `python-pptx-fix-0.6.21.2/pptx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/lang.py` & `python-pptx-fix-0.6.21.2/pptx/enum/lang.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/shapes.py` & `python-pptx-fix-0.6.21.2/pptx/enum/shapes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/enum/text.py` & `python-pptx-fix-0.6.21.2/pptx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/media.py` & `python-pptx-fix-0.6.21.2/pptx/media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/constants.py` & `python-pptx-fix-0.6.21.2/pptx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/oxml.py` & `python-pptx-fix-0.6.21.2/pptx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/package.py` & `python-pptx-fix-0.6.21.2/pptx/opc/package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/packuri.py` & `python-pptx-fix-0.6.21.2/pptx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/serialized.py` & `python-pptx-fix-0.6.21.2/pptx/opc/serialized.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/shared.py` & `python-pptx-fix-0.6.21.2/pptx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/opc/spec.py` & `python-pptx-fix-0.6.21.2/pptx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/__init__.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/action.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/axis.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/chart.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/datalabel.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/legend.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/marker.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/plot.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/series.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/chart/shared.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/chart/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/coreprops.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/dml/color.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/dml/fill.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/ns.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/presentation.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/autoshape.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/connector.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/graphfrm.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/groupshape.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/groupshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/picture.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/shapes/shared.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/shapes/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/simpletypes.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/slide.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/table.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/text.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/theme.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/theme.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/oxml/xmlchemy.py` & `python-pptx-fix-0.6.21.2/pptx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/package.py` & `python-pptx-fix-0.6.21.2/pptx/package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/chart.py` & `python-pptx-fix-0.6.21.2/pptx/parts/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/coreprops.py` & `python-pptx-fix-0.6.21.2/pptx/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/embeddedpackage.py` & `python-pptx-fix-0.6.21.2/pptx/parts/embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/image.py` & `python-pptx-fix-0.6.21.2/pptx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/media.py` & `python-pptx-fix-0.6.21.2/pptx/parts/media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/presentation.py` & `python-pptx-fix-0.6.21.2/pptx/parts/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/parts/slide.py` & `python-pptx-fix-0.6.21.2/pptx/parts/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/presentation.py` & `python-pptx-fix-0.6.21.2/pptx/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/__init__.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/autoshape.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/base.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/connector.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/freeform.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/freeform.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/graphfrm.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/group.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/group.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/picture.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/placeholder.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shapes/shapetree.py` & `python-pptx-fix-0.6.21.2/pptx/shapes/shapetree.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/shared.py` & `python-pptx-fix-0.6.21.2/pptx/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/slide.py` & `python-pptx-fix-0.6.21.2/pptx/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/spec.py` & `python-pptx-fix-0.6.21.2/pptx/spec.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/table.py` & `python-pptx-fix-0.6.21.2/pptx/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/default.pptx` & `python-pptx-fix-0.6.21.2/pptx/templates/default.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/docx-icon.emf` & `python-pptx-fix-0.6.21.2/pptx/templates/docx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/generic-icon.emf` & `python-pptx-fix-0.6.21.2/pptx/templates/generic-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/notes.xml` & `python-pptx-fix-0.6.21.2/pptx/templates/notes.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/notesMaster.xml` & `python-pptx-fix-0.6.21.2/pptx/templates/notesMaster.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/pptx-icon.emf` & `python-pptx-fix-0.6.21.2/pptx/templates/pptx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/theme.xml` & `python-pptx-fix-0.6.21.2/pptx/templates/theme.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/templates/xlsx-icon.emf` & `python-pptx-fix-0.6.21.2/pptx/templates/xlsx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/text/fonts.py` & `python-pptx-fix-0.6.21.2/pptx/text/fonts.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/text/layout.py` & `python-pptx-fix-0.6.21.2/pptx/text/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,13 +306,20 @@
     Metric Units (EMU) when rendered at *point_size* in the font defined in
     *font_file*.
     """
     emu_per_inch = 914400
     px_per_inch = 72.0
 
     font = _Fonts.font(font_file, point_size)
-    px_width, px_height = font.getsize(text)
-
+    
+    try:
+        px_width, px_height = font.getsize(text)
+    except AttributeError:
+        # .getsize() method is removed in Pillow from 10.0.0
+        # .font.getsize() is used instead
+        (width, height), (offset_x, offset_y) = font.font.getsize(text)
+        px_width, px_height = width + offset_x, height+offset_y
+        
     emu_width = int(px_width / px_per_inch * emu_per_inch)
     emu_height = int(px_height / px_per_inch * emu_per_inch)
 
     return emu_width, emu_height
```

### Comparing `python-pptx-fix-0.6.21.1/pptx/text/text.py` & `python-pptx-fix-0.6.21.2/pptx/text/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/pptx/util.py` & `python-pptx-fix-0.6.21.2/pptx/util.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/PKG-INFO` & `python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pptx-fix
-Version: 0.6.21.1
+Version: 0.6.21.2
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/kascodeo/python-pptx
 Author: Steve Canny
 Author-email: python-pptx@googlegroups.com
 Maintainer: Karim
 Maintainer-email: kascodeo@gmail.com
 License: The MIT License (MIT)
@@ -33,28 +33,29 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 .. image:: https://travis-ci.org/scanny/python-pptx.svg?branch=master
    :target: https://travis-ci.org/scanny/python-pptx
 
 *python-pptx-fix* is a Python library for creating and updating PowerPoint (.pptx)
 files.
 
-This project is created to fix bugs and add minor features to the original project 
-by Scanny at https://github.com/scanny/python-pptx. Original project is 
+This project `python-pptx-fix <https://github.com/kascodeo/python-pptx>`_ is 
+created to fix bugs and add minor features to the original project 
+by `Scanny <https://github.com/scanny/python-pptx>`_. Original project is 
 unresponsive at the moment so had to create this project as *python-pptx-fix*. 
 Feel free to contribute to this project.
 
 
 A typical use would be generating a customized PowerPoint presentation from
 database content, downloadable by clicking a link in a web application.
 Several developers have used it to automate production of presentation-ready
@@ -77,14 +78,24 @@
 
 .. :changelog:
 
 Release History
 ---------------
 
 
+0.6.21.2 (2023-07-26)
++++++++++++++++++++++
+
+- Fix #3 handled removal of getsize() api in pillow 10
+- setup.py updated for twine upload to pypi
+- requirements.txt updated with sphinx tox virtualenv tox
+- tox.ini update with py310 in envlist
+
+
+
 0.6.21.1 (2023-07-25)
 +++++++++++++++++++++
 
 - Fix #1 Handling errors related to collections.abc
 - Fix #878 #762 #770 #820 #834 of https://github.com/scanny/python-pptx/issues
```

### Comparing `python-pptx-fix-0.6.21.1/python_pptx_fix.egg-info/SOURCES.txt` & `python-pptx-fix-0.6.21.2/python_pptx_fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/setup.py` & `python-pptx-fix-0.6.21.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Office/Business :: Office Suites",
     "Topic :: Software Development :: Libraries",
 ]
 
 LONG_DESCRIPTION = readme + "\n\n" + history
 
 ZIP_SAFE = False
```

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_axis.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_category.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_chart.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_data.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_data.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_datalabel.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_legend.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_marker.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_plot.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_point.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_point.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_series.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_xlsx.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/chart/test_xmlwriter.py` & `python-pptx-fix-0.6.21.2/tests/chart/test_xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/dml/test_chtfmt.py` & `python-pptx-fix-0.6.21.2/tests/dml/test_chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/dml/test_color.py` & `python-pptx-fix-0.6.21.2/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/dml/test_effect.py` & `python-pptx-fix-0.6.21.2/tests/dml/test_effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/dml/test_fill.py` & `python-pptx-fix-0.6.21.2/tests/dml/test_fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/dml/test_line.py` & `python-pptx-fix-0.6.21.2/tests/dml/test_line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/opc/test_oxml.py` & `python-pptx-fix-0.6.21.2/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/opc/test_package.py` & `python-pptx-fix-0.6.21.2/tests/opc/test_package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/opc/test_packuri.py` & `python-pptx-fix-0.6.21.2/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/opc/test_serialized.py` & `python-pptx-fix-0.6.21.2/tests/opc/test_serialized.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/opc/unitdata/rels.py` & `python-pptx-fix-0.6.21.2/tests/opc/unitdata/rels.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_autoshape.py` & `python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_graphfrm.py` & `python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_groupshape.py` & `python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_groupshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/shapes/test_picture.py` & `python-pptx-fix-0.6.21.2/tests/oxml/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test___init__.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test___init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_dml.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_ns.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_presentation.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_simpletypes.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_slide.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_table.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_theme.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_theme.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/test_xmlchemy.py` & `python-pptx-fix-0.6.21.2/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/unitdata/dml.py` & `python-pptx-fix-0.6.21.2/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/unitdata/shape.py` & `python-pptx-fix-0.6.21.2/tests/oxml/unitdata/shape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/oxml/unitdata/text.py` & `python-pptx-fix-0.6.21.2/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_chart.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_coreprops.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_embeddedpackage.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_image.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_media.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_presentation.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/parts/test_slide.py` & `python-pptx-fix-0.6.21.2/tests/parts/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_autoshape.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_base.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_connector.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_freeform.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_freeform.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_graphfrm.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_group.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_group.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_picture.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_placeholder.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/shapes/test_shapetree.py` & `python-pptx-fix-0.6.21.2/tests/shapes/test_shapetree.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_action.py` & `python-pptx-fix-0.6.21.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_api.py` & `python-pptx-fix-0.6.21.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_enum.py` & `python-pptx-fix-0.6.21.2/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/calibriz.ttf` & `python-pptx-fix-0.6.21.2/tests/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/cdw-logo.eps` & `python-pptx-fix-0.6.21.2/tests/test_files/cdw-logo.eps`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/[Content_Types].xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/_rels/.rels` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/app.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/core.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/presentation.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/slides/slide1.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/theme/theme1.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/expanded_pptx/ppt/viewProps.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/expanded_pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/minimal.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/missing_rels_item.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/missing_rels_item.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/monty-truth.png` & `python-pptx-fix-0.6.21.2/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/no-core-props.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/no-core-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/no-slides.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/no-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/presentation.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/python-icon.jpeg` & `python-pptx-fix-0.6.21.2/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/python-powered.png` & `python-pptx-fix-0.6.21.2/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/python.bmp` & `python-pptx-fix-0.6.21.2/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/slideLayout1.xml` & `python-pptx-fix-0.6.21.2/tests/test_files/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-date.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-float.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-stacked-100.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area-stacked.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-area.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-area.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered-date.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered-float.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-clustered.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-stacked-100.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-bar-stacked.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-bar-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-clustered.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-stacked-100.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-column-stacked.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-column-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-date.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-float.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers-stacked-100.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers-stacked.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-markers.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-stacked-100.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line-stacked.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x2-line.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x2-line.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-bubble-3d.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-bubble-3d.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-bubble.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-bubble.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-lines-no-markers.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-lines-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-lines.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-lines.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy-smooth.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy-smooth.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x3-xy.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x3-xy.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/2x5-radar.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/2x5-radar.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x1-pie-exploded.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x1-pie-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x1-pie.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x1-pie.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x2-doughnut-exploded.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x2-doughnut-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/3x2-doughnut.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/3x2-doughnut.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/4x2-multi-cat-bar.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/4x2-multi-cat-bar.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/adjust-ser-count.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/adjust-ser-count.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/cat-labels.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/cat-labels.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/content-types-xml.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/content-types-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-notes.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-notes.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-notesMaster.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-notesMaster.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/default-theme.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/default-theme.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/freeform.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/freeform.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/package-rels-xml.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/package-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/placeholders.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/placeholders.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/presentation-rels-xml.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/presentation-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/rels-load-from-xml.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/rels-load-from-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/rewrite-ser.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/rewrite-ser.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/snippets/timing.txt` & `python-pptx-fix-0.6.21.2/tests/test_files/snippets/timing.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/test.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_files/test_slides.pptx` & `python-pptx-fix-0.6.21.2/tests/test_files/test_slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_media.py` & `python-pptx-fix-0.6.21.2/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_package.py` & `python-pptx-fix-0.6.21.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_presentation.py` & `python-pptx-fix-0.6.21.2/tests/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_shared.py` & `python-pptx-fix-0.6.21.2/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_slide.py` & `python-pptx-fix-0.6.21.2/tests/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_table.py` & `python-pptx-fix-0.6.21.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/test_util.py` & `python-pptx-fix-0.6.21.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/text/test_fonts.py` & `python-pptx-fix-0.6.21.2/tests/text/test_fonts.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/text/test_layout.py` & `python-pptx-fix-0.6.21.2/tests/text/test_layout.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/text/test_text.py` & `python-pptx-fix-0.6.21.2/tests/text/test_text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/unitdata.py` & `python-pptx-fix-0.6.21.2/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/unitutil/cxml.py` & `python-pptx-fix-0.6.21.2/tests/unitutil/cxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/unitutil/file.py` & `python-pptx-fix-0.6.21.2/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tests/unitutil/mock.py` & `python-pptx-fix-0.6.21.2/tests/unitutil/mock.py`

 * *Files identical despite different names*

### Comparing `python-pptx-fix-0.6.21.1/tox.ini` & `python-pptx-fix-0.6.21.2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [pytest]
 norecursedirs = docs *.egg-info features .git pptx spec .tox
 python_classes = Test Describe
 python_functions = test_ it_ they_ but_ and_it_
 
 [tox]
-envlist = py27, py38
+envlist = py27, py38, py310
 
 [testenv]
 deps =
     behave==1.2.5
     lxml>=3.1.0
     Pillow>=3.3.2
     pyparsing>=2.0.1
```

