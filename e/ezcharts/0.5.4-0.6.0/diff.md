# Comparing `tmp/ezcharts-0.5.4.tar.gz` & `tmp/ezcharts-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.5.4.tar", last modified: Wed Jul 12 14:46:25 2023, max compression
+gzip compressed data, was "ezcharts-0.6.0.tar", last modified: Wed Jul 26 12:44:31 2023, max compression
```

## Comparing `ezcharts-0.5.4.tar` & `ezcharts-0.6.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.276177 ezcharts-0.5.4/
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-07-12 14:41:31.000000 ezcharts-0.5.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-07-12 14:41:31.000000 ezcharts-0.5.4/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-12 14:41:31.000000 ezcharts-0.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5801 2023-07-12 14:46:25.276177 ezcharts-0.5.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-07-12 14:41:31.000000 ezcharts-0.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.228172 ezcharts-0.5.4/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.232173 ezcharts-0.5.4/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/common.py
--rw-rw-rw-   0 root         (0) root         (0)    14124 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/dss.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)    16901 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)    12276 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/modkit.py
--rw-rw-rw-   0 root         (0) root         (0)    13245 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/mosdepth.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.232173 ezcharts-0.5.4/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7295 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/reports/ond.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.212171 ezcharts-0.5.4/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.232173 ezcharts-0.5.4/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/images/OND_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/images/ONT_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)   894078 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/images/dots.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.212171 ezcharts-0.5.4/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.232173 ezcharts-0.5.4/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.232173 ezcharts-0.5.4/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.236173 ezcharts-0.5.4/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)   394601 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/scripts/metagenomics-sankey-util.js
--rw-rw-rw-   0 root         (0) root         (0)    22486 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/scripts/metagenomics-sankey.js
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/scripts/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/scripts/ond.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.236173 ezcharts-0.5.4/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/styles/epi2melabs.scss
--rw-rw-rw-   0 root         (0) root         (0)     2585 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/styles/metagenomics-sankey.css
--rw-rw-rw-   0 root         (0) root         (0)   898896 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/styles/ond.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.244174 ezcharts-0.5.4/ezcharts/data/test/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)  1916228 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/fastcat.stats.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/hg38_some_bands.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)   427338 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/karyomap_vals.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/plot-spec.json
--rwxrwxrwx   0 root         (0) root         (0)      790 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/ref.fa.fai
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/sankey.json
--rw-rw-rw-   0 root         (0) root         (0)  1125122 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_dml.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    35285 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_dmr.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)  1458860 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_modkit.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_modkit_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)     7150 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_mosdepth.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/test_mosdepth_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.244174 ezcharts-0.5.4/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/themes/ond.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.244174 ezcharts-0.5.4/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.212171 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.244174 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.252174 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.256175 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.256175 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.260175 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.260175 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.260175 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.260175 ezcharts-0.5.4/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38201 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)    12531 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.260175 ezcharts-0.5.4/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.264176 ezcharts-0.5.4/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     2119 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7587 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.276177 ezcharts-0.5.4/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)     9172 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/karyomap.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/metagenomics_sankey.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/relational.py
--rwxrwxrwx   0 root         (0) root         (0)     3444 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/sunburst.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-12 14:41:31.000000 ezcharts-0.5.4/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:46:25.228172 ezcharts-0.5.4/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5801 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8876 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:45:00.000000 ezcharts-0.5.4/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-12 14:46:25.000000 ezcharts-0.5.4/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-12 14:41:31.000000 ezcharts-0.5.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:46:25.280177 ezcharts-0.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-07-12 14:41:31.000000 ezcharts-0.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.642672 ezcharts-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-07-26 12:38:53.000000 ezcharts-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-26 12:38:53.000000 ezcharts-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-07-26 12:44:31.642672 ezcharts-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-07-26 12:38:53.000000 ezcharts-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.554664 ezcharts-0.6.0/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.562665 ezcharts-0.6.0/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/bokehchart.py
+-rw-rw-rw-   0 root         (0) root         (0)     6188 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    14124 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/dss.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    16999 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    12869 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/modkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13245 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/mosdepth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.562665 ezcharts-0.6.0/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7295 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.546663 ezcharts-0.6.0/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.570666 ezcharts-0.6.0/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.542663 ezcharts-0.6.0/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.570666 ezcharts-0.6.0/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.570666 ezcharts-0.6.0/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.574666 ezcharts-0.6.0/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)   394601 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/scripts/metagenomics-sankey-util.js
+-rw-rw-rw-   0 root         (0) root         (0)    22486 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/scripts/metagenomics-sankey.js
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/scripts/ond.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.574666 ezcharts-0.6.0/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/styles/metagenomics-sankey.css
+-rw-rw-rw-   0 root         (0) root         (0)   898896 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/styles/ond.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.590667 ezcharts-0.6.0/ezcharts/data/test/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)  1916228 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/fastcat.stats.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/hg38_some_bands.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)   427338 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/karyomap_vals.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/plot-spec.json
+-rwxrwxrwx   0 root         (0) root         (0)      790 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/ref.fa.fai
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/sankey.json
+-rw-rw-rw-   0 root         (0) root         (0)  1125122 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_dml.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    35285 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_dmr.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)  1458860 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_modkit.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_modkit_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_mosdepth.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/test_mosdepth_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.590667 ezcharts-0.6.0/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.590667 ezcharts-0.6.0/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.546663 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.594668 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.602668 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.606669 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.606669 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.614670 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.614670 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.618670 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.618670 ezcharts-0.6.0/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38201 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)    12903 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.618670 ezcharts-0.6.0/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.618670 ezcharts-0.6.0/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7587 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.642672 ezcharts-0.6.0/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)    10263 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/karyomap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/metagenomics_sankey.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/relational.py
+-rwxrwxrwx   0 root         (0) root         (0)     3444 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/sunburst.py
+-rw-rw-rw-   0 root         (0) root         (0)     7208 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-26 12:38:53.000000 ezcharts-0.6.0/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:44:31.554664 ezcharts-0.6.0/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8899 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:43:09.000000 ezcharts-0.6.0/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-26 12:44:31.000000 ezcharts-0.6.0/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-26 12:38:53.000000 ezcharts-0.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 12:44:31.642672 ezcharts-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-07-26 12:38:53.000000 ezcharts-0.6.0/setup.py
```

### Comparing `ezcharts-0.5.4/LICENSE` & `ezcharts-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/PKG-INFO` & `ezcharts-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.5.4
+Version: 0.6.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: LICENSE.md
 
 # ezCharts
 
 (Apologies to non-US English speakers).
 
 ezCharts is a Python library for creating and rendering charts through [eCharts](https://echarts.apache.org/).
 Plots can be contructed through an API similar to [seaborn](https://seaborn.pydata.org/).
```

### Comparing `ezcharts-0.5.4/README.md` & `ezcharts-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/__init__.py` & `ezcharts-0.6.0/ezcharts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.5.4"
+__version__ = "0.6.0"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
```

### Comparing `ezcharts-0.5.4/ezcharts/components/common.py` & `ezcharts-0.6.0/ezcharts/components/common.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/dss.py` & `ezcharts-0.6.0/ezcharts/components/dss.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/ezchart.py` & `ezcharts-0.6.0/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/fastcat.py` & `ezcharts-0.6.0/ezcharts/components/fastcat.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,29 +213,33 @@
         df = util.read_files(seq_summary)[['read_length']]
     else:
         df = seq_summary
 
     mean_length = int(df['read_length'].mean())
     median_length = int(np.median(df['read_length']))
     max_ = int(np.max(df['read_length']))
+    min_ = int(np.min(df['read_length']))
 
     # filter the reads and divide by 1000 to transform into kb
     read_lengths = df['read_length'].values
     if min_len is not None:
         read_lengths = read_lengths[read_lengths >= min_len]
     if max_len is not None:
         read_lengths = read_lengths[read_lengths <= max_len]
     read_lengths = read_lengths / 1000
     if bin_width is not None:
         bin_width /= 1000
 
     plt = ezc.histplot(data=read_lengths, bins=bins, binwidth=bin_width)
     plt.title = dict(
         text=title,
-        subtext=f"Mean: {mean_length:,d}. Median: {median_length:,d}. Max: {max_:,d}"
+        subtext=(
+            f"Mean: {mean_length:,d}. Median: {median_length:,d}. "
+            f"Min: {min_:,d}. Max: {max_:,d}"
+        )
     )
     plt.xAxis.name = 'Read length / kb'
     plt.yAxis.name = 'Number of reads'
 
     if xlim[0] is not None:
         plt.xAxis.min = xlim[0] / 1000
     if xlim[1] is not None:
```

### Comparing `ezcharts-0.5.4/ezcharts/components/modkit.py` & `ezcharts-0.6.0/ezcharts/components/modkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                             with tabs.add_dropdown_tab(sample_id):
                                 DataTable.from_pandas(df_sample, use_index=False)
             # Make modkit bedmethyl karyomap
             if "bedmethyl" in kwargs:
                 if isinstance(kwargs["bedmethyl"], pd.DataFrame):
                     bedmethyl = kwargs["bedmethyl"]
                 else:
-                    bedmethyl = load_bedmethyl(kwargs["bedmethyl"], faidx=faidx)
+                    bedmethyl = load_bedmethyl(
+                        kwargs["bedmethyl"], faidx=faidx, split_all=True)
                 # Check that the file is not empty
                 if bedmethyl.empty:
                     raise pd.errors.EmptyDataError('Bedmethyl is empty')
                 # the following assumes that `fastcat` / `bamstats` has been run
                 # with `-s` which is not necessarily the case (if there was only
                 # one sample) --> create a dummy 'sample_name' column if missing
                 if 'sample_name' not in bedmethyl.columns:
@@ -149,15 +150,15 @@
             if df.empty:
                 cols = relevant_stats_cols_dtypes.update(
                     {'mod': str, 'threshold': str, 'filename': int})
                 dfs.append(pd.DataFrame(columns=cols))
                 continue
             # Convert modification to the appropriate code
             df['mod'] = df.apply(
-                lambda x: MOD_CONVERT.get(x.code, MOD_CONVERT.get(x.base)), axis=1)
+                lambda x: MOD_CONVERT.get(x.code, x.base), axis=1)
             df.astype({'mod': CATEGORICAL})
             # Read and add the thresholds value
             for line in open(f_path):
                 line = line.strip().split()
                 if line[1] == 'pass_threshold_C':
                     threshold = float(line[2])
                     break
@@ -168,25 +169,25 @@
             dfs.append(df)
         except pd.errors.EmptyDataError:
             cols = relevant_stats_cols_dtypes.update({'filename': str})
             dfs.append(pd.DataFrame(columns=cols))
     return pd.concat(dfs).reset_index(drop=True)
 
 
-def load_bedmethyl(bedmethyl_input, faidx=None):
+def load_bedmethyl(bedmethyl_input, faidx=None, split_all=False):
     """Load modkit bedmethyl file.
 
     Input is either a single directory with all the modkit bedmethyls or
     a single modkit bedmethyl file.
 
     Optional inputs can be:
     - faidx: A faidx dataframe with 'chrom' 'length' cols (add missing intervals)
     """
     # Col names
-    relevant_stats_cols_dtypes = {
+    long_cols_dtypes = {
         "chrom": CATEGORICAL,
         "start": int,
         "end": int,
         "mod": CATEGORICAL,
         "score": int,
         "strand": CATEGORICAL,
         "startp": int,
@@ -198,14 +199,26 @@
         "Ncanonical": int,
         "Nother_mod": int,
         "Ndelete": int,
         "Nfail": int,
         "Ndiff": int,
         "Nnocall": int,
     }
+    short_cols_dtypes = {
+        'chrom': CATEGORICAL,
+        'start': int,
+        'end': int,
+        'mod': str,
+        'score': int,
+        'strand': str,
+        'start_p': int,
+        'end_p': int,
+        "colour": CATEGORICAL,
+        'vals': str,
+    }
     # Check inputs
     dfs = []
     if os.path.isdir(bedmethyl_input):
         input_files = [(bedmethyl_input, i) for i in os.listdir(bedmethyl_input)]
     elif os.path.isfile(bedmethyl_input):
         input_files = [(None, bedmethyl_input)]
     else:
@@ -214,27 +227,35 @@
     if len(input_files) == 0:
         raise FileNotFoundError(f'No valid input found in {bedmethyl_input}')
     # Process each file
     for (inpath, fname) in input_files:
         try:
             bedmethyl = fname if not inpath else f'{inpath}/{fname}'
             # Load input bedmethyl
-            df = pd.read_csv(
-                bedmethyl,
-                sep="\t| ",
-                engine='python',
-                names=relevant_stats_cols_dtypes.keys(),
-                dtype=relevant_stats_cols_dtypes)\
-                .drop(columns=['startp', 'endp'])
+            if split_all is True:
+                cols = long_cols_dtypes
+                df = pd.read_csv(
+                    bedmethyl,
+                    sep="\t| ",
+                    engine='python',
+                    names=cols.keys(),
+                    dtype=cols)
+            else:
+                cols = short_cols_dtypes
+                df = pd.read_csv(
+                    bedmethyl,
+                    sep="\t",
+                    engine='python',
+                    names=short_cols_dtypes.keys(),
+                    dtype=short_cols_dtypes)
             # If it's empty, add an empty DF
             if df.empty:
-                cols = relevant_stats_cols_dtypes.update(
+                cols = cols.update(
                     {'total_mean_pos': str, 'filename': int})
-                dfs.append(
-                    pd.DataFrame(columns=cols).drop(columns=['startp', 'endp']))
+                dfs.append(pd.DataFrame(columns=cols))
                 continue
             # If the dataframe is empty, append it directly.
             if isinstance(faidx, pd.DataFrame):
                 if 'length' not in faidx.columns:
                     raise ValueError(
                         'No "length" column found.',
                         'Import the fai with fasta_idx() and try again.')
@@ -257,16 +278,19 @@
             df["total_mean_pos"] = df.apply(
                 lambda x: x.start + total_ref_starts[x.chrom], axis=1)
             # Add file name
             df['filename'] = fname.split('/')[-1]
             # Add to output list
             dfs.append(df)
         except pd.errors.EmptyDataError:
-            cols = relevant_stats_cols_dtypes.update({'filename': str})
-            dfs.append(pd.DataFrame(columns=cols).drop(columns=['startp', 'endp']))
+            if split_all is True:
+                cols = long_cols_dtypes.update({'filename': str})
+            else:
+                cols = short_cols_dtypes.update({'filename': str})
+            dfs.append(pd.DataFrame(columns=cols))
     return pd.concat(dfs).reset_index(drop=True)
 
 
 def main(args):
     """Entry point to demonstrate a modkit component."""
     comp_title = 'ModKit results'
     seq_sum = MKSummary(
```

### Comparing `ezcharts-0.5.4/ezcharts/components/mosdepth.py` & `ezcharts-0.6.0/ezcharts/components/mosdepth.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/nextclade.py` & `ezcharts-0.6.0/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/params.py` & `ezcharts-0.6.0/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/reports/comp.py` & `ezcharts-0.6.0/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/reports/labs.py` & `ezcharts-0.6.0/ezcharts/components/reports/labs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/reports/ond.py` & `ezcharts-0.6.0/ezcharts/components/reports/ond.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/theme.py` & `ezcharts-0.6.0/ezcharts/components/theme.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/components/versions.py` & `ezcharts-0.6.0/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.6.0/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/images/OND_logo.svg` & `ezcharts-0.6.0/ezcharts/data/images/OND_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.6.0/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.6.0/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/images/dots.svg` & `ezcharts-0.6.0/ezcharts/data/images/dots.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.6.0/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.6.0/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.6.0/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/scripts/metagenomics-sankey-util.js` & `ezcharts-0.6.0/ezcharts/data/scripts/metagenomics-sankey-util.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/scripts/metagenomics-sankey.js` & `ezcharts-0.6.0/ezcharts/data/scripts/metagenomics-sankey.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/scripts/ond.js` & `ezcharts-0.6.0/ezcharts/data/scripts/ond.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/styles/epi2melabs.scss` & `ezcharts-0.6.0/ezcharts/data/styles/epi2melabs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/styles/metagenomics-sankey.css` & `ezcharts-0.6.0/ezcharts/data/styles/metagenomics-sankey.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/styles/ond.scss` & `ezcharts-0.6.0/ezcharts/data/styles/ond.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/bamstats.readstats.tsv.gz` & `ezcharts-0.6.0/ezcharts/data/test/bamstats.readstats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/fastcat.stats.gz` & `ezcharts-0.6.0/ezcharts/data/test/fastcat.stats.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.6.0/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.6.0/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/karyomap_vals.tsv.gz` & `ezcharts-0.6.0/ezcharts/data/test/karyomap_vals.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/nextclade.json` & `ezcharts-0.6.0/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/params.json` & `ezcharts-0.6.0/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/plot-spec.json` & `ezcharts-0.6.0/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/ref.fa.fai` & `ezcharts-0.6.0/ezcharts/data/test/ref.fa.fai`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/sankey.json` & `ezcharts-0.6.0/ezcharts/data/test/sankey.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/test_dml.tsv.gz` & `ezcharts-0.6.0/ezcharts/data/test/test_dml.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/test_dmr.tsv.gz` & `ezcharts-0.6.0/ezcharts/data/test/test_dmr.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/test_modkit.bed.gz` & `ezcharts-0.6.0/ezcharts/data/test/test_modkit.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/test/test_mosdepth.bed.gz` & `ezcharts-0.6.0/ezcharts/data/test/test_mosdepth.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.6.0/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/themes/ond.json` & `ezcharts-0.6.0/ezcharts/data/themes/ond.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/themes/walden.json` & `ezcharts-0.6.0/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.6.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.6.0/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.6.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.6.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/demo.py` & `ezcharts-0.6.0/ezcharts/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dominate.tags import p
 import numpy as np
 import pandas as pd
 from pkg_resources import resource_filename
 
 import ezcharts as ezc
 from ezcharts import util
+from ezcharts.components.bokehchart import BokehChart
 from ezcharts.components.common import fasta_idx, HSA_CHROMOSOME_ORDER
 from ezcharts.components.dss import load_dml, load_dmr
 from ezcharts.components.ezchart import EZChart
 from ezcharts.components.fastcat import load_bamstats_flagstat, load_stats
 from ezcharts.components.fastcat import SeqSummary
 from ezcharts.components.modkit import load_bedmethyl, load_modkit_summary
 from ezcharts.components.mosdepth import load_mosdepth_regions, load_mosdepth_summary
@@ -23,15 +24,15 @@
 from ezcharts.layout.snippets import Grid
 from ezcharts.layout.snippets import OffCanvas
 from ezcharts.layout.snippets import Progress
 from ezcharts.layout.snippets import Stats
 from ezcharts.layout.snippets import Tabs
 from ezcharts.layout.snippets.cards import Cards
 from ezcharts.layout.snippets.cards import ICard
-from ezcharts.plots import Plot
+from ezcharts.plots import BokehPlot, Plot
 from ezcharts.plots.ideogram import ideogram
 from ezcharts.plots.karyomap import karyomap
 
 # Setup simple globals
 WORKFLOW_NAME = 'wf-template'
 REPORT_TITLE = f'{WORKFLOW_NAME}-report'
 
@@ -275,15 +276,25 @@
             df = dataset_examples[data_type]
             with tabs.add_tab(data_type):
                 if isinstance(df, tuple) or isinstance(df, tuple):
                     for d in df:
                         DataTable.from_pandas(d.head(10))
                 else:
                     DataTable.from_pandas(df.head(10))
-
+    with report.add_section("Bokeh", "Bokeh"):
+        plot = BokehPlot()
+        plot._fig.circle(
+            [1, 2, 3, 4, 5],
+            [6, 7, 2, 4, 5],
+            size=20,
+            color="navy",
+            alpha=0.5,
+        )
+        plot._fig.title = "Bokeh plot title"
+        BokehChart(plot)
     logger.info('Reticulating splines')
     report.write(args.output)
 
 
 def argparser():
     """Argument parser for entrypoint."""
     parser = argparse.ArgumentParser(
```

### Comparing `ezcharts-0.5.4/ezcharts/layout/base.py` & `ezcharts-0.6.0/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/banner.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/banner.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/cards.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/cards.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/document.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/grid.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/offcanvas.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/progress.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/section.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/stats.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/table.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.6.0/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/layout/util.py` & `ezcharts-0.6.0/ezcharts/layout/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/__init__.py` & `ezcharts-0.6.0/ezcharts/plots/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Plotting functionality via echarts."""
 
 import argparse
 
+from bokeh.plotting import figure
 import pandas as pd
 from pkg_resources import resource_filename
 import sigfig
 
 from ezcharts import util as ezutil
+from ezcharts.components.bokehchart import BokehChart
 from ezcharts.components.ezchart import EZChart
 from ezcharts.components.reports.comp import ComponentReport
 from ezcharts.plots import util
 from ezcharts.plots._model import EChartsOption
 from ezcharts.plots.util import JSCode
 
 # NOTE: the add_x methods below allow for type checking that pydantic V1 would
@@ -228,14 +230,50 @@
 
         For histograms, the first two dataset columns are start/stop
         rectangle x coords. The third column contains bar heights.
         """
         return [self.xAxis, 1], [self.yAxis, 2]
 
 
+class BokehPlot:
+    """Plotting interface for Bokeh."""
+
+    colors = util.choose_palette()
+    tools = "hover,crosshair,pan,box_zoom,zoom_in,zoom_out,reset,save"
+
+    def __init__(self, *args, **kwargs):
+        """Initialize a bokeh figure."""
+        defaults = dict(
+            output_backend="webgl",
+            tools=self.tools,
+            height=300,
+            width=600,
+        )
+        defaults.update(kwargs)
+        self._fig = figure(*args, **defaults)
+        # remove Bokeh logo
+        self._fig.toolbar.logo = None
+
+    @property
+    def logger(self):
+        """Return logger for class."""
+        return _logger
+
+    def render_html(self, output, **kwargs):
+        """Render plot to a file.
+
+        :params output: output file.
+        :param kwargs: passed to `BokehChart`.
+        """
+        title = self._fig.title.text or "Bokeh Plot"
+        chart = BokehChart(self, "epi2melabs", **kwargs)
+        report = ComponentReport(title, chart)
+        report.write(output)
+
+
 class _NoAxisFixPlot(Plot):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def fix_axis_labels(self):
         self.logger.warning("Skipping axis label fixing")
```

### Comparing `ezcharts-0.5.4/ezcharts/plots/_base.py` & `ezcharts-0.6.0/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/_model.py` & `ezcharts-0.6.0/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/categorical.py` & `ezcharts-0.6.0/ezcharts/plots/categorical.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/distribution.py` & `ezcharts-0.6.0/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/ideogram.py` & `ezcharts-0.6.0/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/karyomap.py` & `ezcharts-0.6.0/ezcharts/plots/karyomap.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/matrix.py` & `ezcharts-0.6.0/ezcharts/plots/matrix.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/metagenomics_sankey.py` & `ezcharts-0.6.0/ezcharts/plots/metagenomics_sankey.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/relational.py` & `ezcharts-0.6.0/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/sunburst.py` & `ezcharts-0.6.0/ezcharts/plots/sunburst.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts/plots/util.py` & `ezcharts-0.6.0/ezcharts/plots/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     These are seaborn's qualitative color palettes.
     https://seaborn.pydata.org/tutorial/color_palettes.html
 
     :param: name: name of palette to return colors from.
     :param: ncolours: number of colours.
     """
-    palletes = {
+    palettes = {
         'colorblind': [
             '#0173b2', '#de8f05', '#029e73', '#d55e00', '#cc78bc',
             '#ca9161', '#fbafe4', '#949494', '#ece133', '#56b4e9'],
         'deep': [
             '#4c72b0', '#dd8452', '#55a868', '#c44e52', '#8172b3',
             '#937860', '#da8bc3', '#8c8c8c', '#ccb974', '#64b5cd'],
         'dark': [
@@ -202,17 +202,17 @@
             '#c26f6d'],
         'icefire': [
             '#55a3cd', '#4954b0', '#282739', '#3b2127', '#9c2f45',
             '#e96f36']
     }
 
     if ncolours is None:
-        return palletes[name]
+        return palettes[name]
 
-    cycler = cycle(palletes[name])
+    cycler = cycle(palettes[name])
     return [c for c in islice(cycler, ncolours)]
 
 
 def emptyPlot(**kwargs):
     """Empty plot for when all else fails.
 
     :param kwargs: kwargs for bokeh figure.
```

### Comparing `ezcharts-0.5.4/ezcharts/util.py` & `ezcharts-0.6.0/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.5.4/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.6.0/ezcharts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.5.4
+Version: 0.6.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: LICENSE.md
 
 # ezCharts
 
 (Apologies to non-US English speakers).
 
 ezCharts is a Python library for creating and rendering charts through [eCharts](https://echarts.apache.org/).
 Plots can be contructed through an API similar to [seaborn](https://seaborn.pydata.org/).
```

### Comparing `ezcharts-0.5.4/ezcharts.egg-info/SOURCES.txt` & `ezcharts-0.6.0/ezcharts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 ezcharts/__init__.py
 ezcharts/demo.py
 ezcharts/util.py
@@ -11,14 +10,15 @@
 ezcharts.egg-info/SOURCES.txt
 ezcharts.egg-info/dependency_links.txt
 ezcharts.egg-info/entry_points.txt
 ezcharts.egg-info/not-zip-safe
 ezcharts.egg-info/requires.txt
 ezcharts.egg-info/top_level.txt
 ezcharts/components/__init__.py
+ezcharts/components/bokehchart.py
 ezcharts/components/common.py
 ezcharts/components/dss.py
 ezcharts/components/ezchart.py
 ezcharts/components/fastcat.py
 ezcharts/components/modkit.py
 ezcharts/components/mosdepth.py
 ezcharts/components/nextclade.py
```

### Comparing `ezcharts-0.5.4/setup.py` & `ezcharts-0.6.0/setup.py`

 * *Files identical despite different names*

