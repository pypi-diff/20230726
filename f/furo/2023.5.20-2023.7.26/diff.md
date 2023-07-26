# Comparing `tmp/furo-2023.5.20.tar.gz` & `tmp/furo-2023.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furo-2023.5.20.tar", last modified: Sat May 20 08:55:19 2023, max compression
+gzip compressed data, was "furo-2023.7.26.tar", last modified: Wed Jul 26 18:50:32 2023, max compression
```

## Comparing `furo-2023.5.20.tar` & `furo-2023.7.26.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 08:55:19.653102 furo-2023.5.20/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2023.5.20/CODE_OF_CONDUCT.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2023.5.20/LICENSE
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2023.5.20/README.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 16:46:08.985680 furo-2023.5.20/docs/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2023.5.20/docs/_static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2023.5.20/docs/_static/demo-dark.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2023.5.20/docs/_static/demo-light.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2023.5.20/docs/_static/demo.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2023.5.20/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2023.5.20/docs/_static/readthedocs-dummy.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    18926 2023-05-20 08:54:08.268498 furo-2023.5.20/docs/changelog.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2023-03-27 09:59:45.158525 furo-2023.5.20/docs/conf.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2023.5.20/docs/contributing/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2023.5.20/docs/contributing/design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2023.5.20/docs/contributing/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2023.5.20/docs/contributing/internals.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2023.5.20/docs/contributing/workflow.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 06:29:53.184727 furo-2023.5.20/docs/customisation/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2023.5.20/docs/customisation/announcement.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2023.5.20/docs/customisation/colors.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2023.5.20/docs/customisation/edit-button.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2023.5.20/docs/customisation/fonts.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5214 2023-03-27 09:59:45.158893 furo-2023.5.20/docs/customisation/footer.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2023.5.20/docs/customisation/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2023.5.20/docs/customisation/injecting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      971 2022-12-07 02:12:20.995118 furo-2023.5.20/docs/customisation/landing-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2023.5.20/docs/customisation/logo.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2023.5.20/docs/customisation/sidebar-title.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2023.5.20/docs/customisation/sidebar.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2023.5.20/docs/customisation/toc.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2023.5.20/docs/index.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:39.133954 furo-2023.5.20/docs/kitchen-sink/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2022-12-07 02:12:20.995648 furo-2023.5.20/docs/kitchen-sink/admonitions.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2023.5.20/docs/kitchen-sink/api.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8110 2023-02-25 11:34:51.779610 furo-2023.5.20/docs/kitchen-sink/blocks.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2023.5.20/docs/kitchen-sink/generic.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2023.5.20/docs/kitchen-sink/images.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2023.5.20/docs/kitchen-sink/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2023.5.20/docs/kitchen-sink/lists.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12983 2023-03-23 23:04:54.882119 furo-2023.5.20/docs/kitchen-sink/really-long.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2023.5.20/docs/kitchen-sink/sphinx-design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2023.5.20/docs/kitchen-sink/structure.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5068 2022-12-07 02:12:20.996744 furo-2023.5.20/docs/kitchen-sink/tables.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2023.5.20/docs/kitchen-sink/typography.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2022-12-07 02:12:20.996914 furo-2023.5.20/docs/license.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2023.5.20/docs/quickstart.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2023.5.20/docs/recommendations.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2023.5.20/docs/reference/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2023.5.20/docs/reference/admonitions.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2023.5.20/docs/reference/api.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2023.5.20/docs/reference/code-blocks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2023.5.20/docs/reference/hyperlinks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1922 2022-12-07 02:12:20.997623 furo-2023.5.20/docs/reference/images.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2023.5.20/docs/reference/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2023.5.20/docs/reference/lists.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2023.5.20/docs/reference/tables.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2023.5.20/docs/reference/tabs.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2023.5.20/docs/reference/text-formatting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2023.5.20/docs/requirements.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2023.5.20/docs/stability.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4588 2023-05-20 06:29:59.350803 furo-2023.5.20/noxfile.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)   120224 2023-05-20 06:36:37.700979 furo-2023.5.20/package-lock.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)      421 2023-03-27 12:04:35.297935 furo-2023.5.20/package.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2023.5.20/postcss.config.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1342 2023-05-20 06:34:19.599411 furo-2023.5.20/pyproject.toml
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2023.5.20/src/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 06:29:53.185006 furo-2023.5.20/src/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)    14114 2023-05-20 08:55:13.356395 furo-2023.5.20/src/furo/__init__.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1448 2022-12-07 02:12:21.002879 furo-2023.5.20/src/furo/_demo_module.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2023.5.20/src/furo/assets/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003142 furo-2023.5.20/src/furo/assets/scripts/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2022-12-07 02:12:21.003092 furo-2023.5.20/src/furo/assets/scripts/furo.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12991 2022-12-07 02:12:21.003228 furo-2023.5.20/src/furo/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919042 furo-2023.5.20/src/furo/assets/styles/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     9649 2023-02-25 11:33:38.919397 furo-2023.5.20/src/furo/assets/styles/_scaffold.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2023.5.20/src/furo/assets/styles/_shame.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2023.5.20/src/furo/assets/styles/base/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2023.5.20/src/furo/assets/styles/base/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2023.5.20/src/furo/assets/styles/base/_print.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      300 2022-12-07 02:12:21.003967 furo-2023.5.20/src/furo/assets/styles/base/_screen-readers.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2023.5.20/src/furo/assets/styles/base/_theme.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-07 02:12:21.004155 furo-2023.5.20/src/furo/assets/styles/base/_typography.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919529 furo-2023.5.20/src/furo/assets/styles/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2023.5.20/src/furo/assets/styles/components/_footer.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2023.5.20/src/furo/assets/styles/components/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2023.5.20/src/furo/assets/styles/components/_search.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6094 2022-12-07 02:12:21.005360 furo-2023.5.20/src/furo/assets/styles/components/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1832 2022-12-07 02:12:21.005453 furo-2023.5.20/src/furo/assets/styles/components/_table_of_contents.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:43.172691 furo-2023.5.20/src/furo/assets/styles/content/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1933 2022-12-07 02:12:21.005588 furo-2023.5.20/src/furo/assets/styles/content/_admonitions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2360 2023-02-03 20:59:07.304033 furo-2023.5.20/src/furo/assets/styles/content/_api.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2023.5.20/src/furo/assets/styles/content/_blocks.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2023.5.20/src/furo/assets/styles/content/_captions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3199 2023-03-23 22:59:33.724162 furo-2023.5.20/src/furo/assets/styles/content/_code.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      846 2022-12-07 02:12:21.006385 furo-2023.5.20/src/furo/assets/styles/content/_footnotes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2023.5.20/src/furo/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2023.5.20/src/furo/assets/styles/content/_images.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2023.5.20/src/furo/assets/styles/content/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2023.5.20/src/furo/assets/styles/content/_indexes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2023.5.20/src/furo/assets/styles/content/_lists.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2023.5.20/src/furo/assets/styles/content/_math.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2023.5.20/src/furo/assets/styles/content/_misc.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2023.5.20/src/furo/assets/styles/content/_rubrics.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2023.5.20/src/furo/assets/styles/content/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2023.5.20/src/furo/assets/styles/content/_tables.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2022-12-07 02:12:21.007844 furo-2023.5.20/src/furo/assets/styles/content/_target.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2023.5.20/src/furo/assets/styles/extensions/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2023.5.20/src/furo/assets/styles/extensions/_copybutton.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2023.5.20/src/furo/assets/styles/extensions/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2023.5.20/src/furo/assets/styles/extensions/_readthedocs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-design.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-panels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2023.5.20/src/furo/assets/styles/furo-extensions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2023.5.20/src/furo/assets/styles/furo.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.920180 furo-2023.5.20/src/furo/assets/styles/variables/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2023.5.20/src/furo/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6355 2022-12-26 19:15:34.355902 furo-2023.5.20/src/furo/assets/styles/variables/_colors.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1366 2022-12-07 02:12:21.008944 furo-2023.5.20/src/furo/assets/styles/variables/_fonts.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2023.5.20/src/furo/assets/styles/variables/_icons.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2023.5.20/src/furo/assets/styles/variables/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2023.5.20/src/furo/assets/styles/variables/_layout.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2023.5.20/src/furo/assets/styles/variables/_spacing.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2023.5.20/src/furo/navigation.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2395 2022-12-07 02:12:21.009536 furo-2023.5.20/src/furo/sphinxext.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2023.5.20/src/furo/theme/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013802 furo-2023.5.20/src/furo/theme/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3206 2022-12-07 02:12:21.009927 furo-2023.5.20/src/furo/theme/furo/base.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2023.5.20/src/furo/theme/furo/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2023.5.20/src/furo/theme/furo/components/edit-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2023.5.20/src/furo/theme/furo/domainindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2023.5.20/src/furo/theme/furo/genindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2023.5.20/src/furo/theme/furo/globaltoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2023.5.20/src/furo/theme/furo/layout.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2023.5.20/src/furo/theme/furo/localtoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)    11025 2023-02-19 17:22:59.452178 furo-2023.5.20/src/furo/theme/furo/page.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2023.5.20/src/furo/theme/furo/partials/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2023.5.20/src/furo/theme/furo/partials/_head_css_variables.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2023.5.20/src/furo/theme/furo/partials/icons.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2022-12-07 02:12:21.012606 furo-2023.5.20/src/furo/theme/furo/search.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2023.5.20/src/furo/theme/furo/sidebar/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2023.5.20/src/furo/theme/furo/sidebar/brand.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2023.5.20/src/furo/theme/furo/sidebar/ethical-ads.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2023.5.20/src/furo/theme/furo/sidebar/navigation.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2023.5.20/src/furo/theme/furo/sidebar/rtd-versions.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2023.5.20/src/furo/theme/furo/sidebar/scroll-end.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2023.5.20/src/furo/theme/furo/sidebar/scroll-start.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2023.5.20/src/furo/theme/furo/sidebar/search.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2023.5.20/src/furo/theme/furo/sidebar/variant-selector.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2023.5.20/src/furo/theme/furo/static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2023.5.20/src/furo/theme/furo/static/.gitignore
--rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2023.5.20/src/furo/theme/furo/theme.conf
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2023.5.20/webpack.config.js
--rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 furo-2023.5.20/PKG-INFO
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-26 18:50:32.918170 furo-2023.7.26/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2023.7.26/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2023.7.26/LICENSE
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2023.7.26/README.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 16:46:08.985680 furo-2023.7.26/docs/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2023.7.26/docs/_static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2023.7.26/docs/_static/demo-dark.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2023.7.26/docs/_static/demo-light.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2023.7.26/docs/_static/demo.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2023.7.26/docs/_static/pied-piper-admonition.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2023.7.26/docs/_static/readthedocs-dummy.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    19103 2023-07-26 18:49:45.818598 furo-2023.7.26/docs/changelog.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2023-03-27 09:59:45.158525 furo-2023.7.26/docs/conf.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2023.7.26/docs/contributing/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2023.7.26/docs/contributing/design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2023.7.26/docs/contributing/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2023.7.26/docs/contributing/internals.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2023.7.26/docs/contributing/workflow.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 06:29:53.184727 furo-2023.7.26/docs/customisation/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2023.7.26/docs/customisation/announcement.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2023.7.26/docs/customisation/colors.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2023.7.26/docs/customisation/edit-button.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2023.7.26/docs/customisation/fonts.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5214 2023-03-27 09:59:45.158893 furo-2023.7.26/docs/customisation/footer.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2023.7.26/docs/customisation/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2023.7.26/docs/customisation/injecting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      971 2022-12-07 02:12:20.995118 furo-2023.7.26/docs/customisation/landing-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2023.7.26/docs/customisation/logo.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2023.7.26/docs/customisation/sidebar-title.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2023.7.26/docs/customisation/sidebar.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2023.7.26/docs/customisation/toc.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2023.7.26/docs/index.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:39.133954 furo-2023.7.26/docs/kitchen-sink/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2023-07-15 10:12:04.480639 furo-2023.7.26/docs/kitchen-sink/admonitions.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2023.7.26/docs/kitchen-sink/api.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8422 2023-07-15 10:14:34.416633 furo-2023.7.26/docs/kitchen-sink/blocks.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2023.7.26/docs/kitchen-sink/generic.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2023.7.26/docs/kitchen-sink/images.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2023.7.26/docs/kitchen-sink/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2023.7.26/docs/kitchen-sink/lists.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12941 2023-07-02 07:54:47.884930 furo-2023.7.26/docs/kitchen-sink/really-long.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2023.7.26/docs/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2023.7.26/docs/kitchen-sink/structure.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5200 2023-07-15 08:51:23.625580 furo-2023.7.26/docs/kitchen-sink/tables.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2023.7.26/docs/kitchen-sink/typography.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2022-12-07 02:12:20.996914 furo-2023.7.26/docs/license.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2023.7.26/docs/quickstart.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2023.7.26/docs/recommendations.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2023.7.26/docs/reference/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2023.7.26/docs/reference/admonitions.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2023.7.26/docs/reference/api.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2023.7.26/docs/reference/code-blocks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2023.7.26/docs/reference/hyperlinks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2350 2023-07-15 09:18:08.114960 furo-2023.7.26/docs/reference/images.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2023.7.26/docs/reference/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2023.7.26/docs/reference/lists.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2023.7.26/docs/reference/tables.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2023.7.26/docs/reference/tabs.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2023.7.26/docs/reference/text-formatting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2023.7.26/docs/requirements.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2023.7.26/docs/stability.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4588 2023-05-20 06:29:59.350803 furo-2023.7.26/noxfile.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   120224 2023-05-20 06:36:37.700979 furo-2023.7.26/package-lock.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      421 2023-03-27 12:04:35.297935 furo-2023.7.26/package.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2023.7.26/postcss.config.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1342 2023-05-20 06:34:19.599411 furo-2023.7.26/pyproject.toml
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2023.7.26/src/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-07-26 18:43:04.420100 furo-2023.7.26/src/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    14313 2023-07-26 18:50:26.681915 furo-2023.7.26/src/furo/__init__.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1448 2022-12-07 02:12:21.002879 furo-2023.7.26/src/furo/_demo_module.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2023.7.26/src/furo/assets/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003142 furo-2023.7.26/src/furo/assets/scripts/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2022-12-07 02:12:21.003092 furo-2023.7.26/src/furo/assets/scripts/furo.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12991 2022-12-07 02:12:21.003228 furo-2023.7.26/src/furo/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919042 furo-2023.7.26/src/furo/assets/styles/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     9677 2023-07-02 07:56:27.085085 furo-2023.7.26/src/furo/assets/styles/_scaffold.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2023.7.26/src/furo/assets/styles/_shame.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2023.7.26/src/furo/assets/styles/base/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2023.7.26/src/furo/assets/styles/base/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2023.7.26/src/furo/assets/styles/base/_print.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      300 2022-12-07 02:12:21.003967 furo-2023.7.26/src/furo/assets/styles/base/_screen-readers.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2023.7.26/src/furo/assets/styles/base/_theme.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-07 02:12:21.004155 furo-2023.7.26/src/furo/assets/styles/base/_typography.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919529 furo-2023.7.26/src/furo/assets/styles/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2023.7.26/src/furo/assets/styles/components/_footer.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2023.7.26/src/furo/assets/styles/components/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2023.7.26/src/furo/assets/styles/components/_search.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6094 2022-12-07 02:12:21.005360 furo-2023.7.26/src/furo/assets/styles/components/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1832 2023-07-02 07:57:06.099329 furo-2023.7.26/src/furo/assets/styles/components/_table_of_contents.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:43.172691 furo-2023.7.26/src/furo/assets/styles/content/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1945 2023-07-15 08:52:07.005777 furo-2023.7.26/src/furo/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2281 2023-07-02 07:57:07.496021 furo-2023.7.26/src/furo/assets/styles/content/_api.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2023.7.26/src/furo/assets/styles/content/_blocks.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2023.7.26/src/furo/assets/styles/content/_captions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3231 2023-07-15 10:15:52.575334 furo-2023.7.26/src/furo/assets/styles/content/_code.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      846 2022-12-07 02:12:21.006385 furo-2023.7.26/src/furo/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2023.7.26/src/furo/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2023.7.26/src/furo/assets/styles/content/_images.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2023.7.26/src/furo/assets/styles/content/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2023.7.26/src/furo/assets/styles/content/_indexes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2023.7.26/src/furo/assets/styles/content/_lists.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2023.7.26/src/furo/assets/styles/content/_math.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2023.7.26/src/furo/assets/styles/content/_misc.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2023.7.26/src/furo/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2023.7.26/src/furo/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2023.7.26/src/furo/assets/styles/content/_tables.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2022-12-07 02:12:21.007844 furo-2023.7.26/src/furo/assets/styles/content/_target.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2023.7.26/src/furo/assets/styles/extensions/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2023.7.26/src/furo/assets/styles/extensions/_copybutton.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2023.7.26/src/furo/assets/styles/extensions/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2023.7.26/src/furo/assets/styles/extensions/_readthedocs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-design.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-panels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2023.7.26/src/furo/assets/styles/furo-extensions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2023.7.26/src/furo/assets/styles/furo.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.920180 furo-2023.7.26/src/furo/assets/styles/variables/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2023.7.26/src/furo/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6355 2022-12-26 19:15:34.355902 furo-2023.7.26/src/furo/assets/styles/variables/_colors.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1366 2022-12-07 02:12:21.008944 furo-2023.7.26/src/furo/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2023.7.26/src/furo/assets/styles/variables/_icons.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2023.7.26/src/furo/assets/styles/variables/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2023.7.26/src/furo/assets/styles/variables/_layout.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2023.7.26/src/furo/assets/styles/variables/_spacing.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2023.7.26/src/furo/navigation.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2395 2022-12-07 02:12:21.009536 furo-2023.7.26/src/furo/sphinxext.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2023.7.26/src/furo/theme/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013802 furo-2023.7.26/src/furo/theme/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3206 2022-12-07 02:12:21.009927 furo-2023.7.26/src/furo/theme/furo/base.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2023.7.26/src/furo/theme/furo/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2023.7.26/src/furo/theme/furo/components/edit-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2023.7.26/src/furo/theme/furo/domainindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2023.7.26/src/furo/theme/furo/genindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2023.7.26/src/furo/theme/furo/globaltoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2023.7.26/src/furo/theme/furo/layout.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2023.7.26/src/furo/theme/furo/localtoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    11025 2023-02-19 17:22:59.452178 furo-2023.7.26/src/furo/theme/furo/page.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2023.7.26/src/furo/theme/furo/partials/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2023.7.26/src/furo/theme/furo/partials/_head_css_variables.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2023.7.26/src/furo/theme/furo/partials/icons.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2022-12-07 02:12:21.012606 furo-2023.7.26/src/furo/theme/furo/search.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2023.7.26/src/furo/theme/furo/sidebar/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2023.7.26/src/furo/theme/furo/sidebar/brand.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2023.7.26/src/furo/theme/furo/sidebar/ethical-ads.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2023.7.26/src/furo/theme/furo/sidebar/navigation.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2023.7.26/src/furo/theme/furo/sidebar/rtd-versions.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2023.7.26/src/furo/theme/furo/sidebar/scroll-end.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2023.7.26/src/furo/theme/furo/sidebar/scroll-start.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2023.7.26/src/furo/theme/furo/sidebar/search.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2023.7.26/src/furo/theme/furo/sidebar/variant-selector.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2023.7.26/src/furo/theme/furo/static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2023.7.26/src/furo/theme/furo/static/.gitignore
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2023.7.26/src/furo/theme/furo/theme.conf
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2023.7.26/webpack.config.js
+-rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 furo-2023.7.26/PKG-INFO
```

### Comparing `furo-2023.5.20/CODE_OF_CONDUCT.md` & `furo-2023.7.26/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/LICENSE` & `furo-2023.7.26/LICENSE`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/README.md` & `furo-2023.7.26/README.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/_static/demo-dark.png` & `furo-2023.7.26/docs/_static/demo-dark.png`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/_static/demo-light.png` & `furo-2023.7.26/docs/_static/demo-light.png`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/_static/demo.png` & `furo-2023.7.26/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/_static/pied-piper-admonition.css` & `furo-2023.7.26/docs/_static/pied-piper-admonition.css`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/changelog.md` & `furo-2023.7.26/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 date "+## %Y.%m.%d -- {adjective} {colorname}" | pbcopy
 
 https://patternbasedwriting.com/elementary_writing_success/list-4800-adjectives/
 https://en.wikipedia.org/wiki/Lists_of_colors
 
 -->
 
+## 2023.07.26 -- Vigilant Volt
+
+- Fix compatiblity with Sphinx 7.1.
+- Improve how content overflow is handled.
+- Improve how literal blocks containing inline code are handled.
+
 ## 2023.05.20 -- Unassuming Ultramarine
 
 - ✨ Add support for Sphinx 7.
 - Drop support for Sphinx 5.
 - Improve the screen-reader label for sidebar collapse.
 - Make it easier to create derived themes from Furo.
 - Bump all JS dependencies (NodeJS and npm packages).
```

### Comparing `furo-2023.5.20/docs/conf.py` & `furo-2023.7.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/contributing/design.md` & `furo-2023.7.26/docs/contributing/design.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/contributing/index.md` & `furo-2023.7.26/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/contributing/internals.md` & `furo-2023.7.26/docs/contributing/internals.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/contributing/workflow.md` & `furo-2023.7.26/docs/contributing/workflow.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/announcement.md` & `furo-2023.7.26/docs/customisation/announcement.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/colors.md` & `furo-2023.7.26/docs/customisation/colors.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/edit-button.md` & `furo-2023.7.26/docs/customisation/edit-button.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/fonts.md` & `furo-2023.7.26/docs/customisation/fonts.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/footer.md` & `furo-2023.7.26/docs/customisation/footer.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/index.md` & `furo-2023.7.26/docs/customisation/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/injecting.md` & `furo-2023.7.26/docs/customisation/injecting.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/landing-page.md` & `furo-2023.7.26/docs/customisation/landing-page.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/logo.md` & `furo-2023.7.26/docs/customisation/logo.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/sidebar.md` & `furo-2023.7.26/docs/customisation/sidebar.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/customisation/toc.md` & `furo-2023.7.26/docs/customisation/toc.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/admonitions.rst` & `furo-2023.7.26/docs/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/api.rst` & `furo-2023.7.26/docs/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/blocks.rst` & `furo-2023.7.26/docs/kitchen-sink/blocks.rst`

 * *Files 4% similar despite different names*

```diff
@@ -168,14 +168,29 @@
 
 .. parsed-literal::
 
     # parsed-literal test
     curl -O http://someurl/release-0.1.0.tar-gz
     echo "This is an intentionally very long line because I want to make sure that we are handling scrollable code blocks correctly."
 
+    asyncio.set_event_loop_policy(
+        asyncio.WindowsSelectorEventLoopPolicy()
+    )
+
+With inline code
+~~~~~~~~~~~~~~~~
+
+Here's a parsed literal containing nested inline code:
+
+.. parsed-literal::
+
+    :obj:`asyncio.set_event_loop_policy`\ (
+        :obj:`asyncio.WindowsSelectorEventLoopPolicy`\ ()
+    )
+
 Code Block
 ----------
 
 https://docutils.sourceforge.io/docs/ref/rst/directives.html#code
 
     The "code" directive constructs a literal block [containing code].
```

### Comparing `furo-2023.5.20/docs/kitchen-sink/generic.rst` & `furo-2023.7.26/docs/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/images.rst` & `furo-2023.7.26/docs/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/index.md` & `furo-2023.7.26/docs/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/lists.rst` & `furo-2023.7.26/docs/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/really-long.md` & `furo-2023.7.26/docs/kitchen-sink/really-long.md`

 * *Files 4% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 
 Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque sit temporibus cupiditate in ducimus illum assumenda dolor, dignissimos laboriosam voluptate dolorem dolore eum repellendus minima, nisi sequi? Eveniet, dignissimos asperiores!
 
 ## Heading 16 -- this one is also lots of words that would wrap content
 
 Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque sit temporibus cupiditate in ducimus illum assumenda dolor, dignissimos laboriosam voluptate dolorem dolore eum repellendus minima, nisi sequi? Eveniet, dignissimos asperiores!
 
-## Heading 17
+## Heading_17_is_a_really_long_heading_that_is_not_code_and_should_wrap_when_it_reaches_the_sidebar
 
-Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque sit temporibus cupiditate in ducimus illum assumenda dolor, dignissimos laboriosam voluptate dolorem dolore eum repellendus minima, nisi sequi? Eveniet, dignissimos asperiores!
+This_is_a_really_long_sentence_that_is_not_code_and_needs_more_words_and_should_wrap_when_it_reaches_the_sidebar
 
 ## Heading 18
 
 Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque sit temporibus cupiditate in ducimus illum assumenda dolor, dignissimos laboriosam voluptate dolorem dolore eum repellendus minima, nisi sequi? Eveniet, dignissimos asperiores!
 
 ## Heading 19
```

### Comparing `furo-2023.5.20/docs/kitchen-sink/sphinx-design.md` & `furo-2023.7.26/docs/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/structure.rst` & `furo-2023.7.26/docs/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/kitchen-sink/tables.rst` & `furo-2023.7.26/docs/kitchen-sink/tables.rst`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 ==================================== ===========================================
 Version                              Installing
 ==================================== ===========================================
 Pradyun's pip fork and installer     .. code-block:: bash
 
                                         pip install "pip @ git+https://github.com/pradyunsg/pip#20.3.3" "installer @ git+https://github.com/pradyunsg/installer"
 
+                                     .. note::
+
+                                        This is only reasonable if you're Pradyun.
+
 PyPI                                 .. code-block:: bash
 
                                         pip install pip installer
 
 ==================================== ===========================================
 
 List Tables
```

### Comparing `furo-2023.5.20/docs/kitchen-sink/typography.rst` & `furo-2023.7.26/docs/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/recommendations.md` & `furo-2023.7.26/docs/recommendations.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/admonitions.md` & `furo-2023.7.26/docs/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/api.md` & `furo-2023.7.26/docs/reference/api.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/code-blocks.md` & `furo-2023.7.26/docs/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/hyperlinks.md` & `furo-2023.7.26/docs/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/images.md` & `furo-2023.7.26/docs/reference/images.md`

 * *Files 15% similar despite different names*

```diff
@@ -72,24 +72,44 @@
 ```
 
 ```{image} https://source.unsplash.com/200x200/daily?cute+cats
 :align: center
 :class: only-dark
 ```
 
+```{figure} https://source.unsplash.com/200x200/daily?cute+cats
+:align: center
+:figclass: only-light
+```
+
+```{figure} https://source.unsplash.com/200x200/daily?cute+dogs
+:align: center
+:figclass: only-dark
+```
+
 This is from Markdown.
 
 +++
 
 .. image:: https://source.unsplash.com/200x200/daily?cute+dogs
    :align: center
    :class: only-light
 
 
 .. image:: https://source.unsplash.com/200x200/daily?cute+cats
    :align: center
    :class: only-dark
 
 
+.. figure:: https://source.unsplash.com/200x200/daily?cute+cats
+   :align: center
+   :figclass: only-light
+
+
+.. figure:: https://source.unsplash.com/200x200/daily?cute+dogs
+   :align: center
+   :figclass: only-dark
+
+
 This is from reStructuredText.
 
 ````
```

### Comparing `furo-2023.5.20/docs/reference/index.md` & `furo-2023.7.26/docs/reference/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/lists.md` & `furo-2023.7.26/docs/reference/lists.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/tables.md` & `furo-2023.7.26/docs/reference/tables.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/tabs.md` & `furo-2023.7.26/docs/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/reference/text-formatting.md` & `furo-2023.7.26/docs/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/docs/stability.md` & `furo-2023.7.26/docs/stability.md`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/noxfile.py` & `furo-2023.7.26/noxfile.py`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/package-lock.json` & `furo-2023.7.26/package-lock.json`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/pyproject.toml` & `furo-2023.7.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/__init__.py` & `furo-2023.7.26/src/furo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A clean customisable Sphinx documentation theme."""
 
-__version__ = "2023.05.20"
+__version__ = "2023.07.26"
 
 import hashlib
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional
@@ -152,14 +152,19 @@
     full_path = THEME_PATH / "static" / path
     digest = hashlib.sha1(full_path.read_bytes()).hexdigest()
 
     return f"_static/{path}?digest={digest}"
 
 
 def _add_asset_hashes(static: List[str], add_digest_to: List[str]) -> None:
+    if sphinx.version_info >= (7, 1):
+        # https://github.com/sphinx-doc/sphinx/pull/11415 added the relevant
+        # functionality to Sphinx, so we don't need to do anything.
+        return
+
     for asset in add_digest_to:
         index = static.index("_static/" + asset)
         static[index].filename = _asset_hash(asset)  # type: ignore
 
 
 def _html_page_context(
     app: sphinx.application.Sphinx,
```

### Comparing `furo-2023.5.20/src/furo/_demo_module.py` & `furo-2023.7.26/src/furo/_demo_module.py`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/scripts/furo.js` & `furo-2023.7.26/src/furo/assets/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/scripts/gumshoe-patched.js` & `furo-2023.7.26/src/furo/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/_scaffold.sass` & `furo-2023.7.26/src/furo/assets/styles/_scaffold.sass`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
   height: 100%
   color: var(--color-foreground-primary)
   background: var(--color-background-primary)
 
 article
   color: var(--color-content-foreground)
   background: var(--color-content-background)
+  overflow-wrap: break-word
 
 .page
   display: flex
   // fill the viewport for pages with little content.
   min-height: 100%
 
 .mobile-header
```

### Comparing `furo-2023.5.20/src/furo/assets/styles/base/_print.sass` & `furo-2023.7.26/src/furo/assets/styles/base/_print.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/base/_theme.sass` & `furo-2023.7.26/src/furo/assets/styles/base/_theme.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/base/_typography.sass` & `furo-2023.7.26/src/furo/assets/styles/base/_typography.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/components/_footer.sass` & `furo-2023.7.26/src/furo/assets/styles/components/_footer.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/components/_sidebar.sass` & `furo-2023.7.26/src/furo/assets/styles/components/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/components/_table_of_contents.sass` & `furo-2023.7.26/src/furo/assets/styles/components/_table_of_contents.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_admonitions.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_admonitions.sass`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,16 @@
   > :nth-child(2)
     margin-top: 0
 
   // Last item should have no margin, since we'll control that w/ padding
   > :last-child
     margin-bottom: 0
 
-p.admonition-title, p.topic-title
+.admonition p.admonition-title,
+p.topic-title
   position: relative
   margin: 0 -0.5rem 0.5rem
   padding-left: 2rem
   padding-right: .5rem
   padding-top: .4rem
   padding-bottom: .4rem
```

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_api.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_api.sass`

 * *Files 9% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 
   // adjust the size of the [source] link on the right.
   a.reference
     .viewcode-link
       font-weight: normal
       width: 3.5rem
 
-  // Break words when they're too long
-  span.pre
-    overflow-wrap: anywhere
-
 em.property
   font-style: normal
   &:first-child
     color: var(--color-api-keyword)
 .sig-name
   color: var(--color-api-name)
 .sig-prename
```

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_code.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_code.sass`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 code.literal, .sig-inline
   background: var(--color-inline-code-background)
   border-radius: 0.2em
   // Make the font smaller, and use padding to recover.
   font-size: var(--font-size--small--2)
   padding: 0.1em 0.2em
 
-  overflow-wrap: break-word
+  pre.literal-block &
+    font-size: inherit
+    padding: 0
 
   p &
     border: 1px solid var(--color-background-border)
 
 .sig-inline
   font-family: var(--font-stack--monospace)
```

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_footnotes.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_images.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_lists.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_misc.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_sidebar.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_tables.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/content/_target.sass` & `furo-2023.7.26/src/furo/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/extensions/_copybutton.sass` & `furo-2023.7.26/src/furo/assets/styles/extensions/_copybutton.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/extensions/_readthedocs.sass` & `furo-2023.7.26/src/furo/assets/styles/extensions/_readthedocs.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-design.sass` & `furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-design.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass` & `furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-panels.sass` & `furo-2023.7.26/src/furo/assets/styles/extensions/_sphinx-panels.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/variables/_admonitions.scss` & `furo-2023.7.26/src/furo/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/variables/_colors.scss` & `furo-2023.7.26/src/furo/assets/styles/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/variables/_fonts.scss` & `furo-2023.7.26/src/furo/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/variables/_icons.scss` & `furo-2023.7.26/src/furo/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/assets/styles/variables/_spacing.scss` & `furo-2023.7.26/src/furo/assets/styles/variables/_spacing.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/navigation.py` & `furo-2023.7.26/src/furo/navigation.py`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/sphinxext.py` & `furo-2023.7.26/src/furo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/base.html` & `furo-2023.7.26/src/furo/theme/furo/base.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/components/edit-this-page.html` & `furo-2023.7.26/src/furo/theme/furo/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/domainindex.html` & `furo-2023.7.26/src/furo/theme/furo/domainindex.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/genindex.html` & `furo-2023.7.26/src/furo/theme/furo/genindex.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/page.html` & `furo-2023.7.26/src/furo/theme/furo/page.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/partials/_head_css_variables.html` & `furo-2023.7.26/src/furo/theme/furo/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/partials/icons.html` & `furo-2023.7.26/src/furo/theme/furo/partials/icons.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/search.html` & `furo-2023.7.26/src/furo/theme/furo/search.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/sidebar/brand.html` & `furo-2023.7.26/src/furo/theme/furo/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/sidebar/rtd-versions.html` & `furo-2023.7.26/src/furo/theme/furo/sidebar/rtd-versions.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/sidebar/variant-selector.html` & `furo-2023.7.26/src/furo/theme/furo/sidebar/variant-selector.html`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/src/furo/theme/furo/theme.conf` & `furo-2023.7.26/src/furo/theme/furo/theme.conf`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/webpack.config.js` & `furo-2023.7.26/webpack.config.js`

 * *Files identical despite different names*

### Comparing `furo-2023.5.20/PKG-INFO` & `furo-2023.7.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furo
-Version: 2023.5.20
+Version: 2023.7.26
 Summary: A clean customisable Sphinx documentation theme.
 Author-Email: Pradyun Gedam <mail@pradyunsg.me>
 License: Copyright (c) 2020 Pradyun Gedam <mail@pradyunsg.me>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: furo Version: 2023.5.20 Summary: A clean
+Metadata-Version: 2.1 Name: furo Version: 2023.7.26 Summary: A clean
 customisable Sphinx documentation theme. Author-Email: Pradyun Gedam
 pradyunsg.me> License: Copyright (c) 2020 Pradyun Gedam
 pradyunsg.me> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

