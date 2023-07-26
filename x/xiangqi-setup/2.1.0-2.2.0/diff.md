# Comparing `tmp/xiangqi-setup-2.1.0.tar.gz` & `tmp/xiangqi-setup-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiangqi-setup-2.1.0.tar", last modified: Tue Aug  3 15:15:11 2021, max compression
+gzip compressed data, was "xiangqi-setup-2.2.0.tar", last modified: Wed Jul 26 16:43:26 2023, max compression
```

## Comparing `xiangqi-setup-2.1.0.tar` & `xiangqi-setup-2.2.0.tar`

### file list

```diff
@@ -1,549 +1,567 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.751028 xiangqi-setup-2.1.0/
--rw-r--r--   0 sping     (1000) sping     (1000)      600 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/.flake8
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.478026 xiangqi-setup-2.1.0/.github/
--rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-12-21 01:51:42.000000 xiangqi-setup-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.479026 xiangqi-setup-2.1.0/.github/workflows/
--rw-r--r--   0 sping     (1000) sping     (1000)      933 2021-05-10 16:15:27.000000 xiangqi-setup-2.1.0/.github/workflows/pre-commit-detect-outdated.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      916 2021-05-10 16:15:27.000000 xiangqi-setup-2.1.0/.github/workflows/pre-commit-run.yml
--rw-r--r--   0 sping     (1000) sping     (1000)     1490 2021-05-12 13:06:16.000000 xiangqi-setup-2.1.0/.github/workflows/smoke_test.yml
--rw-r--r--   0 sping     (1000) sping     (1000)       37 2021-08-03 15:14:56.000000 xiangqi-setup-2.1.0/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)       28 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/.isort.cfg
--rw-r--r--   0 sping     (1000) sping     (1000)      824 2021-08-03 15:13:28.000000 xiangqi-setup-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 sping     (1000) sping     (1000)      126 2021-02-16 01:34:04.000000 xiangqi-setup-2.1.0/.style.yapf
--rw-r--r--   0 sping     (1000) sping     (1000)      305 2015-05-11 21:44:18.000000 xiangqi-setup-2.1.0/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)    10189 2021-08-03 15:15:11.751028 xiangqi-setup-2.1.0/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     8879 2021-05-12 13:06:16.000000 xiangqi-setup-2.1.0/README.md
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.487026 xiangqi-setup-2.1.0/doc/
--rw-r--r--   0 sping     (1000) sping     (1000)       17 2015-05-11 20:42:25.000000 xiangqi-setup-2.1.0/doc/.gitignore
--rwxr-xr-x   0 sping     (1000) sping     (1000)     1174 2015-06-14 21:18:47.000000 xiangqi-setup-2.1.0/doc/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)      666 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/doc/demo-arrows-horse-elephant-advisor.xay
--rw-r--r--   0 sping     (1000) sping     (1000)      569 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/doc/demo-arrows-rook-downwards.xay
--rw-r--r--   0 sping     (1000) sping     (1000)      749 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/doc/demo-arrows-rook-leftwards-rightwards.xay
--rw-r--r--   0 sping     (1000) sping     (1000)      569 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/doc/demo-arrows-rook-upwards.xay
--rw-r--r--   0 sping     (1000) sping     (1000)      310 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/doc/demo-last-two-moves.annofen
--rw-r--r--   0 sping     (1000) sping     (1000)      442 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/doc/demo-movement-horse.xay
--rw-r--r--   0 sping     (1000) sping     (1000)      568 2021-01-28 00:14:35.000000 xiangqi-setup-2.1.0/doc/demo-with-history-playok.wxf
--rw-r--r--   0 sping     (1000) sping     (1000)       70 2021-01-10 17:07:08.000000 xiangqi-setup-2.1.0/doc/demo.fen
--rw-r--r--   0 sping     (1000) sping     (1000)      160 2021-02-01 19:56:39.000000 xiangqi-setup-2.1.0/doc/demo.wxf
--rw-r--r--   0 sping     (1000) sping     (1000)    10641 2015-06-14 21:18:47.000000 xiangqi-setup-2.1.0/doc/demo_euro_xiangqi_js.png
--rw-r--r--   0 sping     (1000) sping     (1000)   128843 2021-02-10 10:05:45.000000 xiangqi-setup-2.1.0/doc/demo_euro_xiangqi_js.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10964 2015-06-14 21:18:47.000000 xiangqi-setup-2.1.0/doc/demo_retro_simple.png
--rw-r--r--   0 sping     (1000) sping     (1000)   123322 2021-02-10 10:05:45.000000 xiangqi-setup-2.1.0/doc/demo_retro_simple.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7642 2021-04-02 00:50:50.000000 xiangqi-setup-2.1.0/doc/file_formats.md
--rw-r--r--   0 sping     (1000) sping     (1000)      271 2021-04-01 21:09:11.000000 xiangqi-setup-2.1.0/doc/initial.annofen
--rw-r--r--   0 sping     (1000) sping     (1000)      159 2021-02-01 19:56:39.000000 xiangqi-setup-2.1.0/doc/initial.wxf
--rw-r--r--   0 sping     (1000) sping     (1000)      539 2021-04-01 21:09:11.000000 xiangqi-setup-2.1.0/doc/initial.xay
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2021-08-03 15:15:11.752028 xiangqi-setup-2.1.0/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     2879 2021-02-10 22:05:59.000000 xiangqi-setup-2.1.0/setup.py
--rwxr-xr-x   0 sping     (1000) sping     (1000)     2863 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/test-for-rendering-regressions.sh
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.518026 xiangqi-setup-2.1.0/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)    17656 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-horse-elephant-advisor.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10013 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-downwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)    14548 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-leftwards-rightwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10143 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-upwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)    20270 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-last-two-moves.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10901 2021-02-07 18:27:42.000000 xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-movement-horse.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10122 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-horse-elephant-advisor.png
--rw-r--r--   0 sping     (1000) sping     (1000)     5438 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-downwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)     8203 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-leftwards-rightwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)     5486 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-upwards.png
--rw-r--r--   0 sping     (1000) sping     (1000)    12328 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-last-two-moves.png
--rw-r--r--   0 sping     (1000) sping     (1000)     5550 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-movement-horse.png
--rw-r--r--   0 sping     (1000) sping     (1000)     7789 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-a4_blank_2cm_margin.png
--rw-r--r--   0 sping     (1000) sping     (1000)    22251 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-cambaluc_remake_nolegend.png
--rw-r--r--   0 sping     (1000) sping     (1000)    21970 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-cambaluc_remake_nolegend_nogap.png
--rw-r--r--   0 sping     (1000) sping     (1000)    21943 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-ccbridge_3_0_beta4_default_preview_remake.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10341 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-clean_alpha.png
--rw-r--r--   0 sping     (1000) sping     (1000)    14591 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-clean_beta.png
--rw-r--r--   0 sping     (1000) sping     (1000)    21234 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-commons_xiangqi_board_2008.png
--rw-r--r--   0 sping     (1000) sping     (1000)    12621 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-commons_xiangqi_board_2008_bw_thin.png
--rw-r--r--   0 sping     (1000) sping     (1000)    25602 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-dhtmlxq_2014_remake.png
--rw-r--r--   0 sping     (1000) sping     (1000)    11325 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-latex_xq_remake.png
--rw-r--r--   0 sping     (1000) sping     (1000)    13808 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-minimal.png
--rw-r--r--   0 sping     (1000) sping     (1000)    12065 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-minimal_chinese.png
--rw-r--r--   0 sping     (1000) sping     (1000)    15325 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-minimal_chinese_arabic.png
--rw-r--r--   0 sping     (1000) sping     (1000)    16687 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-playok_2014_remake.png
--rw-r--r--   0 sping     (1000) sping     (1000)    23254 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-western_red_wine.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10955 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-board-xiexie_2_5_0_remake_minimal.png
--rw-r--r--   0 sping     (1000) sping     (1000)    16442 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-ccbridge_3_0_beta4_default_preview_remake.png
--rw-r--r--   0 sping     (1000) sping     (1000)    23238 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010.png
--rw-r--r--   0 sping     (1000) sping     (1000)    19473 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010_bw_heavy.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10019 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-euro_xiangqi_js.png
--rw-r--r--   0 sping     (1000) sping     (1000)    11315 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-latex_xqlarge_2006_chinese_autotrace.png
--rw-r--r--   0 sping     (1000) sping     (1000)    11321 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-latex_xqlarge_2006_chinese_potrace.png
--rw-r--r--   0 sping     (1000) sping     (1000)    25556 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-playok_2014_chinese.png
--rw-r--r--   0 sping     (1000) sping     (1000)    26223 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-playok_2014_chinese_noshadow.png
--rw-r--r--   0 sping     (1000) sping     (1000)    10341 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/tests/expected-pieces-retro_simple.png
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.520026 xiangqi-setup-2.1.0/xiangqi_board/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2014-08-07 18:59:15.000000 xiangqi-setup-2.1.0/xiangqi_board/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3103 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_board/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6918 2021-02-10 22:05:59.000000 xiangqi-setup-2.1.0/xiangqi_board/painter.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.526026 xiangqi-setup-2.1.0/xiangqi_setup/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2014-08-02 18:54:15.000000 xiangqi-setup-2.1.0/xiangqi_setup/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    11146 2021-05-12 13:06:16.000000 xiangqi-setup-2.1.0/xiangqi_setup/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2433 2021-05-12 13:06:16.000000 xiangqi-setup-2.1.0/xiangqi_setup/annotations.py
--rw-r--r--   0 sping     (1000) sping     (1000)     8665 2021-02-10 22:05:59.000000 xiangqi-setup-2.1.0/xiangqi_setup/compose.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1313 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/default_setup.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.531026 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3869 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/annofen.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1425 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/fen.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.531026 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-01-28 00:14:35.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/tests/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     8949 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/tests/test_wxf.py
--rw-r--r--   0 sping     (1000) sping     (1000)    11230 2021-05-12 13:06:16.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/wxf.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1657 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/file_formats/xay.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4177 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/license.py
--rw-r--r--   0 sping     (1000) sping     (1000)      169 2021-01-22 20:34:41.000000 xiangqi-setup-2.1.0/xiangqi_setup/parties.py
--rw-r--r--   0 sping     (1000) sping     (1000)      714 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/pieces.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.532026 xiangqi-setup-2.1.0/xiangqi_setup/themes/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.532026 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.553026 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/
--rw-r--r--   0 sping     (1000) sping     (1000)      182 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    10329 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11637 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13053 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10325 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11673 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11917 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11647 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_3_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11465 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_4_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_5_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_6_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_7_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_8_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13128 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11985 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11980 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_3.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_4.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11975 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_5.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12081 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_6.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12079 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_7.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12080 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_8.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12077 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_9.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13102 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11930 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_3.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11919 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_4.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11926 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_5.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12031 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_6.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12030 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_7.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_8.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_9.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10334 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13167 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10277 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11648 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11651 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11971 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11646 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11595 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_3_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11520 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_4_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_5_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_6_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_7_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_8_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3499 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_bad.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3510 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_good.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3340 2021-02-07 18:51:24.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_move.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3090 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/config.yml
--rw-r--r--   0 sping     (1000) sping     (1000)     2762 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_bad.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     2766 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_good.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3340 2021-02-07 18:51:24.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_move.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.580026 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/
--rw-r--r--   0 sping     (1000) sping     (1000)      182 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    10329 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11637 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13053 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10325 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11673 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11917 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11647 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_3_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11465 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_4_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_5_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_6_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_7_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_8_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13128 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11985 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11980 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_3.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_4.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11975 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_5.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12081 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_6.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12079 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_7.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12080 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_8.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12077 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_9.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13102 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11930 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_3.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11919 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_4.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11926 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_5.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12031 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_6.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12030 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_7.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_8.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_9.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10334 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13167 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10277 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11648 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11651 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11971 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11646 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_1.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11595 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_2.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_3_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11520 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_4_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_5_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_6_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_7_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_8_plus_0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3490 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_bad.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3501 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_good.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3341 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_move.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3088 2021-02-08 19:58:53.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/config.yml
--rw-r--r--   0 sping     (1000) sping     (1000)     3491 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_bad.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3493 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_good.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3341 2021-02-01 16:26:13.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_move.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.580026 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.582027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/
--rw-r--r--   0 sping     (1000) sping     (1000)      150 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       95 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)     2502 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.584027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/
--rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      304 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       66 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    69687 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.586027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/
--rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      317 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    69366 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.590027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/
--rw-r--r--   0 sping     (1000) sping     (1000)      448 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      468 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       58 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    20901 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.594027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/
--rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      209 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    16761 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.596027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/
--rw-r--r--   0 sping     (1000) sping     (1000)      509 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      458 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       52 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    50491 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.598027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/
--rw-r--r--   0 sping     (1000) sping     (1000)      302 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      110 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)   153580 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.601027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/
--rw-r--r--   0 sping     (1000) sping     (1000)   277925 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/Xiangqi_Board.svg
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.603027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/
--rw-r--r--   0 sping     (1000) sping     (1000)      498 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      289 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      110 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)   153173 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.605027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/original/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.607027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/
--rw-r--r--   0 sping     (1000) sping     (1000)      905 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      639 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       56 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    51310 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.608027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/
--rw-r--r--   0 sping     (1000) sping     (1000)      403 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      292 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    55820 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.609027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    39263 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/original/board-text.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.611027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/
--rw-r--r--   0 sping     (1000) sping     (1000)      345 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      326 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       60 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)     2435 2021-01-22 20:40:28.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.613027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/
--rw-r--r--   0 sping     (1000) sping     (1000)      365 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      341 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    39222 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.616027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/
--rw-r--r--   0 sping     (1000) sping     (1000)      365 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      348 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    33081 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.619027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/
--rw-r--r--   0 sping     (1000) sping     (1000)      364 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      370 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       55 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)     6937 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.622027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/
--rw-r--r--   0 sping     (1000) sping     (1000)      150 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      132 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    22104 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.624027 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/
--rw-r--r--   0 sping     (1000) sping     (1000)      478 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      481 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)       60 2021-02-01 20:46:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    20845 2021-01-22 20:25:21.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.625027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/__init__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.632027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/
--rw-r--r--   0 sping     (1000) sping     (1000)      360 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      257 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3014 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4060 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3384 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4318 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3415 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5265 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3576 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_pawn.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3013 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4059 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3382 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3384 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3494 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4497 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3353 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.643027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/
--rw-r--r--   0 sping     (1000) sping     (1000)      254 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      306 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5477 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9128 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7707 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8708 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8666 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9642 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7362 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.644027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/
--rw-r--r--   0 sping     (1000) sping     (1000)   110377 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/Xiangqi_pieces_print.svg
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6544 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8759 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    16217 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7710 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10360 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8404 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6777 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.651027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/
--rw-r--r--   0 sping     (1000) sping     (1000)      632 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5431 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8878 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7578 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8535 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8499 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9359 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7229 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.651027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6796 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8581 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    16115 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7901 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10296 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     8220 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6661 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_pawn.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     2669 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/diamond.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.659027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/
--rw-r--r--   0 sping     (1000) sping     (1000)      285 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3873 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5794 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4071 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5179 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7845 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5888 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3648 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.661027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    39424 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/euro_xiangqi_js.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3847 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4047 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5022 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4687 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5743 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5678 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     3670 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.666027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/
--rw-r--r--   0 sping     (1000) sping     (1000)   187136 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers.svg
--rw-r--r--   0 sping     (1000) sping     (1000)   163298 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__color.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    24099 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__cut.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.679027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/
--rw-r--r--   0 sping     (1000) sping     (1000)      892 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      567 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     7844 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    18114 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    10942 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    17199 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11680 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    16796 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11543 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.680027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    10923 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    15956 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    14864 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    14465 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    16788 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    15806 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    12971 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.691027 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/
--rw-r--r--   0 sping     (1000) sping     (1000)      892 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      567 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5407 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9494 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6959 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9320 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7741 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     9598 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7603 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.710028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/
--rw-r--r--   0 sping     (1000) sping     (1000)       32 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)     1056 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    76259 2014-08-07 01:17:49.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.pdf
--rw-r--r--   0 sping     (1000) sping     (1000)   141598 2014-08-07 01:17:50.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4220 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-text.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    54321 2014-08-07 01:18:02.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.pdf
--rw-r--r--   0 sping     (1000) sping     (1000)   100510 2014-08-07 01:18:03.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4186 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-text.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      270 2006-10-03 21:07:20.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.mf
--rw-r--r--   0 sping     (1000) sping     (1000)    23204 2014-08-07 01:17:49.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)      270 2006-10-03 21:07:20.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.mf
--rw-r--r--   0 sping     (1000) sping     (1000)    20504 2014-08-07 01:18:02.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.ttf
--rw-r--r--   0 sping     (1000) sping     (1000)    10064 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    15216 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13451 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13985 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    14152 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    13658 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)    11097 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.722028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/
--rw-r--r--   0 sping     (1000) sping     (1000)      560 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      472 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5845 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7258 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6256 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7767 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7068 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7344 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6723 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.733028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        9 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/000.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/001.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/002.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/003.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/004.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/005.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/006.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/010.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/011.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/012.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/013.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/014.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/015.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/016.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      464 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1231 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/a0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     1257 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/b0.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6151 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7567 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6517 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6411 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7342 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6566 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6361 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.742028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/
--rw-r--r--   0 sping     (1000) sping     (1000)      560 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      472 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5848 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7267 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6265 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7776 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7091 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7345 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6732 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.743028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/original/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/original/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6174 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7590 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6540 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6444 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     7365 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6592 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     6624 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_pawn.svg
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.750028 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/
--rw-r--r--   0 sping     (1000) sping     (1000)      307 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/LICENSE.json
--rw-r--r--   0 sping     (1000) sping     (1000)      260 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/LICENSE.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4037 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5484 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4285 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5565 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4391 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5103 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4727 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_pawn.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4372 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_advisor.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     5560 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_cannon.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4416 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_chariot.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4610 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_elephant.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4443 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_horse.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4545 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_king.svg
--rw-r--r--   0 sping     (1000) sping     (1000)     4572 2020-02-12 02:45:51.000000 xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_pawn.svg
--rw-r--r--   0 sping     (1000) sping     (1000)      158 2021-08-03 15:14:56.000000 xiangqi-setup-2.1.0/xiangqi_setup/version.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-08-03 15:15:11.528026 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)    10189 2021-08-03 15:15:10.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)    31655 2021-08-03 15:15:11.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2021-08-03 15:15:10.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)      107 2021-08-03 15:15:10.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       53 2021-08-03 15:15:10.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/requires.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       28 2021-08-03 15:15:10.000000 xiangqi-setup-2.1.0/xiangqi_setup.egg-info/top_level.txt
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.598413 xiangqi-setup-2.2.0/
+-rw-r--r--   0 sping     (1000) sping     (1000)      600 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/.flake8
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.466412 xiangqi-setup-2.2.0/.github/
+-rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-12-21 01:51:42.000000 xiangqi-setup-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.466412 xiangqi-setup-2.2.0/.github/workflows/
+-rw-r--r--   0 sping     (1000) sping     (1000)     2221 2023-07-26 16:11:02.000000 xiangqi-setup-2.2.0/.github/workflows/pre-commit-detect-outdated.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     1068 2023-07-26 16:11:02.000000 xiangqi-setup-2.2.0/.github/workflows/pre-commit-run.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     1642 2023-07-26 16:11:02.000000 xiangqi-setup-2.2.0/.github/workflows/smoke_test.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)       37 2021-08-03 15:14:56.000000 xiangqi-setup-2.2.0/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)       28 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/.isort.cfg
+-rw-r--r--   0 sping     (1000) sping     (1000)      810 2023-07-26 16:11:02.000000 xiangqi-setup-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 sping     (1000) sping     (1000)      178 2022-11-15 20:44:12.000000 xiangqi-setup-2.2.0/.style.yapf
+-rw-r--r--   0 sping     (1000) sping     (1000)      305 2015-05-11 21:44:18.000000 xiangqi-setup-2.2.0/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)    10614 2023-07-26 16:43:26.598413 xiangqi-setup-2.2.0/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     9272 2023-04-17 21:57:59.000000 xiangqi-setup-2.2.0/README.md
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.471412 xiangqi-setup-2.2.0/doc/
+-rw-r--r--   0 sping     (1000) sping     (1000)       17 2015-05-11 20:42:25.000000 xiangqi-setup-2.2.0/doc/.gitignore
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     1174 2015-06-14 21:18:47.000000 xiangqi-setup-2.2.0/doc/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)      666 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/doc/demo-arrows-horse-elephant-advisor.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)      569 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/doc/demo-arrows-rook-downwards.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)      749 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/doc/demo-arrows-rook-leftwards-rightwards.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)      569 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/doc/demo-arrows-rook-upwards.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)      310 2023-07-26 16:25:21.000000 xiangqi-setup-2.2.0/doc/demo-last-two-moves.annofen
+-rw-r--r--   0 sping     (1000) sping     (1000)      442 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/doc/demo-movement-horse.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)      568 2021-01-28 00:14:35.000000 xiangqi-setup-2.2.0/doc/demo-with-history-playok.wxf
+-rw-r--r--   0 sping     (1000) sping     (1000)       70 2021-01-10 17:07:08.000000 xiangqi-setup-2.2.0/doc/demo.fen
+-rw-r--r--   0 sping     (1000) sping     (1000)      160 2021-02-01 19:56:39.000000 xiangqi-setup-2.2.0/doc/demo.wxf
+-rw-r--r--   0 sping     (1000) sping     (1000)    10641 2015-06-14 21:18:47.000000 xiangqi-setup-2.2.0/doc/demo_euro_xiangqi_js.png
+-rw-r--r--   0 sping     (1000) sping     (1000)   128843 2021-02-10 10:05:45.000000 xiangqi-setup-2.2.0/doc/demo_euro_xiangqi_js.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10964 2015-06-14 21:18:47.000000 xiangqi-setup-2.2.0/doc/demo_retro_simple.png
+-rw-r--r--   0 sping     (1000) sping     (1000)   123322 2021-02-10 10:05:45.000000 xiangqi-setup-2.2.0/doc/demo_retro_simple.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7642 2021-04-02 00:50:50.000000 xiangqi-setup-2.2.0/doc/file_formats.md
+-rw-r--r--   0 sping     (1000) sping     (1000)      271 2021-04-01 21:09:11.000000 xiangqi-setup-2.2.0/doc/initial.annofen
+-rw-r--r--   0 sping     (1000) sping     (1000)      159 2021-02-01 19:56:39.000000 xiangqi-setup-2.2.0/doc/initial.wxf
+-rw-r--r--   0 sping     (1000) sping     (1000)      539 2021-04-01 21:09:11.000000 xiangqi-setup-2.2.0/doc/initial.xay
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-07-26 16:43:26.598413 xiangqi-setup-2.2.0/setup.cfg
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     2925 2023-07-26 16:11:02.000000 xiangqi-setup-2.2.0/setup.py
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     2975 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/test-for-rendering-regressions.sh
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.479412 xiangqi-setup-2.2.0/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)    17656 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-horse-elephant-advisor.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10013 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-downwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    14548 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-leftwards-rightwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10143 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-upwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    20270 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-last-two-moves.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10901 2021-02-07 18:27:42.000000 xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-movement-horse.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10122 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-horse-elephant-advisor.png
+-rw-r--r--   0 sping     (1000) sping     (1000)     5438 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-downwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)     8203 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-leftwards-rightwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)     5486 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-upwards.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    12328 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-last-two-moves.png
+-rw-r--r--   0 sping     (1000) sping     (1000)     5550 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-movement-horse.png
+-rw-r--r--   0 sping     (1000) sping     (1000)     7789 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-a4_blank_2cm_margin.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    22251 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-cambaluc_remake_nolegend.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    21970 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-cambaluc_remake_nolegend_nogap.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    21943 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-ccbridge_3_0_beta4_default_preview_remake.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10341 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-clean_alpha.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    14591 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-clean_beta.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    21234 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-commons_xiangqi_board_2008.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    12621 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-commons_xiangqi_board_2008_bw_thin.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    25602 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-dhtmlxq_2014_remake.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    11325 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-latex_xq_remake.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    13808 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-minimal.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    12065 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-minimal_chinese.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    15325 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-minimal_chinese_arabic.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    16687 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-playok_2014_remake.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    23254 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-western_red_wine.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10955 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-board-xiexie_2_5_0_remake_minimal.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    16442 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-ccbridge_3_0_beta4_default_preview_remake.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    23238 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    19473 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010_bw_heavy.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10019 2023-03-16 04:22:48.000000 xiangqi-setup-2.2.0/tests/expected-pieces-euro_xiangqi_js.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    19623 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/tests/expected-pieces-euro_xiangqi_js_tricolor.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    11315 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-latex_xqlarge_2006_chinese_autotrace.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    11321 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-latex_xqlarge_2006_chinese_potrace.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    25556 2023-03-16 04:22:48.000000 xiangqi-setup-2.2.0/tests/expected-pieces-playok_2014_chinese.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    26223 2023-03-16 04:22:48.000000 xiangqi-setup-2.2.0/tests/expected-pieces-playok_2014_chinese_noshadow.png
+-rw-r--r--   0 sping     (1000) sping     (1000)    10341 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/tests/expected-pieces-retro_simple.png
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.479412 xiangqi-setup-2.2.0/xiangqi_board/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2014-08-07 18:59:15.000000 xiangqi-setup-2.2.0/xiangqi_board/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3103 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_board/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6919 2022-03-08 16:02:56.000000 xiangqi-setup-2.2.0/xiangqi_board/painter.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.481413 xiangqi-setup-2.2.0/xiangqi_setup/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2014-08-02 18:54:15.000000 xiangqi-setup-2.2.0/xiangqi_setup/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    11128 2022-11-15 20:44:12.000000 xiangqi-setup-2.2.0/xiangqi_setup/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2580 2023-07-26 16:41:34.000000 xiangqi-setup-2.2.0/xiangqi_setup/annotations.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     8665 2021-02-10 22:05:59.000000 xiangqi-setup-2.2.0/xiangqi_setup/compose.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1313 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/default_setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.483412 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3837 2023-07-26 16:41:34.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/annofen.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1425 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/fen.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.484413 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-01-28 00:14:35.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/tests/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     8951 2022-03-08 16:02:56.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/tests/test_wxf.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    11232 2022-03-08 16:02:56.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/wxf.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1657 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/file_formats/xay.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4177 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/license.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      169 2021-01-22 20:34:41.000000 xiangqi-setup-2.2.0/xiangqi_setup/parties.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      715 2022-03-08 16:02:56.000000 xiangqi-setup-2.2.0/xiangqi_setup/pieces.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.484413 xiangqi-setup-2.2.0/xiangqi_setup/themes/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.485412 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.504413 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/
+-rw-r--r--   0 sping     (1000) sping     (1000)      182 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    10329 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11637 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13053 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10325 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11673 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11917 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11647 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_3_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11465 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_4_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_5_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_6_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_7_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_8_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13128 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11985 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11980 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_3.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_4.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11975 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_5.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12081 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_6.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12079 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_7.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12080 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_8.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12077 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_9.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13102 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11930 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_3.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11919 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_4.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11926 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_5.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12031 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_6.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12030 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_7.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_8.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_9.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10334 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13167 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10277 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11648 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11651 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11971 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11646 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11595 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_3_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11520 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_4_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_5_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_6_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_7_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_8_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3499 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_bad.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3510 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_good.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3340 2021-02-07 18:51:24.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_move.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3090 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/config.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     2762 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_bad.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     2766 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_good.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3340 2021-02-07 18:51:24.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_move.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.517413 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/
+-rw-r--r--   0 sping     (1000) sping     (1000)      182 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    10329 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11637 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13053 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10325 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11673 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11917 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11647 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_3_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11465 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_4_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_5_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_6_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11468 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_7_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11467 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_8_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13128 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11985 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11980 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_3.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_4.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11975 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_5.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12081 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_6.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12079 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_7.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12080 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_8.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12077 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_9.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13102 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11968 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11930 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_3.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11919 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_4.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11926 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_5.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12031 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_6.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12030 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_7.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_8.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12028 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_9.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10334 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13167 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10277 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11648 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11651 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11653 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11971 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11646 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_1.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11595 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_2.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11576 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_3_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11520 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_4_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_5_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_6_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11523 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_7_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11522 2021-02-08 19:21:11.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_8_plus_0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3490 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_bad.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3501 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_good.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3341 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_move.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3088 2021-02-08 19:58:53.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/config.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     3491 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_bad.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3493 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_good.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3341 2021-02-01 16:26:13.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_move.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.517413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.518413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/
+-rw-r--r--   0 sping     (1000) sping     (1000)      150 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       95 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)     2502 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.519413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/
+-rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      304 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       66 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    69687 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.520413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/
+-rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      317 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    69366 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.521413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/
+-rw-r--r--   0 sping     (1000) sping     (1000)      448 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      468 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       58 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    20901 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.522413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/
+-rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      209 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    16761 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.523413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/
+-rw-r--r--   0 sping     (1000) sping     (1000)      509 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      458 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       52 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    50491 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.524413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/
+-rw-r--r--   0 sping     (1000) sping     (1000)      302 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      220 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      110 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)   153580 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.525413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)   277925 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/Xiangqi_Board.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.526413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/
+-rw-r--r--   0 sping     (1000) sping     (1000)      498 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      289 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      110 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)   153173 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.527413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/original/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.528413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/
+-rw-r--r--   0 sping     (1000) sping     (1000)      905 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      639 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       56 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    51310 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.529413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/
+-rw-r--r--   0 sping     (1000) sping     (1000)      403 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      292 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    55820 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.530413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    39263 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/original/board-text.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.531413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/
+-rw-r--r--   0 sping     (1000) sping     (1000)      345 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      326 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       60 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)     2435 2021-01-22 20:40:28.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.533413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/
+-rw-r--r--   0 sping     (1000) sping     (1000)      365 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      341 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    39222 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.534413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/
+-rw-r--r--   0 sping     (1000) sping     (1000)      365 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      348 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       68 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    33081 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.535413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/
+-rw-r--r--   0 sping     (1000) sping     (1000)      364 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      370 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       55 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)     6937 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.536413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/
+-rw-r--r--   0 sping     (1000) sping     (1000)      150 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      132 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       56 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    22104 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.537413 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/
+-rw-r--r--   0 sping     (1000) sping     (1000)      478 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      481 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       60 2021-02-01 20:46:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    20845 2021-01-22 20:25:21.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.538413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/__init__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.542413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/
+-rw-r--r--   0 sping     (1000) sping     (1000)      360 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      257 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3014 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4060 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3384 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4318 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3415 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5265 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3576 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_pawn.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3013 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4059 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3382 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3384 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3494 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4497 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3353 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.545413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/
+-rw-r--r--   0 sping     (1000) sping     (1000)      254 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      306 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5477 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9128 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7707 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8708 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8666 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9642 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7362 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.546413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)   110377 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/Xiangqi_pieces_print.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6544 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8759 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    16217 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7710 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10360 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8404 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6777 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.552413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/
+-rw-r--r--   0 sping     (1000) sping     (1000)      632 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      397 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5431 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8878 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7578 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8535 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8499 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9359 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7229 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.552413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6796 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8581 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    16115 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7901 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10296 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     8220 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6661 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_pawn.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     2669 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/diamond.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.557413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/
+-rw-r--r--   0 sping     (1000) sping     (1000)      285 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3873 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5794 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4071 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5179 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7845 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5888 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3648 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.558413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    39424 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/euro_xiangqi_js.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3847 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4047 2023-03-15 01:04:29.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5022 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4687 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5743 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5678 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3670 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.559413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/
+-rw-r--r--   0 sping     (1000) sping     (1000)   187136 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)   163298 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__color.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    24099 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__cut.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.564413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/
+-rw-r--r--   0 sping     (1000) sping     (1000)      285 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4071 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4377 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5274 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4849 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6270 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6129 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3875 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_pawn.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4084 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4341 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5270 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4845 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6266 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6125 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     3871 2023-03-18 19:50:39.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.569413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/
+-rw-r--r--   0 sping     (1000) sping     (1000)      892 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      567 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7844 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    18114 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10942 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    17199 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11680 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    16796 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11543 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.570413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    10923 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    15956 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    14864 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    14465 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    16788 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    15806 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    12971 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.573413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/
+-rw-r--r--   0 sping     (1000) sping     (1000)      892 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      567 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5407 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9494 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6959 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9320 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7741 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     9598 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7603 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.580413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)       32 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)     1056 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    76259 2014-08-07 01:17:49.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.pdf
+-rw-r--r--   0 sping     (1000) sping     (1000)   141598 2014-08-07 01:17:50.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4220 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-text.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    54321 2014-08-07 01:18:02.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.pdf
+-rw-r--r--   0 sping     (1000) sping     (1000)   100510 2014-08-07 01:18:03.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4186 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-text.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      270 2006-10-03 21:07:20.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.mf
+-rw-r--r--   0 sping     (1000) sping     (1000)    23204 2014-08-07 01:17:49.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)      270 2006-10-03 21:07:20.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.mf
+-rw-r--r--   0 sping     (1000) sping     (1000)    20504 2014-08-07 01:18:02.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.ttf
+-rw-r--r--   0 sping     (1000) sping     (1000)    10064 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    15216 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13451 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13985 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    14152 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    13658 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)    11097 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.584413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/
+-rw-r--r--   0 sping     (1000) sping     (1000)      560 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      472 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5845 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7258 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6256 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7767 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7068 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7344 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6723 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.589413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        9 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/000.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/001.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/002.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/003.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/004.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/005.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      384 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/006.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/010.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/011.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/012.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/013.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/014.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/015.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      383 2021-02-01 19:53:54.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/016.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      464 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1231 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/a0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     1257 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/b0.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6151 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7567 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6517 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6411 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7342 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6566 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6361 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.593413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/
+-rw-r--r--   0 sping     (1000) sping     (1000)      560 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      472 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5848 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7267 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6265 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7776 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7091 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7345 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6732 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.593413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/original/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/original/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6174 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7590 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6540 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6444 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     7365 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6592 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     6624 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_pawn.svg
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.597413 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/
+-rw-r--r--   0 sping     (1000) sping     (1000)      307 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/LICENSE.json
+-rw-r--r--   0 sping     (1000) sping     (1000)      260 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/LICENSE.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4037 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5484 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4285 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5565 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4391 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5103 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4727 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_pawn.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4372 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_advisor.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     5560 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_cannon.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4416 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_chariot.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4610 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_elephant.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4443 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_horse.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4545 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_king.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)     4572 2020-02-12 02:45:51.000000 xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_pawn.svg
+-rw-r--r--   0 sping     (1000) sping     (1000)      158 2023-07-26 16:42:27.000000 xiangqi-setup-2.2.0/xiangqi_setup/version.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-07-26 16:43:26.482412 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)    10614 2023-07-26 16:43:25.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)    32801 2023-07-26 16:43:26.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-07-26 16:43:25.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)      106 2023-07-26 16:43:25.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       53 2023-07-26 16:43:25.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/requires.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       28 2023-07-26 16:43:25.000000 xiangqi-setup-2.2.0/xiangqi_setup.egg-info/top_level.txt
```

### Comparing `xiangqi-setup-2.1.0/.flake8` & `xiangqi-setup-2.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/.github/workflows/pre-commit-run.yml` & `xiangqi-setup-2.2.0/.github/workflows/pre-commit-run.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Copyright (C) 2021 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GNU Affero General Public License version 3.0 or later
 
 name: Run pre-commit on all files
 
 on:
-- pull_request
-- push
+  pull_request:
+  push:
+  schedule:
+    - cron: '0 16 * * 5'  # Every Friday 4pm
 
 jobs:
   run_pre_commit:
     name: Run pre-commit on all files
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9  # v3.5.3
 
-      - name: Set up Python 3.9
-        uses: actions/setup-python@v2.2.2
+      - name: Set up Python 3.11
+        uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1  # v4.7.0
         with:
-          python-version: 3.9
+          python-version: 3.11
 
       - name: Install pre-commit
         run: |-
           pip install \
             --disable-pip-version-check \
             --user \
             --no-warn-script-location \
```

### Comparing `xiangqi-setup-2.1.0/.github/workflows/smoke_test.yml` & `xiangqi-setup-2.2.0/.github/workflows/smoke_test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright (C) 2021 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GNU Affero General Public License version 3.0 or later
 
 name: Build and smoke test
 
 on:
-- pull_request
-- push
+  pull_request:
+  push:
+  schedule:
+    - cron: '0 16 * * 5'  # Every Friday 4pm
 
 jobs:
   build_and_test:
     strategy:
       matrix:
-        python-version: [3.6, 3.9]
+        python-version: [3.8, 3.11]
     name: Build and smoke test
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9  # v3.5.3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2.2.2
+        uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1  # v4.7.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install
         run: |-
           sudo apt-get update
           sudo apt-get install --yes --no-install-recommends imagemagick inkscape
```

### Comparing `xiangqi-setup-2.1.0/.pre-commit-config.yaml` & `xiangqi-setup-2.2.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Copyright (C) 2021 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GNU Affero General Public License version 3.0 or later
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.23.2
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
-        args: ['--py36-plus']
+        args: ['--py38-plus']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: check-json
       - id: check-yaml
       - id: check-merge-conflict
       - id: end-of-file-fixer
         exclude: '\.svg$'
       - id: trailing-whitespace
         exclude: '\.wxf$'
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
 
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.9.3
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/google/yapf
-    rev: v0.31.0
+    rev: v0.40.0
     hooks:
       - id: yapf
```

### Comparing `xiangqi-setup-2.1.0/PKG-INFO` & `xiangqi-setup-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: xiangqi-setup
-Version: 2.1.0
+Version: 2.2.0
 Summary: Command line tool to generate razor-sharp Xiangqi (Chinese chess) setup graphics
 Home-page: https://github.com/hartwork/xiangqi-setup
+Download-URL: https://github.com/hartwork/xiangqi-setup/archive/2.2.0.tar.gz
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GNU Affero General Public License version 3.0 or later
-Download-URL: https://github.com/hartwork/xiangqi-setup/archive/2.1.0.tar.gz
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Build and smoke test](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml/badge.svg)](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml)
+
+
 # xiangqi-setup (and xiangqi-board)
 
 ## Overview
 
 **xiangqi-setup** is a command line tool using [svgutils](https://pypi.org/project/svgutils/) 0.3.4 to
 render [Xiangqi](https://en.wikipedia.org/wiki/Xiangqi) (Chinese chess) board setups from WXF/FEN/[annoFEN](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#annofen)/[XAY](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#xay) files to SVG images.
 With WXF files that contain move history, **xiangqi-setup** can replay these moves on top of the initial setup —
@@ -158,19 +162,20 @@
   minimal                                    (license: CC0-1.0)
   minimal_chinese                            (license: CC0-1.0)
   minimal_chinese_arabic                     (license: CC0-1.0)
   playok_2014_remake                         (license: CC0-1.0)
   western_red_wine                           (license: CC0-1.0)
   xiexie_2_5_0_remake_minimal                (license: CC0-1.0)
 
-piece themes (9 available, in alphabetic order):
+piece themes (10 available, in alphabetic order):
   ccbridge_3_0_beta4_default_preview_remake  (license: CC0-1.0)
   commons_xiangqi_pieces_print_2010          (license: FDL-1.2+ / CC-BY-SA-4.0)
   commons_xiangqi_pieces_print_2010_bw_heavy (license: FDL-1.2+ / CC-BY-SA-4.0)
   euro_xiangqi_js                            (license: CC-BY-4.0)
+  euro_xiangqi_js_tricolor                   (license: CC-BY-4.0)
   latex_xqlarge_2006_chinese_autotrace       (license: non-commercial)
   latex_xqlarge_2006_chinese_potrace         (license: non-commercial)
   playok_2014_chinese                        (license: CC0-1.0)
   playok_2014_chinese_noshadow               (license: CC0-1.0)
   retro_simple                               (license: CC0-1.0)
 
 annotation themes (2 available, in alphabetic order):
@@ -212,9 +217,7 @@
                         Width of starting position cross segments in pixel
                         (default: 10)
   --cross-thickness-px FLOAT
                         Line thickness of starting position cross in pixel
                         (default: 1)
   --cross-gap-px FLOAT  Gap to starting position cross in pixel (default: 4)
 ```
-
-
```

### Comparing `xiangqi-setup-2.1.0/README.md` & `xiangqi-setup-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Build and smoke test](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml/badge.svg)](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml)
+
+
 # xiangqi-setup (and xiangqi-board)
 
 ## Overview
 
 **xiangqi-setup** is a command line tool using [svgutils](https://pypi.org/project/svgutils/) 0.3.4 to
 render [Xiangqi](https://en.wikipedia.org/wiki/Xiangqi) (Chinese chess) board setups from WXF/FEN/[annoFEN](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#annofen)/[XAY](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#xay) files to SVG images.
 With WXF files that contain move history, **xiangqi-setup** can replay these moves on top of the initial setup —
@@ -127,19 +131,20 @@
   minimal                                    (license: CC0-1.0)
   minimal_chinese                            (license: CC0-1.0)
   minimal_chinese_arabic                     (license: CC0-1.0)
   playok_2014_remake                         (license: CC0-1.0)
   western_red_wine                           (license: CC0-1.0)
   xiexie_2_5_0_remake_minimal                (license: CC0-1.0)
 
-piece themes (9 available, in alphabetic order):
+piece themes (10 available, in alphabetic order):
   ccbridge_3_0_beta4_default_preview_remake  (license: CC0-1.0)
   commons_xiangqi_pieces_print_2010          (license: FDL-1.2+ / CC-BY-SA-4.0)
   commons_xiangqi_pieces_print_2010_bw_heavy (license: FDL-1.2+ / CC-BY-SA-4.0)
   euro_xiangqi_js                            (license: CC-BY-4.0)
+  euro_xiangqi_js_tricolor                   (license: CC-BY-4.0)
   latex_xqlarge_2006_chinese_autotrace       (license: non-commercial)
   latex_xqlarge_2006_chinese_potrace         (license: non-commercial)
   playok_2014_chinese                        (license: CC0-1.0)
   playok_2014_chinese_noshadow               (license: CC0-1.0)
   retro_simple                               (license: CC0-1.0)
 
 annotation themes (2 available, in alphabetic order):
```

### Comparing `xiangqi-setup-2.1.0/doc/Makefile` & `xiangqi-setup-2.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo-arrows-horse-elephant-advisor.xay` & `xiangqi-setup-2.2.0/doc/demo-arrows-horse-elephant-advisor.xay`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo-arrows-rook-downwards.xay` & `xiangqi-setup-2.2.0/doc/demo-arrows-rook-downwards.xay`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo-arrows-rook-leftwards-rightwards.xay` & `xiangqi-setup-2.2.0/doc/demo-arrows-rook-leftwards-rightwards.xay`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo-arrows-rook-upwards.xay` & `xiangqi-setup-2.2.0/doc/demo-arrows-rook-upwards.xay`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo-with-history-playok.wxf` & `xiangqi-setup-2.2.0/doc/demo-with-history-playok.wxf`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo_euro_xiangqi_js.png` & `xiangqi-setup-2.2.0/doc/demo_euro_xiangqi_js.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo_euro_xiangqi_js.svg` & `xiangqi-setup-2.2.0/doc/demo_euro_xiangqi_js.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo_retro_simple.png` & `xiangqi-setup-2.2.0/doc/demo_retro_simple.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/demo_retro_simple.svg` & `xiangqi-setup-2.2.0/doc/demo_retro_simple.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/file_formats.md` & `xiangqi-setup-2.2.0/doc/file_formats.md`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/doc/initial.xay` & `xiangqi-setup-2.2.0/doc/initial.xay`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/setup.py` & `xiangqi-setup-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,15 @@
         for root, dirs, files in os.walk('xiangqi_setup/themes')
     }
 
 
 if __name__ == '__main__':
     setup(
         name='xiangqi-setup',
-        description=
-        'Command line tool to generate razor-sharp Xiangqi (Chinese chess) setup graphics',
+        description='Command line tool to generate razor-sharp Xiangqi (Chinese chess) setup graphics',
         long_description=open('README.md').read(),
         long_description_content_type='text/markdown',
         license='GNU Affero General Public License version 3.0 or later',
         version=VERSION_STR,
         author='Sebastian Pipping',
         author_email='sebastian@pipping.org',
         url='https://github.com/hartwork/xiangqi-setup',
@@ -42,15 +41,15 @@
         package_data=_generate_package_data(),
         entry_points={
             'console_scripts': [
                 'xiangqi-board = xiangqi_board.__main__:main',
                 'xiangqi-setup = xiangqi_setup.__main__:main',
             ],
         },
-        python_requires='>=3.6',
+        python_requires='>=3.8',
         setup_requires=[
             'setuptools>=38.6.0',  # for long_description_content_type
         ],
         install_requires=[
             'pyyaml',
             # NOTE: svgutils 0.3.2 was incompatible to 0.3.1 plus semver guarantees
             #       start from >=1.0.0 only (rule 4) so svgutils is pinned here.
@@ -64,17 +63,18 @@
             'Environment :: Console',
             'Intended Audience :: Education',
             'Intended Audience :: Other Audience',
             'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
             'Natural Language :: English',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.6',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Programming Language :: Python :: 3 :: Only',
             'Topic :: Artistic Software',
             'Topic :: Games/Entertainment :: Board Games',
             'Topic :: Multimedia :: Graphics',
             'Topic :: Printing',
             'Topic :: Utilities',
         ],
```

### Comparing `xiangqi-setup-2.1.0/test-for-rendering-regressions.sh` & `xiangqi-setup-2.2.0/test-for-rendering-regressions.sh`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 set -e
 set -x
 
 any_file_missing=0
 
 convert -version
 
-assert_images_identical() {
+assert_images_equal_enough() {
     local a="${1}"
     local b="${2}"
     local diff_output="${3}"
-    compare -metric AE "${a}" "${b}" "${diff_output}"
+    local diff_pixel_count="$(compare -metric AE "${a}" "${b}" "${diff_output}" 2>&1)"
+    [[ "${diff_pixel_count}" =~ [0-9]+ && "${diff_pixel_count}" -le 8 ]]
 }
 
 render_and_compare() {
     local theme_type="${1}"
     local theme_name="${2}"
     local input_file="${3:-doc/demo.wxf}"
     local suffix="${4:-}"
@@ -25,15 +26,15 @@
     local prefix_expected="tests/expected-${theme_type}-${theme_name}${suffix}"
     local prefix_difference="tests/difference-${theme_type}-${theme_name}${suffix}"
 
     if [[ -e "${prefix_expected}".png ]]; then
         # We have an image to compare to, so let's do that
         xiangqi-setup "--${theme_type}" "${theme_name}" "${input_file}" "${prefix_actual}".svg > /dev/null
         convert -verbose -background none "${prefix_actual}".{svg,png}
-        assert_images_identical {"${prefix_expected}","${prefix_actual}","${prefix_difference}"}.png
+        assert_images_equal_enough {"${prefix_expected}","${prefix_actual}","${prefix_difference}"}.png
 
         rm "${prefix_actual}".{png,svg}
         rm "${prefix_difference}".png
     else
         # We do not have an image to compare to, so let's generate it and signal failure to the outside
         any_file_missing=1
         xiangqi-setup "--${theme_type}" "${theme_name}" "${input_file}" "${prefix_expected}".svg > /dev/null
```

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-horse-elephant-advisor.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-horse-elephant-advisor.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-downwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-downwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-leftwards-rightwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-leftwards-rightwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-arrows-rook-upwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-arrows-rook-upwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-last-two-moves.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-last-two-moves.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-colors_alpha-movement-horse.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-colors_alpha-movement-horse.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-horse-elephant-advisor.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-horse-elephant-advisor.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-downwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-downwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-leftwards-rightwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-leftwards-rightwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-arrows-rook-upwards.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-arrows-rook-upwards.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-last-two-moves.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-last-two-moves.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-annotations-gray_alpha-movement-horse.png` & `xiangqi-setup-2.2.0/tests/expected-annotations-gray_alpha-movement-horse.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-a4_blank_2cm_margin.png` & `xiangqi-setup-2.2.0/tests/expected-board-a4_blank_2cm_margin.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-cambaluc_remake_nolegend.png` & `xiangqi-setup-2.2.0/tests/expected-board-cambaluc_remake_nolegend.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-cambaluc_remake_nolegend_nogap.png` & `xiangqi-setup-2.2.0/tests/expected-board-cambaluc_remake_nolegend_nogap.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-ccbridge_3_0_beta4_default_preview_remake.png` & `xiangqi-setup-2.2.0/tests/expected-board-ccbridge_3_0_beta4_default_preview_remake.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-clean_alpha.png` & `xiangqi-setup-2.2.0/tests/expected-board-clean_alpha.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-clean_beta.png` & `xiangqi-setup-2.2.0/tests/expected-board-clean_beta.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-commons_xiangqi_board_2008.png` & `xiangqi-setup-2.2.0/tests/expected-board-commons_xiangqi_board_2008.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-commons_xiangqi_board_2008_bw_thin.png` & `xiangqi-setup-2.2.0/tests/expected-board-commons_xiangqi_board_2008_bw_thin.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-dhtmlxq_2014_remake.png` & `xiangqi-setup-2.2.0/tests/expected-board-dhtmlxq_2014_remake.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-latex_xq_remake.png` & `xiangqi-setup-2.2.0/tests/expected-board-latex_xq_remake.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-minimal.png` & `xiangqi-setup-2.2.0/tests/expected-board-minimal.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-minimal_chinese.png` & `xiangqi-setup-2.2.0/tests/expected-board-minimal_chinese.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-minimal_chinese_arabic.png` & `xiangqi-setup-2.2.0/tests/expected-board-minimal_chinese_arabic.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-playok_2014_remake.png` & `xiangqi-setup-2.2.0/tests/expected-board-playok_2014_remake.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-western_red_wine.png` & `xiangqi-setup-2.2.0/tests/expected-board-western_red_wine.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-board-xiexie_2_5_0_remake_minimal.png` & `xiangqi-setup-2.2.0/tests/expected-board-xiexie_2_5_0_remake_minimal.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-ccbridge_3_0_beta4_default_preview_remake.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-ccbridge_3_0_beta4_default_preview_remake.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010_bw_heavy.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-commons_xiangqi_pieces_print_2010_bw_heavy.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-euro_xiangqi_js.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-euro_xiangqi_js.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-latex_xqlarge_2006_chinese_autotrace.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-latex_xqlarge_2006_chinese_autotrace.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-latex_xqlarge_2006_chinese_potrace.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-latex_xqlarge_2006_chinese_potrace.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-playok_2014_chinese.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-playok_2014_chinese.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-playok_2014_chinese_noshadow.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-playok_2014_chinese_noshadow.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/tests/expected-pieces-retro_simple.png` & `xiangqi-setup-2.2.0/tests/expected-pieces-retro_simple.png`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_board/__main__.py` & `xiangqi-setup-2.2.0/xiangqi_board/__main__.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_board/painter.py` & `xiangqi-setup-2.2.0/xiangqi_board/painter.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         ' (https://github.com/btel/svg_utils) first,'
         ' e.g. by running "pip install svgutils==0.3.4".',
         file=sys.stderr)
     sys.exit(1)
 
 
 class BoardPainter:
+
     def __init__(
         self,
         line_thickness_pixel,
         field_width_px,
         field_height_px,
         border_thickness_pixel,
         border_gap_width_pixel,
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/__main__.py` & `xiangqi-setup-2.2.0/xiangqi_setup/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,25 +196,23 @@
                                        ' (default: %(default)s)'))
     scaling_options.add_argument(
         '--scale-pieces',
         dest='piece_scale',
         metavar='FACTOR',
         type=float,
         default=0.9,
-        help=
-        f'factor to scale pieces by ({_PIECE_SCALE_MIN:.1f} to {_PIECE_SCALE_MAX:.1f}, default: %(default)s)'
+        help=f'factor to scale pieces by ({_PIECE_SCALE_MIN:.1f} to {_PIECE_SCALE_MAX:.1f}, default: %(default)s)'
     )
     scaling_options.add_argument(
         '--scale-annotations',
         dest='annotation_scale',
         metavar='FACTOR',
         type=float,
         default=0.9,
-        help=
-        f'factor to scale annotations by ({_PIECE_SCALE_MIN:.1f} to {_PIECE_SCALE_MAX:.1f}, default: %(default)s)'
+        help=f'factor to scale annotations by ({_PIECE_SCALE_MIN:.1f} to {_PIECE_SCALE_MAX:.1f}, default: %(default)s)'
     )
 
     wxf_options = parser.add_argument_group('WXF format arguments')
     wxf_options.add_argument('--moves',
                              default='0',
                              dest='moves_to_play',
                              metavar='COUNT',
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/annotations.py` & `xiangqi-setup-2.2.0/xiangqi_setup/annotations.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,11 +61,18 @@
     'pb': 'piece_bad',
     'pg': 'piece_good',
     'pm': ANNOTATION_NAME_PIECE_MOVE,
 }
 
 
 class PutAnnotation:
+
     def __init__(self, annotation_name: str, x: float, y: float):
         self.annotation_name = annotation_name
         self.x = x
         self.y = y
+
+
+class InvalidAnnotationCode(ValueError):
+
+    def __init__(self, atom_code):
+        super().__init__(f'Invalid annotation code {atom_code!r}')
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/compose.py` & `xiangqi-setup-2.2.0/xiangqi_setup/compose.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/default_setup.py` & `xiangqi-setup-2.2.0/xiangqi_setup/default_setup.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/file_formats/annofen.py` & `xiangqi-setup-2.2.0/xiangqi_setup/file_formats/annofen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # Copyright (C) 2021 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GNU Affero General Public License version 3.0 or later
 
 import re
 
-from ..annotations import ANNOTATION_NAME_OF_ATOM_CODE, PutAnnotation
+from ..annotations import ANNOTATION_NAME_OF_ATOM_CODE, InvalidAnnotationCode, PutAnnotation
 from ..parties import BLACK, RED
 from ..pieces import PutPiece
 from .fen import PIECE_OF_UPPER_LETTER
 
 _piece_letters = list(
     PIECE_OF_UPPER_LETTER.keys()) + [letter.lower() for letter in PIECE_OF_UPPER_LETTER.keys()]
-_escaped_annotation_names = [
-    re.escape(atom_code) for atom_code in ANNOTATION_NAME_OF_ATOM_CODE.keys()
-]
-
 _single_piece_pattern = '[' + ''.join(_piece_letters) + ']'
-_single_annotation_pattern = '<(?:' + '|'.join(_escaped_annotation_names) + ')>'
+_single_annotation_pattern = '<(?:[^>]+)>'
 _single_annotation_plus_capture_pattern = _single_annotation_pattern.replace(
     '(?:', '(?P<atom_code>')
 _atom_pattern = f'(?:{_single_piece_pattern}|{_single_annotation_pattern})'
 _stacked_atoms_pattern = '\\[(?P<atoms>(?:' + _atom_pattern + ')+)\\]'
 
 _annofen_tokens_pattern = '(?:' + '|'.join(f'(?P<{name}>{pattern})' for name, pattern in (
     ('end_of_row', '/'),
@@ -37,21 +33,25 @@
 
 
 def is_annofen_content(content: str) -> bool:
     return any(line.startswith('v1 ') for line in content.split('\n'))
 
 
 def iterate_annofen_tokens(content: str):
+
     def _create_piece(x: int, y: int, letter: str) -> PutPiece:
         party = BLACK if letter.islower() else RED
         piece = PIECE_OF_UPPER_LETTER[letter.upper()]
         return PutPiece(party, piece, x, y)
 
     def _create_annotation(x: int, y: int, atom_code: str) -> PutAnnotation:
-        annotation_name = ANNOTATION_NAME_OF_ATOM_CODE[atom_code]
+        try:
+            annotation_name = ANNOTATION_NAME_OF_ATOM_CODE[atom_code]
+        except KeyError:
+            raise InvalidAnnotationCode(atom_code)
         return PutAnnotation(annotation_name=annotation_name, x=x, y=y)
 
     seen_fen_before = False
     for i, line in enumerate(content.split('\n')):
         line = line.strip()
 
         if line.startswith('#') or not line:
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/file_formats/fen.py` & `xiangqi-setup-2.2.0/xiangqi_setup/file_formats/fen.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/file_formats/tests/test_wxf.py` & `xiangqi-setup-2.2.0/xiangqi_setup/file_formats/tests/test_wxf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ...parties import BLACK, RED
 from ...pieces import ADVISOR, CANNON, CHARIOT, ELEPHANT, HORSE, KING, PAWN, PutPiece
 from ..fen import PIECE_OF_UPPER_LETTER
 from ..wxf import _Board, _PlayerRelativeView
 
 
 class PlayerRelativeViewTest(TestCase):
+
     @parameterized.expand([
         (RED, 1, 8),
         (RED, 9, 0),
         (BLACK, 1, 0),
         (BLACK, 9, 8),
     ])
     def test_x_index_from(self, party, player_relative_x_pos, expected_internal_x_index):
@@ -46,14 +47,15 @@
                                                         *expected_furthest_up_the_board_x_y)
         actual_piece_furthest_up_the_board = sorted(x_y_put_pieces,
                                                     key=view.further_up_the_board_sort_key)[-1]
         self.assertEqual(actual_piece_furthest_up_the_board, expected_piece_furthest_up_the_board)
 
 
 class BoardTest(TestCase):
+
     @parameterized.expand([
         (CHARIOT, RED, (3, 5), '+', '3', (3, 8)),
         (CHARIOT, BLACK, (3, 5), '+', '3', (3, 2)),
         (CHARIOT, RED, (3, 5), '-', '3', (3, 2)),
         (CHARIOT, BLACK, (3, 5), '-', '3', (3, 8)),
         (CHARIOT, RED, (3, 5), '.', '1', (8, 5)),
         (CHARIOT, RED, (3, 5), '.', '9', (0, 5)),
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/file_formats/wxf.py` & `xiangqi-setup-2.2.0/xiangqi_setup/file_formats/wxf.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     -------------------------------  # river
        .     . . . . . . .     .
        .     . . . . . . .     .
        .     . . . . . . .     .
        .     . . . . . . .     .
     (1, ?+9) . . . . . . . (9, ?+9)  # red player home base
     """
+
     def __init__(self, party):
         self._party = party
 
     def x_index_from(self, x: int) -> int:
         if self._party == RED:
             return 9 - x
         else:
@@ -97,14 +98,15 @@
         return y if self._party == RED else -y
 
     def further_up_the_board_sort_key(self, put_piece: PutPiece):
         return self.y_diff_from(put_piece.y)
 
 
 class _Board:
+
     def __init__(self):
         self._board = [[None for _column in range(9)] for _row in range(10)]
         self._move_locations = set()
 
     def put(self, piece: PutPiece):
         self._board[piece.y][piece.x] = piece
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/file_formats/xay.py` & `xiangqi-setup-2.2.0/xiangqi_setup/file_formats/xay.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/license.py` & `xiangqi-setup-2.2.0/xiangqi_setup/license.py`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/pieces.py` & `xiangqi-setup-2.2.0/xiangqi_setup/pieces.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 KING, \
 CANNON, \
 PAWN, \
 = list(range(7))
 
 
 class PutPiece:
+
     def __init__(self, party, piece, x, y):
         self.party = party
         self.piece = piece
         self.x = x
         self.y = y
 
     def __str__(self):
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_1_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_2_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_3_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_3_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_4_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_4_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_5_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_5_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_6_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_6_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_7_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_7_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_8_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_minus_8_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_3.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_3.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_4.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_4.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_5.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_5.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_6.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_6.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_7.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_7.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_8.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_8.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_9.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_minus_9.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_3.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_3.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_4.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_4.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_5.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_5.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_6.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_6.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_7.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_7.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_8.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_8.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_9.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_0_plus_9.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_1_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_2_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_3_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_3_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_4_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_4_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_5_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_5_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_6_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_6_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_7_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_7_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_8_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/arrow_plus_8_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_bad.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_bad.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_good.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_good.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/blank_move.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/blank_move.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/config.yml` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/config.yml`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_bad.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_bad.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_good.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_good.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/colors_alpha/piece_move.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/colors_alpha/piece_move.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_1_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_2_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_3_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_3_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_4_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_4_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_5_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_5_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_6_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_6_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_7_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_7_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_8_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_minus_8_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_3.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_3.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_4.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_4.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_5.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_5.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_6.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_6.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_7.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_7.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_8.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_8.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_9.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_minus_9.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_3.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_3.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_4.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_4.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_5.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_5.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_6.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_6.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_7.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_7.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_8.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_8.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_9.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_0_plus_9.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_1_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_minus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_1.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_1.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_2.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_2_plus_2.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_3_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_3_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_4_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_4_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_5_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_5_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_6_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_6_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_7_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_7_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_8_plus_0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/arrow_plus_8_plus_0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_bad.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_bad.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_good.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_good.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/blank_move.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/blank_move.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/config.yml` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/config.yml`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_bad.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_bad.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_good.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_good.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/annotations/gray_alpha/piece_move.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/annotations/gray_alpha/piece_move.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/a4_blank_2cm_margin/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/cambaluc_remake_nolegend_nogap/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/ccbridge_3_0_beta4_default_preview_remake/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_alpha/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_alpha/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/clean_beta/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/clean_beta/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/Xiangqi_Board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008/original/Xiangqi_Board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/commons_xiangqi_board_2008_bw_thin/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.txt` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/dhtmlxq_2014_remake/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/latex_xq_remake/original/board-text.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/latex_xq_remake/original/board-text.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/minimal_chinese_arabic/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/playok_2014_remake/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/playok_2014_remake/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/western_red_wine/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/western_red_wine/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/board/xiexie_2_5_0_remake_minimal/board.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/ccbridge_3_0_beta4_default_preview_remake/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/Xiangqi_pieces_print.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/original/Xiangqi_pieces_print.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/commons_xiangqi_pieces_print_2010_bw_heavy/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/diamond.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/diamond.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/euro_xiangqi_js.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/original/euro_xiangqi_js.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__color.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__color.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__cut.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__cut.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.txt` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.txt` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/Makefile` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/Makefile`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.pdf` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.pdf`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-path.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-text.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-autotrace-text.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.pdf` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.pdf`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-path.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-text.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/chinese-potrace-text.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.ttf` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-autotrace.ttf`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.ttf` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/original/xqlarge-potrace.ttf`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_potrace/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/a0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/a0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/b0.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/original/b0.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.json` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/LICENSE.json`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/playok_2014_chinese_noshadow/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/black_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/black_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_advisor.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_advisor.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_cannon.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_cannon.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_chariot.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_chariot.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_elephant.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_elephant.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_horse.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_horse.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_king.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_king.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup/themes/pieces/retro_simple/red_pawn.svg` & `xiangqi-setup-2.2.0/xiangqi_setup/themes/pieces/retro_simple/red_pawn.svg`

 * *Files identical despite different names*

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup.egg-info/PKG-INFO` & `xiangqi-setup-2.2.0/xiangqi_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: xiangqi-setup
-Version: 2.1.0
+Version: 2.2.0
 Summary: Command line tool to generate razor-sharp Xiangqi (Chinese chess) setup graphics
 Home-page: https://github.com/hartwork/xiangqi-setup
+Download-URL: https://github.com/hartwork/xiangqi-setup/archive/2.2.0.tar.gz
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GNU Affero General Public License version 3.0 or later
-Download-URL: https://github.com/hartwork/xiangqi-setup/archive/2.1.0.tar.gz
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Build and smoke test](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml/badge.svg)](https://github.com/hartwork/xiangqi-setup/actions/workflows/smoke_test.yml)
+
+
 # xiangqi-setup (and xiangqi-board)
 
 ## Overview
 
 **xiangqi-setup** is a command line tool using [svgutils](https://pypi.org/project/svgutils/) 0.3.4 to
 render [Xiangqi](https://en.wikipedia.org/wiki/Xiangqi) (Chinese chess) board setups from WXF/FEN/[annoFEN](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#annofen)/[XAY](https://github.com/hartwork/xiangqi-setup/blob/master/doc/file_formats.md#xay) files to SVG images.
 With WXF files that contain move history, **xiangqi-setup** can replay these moves on top of the initial setup —
@@ -158,19 +162,20 @@
   minimal                                    (license: CC0-1.0)
   minimal_chinese                            (license: CC0-1.0)
   minimal_chinese_arabic                     (license: CC0-1.0)
   playok_2014_remake                         (license: CC0-1.0)
   western_red_wine                           (license: CC0-1.0)
   xiexie_2_5_0_remake_minimal                (license: CC0-1.0)
 
-piece themes (9 available, in alphabetic order):
+piece themes (10 available, in alphabetic order):
   ccbridge_3_0_beta4_default_preview_remake  (license: CC0-1.0)
   commons_xiangqi_pieces_print_2010          (license: FDL-1.2+ / CC-BY-SA-4.0)
   commons_xiangqi_pieces_print_2010_bw_heavy (license: FDL-1.2+ / CC-BY-SA-4.0)
   euro_xiangqi_js                            (license: CC-BY-4.0)
+  euro_xiangqi_js_tricolor                   (license: CC-BY-4.0)
   latex_xqlarge_2006_chinese_autotrace       (license: non-commercial)
   latex_xqlarge_2006_chinese_potrace         (license: non-commercial)
   playok_2014_chinese                        (license: CC0-1.0)
   playok_2014_chinese_noshadow               (license: CC0-1.0)
   retro_simple                               (license: CC0-1.0)
 
 annotation themes (2 available, in alphabetic order):
@@ -212,9 +217,7 @@
                         Width of starting position cross segments in pixel
                         (default: 10)
   --cross-thickness-px FLOAT
                         Line thickness of starting position cross in pixel
                         (default: 1)
   --cross-gap-px FLOAT  Gap to starting position cross in pixel (default: 4)
 ```
-
-
```

### Comparing `xiangqi-setup-2.1.0/xiangqi_setup.egg-info/SOURCES.txt` & `xiangqi-setup-2.2.0/xiangqi_setup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 tests/expected-board-playok_2014_remake.png
 tests/expected-board-western_red_wine.png
 tests/expected-board-xiexie_2_5_0_remake_minimal.png
 tests/expected-pieces-ccbridge_3_0_beta4_default_preview_remake.png
 tests/expected-pieces-commons_xiangqi_pieces_print_2010.png
 tests/expected-pieces-commons_xiangqi_pieces_print_2010_bw_heavy.png
 tests/expected-pieces-euro_xiangqi_js.png
+tests/expected-pieces-euro_xiangqi_js_tricolor.png
 tests/expected-pieces-latex_xqlarge_2006_chinese_autotrace.png
 tests/expected-pieces-latex_xqlarge_2006_chinese_potrace.png
 tests/expected-pieces-playok_2014_chinese.png
 tests/expected-pieces-playok_2014_chinese_noshadow.png
 tests/expected-pieces-retro_simple.png
 xiangqi_board/__init__.py
 xiangqi_board/__main__.py
@@ -372,14 +373,30 @@
 xiangqi_setup/themes/pieces/euro_xiangqi_js/red_king.svg
 xiangqi_setup/themes/pieces/euro_xiangqi_js/red_pawn.svg
 xiangqi_setup/themes/pieces/euro_xiangqi_js/original/__init__.py
 xiangqi_setup/themes/pieces/euro_xiangqi_js/original/euro_xiangqi_js.svg
 xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers.svg
 xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__color.svg
 xiangqi_setup/themes/pieces/euro_xiangqi_js/stickers/euro_xiangqi_js_stickers__cut.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/LICENSE.json
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/__init__.py
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_advisor.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_cannon.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_chariot.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_elephant.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_horse.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_king.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/black_pawn.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_advisor.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_cannon.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_chariot.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_elephant.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_horse.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_king.svg
+xiangqi_setup/themes/pieces/euro_xiangqi_js_tricolor/red_pawn.svg
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.json
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/LICENSE.txt
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/__init__.py
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_advisor.svg
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_cannon.svg
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_chariot.svg
 xiangqi_setup/themes/pieces/latex_xqlarge_2006_chinese_autotrace/black_elephant.svg
```

