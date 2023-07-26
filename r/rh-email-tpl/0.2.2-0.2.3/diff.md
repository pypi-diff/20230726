# Comparing `tmp/rh_email_tpl-0.2.2.tar.gz` & `tmp/rh_email_tpl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rh_email_tpl-0.2.2.tar", last modified: Fri Jan 20 16:37:34 2023, max compression
+gzip compressed data, was "rh_email_tpl-0.2.3.tar", last modified: Wed Jul 26 10:46:12 2023, max compression
```

## Comparing `rh_email_tpl-0.2.2.tar` & `rh_email_tpl-0.2.3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/
--rw-r--r--   0 root         (0) root         (0)       60 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     5550 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl/
--rw-r--r--   0 root         (0) root         (0)       99 2023-01-20 16:36:49.000000 rh_email_tpl-0.2.2/rh_email_tpl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/apps.py
--rw-r--r--   0 root         (0) root         (0)     9142 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/email_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl/static/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.586513 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/
--rw-r--r--   0 root         (0) root         (0)     5555 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/cta.png
--rw-r--r--   0 root         (0) root         (0)      773 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/eyecatcher_impressions.png
--rw-r--r--   0 root         (0) root         (0)     1338 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-date_range.png
--rw-r--r--   0 root         (0) root         (0)     2990 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-find_in_page.png
--rw-r--r--   0 root         (0) root         (0)     2646 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-info.png
--rw-r--r--   0 root         (0) root         (0)     1151 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-laptop.png
--rw-r--r--   0 root         (0) root         (0)     3386 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-record_voice_over.png
--rw-r--r--   0 root         (0) root         (0)     3850 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-visibility.png
--rw-r--r--   0 root         (0) root         (0)     7136 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_regiohelden_omnea.png
--rw-r--r--   0 root         (0) root         (0)    10959 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_som.png
--rw-r--r--   0 root         (0) root         (0)    16003 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_stroeer_regiohelden_omnea.png
--rw-r--r--   0 root         (0) root         (0)     1745 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_display.png
--rw-r--r--   0 root         (0) root         (0)     1547 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_facebook.png
--rw-r--r--   0 root         (0) root         (0)     1425 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_googleads.png
--rw-r--r--   0 root         (0) root         (0)     1979 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_inapp.png
--rw-r--r--   0 root         (0) root         (0)     1923 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_listings.png
--rw-r--r--   0 root         (0) root         (0)     2222 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_seo.png
--rw-r--r--   0 root         (0) root         (0)     1379 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_website.png
--rw-r--r--   0 root         (0) root         (0)      765 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/warning.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.586513 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/
--rw-r--r--   0 root         (0) root         (0)      168 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/base.txt
--rw-r--r--   0 root         (0) root         (0)      417 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/footer.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.586513 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/
--rw-r--r--   0 root         (0) root         (0)      747 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/base.html
--rw-r--r--   0 root         (0) root         (0)      183 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/base.txt
--rw-r--r--   0 root         (0) root         (0)    14703 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/email_template_components.html
--rw-r--r--   0 root         (0) root         (0)    24872 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/empty.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/bold.html
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/bold.txt
--rw-r--r--   0 root         (0) root         (0)      489 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/button.html
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/button.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/center.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/center.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/code.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/code.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/color.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/color.txt
--rw-r--r--   0 root         (0) root         (0)      117 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/color_preview.html
--rw-r--r--   0 root         (0) root         (0)       60 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/color_preview.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/content.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/content.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/del.html
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/del.txt
--rw-r--r--   0 root         (0) root         (0)      680 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/eyecatcher.html
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/eyecatcher.txt
--rw-r--r--   0 root         (0) root         (0)     2975 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/footer.html
--rw-r--r--   0 root         (0) root         (0)      450 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/footer.txt
--rw-r--r--   0 root         (0) root         (0)      775 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/header.html
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/header.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/heading.html
--rw-r--r--   0 root         (0) root         (0)       89 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/heading.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/html_escape.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/html_escape.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/image.html
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/image.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/italic.html
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/italic.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/line_break.html
--rw-r--r--   0 root         (0) root         (0)       45 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/line_break.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/link.html
--rw-r--r--   0 root         (0) root         (0)      116 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/link.txt
--rw-r--r--   0 root         (0) root         (0)      197 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/list.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/list.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/list_item.html
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/list_item.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/medium.html
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/medium.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/meta/
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/meta/salutation.html
--rw-r--r--   0 root         (0) root         (0)       56 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/nowrap.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/nowrap.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/paragraph.html
--rw-r--r--   0 root         (0) root         (0)      132 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/paragraph.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/pre.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/pre.txt
--rw-r--r--   0 root         (0) root         (0)      480 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/section.html
--rw-r--r--   0 root         (0) root         (0)       74 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/section.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/section_headline.html
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/section_headline.txt
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/service_employee.html
--rw-r--r--   0 root         (0) root         (0)      142 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/service_employee.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/small.html
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/small.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/spacer.html
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/spacer.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/star.html
--rw-r--r--   0 root         (0) root         (0)        2 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/star.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/star_rating.html
--rw-r--r--   0 root         (0) root         (0)      103 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/star_rating.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/stripline.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/stripline.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table.html
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_noborder.html
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_noborder.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_tbody.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_tbody.txt
--rw-r--r--   0 root         (0) root         (0)      128 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_td.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_td.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_th.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_th.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_thead.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_thead.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_tr.html
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/table_tr.txt
--rw-r--r--   0 root         (0) root         (0)      354 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/warning.html
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/warning.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19834 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templatetags/email_components.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templatetags/phone_format.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/templatetags/premailer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/tests/premailer_templates/
--rw-r--r--   0 root         (0) root         (0)      113 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/premailer_templates/basic-base-url.expected.html
--rw-r--r--   0 root         (0) root         (0)      172 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/premailer_templates/basic-base-url.html
--rw-r--r--   0 root         (0) root         (0)      332 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/premailer_templates/basic.expected.html
--rw-r--r--   0 root         (0) root         (0)      358 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/premailer_templates/basic.html
--rw-r--r--   0 root         (0) root         (0)     2354 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/tests/test_premailer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/rh_email_tpl/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/utils/__init__py
--rw-r--r--   0 root         (0) root         (0)      545 2023-01-20 09:34:15.000000 rh_email_tpl-0.2.2/rh_email_tpl/utils/translation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 16:37:34.582513 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-20 16:37:34.000000 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6183 2023-01-20 16:37:34.000000 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-20 16:37:34.000000 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-01-20 16:37:34.000000 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-20 16:37:34.000000 rh_email_tpl-0.2.2/rh_email_tpl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-01-20 16:37:34.602513 rh_email_tpl-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2048 2023-01-20 15:26:07.000000 rh_email_tpl-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.250930 rh_email_tpl-0.2.3/rh_email_tpl/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/apps.py
+-rw-r--r--   0 root         (0) root         (0)     9142 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/email_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.250930 rh_email_tpl-0.2.3/rh_email_tpl/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.250930 rh_email_tpl-0.2.3/rh_email_tpl/static/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.250930 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.254930 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/cta.png
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/eyecatcher_impressions.png
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-date_range.png
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-find_in_page.png
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-info.png
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-laptop.png
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-record_voice_over.png
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-visibility.png
+-rw-r--r--   0 root         (0) root         (0)     7136 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_regiohelden_omnea.png
+-rw-r--r--   0 root         (0) root         (0)    10959 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_som.png
+-rw-r--r--   0 root         (0) root         (0)    16003 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_stroeer_regiohelden_omnea.png
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_display.png
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_facebook.png
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_googleads.png
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_inapp.png
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_listings.png
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_seo.png
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_website.png
+-rw-r--r--   0 root         (0) root         (0)      765 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/warning.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.250930 rh_email_tpl-0.2.3/rh_email_tpl/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.254930 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/base.txt
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/footer.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.254930 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/base.html
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/base.txt
+-rw-r--r--   0 root         (0) root         (0)    14703 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/email_template_components.html
+-rw-r--r--   0 root         (0) root         (0)    24872 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/empty.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.262930 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/bold.html
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/bold.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/button.html
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/button.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/center.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/center.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/code.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/code.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/color.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/color.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/color_preview.html
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/color_preview.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/content.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/content.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/del.html
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/del.txt
+-rw-r--r--   0 root         (0) root         (0)      680 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/eyecatcher.html
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/eyecatcher.txt
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/footer.html
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/footer.txt
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/header.html
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/header.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/heading.html
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/heading.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/html_escape.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/html_escape.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/image.html
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/image.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/italic.html
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/italic.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/line_break.html
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/line_break.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/link.html
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/link.txt
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/list.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/list.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/list_item.html
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/list_item.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/medium.html
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/medium.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.262930 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/meta/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/meta/salutation.html
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/nowrap.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/nowrap.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/paragraph.html
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/paragraph.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/pre.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/pre.txt
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/section.html
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/section.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/section_headline.html
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/section_headline.txt
+-rw-r--r--   0 root         (0) root         (0)      858 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/service_employee.html
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/service_employee.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/small.html
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/small.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/spacer.html
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/spacer.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/star.html
+-rw-r--r--   0 root         (0) root         (0)        2 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/star.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/star_rating.html
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/star_rating.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/stripline.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/stripline.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table.html
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_noborder.html
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_noborder.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_tbody.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_tbody.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_td.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_td.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_th.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_th.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_thead.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_thead.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_tr.html
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/table_tr.txt
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/warning.html
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/warning.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/rh_email_tpl/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19834 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templatetags/email_components.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templatetags/phone_format.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/templatetags/premailer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/rh_email_tpl/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/rh_email_tpl/tests/premailer_templates/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/premailer_templates/basic-base-url.expected.html
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/premailer_templates/basic-base-url.html
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/premailer_templates/basic.expected.html
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/premailer_templates/basic.html
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/tests/test_premailer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/rh_email_tpl/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/utils/__init__py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/rh_email_tpl/utils/translation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:46:12.254930 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-07-26 10:46:12.000000 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-07-26 10:46:12.000000 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:46:12.000000 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-26 10:46:12.000000 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 10:46:12.000000 rh_email_tpl-0.2.3/rh_email_tpl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-26 10:46:12.266930 rh_email_tpl-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-26 10:28:07.000000 rh_email_tpl-0.2.3/setup.py
```

### Comparing `rh_email_tpl-0.2.2/PKG-INFO` & `rh_email_tpl-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rh_email_tpl
-Version: 0.2.2
+Version: 0.2.3
 Summary: Internal RegioHelden tool for building styled html emails
 Home-page: 
 Download-URL: 
 Author: RegioHelden <entwicklung@regiohelden.de>
 Author-email: entwicklung@regiohelden.de
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rh_email_tpl-0.2.2/README.md` & `rh_email_tpl-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/pyproject.toml` & `rh_email_tpl-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -124,7 +124,67 @@
 [tool.pylint.design]
 max-branches = 16
 max-args = 10
 max-parents = 15
 max-attributes = 10
 min-public-methods = 0
 max-public-methods = 50
+
+[tool.ruff]
+exclude = [
+    ".git",
+    "__pycache",
+    "migrations",
+    "src",
+    "docs",
+    "rh_django_shared",
+]
+line-length = 88
+# See https://github.com/charliermarsh/ruff#supported-rules
+# for all supported rules
+select = [
+    "A",
+    "B",
+    "BLE",
+    "C",
+    "C4",
+    "C90",
+    "COM",
+    "DJ",
+    "DTZ",
+    "E",
+    "ERA",
+    "F",
+    "G",
+    "I",
+    "ICN",
+    "INP",
+    "N",
+    "PIE",
+    "PGH",
+    "PL",
+    "PTH",
+    "RET",
+    "RSE",
+    "RUF",
+    "S",
+    "SIM",
+    "T20",
+    "UP",
+    "W",
+    "YTT",
+]
+ignore = [
+    "N802",     # Function name `{name}` should be lowercase
+    "N803",     # Argument name `{name}` should be lowercase
+    "N806",     # Variable `{name}` in function should be lowercase
+    "N815",     # Variable `{name}` in class scope should not be mixedCase
+    "N818",     # Exception name `{name}` should be named with an Error suffix
+    "A003",     # Class attribute `{name}` is shadowing a python builtin
+    "S101",     # Use of `assert` detected
+    "UP007",    # Use `X | Y` for type annotations
+    "S105",     # Possible hardcoded password: "{}"
+    "PLR0913",  # Too many arguments to function call ({c_args}/{max_args})
+]
+
+[tool.ruff.mccabe]
+max-complexity = 16
```

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/email_message.py` & `rh_email_tpl-0.2.3/rh_email_tpl/email_message.py`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/cta.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/cta.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/eyecatcher_impressions.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/eyecatcher_impressions.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-date_range.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-date_range.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-find_in_page.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-find_in_page.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-info.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-info.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-laptop.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-laptop.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-record_voice_over.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-record_voice_over.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/icon-visibility.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/icon-visibility.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_regiohelden_omnea.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_regiohelden_omnea.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_som.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_som.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/logo_stroeer_regiohelden_omnea.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/logo_stroeer_regiohelden_omnea.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_display.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_display.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_facebook.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_facebook.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_googleads.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_googleads.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_inapp.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_inapp.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_listings.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_listings.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_seo.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_seo.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/product_website.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/product_website.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/static/img/email/som/warning.png` & `rh_email_tpl-0.2.3/rh_email_tpl/static/img/email/som/warning.png`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/base.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/base.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/email_template_components.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/email_template_components.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/empty.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/empty.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/eyecatcher.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/eyecatcher.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/footer.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/footer.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/header.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/header.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/meta/salutation.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/meta/salutation.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templates/email/som/tags/service_employee.html` & `rh_email_tpl-0.2.3/rh_email_tpl/templates/email/som/tags/service_employee.html`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templatetags/email_components.py` & `rh_email_tpl-0.2.3/rh_email_tpl/templatetags/email_components.py`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/templatetags/premailer.py` & `rh_email_tpl-0.2.3/rh_email_tpl/templatetags/premailer.py`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/tests/test_premailer.py` & `rh_email_tpl-0.2.3/rh_email_tpl/tests/test_premailer.py`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl/utils/translation.py` & `rh_email_tpl-0.2.3/rh_email_tpl/utils/translation.py`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl.egg-info/PKG-INFO` & `rh_email_tpl-0.2.3/rh_email_tpl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rh-email-tpl
-Version: 0.2.2
+Version: 0.2.3
 Summary: Internal RegioHelden tool for building styled html emails
 Home-page: 
 Download-URL: 
 Author: RegioHelden <entwicklung@regiohelden.de>
 Author-email: entwicklung@regiohelden.de
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rh_email_tpl-0.2.2/rh_email_tpl.egg-info/SOURCES.txt` & `rh_email_tpl-0.2.3/rh_email_tpl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rh_email_tpl-0.2.2/setup.py` & `rh_email_tpl-0.2.3/setup.py`

 * *Files identical despite different names*

