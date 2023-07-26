# Comparing `tmp/hcs-cli-0.1.46.tar.gz` & `tmp/hcs-cli-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.46.tar", last modified: Fri Jul 14 04:31:15 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.47.tar", last modified: Wed Jul 26 02:23:36 2023, max compression
```

## Comparing `hcs-cli-0.1.46.tar` & `hcs-cli-0.1.47.tar`

### file list

```diff
@@ -1,297 +1,330 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.697916 hcs-cli-0.1.46/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.46/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.372772 hcs-cli-0.1.46/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2941 2023-07-12 18:10:42.000000 hcs-cli-0.1.46/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.46/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.46/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.46/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.46/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.46/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-14 04:31:15.697112 hcs-cli-0.1.46/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.46/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.380883 hcs-cli-0.1.46/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.46/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.46/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.46/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.46/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     3763 2023-07-11 20:40:34.000000 hcs-cli-0.1.46/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.387186 hcs-cli-0.1.46/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     6946 2023-07-14 04:31:15.000000 hcs-cli-0.1.46/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.306710 hcs-cli-0.1.46/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.388265 hcs-cli-0.1.46/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.46/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.46/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.46/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-14 04:31:15.698150 hcs-cli-0.1.46/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-14 04:31:10.000000 hcs-cli-0.1.46/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.390655 hcs-cli-0.1.46/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.46/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.391685 hcs-cli-0.1.46/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.392596 hcs-cli-0.1.46/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.396210 hcs-cli-0.1.46/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.398965 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.402135 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.407019 hcs-cli-0.1.46/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.46/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.410360 hcs-cli-0.1.46/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.414366 hcs-cli-0.1.46/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.416297 hcs-cli-0.1.46/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.417389 hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.423146 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.428624 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)     2220 2023-07-12 20:50:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.433681 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.437942 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.439435 hcs-cli-0.1.46/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.442416 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.446258 hcs-cli-0.1.46/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.453579 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     3935 2023-07-13 00:26:26.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.457316 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3292 2023-07-12 23:34:52.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.461261 hcs-cli-0.1.46/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.466800 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.468362 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.474225 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.482054 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.46/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.327338 hcs-cli-0.1.46/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.491886 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.496451 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.504490 hcs-cli-0.1.46/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.510119 hcs-cli-0.1.46/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1777 2023-07-11 20:14:16.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-11 20:14:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1660 2023-07-11 23:15:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/graph.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.511950 hcs-cli-0.1.46/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.519260 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-11 20:54:29.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.526642 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-11 20:55:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.534427 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 20:56:15.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-11 20:56:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      948 2023-07-11 20:56:50.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-11 20:56:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.536976 hcs-cli-0.1.46/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.46/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.538174 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.541959 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.46/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.548259 hcs-cli-0.1.46/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.566068 hcs-cli-0.1.46/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.46/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.46/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.46/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.570866 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.46/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.46/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.46/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.46/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.46/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.46/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.46/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.46/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.46/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.46/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.46/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.580641 hcs-cli-0.1.46/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.46/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.46/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.46/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.46/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.46/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.46/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.46/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.583133 hcs-cli-0.1.46/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.46/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.590341 hcs-cli-0.1.46/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       74 2023-07-11 20:07:10.000000 hcs-cli-0.1.46/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    15274 2023-07-12 18:20:35.000000 hcs-cli-0.1.46/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     6862 2023-07-13 01:02:57.000000 hcs-cli-0.1.46/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.46/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.591840 hcs-cli-0.1.46/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.46/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.602671 hcs-cli-0.1.46/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5381 2023-07-13 00:28:42.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1331 2023-07-12 23:43:03.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1879 2023-07-12 23:43:40.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-11 21:11:11.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 21:13:28.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1259 2023-07-12 00:09:22.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.606245 hcs-cli-0.1.46/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.617878 hcs-cli-0.1.46/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-11 08:52:37.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1227 2023-07-12 00:45:19.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     1188 2023-07-12 20:31:23.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-11 21:01:33.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.620168 hcs-cli-0.1.46/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.628700 hcs-cli-0.1.46/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.46/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.46/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.46/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.46/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1313 2023-07-12 20:33:06.000000 hcs-cli-0.1.46/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.46/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.631401 hcs-cli-0.1.46/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.46/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.46/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.636248 hcs-cli-0.1.46/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.641423 hcs-cli-0.1.46/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.46/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.46/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.644797 hcs-cli-0.1.46/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.46/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.46/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.46/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.648563 hcs-cli-0.1.46/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.46/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.46/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.46/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.651140 hcs-cli-0.1.46/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.46/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.46/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.657052 hcs-cli-0.1.46/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.46/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.46/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-07-11 20:55:47.000000 hcs-cli-0.1.46/vhcs/service/portal/pool.py
--rw-r--r--   0 nanw       (501) staff       (20)     1336 2023-07-11 21:02:10.000000 hcs-cli-0.1.46/vhcs/service/portal/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.659555 hcs-cli-0.1.46/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.46/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.46/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.663014 hcs-cli-0.1.46/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.46/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.676442 hcs-cli-0.1.46/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.46/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.46/vhcs/support/daas/cidr_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3580 2023-07-12 00:03:12.000000 hcs-cli-0.1.46/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.46/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1280 2023-07-12 21:56:02.000000 hcs-cli-0.1.46/vhcs/support/daas/infra_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.46/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.349086 hcs-cli-0.1.46/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.684412 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)      394 2023-07-11 23:33:48.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      220 2023-07-12 23:47:56.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3690 2023-07-12 23:33:06.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      239 2023-07-12 23:32:53.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.46/vhcs/support/daas/tenant.py.xx
--rw-r--r--   0 nanw       (501) staff       (20)     4088 2023-07-12 23:12:58.000000 hcs-cli-0.1.46/vhcs/support/daas/tenant_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.46/vhcs/support/plan_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.46/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.695813 hcs-cli-0.1.46/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.46/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.746806 hcs-cli-0.1.47/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.47/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.541936 hcs-cli-0.1.47/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     4099 2023-07-26 01:38:46.000000 hcs-cli-0.1.47/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      391 2023-07-26 01:21:48.000000 hcs-cli-0.1.47/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.47/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.47/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.47/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.47/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-26 02:23:36.745650 hcs-cli-0.1.47/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.47/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.548447 hcs-cli-0.1.47/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.47/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.47/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.47/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.47/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6164 2023-07-18 01:31:14.000000 hcs-cli-0.1.47/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.553564 hcs-cli-0.1.47/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     7841 2023-07-26 02:23:36.000000 hcs-cli-0.1.47/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.495096 hcs-cli-0.1.47/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.554481 hcs-cli-0.1.47/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.47/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.47/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.47/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-26 02:23:36.747286 hcs-cli-0.1.47/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-26 02:23:28.000000 hcs-cli-0.1.47/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.557622 hcs-cli-0.1.47/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/conftest.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)       85 2023-07-26 00:47:17.000000 hcs-cli-0.1.47/tests/test.sh
+-rw-r--r--   0 nanw       (501) staff       (20)     3363 2023-07-26 01:38:26.000000 hcs-cli-0.1.47/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.558419 hcs-cli-0.1.47/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.559217 hcs-cli-0.1.47/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.562121 hcs-cli-0.1.47/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.563497 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.564862 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9408 2023-07-26 02:20:32.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.566270 hcs-cli-0.1.47/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.47/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.567533 hcs-cli-0.1.47/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.569400 hcs-cli-0.1.47/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.569992 hcs-cli-0.1.47/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.572439 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/
+-rw-r--r--   0 nanw       (501) staff       (20)      636 2023-07-24 16:33:32.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      984 2023-07-24 16:35:03.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      943 2023-07-24 16:35:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      855 2023-07-24 16:35:24.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.572966 hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1016 2023-07-19 21:52:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.575215 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2303 2023-07-24 18:15:37.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 21:53:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      861 2023-07-25 02:42:47.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.577491 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     2606 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1039 2023-07-24 18:12:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1059 2023-07-19 21:54:27.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-19 21:54:48.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.579903 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1119 2023-07-24 21:42:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:54:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1845 2023-07-24 21:40:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.581720 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-19 21:55:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:55:32.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.584237 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-07-17 17:45:02.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-21 02:40:22.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      922 2023-07-19 22:38:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      857 2023-07-19 22:46:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.584885 hcs-cli-0.1.47/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.586249 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-24 16:53:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.586867 hcs-cli-0.1.47/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.588687 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4488 2023-07-19 00:05:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.589817 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3366 2023-07-21 18:06:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.592617 hcs-cli-0.1.47/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      969 2023-07-25 21:09:30.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      907 2023-07-25 15:46:38.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-25 00:33:49.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-24 23:58:01.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.595291 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-07-18 20:31:16.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1722 2023-07-24 18:08:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1284 2023-07-24 18:08:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1144 2023-07-19 21:58:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.596978 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1049 2023-07-19 21:58:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-19 21:58:43.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.597552 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.599933 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      971 2023-07-19 21:58:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.603324 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1992 2023-07-19 22:34:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1063 2023-07-19 21:59:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1572 2023-07-19 21:59:58.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-07-19 22:32:52.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.509862 hcs-cli-0.1.47/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.604495 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      981 2023-07-19 22:00:09.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.605645 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:00:19.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.609084 hcs-cli-0.1.47/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1139 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1788 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.611362 hcs-cli-0.1.47/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2131 2023-07-21 03:10:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1853 2023-07-25 02:15:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1682 2023-07-20 01:42:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.611928 hcs-cli-0.1.47/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.616015 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-24 21:35:27.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      862 2023-07-24 21:32:49.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.620846 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      940 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-24 21:37:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.624714 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1108 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      912 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      934 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      837 2023-07-21 18:40:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-21 18:42:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/set-edge.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.625914 hcs-cli-0.1.47/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.626467 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.628155 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.47/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.630514 hcs-cli-0.1.47/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.639062 hcs-cli-0.1.47/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.47/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.47/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.47/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.640839 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.47/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.47/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.47/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.47/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.47/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.47/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.47/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.47/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6812 2023-07-25 22:42:34.000000 hcs-cli-0.1.47/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.47/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.47/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.645627 hcs-cli-0.1.47/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.47/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1808 2023-07-19 22:44:47.000000 hcs-cli-0.1.47/vhcs/common/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.47/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-18 18:53:18.000000 hcs-cli-0.1.47/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.47/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.47/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      600 2023-07-19 22:16:46.000000 hcs-cli-0.1.47/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9986 2023-07-19 00:35:32.000000 hcs-cli-0.1.47/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.647378 hcs-cli-0.1.47/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.47/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.652955 hcs-cli-0.1.47/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-07-25 17:16:12.000000 hcs-cli-0.1.47/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      103 2023-07-25 20:51:20.000000 hcs-cli-0.1.47/vhcs/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)      113 2023-07-25 17:15:18.000000 hcs-cli-0.1.47/vhcs/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    15923 2023-07-26 02:14:28.000000 hcs-cli-0.1.47/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7169 2023-07-26 01:45:08.000000 hcs-cli-0.1.47/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6243 2023-07-20 01:40:19.000000 hcs-cli-0.1.47/vhcs/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5070 2023-07-26 02:12:47.000000 hcs-cli-0.1.47/vhcs/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.654144 hcs-cli-0.1.47/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.659016 hcs-cli-0.1.47/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5381 2023-07-13 00:28:42.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      563 2023-07-17 22:53:19.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1436 2023-07-20 00:02:39.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1983 2023-07-20 00:02:46.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1310 2023-07-20 00:02:49.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-20 00:02:52.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1364 2023-07-20 00:02:56.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.660711 hcs-cli-0.1.47/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-20 01:40:39.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.668383 hcs-cli-0.1.47/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1325 2023-07-24 16:43:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2144 2023-07-25 02:48:50.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1150 2023-07-20 00:01:09.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-07-24 16:56:20.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/identity_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3162 2023-07-25 23:34:57.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/image.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1431 2023-07-20 00:03:09.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1332 2023-07-20 00:03:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1882 2023-07-21 02:43:52.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1456 2023-07-20 00:03:22.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-07-20 02:11:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/site.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1831 2023-07-25 22:45:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.669438 hcs-cli-0.1.47/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5494 2023-07-25 18:36:04.000000 hcs-cli-0.1.47/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.673476 hcs-cli-0.1.47/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       68 2023-07-24 16:34:10.000000 hcs-cli-0.1.47/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      853 2023-07-24 16:32:50.000000 hcs-cli-0.1.47/vhcs/service/admin/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.47/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-07-25 18:27:51.000000 hcs-cli-0.1.47/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1082 2023-07-24 17:45:25.000000 hcs-cli-0.1.47/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1459 2023-07-18 19:54:38.000000 hcs-cli-0.1.47/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1934 2023-07-25 18:21:27.000000 hcs-cli-0.1.47/vhcs/service/admin/template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2279 2023-07-25 18:16:29.000000 hcs-cli-0.1.47/vhcs/service/admin/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.674494 hcs-cli-0.1.47/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.47/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      879 2023-07-24 17:10:24.000000 hcs-cli-0.1.47/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.677368 hcs-cli-0.1.47/vhcs/service/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)       71 2023-07-18 21:11:37.000000 hcs-cli-0.1.47/vhcs/service/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2231 2023-07-25 23:34:52.000000 hcs-cli-0.1.47/vhcs/service/ims/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      944 2023-07-19 21:57:09.000000 hcs-cli-0.1.47/vhcs/service/ims/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1912 2023-07-25 22:16:59.000000 hcs-cli-0.1.47/vhcs/service/ims/images.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3140 2023-07-25 18:34:44.000000 hcs-cli-0.1.47/vhcs/service/ims/version.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.678380 hcs-cli-0.1.47/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.47/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.47/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.680609 hcs-cli-0.1.47/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.47/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.47/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2755 2023-07-21 02:58:07.000000 hcs-cli-0.1.47/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.682275 hcs-cli-0.1.47/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.47/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.47/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.47/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.683427 hcs-cli-0.1.47/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.47/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.47/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.685924 hcs-cli-0.1.47/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.47/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-24 21:34:40.000000 hcs-cli-0.1.47/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-24 21:37:58.000000 hcs-cli-0.1.47/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-21 18:45:40.000000 hcs-cli-0.1.47/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.687646 hcs-cli-0.1.47/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.47/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.47/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.689797 hcs-cli-0.1.47/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.47/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.715250 hcs-cli-0.1.47/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.47/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.47/vhcs/support/daas/cidr_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-07-21 18:07:07.000000 hcs-cli-0.1.47/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1794 2023-07-17 22:53:28.000000 hcs-cli-0.1.47/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3971 2023-07-25 17:39:54.000000 hcs-cli-0.1.47/vhcs/support/daas/infra_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.47/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.526387 hcs-cli-0.1.47/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.731636 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)     7411 2023-07-20 16:47:59.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      517 2023-07-20 02:14:59.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3690 2023-07-12 23:33:06.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      236 2023-07-17 22:53:38.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     4102 2023-07-18 23:24:45.000000 hcs-cli-0.1.47/vhcs/support/daas/tenant_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.47/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.47/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.743398 hcs-cli-0.1.47/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1929 2023-07-18 18:58:54.000000 hcs-cli-0.1.47/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.46/.gitignore` & `hcs-cli-0.1.47/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/.vscode/launch.json` & `hcs-cli-0.1.47/.vscode/launch.json`

 * *Files 13% similar despite different names*

```diff
@@ -46,41 +46,71 @@
             "name": "hcs plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "nanw.plan.yml", "--sequential"]
+            "args" : ["plan", "deploy", "-f", "infra.plan.yml", "--sequential"]
         },
         {
             "name": "hcs destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "destroy", "-f", "nanw.plan.yml"]
         },
         {
-            "name": "plan deploy t",
+            "name": "plan deploy",
+            "type": "python",
+            "request": "launch",
+            "program": "/usr/local/bin/hcs",
+            "console": "integratedTerminal",
+            "justMyCode": false,
+            "cwd": "${workspaceFolder}/lab",
+            "args" : ["plan", "deploy", "-f", "infra.plan.yml", "-r", "myImageMultiSession"]
+        },
+        {
+            "name": "plan destroy",
+            "type": "python",
+            "request": "launch",
+            "program": "/usr/local/bin/hcs",
+            "console": "integratedTerminal",
+            "justMyCode": false,
+            "cwd": "${workspaceFolder}/lab",
+            "args" : ["plan", "destroy", "-f", "infra.plan.yml", "-r", "myImage", "--sequential"]
+        },
+        {
+            "name": "plan deploy -f t",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "deploy", "-f", "t.plan.yml"]
         },
         {
-            "name": "plan destroy t",
+            "name": "plan destroy -f t",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "destroy", "-f", "t.plan.yml"]
         },
+        {
+            "name": "UT",
+            "type": "python",
+            "request": "launch",
+            "program": "/usr/local/bin/python3",
+            "console": "integratedTerminal",
+            "justMyCode": false,
+            "cwd": "${workspaceFolder}/tests",
+            "args" : ["-m", "unittest", "vhcs.cli.cmds.plan.test_plan.TestPlan", "-v", "--failfast"]
+        },
     ]
 }
```

### Comparing `hcs-cli-0.1.46/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.47/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.47/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/GOVERNANCE.md` & `hcs-cli-0.1.47/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/LICENSE` & `hcs-cli-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/Makefile` & `hcs-cli-0.1.47/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/PKG-INFO` & `hcs-cli-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.46
+Version: 0.1.47
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.46/README.md` & `hcs-cli-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/doc/az-cheatsheet.md` & `hcs-cli-0.1.47/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/doc/dev-setup.md` & `hcs-cli-0.1.47/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.47/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.47/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.47/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.46
+Version: 0.1.47
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.46/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.47/hcs_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 hcs_cli.egg-info/dependency_links.txt
 hcs_cli.egg-info/entry_points.txt
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
 payload/lcm/zero.json
 tests/__init__.py
 tests/conftest.py
+tests/test.sh
 tests/test_utils.py
 tests/vhcs/__init__.py
 tests/vhcs/cli/__init__.py
 tests/vhcs/cli/cmds/__init__.py
 tests/vhcs/cli/cmds/test_context.py
 tests/vhcs/cli/cmds/test_login.py
 tests/vhcs/cli/cmds/test_profile.py
@@ -43,39 +44,56 @@
 vhcs/__main__.py
 vhcs/cli/__init__.py
 vhcs/cli/main.py
 vhcs/cli/cmds/__init__.py
 vhcs/cli/cmds/login.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/admin/__init__.py
+vhcs/cli/cmds/admin/ad/__init__.py
+vhcs/cli/cmds/admin/ad/delete.py
+vhcs/cli/cmds/admin/ad/get.py
+vhcs/cli/cmds/admin/ad/list.py
 vhcs/cli/cmds/admin/azure-infra/main.py
 vhcs/cli/cmds/admin/edge/__init__.py
+vhcs/cli/cmds/admin/edge/delete.py
 vhcs/cli/cmds/admin/edge/get.py
 vhcs/cli/cmds/admin/edge/list.py
 vhcs/cli/cmds/admin/provider/create.py
+vhcs/cli/cmds/admin/provider/delete.py
 vhcs/cli/cmds/admin/provider/get.py
 vhcs/cli/cmds/admin/provider/list.py
 vhcs/cli/cmds/admin/template/__init__.py
+vhcs/cli/cmds/admin/template/delete.py
 vhcs/cli/cmds/admin/template/get.py
 vhcs/cli/cmds/admin/template/list.py
 vhcs/cli/cmds/admin/template/vm/__init__.py
 vhcs/cli/cmds/admin/template/vm/get.py
 vhcs/cli/cmds/admin/template/vm/list.py
+vhcs/cli/cmds/admin/uag/__init__.py
+vhcs/cli/cmds/admin/uag/delete.py
+vhcs/cli/cmds/admin/uag/get.py
+vhcs/cli/cmds/admin/uag/list.py
 vhcs/cli/cmds/auth/__init__.py
 vhcs/cli/cmds/auth/admin/__init__.py
 vhcs/cli/cmds/auth/admin/get_org_idp_map.py
 vhcs/cli/cmds/daas/__init__.py
 vhcs/cli/cmds/daas/infra/__init__.py
 vhcs/cli/cmds/daas/infra/basic.py
 vhcs/cli/cmds/daas/infra/plan.py
 vhcs/cli/cmds/daas/tenant/__init__.py
 vhcs/cli/cmds/daas/tenant/plan.py
 vhcs/cli/cmds/ims/__init__.py
+vhcs/cli/cmds/ims/delete.py
+vhcs/cli/cmds/ims/get.py
 vhcs/cli/cmds/ims/list.py
 vhcs/cli/cmds/ims/list_copies.py
+vhcs/cli/cmds/ims/version/__init__.py
+vhcs/cli/cmds/ims/version/delete.py
+vhcs/cli/cmds/ims/version/get.py
+vhcs/cli/cmds/ims/version/list.py
 vhcs/cli/cmds/inventory/__init__.py
 vhcs/cli/cmds/inventory/get.py
 vhcs/cli/cmds/inventory/list.py
 vhcs/cli/cmds/lcm/__init__.py
 vhcs/cli/cmds/lcm/provider/__init__.py
 vhcs/cli/cmds/lcm/provider/delete.py
 vhcs/cli/cmds/lcm/provider/get.py
@@ -110,14 +128,15 @@
 vhcs/cli/cmds/portal/pool/get.py
 vhcs/cli/cmds/portal/pool/list.py
 vhcs/cli/cmds/portal/site/__init__.py
 vhcs/cli/cmds/portal/site/create.py
 vhcs/cli/cmds/portal/site/delete.py
 vhcs/cli/cmds/portal/site/get.py
 vhcs/cli/cmds/portal/site/list.py
+vhcs/cli/cmds/portal/site/set-edge.py
 vhcs/cli/cmds/profile/__init__.py
 vhcs/cli/cmds/profile/init.py
 vhcs/cli/cmds/vmhub/__init__.py
 vhcs/cli/cmds/vmhub/otp/__init__.py
 vhcs/cli/cmds/vmhub/otp/redeem.py
 vhcs/cli/cmds/vmhub/otp/request.py
 vhcs/common/__init__.py
@@ -139,59 +158,71 @@
 vhcs/common/ctxp/util.py
 vhcs/common/ctxp/var_template.py
 vhcs/common/ctxp/built_in_cmds/__init__.py
 vhcs/common/ctxp/built_in_cmds/context.py
 vhcs/common/ctxp/built_in_cmds/profile.py
 vhcs/common/sglib/__init__.py
 vhcs/common/sglib/auth.py
+vhcs/common/sglib/cli_options.py
 vhcs/common/sglib/csp.py
 vhcs/common/sglib/ez_client.py
 vhcs/common/sglib/hcs_client.py
 vhcs/common/sglib/login_support.py
 vhcs/common/sglib/util.py
 vhcs/config/__init__.py
 vhcs/config/hcs-deployments.yaml
 vhcs/plan/__init__.py
+vhcs/plan/actions.py
+vhcs/plan/context.py
 vhcs/plan/core.py
 vhcs/plan/dag.py
 vhcs/plan/helper.py
+vhcs/plan/kop.py
 vhcs/plan/provider/__init__.py
 vhcs/plan/provider/azure/__init__.py
 vhcs/plan/provider/azure/_az_facade.py
 vhcs/plan/provider/azure/_prepare.py
 vhcs/plan/provider/azure/aad_group.py
 vhcs/plan/provider/azure/aad_user.py
 vhcs/plan/provider/azure/nsg.py
 vhcs/plan/provider/azure/resource_group.py
 vhcs/plan/provider/azure/subnet.py
 vhcs/plan/provider/dev/__init__.py
 vhcs/plan/provider/dev/_prepare.py
 vhcs/plan/provider/dev/dummy.py
 vhcs/plan/provider/hcs/__init__.py
 vhcs/plan/provider/hcs/_prepare.py
+vhcs/plan/provider/hcs/ad.py
+vhcs/plan/provider/hcs/edge.py
 vhcs/plan/provider/hcs/entitlement.py
+vhcs/plan/provider/hcs/identity_provider.py
+vhcs/plan/provider/hcs/image.py
 vhcs/plan/provider/hcs/launch_item.py
 vhcs/plan/provider/hcs/pool_group.py
 vhcs/plan/provider/hcs/pool_template.py
 vhcs/plan/provider/hcs/provider.py
 vhcs/plan/provider/hcs/site.py
+vhcs/plan/provider/hcs/uag.py
 vhcs/service/__init__.py
 vhcs/service/_util.py
 vhcs/service/admin/__init__.py
+vhcs/service/admin/ad.py
 vhcs/service/admin/azure_infra.py
 vhcs/service/admin/edge.py
 vhcs/service/admin/helper.py
 vhcs/service/admin/provider.py
 vhcs/service/admin/template.py
+vhcs/service/admin/uag.py
 vhcs/service/auth/__init__.py
 vhcs/service/auth/admin.py
-vhcs/service/ims_catalog/__init__.py
-vhcs/service/ims_catalog/helper.py
-vhcs/service/ims_catalog/image_copies.py
-vhcs/service/ims_catalog/images.py
+vhcs/service/ims/__init__.py
+vhcs/service/ims/helper.py
+vhcs/service/ims/image_copies.py
+vhcs/service/ims/images.py
+vhcs/service/ims/version.py
 vhcs/service/inventory/__init__.py
 vhcs/service/inventory/vm.py
 vhcs/service/lcm/__init__.py
 vhcs/service/lcm/provider.py
 vhcs/service/lcm/template.py
 vhcs/service/org_service/__init__.py
 vhcs/service/org_service/datacenter.py
@@ -209,15 +240,14 @@
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
 vhcs/support/daas/cidr_util.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
 vhcs/support/daas/infra_calc.py
 vhcs/support/daas/template.py
-vhcs/support/daas/tenant.py.xx
 vhcs/support/daas/tenant_calc.py
 vhcs/support/daas/templates/v1/infra.blueprint.yml
 vhcs/support/daas/templates/v1/infra.vars.yml
 vhcs/support/daas/templates/v1/tenant.blueprint.yml
 vhcs/support/daas/templates/v1/tenant.vars.yml
 vhcs/util/__init__.py
 vhcs/util/check_license.py
```

### Comparing `hcs-cli-0.1.46/payload/lcm/zero.json` & `hcs-cli-0.1.47/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/pyproject.toml` & `hcs-cli-0.1.47/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/setup.py` & `hcs-cli-0.1.47/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.46"
+VERSION = "0.1.47"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.46/tests/conftest.py` & `hcs-cli-0.1.47/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/tests/test_utils.py` & `hcs-cli-0.1.47/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             raise Exception("Expect non-empty json, but got empty.")
         d = json.loads(data)
         if len(d) == 0:
             raise Exception("Expect non-empty json, but got empty dict.")
 
     def verify(self, cmd: str, expected_data: any, expected_return_code: int = 0, expect_stderr_empty: bool = True, stdin_payload: str = None):
         stdout, stderr, returncode = _run(cmd, stdin_payload)
-
         try:
 
             # verify return code
             self.assertEqual(returncode, expected_return_code, "Invalid return code.")
 
             # verify stderr
             actual_stderr_empty = stderr is None or len(stderr) == 0
```

### Comparing `hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 import yaml
 import os
 import re
 import unittest
 from test_utils import CliTest
-from vhcs.common import util
+from vhcs.common.util import deep_get_attr
 
 class _blueprints:
     d10_basic = """
 deploymentId: d10
 resources:
   r1:
     kind: dev/dummy
@@ -46,15 +46,15 @@
 
     d12_basic_parallel = """
 deploymentId: d12
 resources:
   r1:
     kind: dev/dummy
     data:
-        delay: 1s
+        delay: 2s
   r2:
     kind: dev/dummy
 """
 
     d13_basic_error_sequential = """
 deploymentId: d13
 resources:
@@ -115,75 +115,115 @@
     kind: dev/dummy
     for: text in vars.userEmails
   r2:
     kind: dev/dummy
     data:
       agg: "${[for r in r1: r.outputText]}"
 """
+
+    d60_basic_condition = """
+deploymentId: d60
+vars:
+  guest1: Alice
+  guest2:
+resources:
+  r1:
+    kind: dev/dummy
+    conditions:
+      has_guest1: ${vars.guest1}
+    data:
+      text: hello
+  r2:
+    kind: dev/dummy
+    conditions:
+      has_guest2: ${vars.guest2}
+    data:
+      text: hello
+  r11:
+    kind: dev/dummy
+    conditions:
+      has_r1: ${r1.outputText}
+  r21:
+    kind: dev/dummy
+    conditions:
+      has_r2: ${r2.outputText}
+"""
 class TestPlan(CliTest):
     @classmethod
     def setUpClass(cls):
         _cleanup_states()
 
     @classmethod
     def tearDownClass(cls):
         _cleanup_states()
 
     def test10_basic(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d10_basic, expected_data='', expect_stderr_empty=False)
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d10_basic, expected_data='', expect_stderr_empty=False)
+        self.verify_deploy(_blueprints.d10_basic)
+        self.verify_destroy(_blueprints.d10_basic)
 
     def test11_basic_dep(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d11_basic_dep, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d11', 'deploy', "r2 must be deployed after r1", precise_order=['start/r1', 'success/r1', 'start/r2', 'success/r2'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d11_basic_dep, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d11', 'destroy', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
+        self.verify_deploy(_blueprints.d11_basic_dep)
+        self.verify_execution_log('d11', 'create', "r2 must be deployed after r1", precise_order=['start/r1', 'success/r1', 'start/r2', 'success/r2'])
+        self.verify_destroy(_blueprints.d11_basic_dep)
+        self.verify_execution_log('d11', 'delete', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
 
     def test12_basic_parallel(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d12_basic_parallel, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d12', 'deploy', "success of r2 must before success of r1", partial_order=['success/r2', 'success/r1'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d12_basic_parallel, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d12', 'destroy', "both r1 and r2 must be destroyed", any_order=['success/r2', 'success/r1'])
+        self.verify_deploy(_blueprints.d12_basic_parallel)
+        self.verify_execution_log('d12', 'create', "success of r2 must before success of r1", partial_order=['success/r2', 'success/r1'])
+        self.verify_destroy(_blueprints.d12_basic_parallel)
+        self.verify_execution_log('d12', 'delete', "both r1 and r2 must be destroyed", any_order=['success/r2', 'success/r1'])
         
     def test13_basic_error_sequential(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d13_basic_error_sequential, expected_data='', expected_return_code=1, expect_stderr_empty=False)
-        self.verify_execution_log('d13', 'deploy', "r2 must not be deployed, due to failure in r1", precise_order=['start/r1', 'error/r1'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d13_basic_error_sequential, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d13', 'destroy', "r2 must not be destroyed, since it's not deployed", precise_order=['skipped/r2', 'start/r1', 'success/r1'])
+        self.verify_deploy(_blueprints.d13_basic_error_sequential, expected_return_code=1)
+        self.verify_execution_log('d13', 'create', "r2 must not be deployed, due to failure in r1", precise_order=['start/r1', 'error/r1'])
+        self.verify_destroy(_blueprints.d13_basic_error_sequential)
+        self.verify_execution_log('d13', 'delete', "r2 must not be destroyed, since it's not deployed", precise_order=['skip/r2', 'start/r1', 'success/r1'])
 
     def test14_basic_error_parallel(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d14_basic_error_parallel, expected_data='', expected_return_code=1, expect_stderr_empty=False)
-        self.verify_execution_log('d14', 'deploy', "success of r2 must before error of r1", partial_order=['success/r2', 'error/r1'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d14_basic_error_parallel, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d14', 'destroy', "both r1 and r2 must be cleaned up", any_order=['success/r2', 'success/r1'])
+        self.verify_deploy(_blueprints.d14_basic_error_parallel, expected_return_code=1)
+        self.verify_execution_log('d14', 'create', "success of r2 must before error of r1", partial_order=['success/r2', 'error/r1'])
+        self.verify_destroy(_blueprints.d14_basic_error_parallel)
+        self.verify_execution_log('d14', 'delete', "both r1 and r2 must be cleaned up", any_order=['success/r2', 'success/r1'])
 
     def test30_basic_statement_after(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d30_basic_statement_after, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d30', 'deploy', "r2 must be deployed after r1", precise_order=['start/r1', 'success/r1', 'start/r2', 'success/r2'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d30_basic_statement_after, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d30', 'destroy', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
+        self.verify_deploy(_blueprints.d30_basic_statement_after)
+        self.verify_execution_log('d30', 'create', "r2 must be deployed after r1", precise_order=['start/r1', 'success/r1', 'start/r2', 'success/r2'])
+        self.verify_destroy(_blueprints.d30_basic_statement_after)
+        self.verify_execution_log('d30', 'delete', "r2 must be destroyed before r1", precise_order=['start/r2', 'success/r2', 'start/r1', 'success/r1'])
 
 
     def test40_basic_statement_for(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d40_basic_statement_for, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d40', 'deploy', "r1 must be deployed twice", partial_order=['success/r1', 'success/r1'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d40_basic_statement_for, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d40', 'destroy', "r1 must be destroyed twice", any_order=['success/r1', 'success/r1'])
+        self.verify_deploy(_blueprints.d40_basic_statement_for)
+        self.verify_execution_log('d40', 'create', "r1 must be deployed twice with an additional one for the group", partial_order=['success/r1', 'success/r1', 'success/r1'])
+        self.verify_destroy(_blueprints.d40_basic_statement_for)
+        self.verify_execution_log('d40', 'delete', "r1 must be destroyed twice with an additional one for the group", any_order=['success/r1', 'success/r1', 'success/r1'])
 
     def test50_list_map_expression(self):
-        self.verify("hcs plan deploy -f -", stdin_payload=_blueprints.d50_list_map_expression, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d50', 'deploy', "two r1 instances must be created before r2 start", partial_order=['success/r1', 'success/r1', 'start/r2', 'success/r2'])
+        self.verify_deploy(_blueprints.d50_list_map_expression)
+        self.verify_execution_log('d50', 'create', "three r1 instances must be created before r2 start", partial_order=['success/r1', 'success/r1', 'success/r1', 'start/r2', 'success/r2'])
         self.verify_output('d50', "output.r2.agg", ['a@t.com', 'b@t.com'])
-        self.verify("hcs plan destroy -f -", stdin_payload=_blueprints.d50_list_map_expression, expected_data='', expect_stderr_empty=False)
-        self.verify_execution_log('d50', 'destroy', "two r1 must be deleted after r2", partial_order=['start/r2', 'success/r2', 'start/r1', 'start/r1'])
+        self.verify_destroy(_blueprints.d50_list_map_expression)
+        self.verify_execution_log('d50', 'delete', "three r1 must be deleted after r2", partial_order=['start/r2', 'success/r2', 'start/r1', 'start/r1', 'start/r1'])
+
+    def test60_basic_condition(self):
+        self.verify_deploy(_blueprints.d60_basic_condition)
+        self.verify_execution_log('d60', 'create', "r1 and r11 are deployed. r2 and r21 are not.", partial_order=['success/r1', 'success/r11'], any_order=['skip/r2', 'skip/r21'])
+        self.verify_destroy(_blueprints.d60_basic_condition)
+        self.verify_execution_log('d60', 'delete', "r1 and r11 are destroyed. r2 and r22 are not.", partial_order=['success/r11', 'success/r1'], any_order=['skip/r2', 'skip/r21'])
+
+    def verify_deploy(self, stdin_payload: str, expected_return_code: int = 0):
+        self.verify("hcs plan deploy -f -", expected_data = '', expected_return_code = expected_return_code, expect_stderr_empty = False, stdin_payload = stdin_payload)
+    
+    def verify_destroy(self, stdin_payload: str, expected_return_code: int = 0):
+        self.verify("hcs plan destroy -f -", expected_data = '', expected_return_code = expected_return_code, expect_stderr_empty = False, stdin_payload = stdin_payload)
 
     def verify_output(self, deployment_id: str, res_path: str, expected_value):
         with open(f'{deployment_id}.state.yml', 'rt') as file:
             state = yaml.safe_load(file)
-        v = util.deep_get_attr(state, res_path)
+        v = deep_get_attr(state, res_path)
         self.assertEqual(v, expected_value)
 
     def verify_execution_log(self, deployment_id: str, method: str, description: str, precise_order: list[str] = None, partial_order: list[str] = None, any_order: list[str] = None):
         with open(f'{deployment_id}.state.yml', 'rt') as file:
             state = yaml.safe_load(file)
         exec_logs = state['log'][method]
```

### Comparing `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/__main__.py` & `hcs-cli-0.1.47/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 import click
 from vhcs.service.admin import azure_infra
-from vhcs.common.sglib.util import option_org_id, option_sort, option_limit, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-@option_limit
-@option_sort
+@cli.org_id
+@cli.limit
+@cli.sort
 @click.option(
     "--provider", "-p", 
     type=str,
     required=True, 
     help="Specify the provider instance id")
 def get_compute_vm_skus(provider: str, **kwargs):
     """List compute VM SKUs"""
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service.lcm import template
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@option_org_id
-def get(id: str, org: str):
-    """Get edge by ID"""
-    ret = admin.edge.get(id, org_id=get_org_id(org))
+def get(id: str):
+    """Get template by ID"""
+    ret = template.get(id)
     if ret:
         return ret
     return ret, 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
+@cli.org_id
+@cli.search
 def list(org: str, **kwargs):
     """List edges"""
-    return admin.edge.list(org_id=get_org_id(org), **kwargs)
+    org_id = cli.get_org_id(org)
+    return admin.edge.list(org_id, **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/create.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/create.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,57 +12,73 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
 from vhcs.common.ctxp import panic
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-@click.option("--label", "-l", type=str, required=False, default="AZURE")
-@click.option("--name", "-n", type=str, required=True)
-@click.option("--data", "-d", type=str, required=True, multiple=True, help="key-value separated by '='. This parameter can be specified multiple times.")
+@cli.org_id
+@click.option(
+    "--label",
+    "-l",
+    type=str,
+    required=False,
+    default="AZURE",
+    help="Provider label. E.g. Azure, vSphere. Default: Azure.",
+)
+@click.option("--name", "-n", type=str, required=True, help="Name of the provider.")
+@click.option(
+    "--data",
+    "-d",
+    type=str,
+    required=True,
+    multiple=True,
+    help="key-value separated by '='. This parameter can be specified multiple times.",
+)
 def create(org: str, label: str, name: str, data):
-    """Create a provider instance."""
+    """Create a provider instance.
+
+    Example:
+      hcs admin provider create -n nanw-test1 -d subscriptionId=a2ef2de8-f2b5-43da-bf68-2b182dd5f928 -d directoryId=45a54f44-5305-4388-97a6-aa39bc8b451b -d region=westus2 -d applicationId=<app-id> -d applicationKey=<app-key>
+    """
     data_obj = {}
     for d in data:
-        k, v = d.split('=')
+        k, v = d.split("=")
         data_obj[k] = v
 
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     _validate(label, data_obj)
 
     payload = {
         "orgId": org_id,
         "providerLabel": label,
-		"name": name,
-		"edgeGatewayNeeded": True,
-		"providerDetails": {
-			"method": "ByAppRegistration",
-			"data": data_obj
-		}
-	}
+        "name": name,
+        "edgeGatewayNeeded": True,
+        "providerDetails": {"method": "ByAppRegistration", "data": data_obj},
+    }
     ret = admin.provider.create(label, payload)
     if ret:
         return ret
     return "", 1
 
+
 def _validate(label: str, data: dict):
     def _ensure_key_matches(required_keys, actual_keys):
         s1 = set(required_keys)
         s2 = set(actual_keys)
         missing = s1 - s2
         if missing:
             panic(f"Missing data: {missing}")
         extra = s2 - s1
         if extra:
             panic(f"Unexpected data: {extra}")
 
     label = label.upper()
-    if label == 'AZURE':
-        required_keys = ['subscriptionId', 'directoryId', 'applicationId', 'applicationKey', 'region']
+    if label == "AZURE":
+        required_keys = ["subscriptionId", "directoryId", "applicationId", "applicationKey", "region"]
         _ensure_key_matches(required_keys, data.keys())
     else:
         panic("Provider is not supported by CLI yet: " + label)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/get.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @click.option("--label", type=str, required=False, default="azure")
-def get(label: str, id: str):
+@cli.org_id
+def get(label: str, id: str, org: str, **kwargs):
     """Get template by ID"""
-    ret = admin.provider.get(label, id)
+    org_id = cli.get_org_id(org)
+    ret = admin.provider.get(label, id, org_id=org_id, **kwargs)
     if ret:
         return ret
     return "", 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/list.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, option_sort, option_limit, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-@option_limit
-@option_sort
+@cli.org_id
+@cli.limit
+@cli.sort
+@click.option("--search", type=str, required=False, help="Search expression. E.g. --search 'name $eq myProvider1'")
 @click.option(
     "--label", 
     type=click.Choice(["azure", "vsphere"]),
     required=False, 
     default="azure", 
     help="Specify the provider label")
 def list(org: str, label: str, **kwargs):
     """List provider instances"""
     return admin.provider.list(
-        org_id=get_org_id(org),
+        org_id = cli.get_org_id(org),
         label=label,
         **kwargs
     )
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@option_org_id
+@cli.org_id
 def get(id: str, org: str):
     """Get template by ID"""
-    ret = admin.template.get(id, org_id=get_org_id(org))
+    ret = admin.template.get(id, org_id= cli.get_org_id(org))
     if ret:
         return ret
-    return ret, 1
+    return '', 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
+@cli.org_id
 @click.option("--limit", "-l", type=int, required=False, default=20, help="Optionally, specify cloud provider type.")
-@option_org_id
 @click.option("--brokerable-only", type=bool, required=False, default=False)
 @click.option("--expanded", type=bool, required=False, default=False)
 @click.option(
     "--reported-search",
     type=str,
     required=False,
     help="Search expression for selection of template reported properties",
@@ -32,20 +32,21 @@
 @click.option("--template-search", type=str, required=False, help="Search expression for selection of templates")
 @click.option(
     "--sort",
     type=str,
     required=False,
     help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
 )
-def list(
-    limit: int, org: str, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
+def list(org: str, 
+    limit: int, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
 ):
     """List templates"""
+    org_id = cli.get_org_id(org)
     return admin.template.list(
+        org_id=org_id,
         limit=limit,
-        org_id=get_org_id(org),
         borkerable_only=brokerable_only,
         expanded=expanded,
         reported_search=reported_search,
         template_search=template_search,
         sort=sort,
     )
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 
 @click.command()
 @click.argument('template-id', type=str, required=True)
 @click.argument('vm-id', type=str, required=True)
-@option_org_id
+@cli.org_id
 def get(template_id: str, vm_id: str, org: str, **kwargs):
     """Get template VM"""
-    return admin.template.get_vm(template_id, vm_id, org_id=get_org_id(org), **kwargs)
+    return admin.template.get_vm(template_id, vm_id, org_id=cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
+from vhcs.service.vmhub import otp
 
 
 @click.command()
-@click.argument('template-id', type=str, required=True)
-@option_org_id
-def list(template_id: str, org: str, **kwargs):
-    """List template VMs"""
-    return admin.template.list_vms(template_id, org_id=get_org_id(org), **kwargs)
+@cli.org_id
+@click.option(
+    "--region",
+    type=str,
+    default=None,
+    required=False,
+    help="Specify region name",
+)
+@click.argument("resource-name", type=str, required=True)
+def request(org: str, region: str, resource_name: str):
+    """Request an one-time password for a specific resource"""
+    org_id = cli.get_org_id(org)
+    otp.use_region(region)
+    return otp.request_otp(org_id, resource_name)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/get.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,30 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import auth
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import ims
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-def get_org_idp_map(org: str):
-    """Get org-idp-map by ID"""
-    org_id = get_org_id(org)
-    ret = auth.admin.get_org_idp_map(org_id=org_id)
-    if ret:
-        return ret
-    return ret, 1
+@click.option("--image", "-i", type=str, required=False, help="Image ID")
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def get(image: str, id: str, org: str, **kwargs):
+    """Get image version by ID"""
+    org_id = cli.get_org_id(org)
+    if image:
+        ret = ims.version(image, org_id).get(id)
+        if ret:
+            return ret
+    else:
+        images = ims.images.list(org_id)
+        for i in images:
+            image_id = i['id']
+            ret = ims.version(image_id, org_id).get(id)
+            if ret:
+                return ret
+    return '', 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,58 +11,74 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import vhcs.common.ctxp as ctxp
-from vhcs.common.ctxp import panic, choose
+from vhcs.common.ctxp import choose
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.support.daas import infra
 from vhcs.service import admin
 from vhcs.support.daas import infra, helper, cidr_util
 
 file_name = '.plan.yml'
 
 @click.command()
 @click.argument("name", type=str, required=True)
 def plan(name: str):
     """Interactive setup for shared infrastructure."""
 
     def collect_information(data):
         vars = data['vars']
-        _select_provider(vars['provider'])
-        _input_azure_sp(vars['provider'])
+        org_id = vars['orgId']
+        _select_provider(vars, org_id)
         _select_vnet(vars['network'])
         _config_desktop_defaults(vars['desktop'])
         infra.save(data)
 
     return helper.prepare_plan_file(name, 'v1/infra.blueprint.yml', collect_information)
+
     
 
-def _select_provider(data):
-    providers = admin.provider.list(label='azure')
-    if not providers:
-        panic("No provider configured. Configure in HCS admin console first.")
-
-    fn_provider_text = lambda p: f"{p['providerDetails']['data']['region']}, {p['name']}/{p['id']}"
-
-    if len(providers) == 1:
-        p = providers[0]
-        click.echo("There's only one provider configured, and will be used: " + fn_provider_text(p))
-    else:
+def _select_provider(vars, org_id):
+    providers = admin.provider.list('azure', org_id)
+    if providers:
+        def _is_create_new(p):
+            return isinstance(p, str)
+
+        def fn_provider_text(p):
+            if _is_create_new(p):
+                return p
+            return f"{p['providerDetails']['data']['region']}, {p['name']}/{p['id']}"
+
+        providers.append("<Create New Provider>")
         p = choose("Select region and provider", providers, fn_provider_text)
         if not p:
             return
-    data['id'] = p['id']
+        if not _is_create_new(p):
+            vars['provider']['id'] = p['id']
+            return p
+    else:
+        click.echo("No provider configured. Need to create a new provider.")
+    _input_azure_sp(vars['newProvider'])
+    
 
 def _input_azure_sp(data):
-    data['applicationId'] = click.prompt("Input Azure service principle application ID", default=data['applicationId'] or "")
-    data['applicationSecret'] = click.prompt("Input Azure service principle application secret", default=data['applicationSecret'] or "")
-
+    data['subscriptionId'] = click.prompt("Azure subscription ID", default=data['subscriptionId'])
+    data['region'] = click.prompt("Azure Region", default=data['region'])
+    data['directoryId'] = click.prompt("Azure Directory ID", default=data['directoryId'])
+    data['applicationId'] = click.prompt("Azure service principle application ID", default=data['applicationId'])
+    data['applicationKey'] = click.prompt("Azure service principle application key", default=data['applicationKey'])
+
+    ret = az.login(data['applicationId'], data['applicationKey'], data['directoryId'])
+    print(ret)
+    ret = az.set_subscription(data['subscriptionId'])
+    print(ret)
+    
 def _select_vnet(data):
     vnets = az.network.vnet.list()
     fn_get_text = lambda vnet: f"{vnet['name']} ({','.join(vnet['addressSpace']['addressPrefixes'])})"
     vnet = choose("Select vNet:", vnets, fn_get_text)
     data['vNetId'] = vnet['id']
     
     while True:
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin, ims_catalog
+from vhcs.service import admin, ims
 from vhcs.common.ctxp import choose, util as cli_util
+from vhcs.common.sglib.cli_options import get_org_id
 from vhcs.support.daas import infra, helper
 
 
 @click.command()
 @click.argument("name", type=str, required=True)
 def plan(name: str):
     """Interactive command to request a DaaS tenant"""
@@ -28,17 +29,17 @@
 def _collect_info(data):
     #_fill_info_from_infra()
     vars = data['vars']
     _config_desktop(vars)
     _input_user_emails(vars)
 
 def _config_desktop(data):
-
+    org_id = get_org_id(None)
     def _select_image_and_vm_sku(data):
-        images = ims_catalog.helper.get_images_by_provider_instance_with_asset_details(data['provider']['id'])
+        images = ims.helper.get_images_by_provider_instance_with_asset_details(data['provider']['id'], org_id)
         fn_get_text = lambda d: f"{d['name']}: {d['description']}"
         prev_selected_image = None
         if data['desktop']['streamId']:
             for i in images:
                 if i['id'] == data['desktop']['streamId']:
                     prev_selected_image = i
                     break
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/upgrade.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import ims_catalog
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import subprocess
+import sys
 
 
-@click.command()
-@click.option("--limit", "-l", type=int, required=False, default=20)
-@option_org_id
-def list(**kwargs):
-    """List images"""
-    return ims_catalog.images.list(
-        **kwargs
-    )
+@click.group(invoke_without_command=True)
+def upgrade():
+    """Upgrade hcs-cli."""
+    cmd = f"pip3 install -U hcs-cli --upgrade-strategy eager --no-cache-dir"
+    p = subprocess.run(cmd, stdout=sys.stdout, stderr=sys.stderr, text=False, shell=True, check=False)
+    return p.returncode
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,20 +10,30 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import ims_catalog
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service.vmhub import otp
+from vhcs.util import pki_util
 
 
 @click.command()
-@click.option("--limit", "-l", type=int, required=False, default=20)
-@click.option("--include-catalog-details/--no-catalog-details", type=bool, required=False, default=True)
-@option_org_id
-def list_copies(**kwargs):
-    """List images"""
-    return ims_catalog.image_copies.list(
-        **kwargs
-    )
+@click.option(
+    "--region",
+    type=str,
+    default=None,
+    required=False,
+    help="Specify region name",
+)
+@click.argument("resource-name", type=str, required=True)
+@click.argument("otp", type=str, required=True)
+def redeem(region: str, resource_name: str, otp: str):
+    """Redeem OTP with CSR, receive resource cert."""
+
+    otp.use_region(region)
+    csr_pem, private_key_pem = pki_util.generate_CSR(resource_name)
+
+    ret = otp.redeem_otp(resource_name, otp, csr_pem)
+    ret.private_key = private_key_pem
+    return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import inventory
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--template", "-t", type=str, required=True, help="Template id")
 @click.option("--vm", "-v", type=str, required=True, help="VM id")
-@option_org_id
+@cli.org_id
 def get(template: str, vm: str, org: str):
     """Get template by ID"""
-    ret = inventory.get(template, vm, get_org_id(org))
+    ret = inventory.get(template, vm, cli.get_org_id(org))
     if ret:
         return ret
     return ret, 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import inventory
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import portal
+import vhcs.common.sglib.cli_options as cli
+
 
 @click.command()
-@click.argument("template", type=str, required=True)
-@option_org_id
-def list(template: str, org: str):
-    """List template VMs"""
-    ret = inventory.list(template, get_org_id(org))
-    if ret:
-        return ret
-    return ret, 1
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def delete(id: str, org: str):
+    """Get entitlement by ID"""
+    org_id = cli.get_org_id(org)
+    ret = portal.entitlement.delete(id, org_id)
+    return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import provider
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
+@cli.org_id
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 def list(org: str, type: str):
     """List providers"""
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     return provider.list(org_id=org_id, type=type)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,50 +13,54 @@
 limitations under the License.
 """
 
 import sys
 import json
 import random
 import click
-from vhcs.service import lcm
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.duration as duration
+import vhcs.service.lcm as lcm
+import vhcs.common.sglib.cli_options as cli
 from vhcs.common.ctxp.util import option_id_only
 
 
 @click.command()
 @click.option(
     "--file",
     "-f",
     type=click.File("rt"),
     default=sys.stdin,
     help="Specify the template file name. If not specified, STDIN will be used.",
 )
-@option_org_id
+@cli.org_id
+@cli.wait
 @option_id_only
-def create(file: str, org: str, id_only: bool):
+def create(file: str, org: str, wait: str, id_only: bool):
     """Create a template"""
 
     with file:
         payload = file.read()
 
     try:
         template = json.loads(payload)
     except Exception as e:
         msg = "Invalid template: " + str(e)
         return msg, 1
 
     template["id"] = _rand_id(16)
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     template["orgId"] = org_id
 
     provider = _create_zerocloud_provider(org_id)
     template["provider"]["providerAccessId"] = provider["id"]
 
     ret = lcm.template.create(template)
 
+    if wait != '0':
+        template = lcm.template.wait(id, duration.to_seconds(wait))
     if id_only:
         return ret.get("id")
     return ret
 
 
 def _rand_id(n: int):
     return "".join(random.choices("abcdefghijkmnpqrstuvwxyz23456789", k=n))
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import template
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@option_org_id
+@cli.org_id
 @click.option(
     "--force/--safe", default=True, help="In 'force' mode, the template deletion will continue and ignore any error."
 )
 def delete(id: str, org: str, force: bool):
     """Delete template by ID"""
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     return template.delete(id, org_id, force)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.lcm import template
-
+from vhcs.service import inventory
+import vhcs.common.sglib.cli_options as cli
 
 @click.command()
-@click.argument("id", type=str, required=True)
-def get(id: str):
-    """Get template by ID"""
-    ret = template.get(id)
+@click.argument("template", type=str, required=True)
+@cli.org_id
+def list(template: str, org: str):
+    """List template VMs"""
+    ret = inventory.list(template, cli.get_org_id(org))
     if ret:
         return ret
-    return ret, 1
+    return ret, 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import template
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 from vhcs.common.ctxp.util import option_id_only
 
 
 @click.command("list")
 @click.option(
     "--limit", "-l", type=int, required=False, default=20, help="Optionally, specify the number of records to return."
 )
-@option_org_id
+@cli.org_id
 @option_id_only
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 @click.option("--name", "-n", type=str, required=False, help="Optionally, specify name pattern to find.")
 def list_templates(limit: int, org: str, id_only: bool, type: str, name: str):
     """List templates"""
     if org == "all":
         ret = template.list(limit=limit, name=name, type=type)
     else:
-        ret = template.list(limit=limit, org_id=get_org_id(org), name=name, type=type)
+        ret = template.list(limit=limit, org_id=cli.get_org_id(org), name=name, type=type)
 
     if id_only:
 
         def _get_id_only(t):
             return t.get("id")
 
         return list(map(_get_id_only, ret))
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     exclude_status = []
     if fail_fast:
         if "READY" not in expected_status:
             exclude_status.append("READY")
         if "ERROR" not in expected_status:
             exclude_status.append("ERROR")
     try:
-        template = lcm.template.wait(id, expected_status, timeout_seconds, exclude_status)
+        template = lcm.template.wait(id, timeout_seconds, expected_status, exclude_status)
         return template if not silent else None
     except Exception as e:
         return str(e), 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.org_service import datacenter
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import admin
+import vhcs.common.sglib.cli_options as cli
 
 
-@click.command("list")
-@option_org_id
-def list_datacenters(org: str):
-    """List all datacenters"""
+@click.command()
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def delete(id: str, org: str, **kwargs):
+    """Delete Active Directory record by ID"""
 
-    if org == "" or org == "all":
-        ret = datacenter.list()
-    else:
-        org_id = get_org_id(org)
-        return datacenter.find_by_org(org_id)
+    org_id = cli.get_org_id(org)
 
+    ret = admin.ad.delete(id, org_id)
+    if not ret:
+        return '', 1
     return ret
+
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.org_service import details
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import portal
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-def get(org: str):
-    """Get org details"""
-    org_id = get_org_id(org)
-    ret = details.get(org_id)
-    if ret:
-        return ret
-    return ret, 1
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def delete(id: str, org: str):
+    """Delete a site."""
+    org_id = cli.get_org_id(org)
+    ret = portal.site.delete(id, org_id)
+    return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.common.ctxp import panic
 from vhcs.service.pki import certificate
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
+@cli.org_id
 @click.option("--confirm/--no-confirm", default=False)
 def delete_org_cert(org: str, confirm: bool):
     """Delete the signing certificate of a specific org"""
 
     if not confirm:
         panic('Delete an org certificate will impact some service. Specify "--confirm" to perform the deletion.')
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     return certificate.delete_org_cert(org_id)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,12 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.pki import certificate
-from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
-@click.command()
-@option_org_id
-def get_org_cert(org: str):
-    """Get the signing certificate of a specific org"""
-    org_id = get_org_id(org)
-    return certificate.get_org_cert(org_id)
+@click.command(hidden=True)
+def test():
+    return certificate.test()
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 limitations under the License.
 """
 
 import click
 from vhcs.common.ctxp import profile
 from vhcs.service.pki import certificate
 from vhcs.util import pki_util
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 def _write_file(file_path: str, text: str):
     with open(file_path, "w") as file:
         file.write(text)
 
 
@@ -30,18 +30,18 @@
 @click.option(
     "--key-length",
     type=int,
     default=2048,
     required=False,
     help="Private key length",
 )
-@option_org_id
+@cli.org_id
 def sign_resource_cert(resource_name: str, key_length: int, org: str):
     """Get the certificate for a specific resource"""
-    org_id = get_org_id(org)
+    org_id = cli.get_org_id(org)
     csr_pem, private_key_pem = pki_util.generate_CSR(resource_name, key_length=key_length)
     ret = certificate.sign_resource_cert(org_id, csr_pem)
 
     long_name = f"{profile.name()}-{org_id}-{resource_name}"
     key_file = resource_name + ".key"
     print("Private key (generated by CLI): " + key_file)
     _write_file(key_file, private_key_pem)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,13 +10,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.pki import certificate
+from vhcs.service import portal
+import vhcs.common.sglib.cli_options as cli
 
 
-@click.command(hidden=True)
-def test():
-    return certificate.test()
+@click.command()
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def get(id: str, org: str):
+    """Get entitlement by ID"""
+    org_id = cli.get_org_id(org)
+    ret = portal.entitlement.get(id, org_id)
+    if ret:
+        return ret
+    return '', 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/plan/deploy.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import vhcs.plan as plan
 import vhcs.support.plan_util as util
+from vhcs.common.ctxp.util import error_details
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.")
+@click.option("--include-related-resources/--single-resource-only", type=bool, default=True, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-def deploy(file, resource: str, parallel: bool):
+def deploy(file, resource: str, include_related_resources: bool, parallel: bool):
 
     data, extra = util.load_plan(file)
     concurrency = 10 if parallel else 1
 
     try:        
-        return plan.deploy(data, extra, resource, concurrency)
-    except (FileNotFoundError, plan.PlanException) as e:
-        return str(e), 1
+        return plan.deploy(data, extra, resource, include_related_resources, concurrency)
+    except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
+        return error_details(e), 1
 
 # def _identify_files(file: list[str], name: str):
 #     if not file and not name:
 #         panic("Either --file or --name must be specified")
 #     if file and name:
 #         panic("--file and --name must not be specified together")
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/plan/destroy.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import vhcs.plan as plan
 import vhcs.support.plan_util as util
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
+@click.option("--include-related-resources/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-def destroy(file, resource: str, parallel: bool, force: bool):
+def destroy(file, resource: str, include_related_resources: bool, parallel: bool, force: bool):
 
     data, extra = util.load_plan(file)
     concurrency = 10 if parallel else 1
     try:
-        return plan.destroy(data, force, resource, concurrency, extra)
-    except (FileNotFoundError, plan.PlanException) as e:
+        return plan.destroy(data, force, resource, include_related_resources, concurrency, extra)
+    except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
         return str(e), 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/plan/graph.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/plan/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     try:
         data, extra = util.load_plan(file)
         g = plan.graph(data, extra, simplify)
         if view:
             _view_graph(g.source)
         return g.source
-    except (FileNotFoundError, plan.PlanException) as e:
+    except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
         return str(e), 1
     
 
 def _view_graph(src):
     import urllib.parse
     import webbrowser
     url = 'https://dreampuf.github.io/GraphvizOnline/#' + urllib.parse.quote(src)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@option_org_id
+@cli.org_id
 def delete(id: str, org: str):
-    """Get entitlement by ID"""
-    org_id = get_org_id(org)
-    ret = portal.entitlement.delete(id, org_id)
+    """Delete pool by ID"""
+    org_id = cli.get_org_id(org)
+    ret = portal.pool.delete(id, org_id)
     return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service.pki import certificate
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
-@option_org_id
-def get(id: str, org: str):
-    """Get entitlement by ID"""
-    org_id=get_org_id(org)
-    ret = portal.entitlement.get(id, org_id)
-    if ret:
-        return ret
-    return ret, 1
+@cli.org_id
+def get_org_cert(org: str):
+    """Get the signing certificate of a specific org"""
+    org_id = cli.get_org_id(org)
+    return certificate.get_org_cert(org_id)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
+@cli.org_id
 def list(org: str, **kwargs):
-    """List entitlements"""
-    return portal.entitlement.list(org_id=get_org_id(org), **kwargs)
-
+    """List sites"""
+    return portal.site.list(org_id=cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/delete.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@option_org_id
-def delete(id: str, org: str):
-    """Delete pool by ID"""
-    org_id=get_org_id(org)
-    ret = portal.pool.delete(id, org_id)
-    return ret
+@cli.org_id
+def get(id: str, org: str):
+    """Get pool by ID"""
+    org_id = cli.get_org_id(org)
+    ret = portal.pool.get(id, org_id)
+    if ret:
+        return ret
+    return ret, 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,20 +11,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
-@option_org_id
-def get(id: str, org: str):
-    """Get pool by ID"""
-    org_id=get_org_id(org)
-    ret = portal.pool.get(id, org_id)
-    if ret:
-        return ret
-    return ret, 1
+@cli.org_id
+def list(org: str, **kwargs):
+    """List entitlements"""
+    org_id=cli.get_org_id(org)
+    return portal.entitlement.list(org_id, **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,18 +10,28 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import ims
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.option("--search", "-s", type=str, required=False, help="Search condition")
-@option_org_id
-def list(org: str, **kwargs):
-    """List pools"""
-    return portal.pool.list(org_id=get_org_id(org), **kwargs)
+@click.option("--image", "-i", type=str, required=False, help="Image ID")
+@cli.org_id
+def list(image: str, org: str, **kwargs):
+    """List image versions"""
+
+    org_id = cli.get_org_id(org)
+    if image:
+        return ims.version(image, org_id).list(**kwargs)
+    
+    images = ims.images.list(org_id)
+    ret = []
+    for i in images:
+        image_id = i['id']
+        ret.extend(ims.version(image_id, org_id).list())
+    return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/create.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/get.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,27 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import admin
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.option("--name", "-n", type=str, required=True)
-@click.option("--description", "-d", type=str, required=False)
-@option_org_id
-def create(name: str, description: str, org: str):
-    """Create a site."""
-    org_id = get_org_id(org)
-    payload = {
-        "name": name,
-        "description": description,
-        "orgId": org_id
-    }
-    ret = portal.site.create(payload)
+@click.argument("id", type=str, required=True)
+@cli.org_id
+def get(id: str, org: str):
+    """Get Active Directory record by ID"""
+    ret = admin.ad.get(id, org_id = cli.get_org_id(org))
     if ret:
         return ret
-    return ret, 1
+    return '', 1
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/delete.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/ims/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import ims
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
-@option_org_id
-def delete(id: str, org: str):
-    """Delete a site."""
-    org_id = get_org_id(org)
-    ret = portal.site.delete(id, org_id)
-    return ret
+@click.argument("ids", type=str, required=True, nargs=-1)
+@cli.org_id
+@cli.wait
+def delete(ids: list[str], org: str, wait: str, **kwargs):
+    """Delete an image by ID"""
+
+    org_id = cli.get_org_id(org)
+    ims.helper.delete_image_and_versions(ids, org_id, wait)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/get.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
-@option_org_id
-def get(id: str, org: str):
-    """Get site."""
-    org_id=get_org_id(org)
-    ret = portal.site.get(id, org_id)
-    if ret:
-        return ret
-    return '', 1
+@click.option("--search", "-s", type=str, required=False, help="Search condition")
+@cli.org_id
+def list(org: str, **kwargs):
+    """List pools"""
+    org_id=cli.get_org_id(org)
+    return portal.pool.list(org_id, **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/list.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-from vhcs.common.sglib.util import option_org_id, get_org_id
+from vhcs.service import admin
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
+@cli.org_id
 def list(org: str, **kwargs):
-    """List sites"""
-    return portal.site.list(org_id=get_org_id(org), **kwargs)
+    """List Active Directory records"""
+    return admin.ad.list(org_id = cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.47/vhcs/service/org_service/details.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-import subprocess
-import sys
+from .._util import hdc_service_client
+from vhcs.util.query_util import with_query, PageRequest
 
+_client = hdc_service_client("org-service")
 
-@click.group(invoke_without_command=True)
-def upgrade():
-    """Upgrade hcs-cli."""
-    cmd = f"pip3 install -U hcs-cli --upgrade-strategy eager --no-cache-dir"
-    p = subprocess.run(cmd, stdout=sys.stdout, stderr=sys.stderr, text=False, shell=True, check=False)
-    return p.returncode
+
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/org-details/{id}", **kwargs)
+    return _client.get(url)
+
+def list(**kwargs):
+    def _get_page(query_string):
+        url = "/v1/org-details?" + query_string
+        return _client.get(url)
+
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.47/vhcs/common/sglib/cli_options.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,30 +10,53 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.vmhub import otp
-from vhcs.util import pki_util
+from vhcs.common.ctxp import CtxpException
 
-
-@click.command()
-@click.option(
-    "--region",
+org_id = click.option(
+    "--org",
     type=str,
     default=None,
     required=False,
-    help="Specify region name",
+    help="Specify org ID. If not specified, org ID from the current auth token will be used.",
+)
+wait = click.option(
+    "--wait", "-w",
+    type=str, 
+    required=False, 
+    default='10m', 
+    help="Wait time. E.g. '30s', or '5m'. Default: 10m. Specify '0' to disable waiting and return immediately."
+)
+search = click.option(
+    "--search", "-s",
+    type=str,
+    required=False,
+    help="Specify REST search. E.g. 'name $eq something'. Note: use single quote in bash/sh."
 )
-@click.argument("resource-name", type=str, required=True)
-@click.argument("otp", type=str, required=True)
-def redeem(region: str, resource_name: str, otp: str):
-    """Redeem OTP with CSR, receive resource cert."""
+sort = click.option(
+    "--sort", 
+    type=str,
+    required=False,
+    help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
+)
+limit = click.option(
+    "--limit", 
+    type=int, 
+    required=False, 
+    default=20, 
+    help="Optionally, specify the number of records to fetch."
+)
+
+def get_org_id(org: str) -> str:
+    if org:
+        return org
 
-    otp.use_region(region)
-    csr_pem, private_key_pem = pki_util.generate_CSR(resource_name)
+    from vhcs.common.sglib import auth
 
-    ret = otp.redeem_otp(resource_name, otp, csr_pem)
-    ret.private_key = private_key_pem
-    return ret
+    auth_info = auth.details(False)
+    if not auth_info:
+        raise CtxpException("Not authorized. See 'hcs login --help'.")
+    return auth_info.org.id
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,27 +9,33 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import httpx
 import click
-from vhcs.common.sglib.util import option_org_id, get_org_id
-from vhcs.service.vmhub import otp
+from vhcs.service import admin
+import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
-@option_org_id
-@click.option(
-    "--region",
-    type=str,
-    default=None,
-    required=False,
-    help="Specify region name",
-)
-@click.argument("resource-name", type=str, required=True)
-def request(org: str, region: str, resource_name: str):
-    """Request an one-time password for a specific resource"""
-    org_id = get_org_id(org)
-    otp.use_region(region)
-    return otp.request_otp(org_id, resource_name)
+@click.argument("id", type=str, required=True)
+@cli.org_id
+@cli.wait
+def delete(id: str, org: str, wait: str):
+    """Delete UAG by ID"""
+
+    org_id=cli.get_org_id(org)
+    try:
+        ret = admin.uag.delete(id, org_id)
+        if not ret:
+            return '', 1
+    except httpx.HTTPStatusError as e:
+        if e.response.status_code == 409:
+            pass
+        else:
+            raise
+    if wait == '0':
+        return ret
+    admin.uag.wait_for_deleted(id, org_id, wait)
```

### Comparing `hcs-cli-0.1.46/vhcs/cli/main.py` & `hcs-cli-0.1.47/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.47/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,18 +83,17 @@
                 raise Exception(f"Unexpected output format: {output}")
         except Exception as e:
             print("Fail converting object:", e, file=sys.stderr)
             text = data
     print(text, end="", file=file)
 
 def print_error(error):
-    if isinstance(error, httpx.HTTPStatusError):
-        print(type(error).__name__, error, file=sys.stderr)
-    elif isinstance(error, CtxpException):
-        print(error, file=sys.stderr)
+    if isinstance(error, httpx.HTTPStatusError) or isinstance(error, CtxpException) or isinstance(error, TimeoutError) or isinstance(error, subprocess.CalledProcessError):
+        msg = error_details(error)
+        print(msg, file=sys.stderr)
     else:
         traceback.print_exception(type(error), error, error.__traceback__, file=sys.stderr)
 
 def _convert_generator(data: Any):
     if isinstance(data, types.GeneratorType):
         return list(data)
     return data
@@ -172,14 +171,27 @@
         return []
     parts = input_value.split(",")
     ret = []
     for p in parts:
         ret.append(p.strip())
     return ret
 
+def error_details(e: Exception | Any):
+    if isinstance(e, Exception):
+        details = e.__class__.__name__ + ': ' + str(e)
+        cause = e.__cause__
+        if cause and cause != e:
+            details += " | Caused by: " + error_details(cause)
+
+        if isinstance(e, httpx.HTTPStatusError):
+            details += "\n" + e.response.text
+        return details
+    else:
+        return str(e)
+
 option_verbose = click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="Print debug logs",
 )
```

### Comparing `hcs-cli-0.1.46/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.47/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/duration.py` & `hcs-cli-0.1.47/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/logger.py` & `hcs-cli-0.1.47/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.47/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.47/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.47/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.47/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.47/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.47/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/common/sglib/util.py` & `hcs-cli-0.1.47/vhcs/service/lcm/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.common.ctxp import CtxpException
+import json
+from typing import Any
+from .._util import hdc_service_client
+from vhcs.util.query_util import with_query, PageRequest
 
-option_org_id = click.option(
-    "--org",
-    type=str,
-    default=None,
-    required=False,
-    help="Specify org ID. If not specified, org ID from the current auth token will be used.",
-)
-
-option_sort = click.option(
-    "--sort",
-    type=str,
-    required=False,
-    help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
-)
-
-option_limit = click.option(
-    "--limit", 
-    type=int, 
-    required=False, 
-    default=20, 
-    help="Optionally, specify the number of records to fetch.")
-
-def get_org_id(org: str) -> str:
-    if org:
-        return org
-
-    from vhcs.common.sglib import auth
-
-    auth_info = auth.details(False)
-    if not auth_info:
-        raise CtxpException("Not authorized. See 'hcs login --help'.")
-    return auth_info.org.id
+_client = hdc_service_client("lcm")
+
+
+def get(id: str, **kwargs: Any):
+    url = with_query(f"/v1/providers/{id}", **kwargs)
+    return _client.get(url)
+
+def list(**kwargs):
+    def _get_page(query_string):
+        url = "/v1/providers?" + query_string
+        return _client.get(url)
+
+    return PageRequest(_get_page, **kwargs).get()
+
+def delete(id: str):
+    resp = _client.delete(f"/v1/providers/{id}")
+    return _convert_resp(resp)
+
+def create(data: dict):
+    url = "/v1/providers/" + data["type"].lower()
+    return _client.post(url, json=data)
+
+
+def _convert_resp(resp):
+    if resp:
+        resp.read()
+        try:
+            json.loads(resp.text)
+        except:
+            return resp.text
```

### Comparing `hcs-cli-0.1.46/vhcs/common/util.py` & `hcs-cli-0.1.47/vhcs/common/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import path
 from typing import Tuple, Any
 import json
 import yaml
 import re
+from vhcs.common.ctxp.util import CtxpException
 
 def load_data(file_name: str, class_type: str):
     data = load_data_file(file_name)
     if data == None:
         return
     return strict_dict_to_class(data, class_type)
 
@@ -210,29 +211,29 @@
 _pattern_var = re.compile('.*?\$\{(.+?)\}.*')
 _pattern_var_list = re.compile('\$\{\s*\[\s*for\s+(.+?)\s+in\s+(.+?)\s*\:\s*(.+)\s*]\s*\}')
 def _process_variables_impl(obj: dict, fn_get_var = None):
     changed = {}
     pending = {}
 
     def fn_change(path, v):
-        resolved, pending_var = resolve_expression(v, fn_get_var)
+        resolved, pending_var = resolve_expression(v, fn_get_var, path)
         if pending_var:
             pending[path] = pending_var
         elif resolved != v:
             changed[path] = v
         return resolved
 
     data = deep_update_object_value(obj, fn_change)
     return {
         'changed': changed,
         'pending': pending,
         'data': data
     }
 
-def resolve_expression(expr, fn_get_value) -> Tuple[Any, str]:
+def resolve_expression(expr, fn_get_value, referencing_attr_path) -> Tuple[Any, str]:
     """Try resolving expression. Returned updated value and None, or value and pending var name"""
     
     if not isinstance(expr, str):
         return expr, None
     # get variable names from expr
     m1 = _pattern_var.match(expr)
     if not m1:
@@ -244,17 +245,17 @@
         src_var_name = m2.group(2)
         mapped_value = m2.group(3)
 
         target_value, found = fn_get_value(src_var_name)
         if not found:
             return expr, src_var_name
         if not isinstance(target_value, list):
-            raise Exception(f"Invalid variable value for expression. Expect list, actual {type(replacement).__name__}. attr_path={path}, src_var_name={src_var_name}")
+            raise CtxpException(f"Invalid variable value for expression. Expect list, actual {type(target_value).__name__}. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
         if not mapped_value.startswith(tmp_var_name + '.'):
-            raise Exception(f"Unsupported expression. attr_path={path}, src_var_name={src_var_name}")
+            raise CtxpException(f"Unsupported expression. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
         new_attr_path = mapped_value[len(tmp_var_name) + 1:]
         ret = []
         for i in target_value:
             item = deep_get_attr(i, new_attr_path)
             ret.append(item)
         return ret, None  #replace the entire value using the new value.
     else:
@@ -263,15 +264,15 @@
         actual_value, found = fn_get_value(var_name)
         if not found:
             return expr, var_name
         if isinstance(actual_value, str):
             return expr.replace('${' + var_name + '}', actual_value), None
         # replacement is an object. Make sure this var is the entire value.
         if len(expr) != len(var_name) + 3:
-            raise Exception(f"Invalid replacing variable with object. attr_path={attr_path}, var_name={var_name}, replacement={str(value)}")
+            raise CtxpException(f"Invalid variable: can not replace variable in string with non-string. attr_path={referencing_attr_path}, var_name={var_name}, replacement={actual_value}, expr={expr}")
         return actual_value, None
         
 def to_json(o) -> str:
     class SetEncoder(json.JSONEncoder):
         def default(self, obj):
             if isinstance(obj, set):
                 return list(obj)
```

### Comparing `hcs-cli-0.1.46/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.47/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/plan/core.py` & `hcs-cli-0.1.47/vhcs/plan/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,81 +10,96 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import threading
-import traceback
 import typing
 import inspect
-import time
 import re
 from subprocess import CalledProcessError
 from copy import deepcopy
 import vhcs.common.util as util
-from . import helper
 from . import dag
-from .helper import PlanException
+from . import context
+from .helper import PlanException, process_template
+from .actions import actions
+from .kop import KOP
 from importlib import import_module
 
 import logging
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
-def _prepare_data(data: dict, additional_context: dict):
+def _prepare_data(data: dict, additional_context: dict, resource_name: str):
     if additional_context:
         common_items = util.get_common_items(additional_context.keys(), data.keys())
         if common_items:
             raise PlanException("blueprint and context have conflict keys: " + str(common_items))
         data.update(additional_context)
-    blueprint, pending = helper.process_template(data)
+    blueprint, pending = process_template(data)
+    if resource_name and resource_name not in blueprint['resources']:
+        raise PlanException("Resource target not found: " + resource_name)
+    
+    for k, v in pending.items():
+        if v.startswith('defaults.') or v.startswith('vars.'):
+            raise PlanException(f"Invalid blueprint. Unresolved static references. Variable not found: {v}. Required by {k}")
     deployment_id = blueprint['deploymentId']
     state_file = deployment_id + '.state.yml'
     prev = _load_state(state_file)
     state = {'pending': pending}
     state.update(blueprint)
     state.update(prev)
 
+    context.set('deploymentId', state['deploymentId'])
+    
     # try solving more variables
     # for k, v in state['output'].items():
     #     if not v:
     #         continue
     #     if not _has_successful_deployment(state, k):
     #         continue
     #     _resolve_pending_keys(state, k)
     
     return blueprint, state, state_file
 
 # def _has_successful_deployment(state, name):
-#     for v in state['log']['deploy']:
+#     for v in state['log']['create']:
 #         if v['name'] != name:
 #             continue
 #         if v['action'] == 'success':
 #             return True
         
-def deploy(data: dict, additional_context: dict = None, resource_name: str = None, concurrency: int = 4):
+def deploy(data: dict, additional_context: dict = None, resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4):
     
-    blueprint, state, state_file = _prepare_data(data, additional_context)
-    state['log']['deploy'] = []    # clear deploy log
+    blueprint, state, state_file = _prepare_data(data, additional_context, resource_name)
+    state['log']['create'] = []    # clear deploy log
 
     def process_resource(name: str):
         # ignore functional nodes (defaults, providers)
         if name not in blueprint['resources']:
             return
         res_data = blueprint['resources'][name]
         
-        _deploy_res(name, res_data, state)
-        #_resolve_pending_keys(state, name)
-        util.save_data_file(state, state_file)
+        if resource_name:
+            if name == resource_name or include_related_resources:
+                need_deploy = True
+            else:
+                need_deploy = False
+        else:
+            need_deploy = True
+        if need_deploy:
+            _deploy_res(name, res_data, state)
+            util.save_data_file(state, state_file)
         if resource_name and name == resource_name:
-            return False
+            return False    # quit dag.process_blueprint
 
     try:
-        dag.process_blueprint(blueprint, process_resource, concurrency)
+        dag.process_blueprint(blueprint, process_resource, False, concurrency)
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
         util.save_data_file(state, state_file)
 
 def _load_state(state_file):
     state = util.load_data_file(state_file, default={})
@@ -162,89 +177,77 @@
         
     if resource_name in state:
         try:
             return util.deep_get_attr(state, var_name), True
         except Exception as e:
             log.debug(e)
             return None, False
+    return None, False
 
 def _deploy_res(name, res, state):
-    def add_log(action: str, details: str = None):
-        _add_log(state, 'deploy', res['kind'], name, action, details)
-
-    def fn_deploy1(handler, res_data, res_state, fn_set_state):
-        if res_state and not _is_runtime(res):
-            add_log('skipped')
+    def fn_deploy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
+        if _is_runtime(res):
+            kop.start(KOP.MODE.create)
+            new_state = handler.process(res_data, deepcopy(state))
+            if new_state:
+                fn_set_state(new_state)
+            return
+        
+        if not res_state:
+            action = actions.create
+        else:
+            action = handler.decide(res_data, res_state)
+            
+        if action == actions.skip:
+            kop.skip('Already deployed')
             return
         
-        add_log('start')
-        if _has_save_state(handler.deploy):
-            new_state = handler.deploy(res_data, fn_set_state)
+        if action == actions.recreate:
+            with KOP(state, res['kind'], name) as kop2:
+                kop2.id = res_state.get('id')
+                kop2.start(KOP.MODE.delete)
+                handler.destroy(res_data, res_state)
+            action = actions.create
+
+        new_state = None
+        if action == actions.create:
+            kop.start(KOP.MODE.create)
+            if _has_save_state(handler.deploy):
+                new_state = handler.deploy(res_data, res_state, fn_set_state)
+            else:
+                new_state = handler.deploy(res_data, res_state)
+            kop.id(None if not new_state else new_state.get('id'))
+        elif action == actions.update:
+            kop.id(res_state.get('id'))
+            kop.start(KOP.MODE.update)
+            if _has_save_state(handler.update):
+                new_state = handler.update(res_data, res_state, fn_set_state)
+            else:
+                new_state = handler.update(res_data, res_state)
         else:
-            new_state = handler.deploy(res_data)
+            raise PlanException(f"Unknown action. Plugin={name}, action={action}")
+        
         if new_state:
             fn_set_state(new_state)
-        add_log('success')
-    
-    _handle_resource(name, res, state, True, add_log, fn_deploy1)
+    _handle_resource(name, res, state, True, fn_deploy1)
 
 def _is_runtime(res):
     kind = res.get('kind')
     return kind and kind.startswith('runtime/')
 
 def _has_save_state(fn):
     signature = inspect.signature(fn)
     args = list(signature.parameters.keys())
-    if len(args) < 2:
+    if len(args) < 3:
         return False
-    name = args[1]
+    name = args[2]
     if name == 'save_state':
         return True
-    p = signature.parameters[args[1]]
+    p = signature.parameters[args[2]]
     return p.annotation == typing.Callable
-    
-# def _convert_resource_path_to_readable_path(state, attr_path: str):
-#     pattern = r'resources\[(\d+)\]\..+'
-#     match = re.search(pattern, attr_path)
-#     if match:
-#         i = int(match.group(1))
-#         name = state['resources'][i]['name']
-#         n = attr_path.index(']')
-#         readable_path = 'resources.' + name + attr_path[n + 1:]
-#         return readable_path
-#     return attr_path
-
-# def _resolve_pending_keys(state, resource_name):
-#     prefix = resource_name + "."
-#     for attr_path, var_name in state['pending'].items():
-#         if not var_name.startswith(prefix) and var_name != resource_name:
-#             continue
-#         # found a key to solve
-        
-#         # update that key
-#         expr = util.deep_get_attr(state, attr_path)
-#         def _get_value(path):
-#             return _get_value_by_path(state, path, attr_path), True
-#         resolved_value, _pending_var = util.resolve_expression(expr, _get_value)
-
-#         log.debug('Resolved. %s: %s -> %s', attr_path, var_name, resolved_value)
-#         util.deep_set_attr(state, attr_path, resolved_value)
-
-def _resolve_vars(data, state, resource_name, raise_on_unresolvable):
-    data = deepcopy(data)
-    def _get_value(path):
-        return _get_value_by_path2(state, path)
-    ret = util.process_variables(data, _get_value)
-    if raise_on_unresolvable:
-        if ret['pending']:
-            msg = f"Fail resolving variables for resource '{resource_name}'. Unresolvable variables: {ret['pending']}"
-            raise PlanException(msg)
-    
-    state['resources'][resource_name]['data'] = data
-    return data
 
 def _assert_all_vars_resolved(data, name):
     def fn_on_value(path, value):
         if isinstance(value, str) and value.find('${') >= 0:
             raise PlanException(f"Unresolved variable '{path}' for plugin '{name}'. Value={value}")
         return value
     util.deep_update_object_value(data, fn_on_value)
@@ -273,152 +276,154 @@
             _providers[provider_type] = 1
     module_name = f"vhcs.plan.provider.{provider_type}.{res_handler_type}"
     return import_module(module_name)
 
 def get_common_items(iter1, iter2):
     return set(iter1).intersection(set(iter2))
 
-def _handle_resource(name, res, state, vars_must_resolve: bool, add_log: typing.Callable, fn_process: typing.Callable):
-    try:
-        kind = res['kind']
+def _handle_resource(name, res, state, for_deploy: bool, fn_process: typing.Callable):
+    kind = res['kind']
+
+    kop_mode = KOP.MODE.create if for_deploy else KOP.MODE.delete
+    with KOP(state, kind, name, kop_mode) as kop:
         data = res.get('data', {})
+
+        # resolve vars
+        def _get_value(path):
+            return _get_value_by_path2(state, path)
+        
         if data:
-            data = _resolve_vars(data, state, name, vars_must_resolve)
+            data = deepcopy(data)
+            ret = util.process_variables(data, _get_value)
+            if for_deploy:
+                if ret['pending']:
+                    msg = f"Fail resolving variables for resource '{name}'. Unresolvable variables: {ret['pending']}"
+                    raise PlanException(msg)
+        state['resources'][name] = dict(res)
+        state['resources'][name]['data'] = data
+
+        conditions = res.get('conditions')
+        if conditions:
+            conditions = deepcopy(conditions)
+            ret = util.process_variables(conditions, _get_value)
+            unsatisfied_condition_name = _get_unsatisfied_condition_name(conditions)
+            if unsatisfied_condition_name:
+                kop.skip('Condition not met: ' + unsatisfied_condition_name)
+                return
+
 
         handler = _get_resource_handler(kind, state)
-        def _handle_resource_1(resource_data, resource_state, fn_set_state):
+        def _handle_resource_1(resource_data, resource_state, fn_set_state, kop):
             if _is_runtime(res):   # runtime has no refresh
                 pass
             else:
                 new_state = handler.refresh(resource_data, resource_state)
-                if new_state:
-                    fn_set_state(new_state)
-                    resource_state = new_state
+                fn_set_state(new_state)
+                resource_state = new_state
 
-            fn_process(handler, resource_data, resource_state, fn_set_state)
+            fn_process(handler, resource_data, resource_state, fn_set_state, kop)
 
         for_var_name, values = _parse_statement_for(name, state)
         if for_var_name:
             if for_var_name in data:
                 raise PlanException(f"Invalid blueprint: variable name defined in for-statement already exists in data declaration. Resource: {name}. Conflicting names: {common}")
-            
+            kop.id('(group)')
+            kop.start()
             size = len(values)
             # ensure output array placeholder
             output = state['output'].setdefault(name, [])
             while len(output) < size:
                 output.append(None)
             for i in range(size):
                 v = values[i]
-                resource_state = output[i]
-                def _fn_set_state(o):
-                    output[i] = deepcopy(o)
-                resource_data = deepcopy(data)
-                resource_data[for_var_name] = v
-                _handle_resource_1(resource_data, resource_state, _fn_set_state)
+                with KOP(state, kind, name, kop_mode) as kop_per_item:
+                    kop_per_item.id(str(i))
+                    resource_state = output[i]
+                    def _fn_set_state(o):
+                        output[i] = deepcopy(o)
+                    resource_data = deepcopy(data)
+                    resource_data[for_var_name] = v
+                    _handle_resource_1(resource_data, resource_state, _fn_set_state, kop_per_item)
         else:
             resource_state = state['output'].get(name)
             def _fn_set_state(o):
                 state['output'][name] = deepcopy(o)
             resource_data = deepcopy(data)
-            _handle_resource_1(resource_data, resource_state, _fn_set_state)
-    except Exception as e:
-        add_log('error', e)
-        raise
+            _handle_resource_1(resource_data, resource_state, _fn_set_state, kop)
+
+def _get_unsatisfied_condition_name(conditions):
+    if not conditions:
+        return
+    for condition_name, expr in conditions.items():
+        if not expr:
+            return condition_name
+        if expr.find('${') >= 0: # still have unresolved variables
+            return condition_name
 
-    
-def _add_log(state: dict, mode: str, kind: str, name: str, action: str, details = None):
-    if mode == 'deploy':
-        labels = {
-            'start':   '[creating]',
-            'success': '[created ]',
-            'skipped': '[skipped ]',
-            'error':   '[error   ]'
-        }
-    elif mode == 'destroy':
-        labels = {
-            'start':   '[deleting]',
-            'success': '[deleted ]',
-            'skipped': '[skipped ]',
-            'error':   '[error   ]'
-        }
-    else:
-        raise PlanException("Invalid log mode: " + mode)
-    log.info(f'{labels[action]} {kind}:{name}')
-    entry = {
-        'name': name,
-        'time': time.time(),
-        'action': action
-    }
-    if details:
-        if isinstance(details, Exception):
-            if isinstance(details, PlanException) or isinstance(details, CalledProcessError):
-                pass
-            else:
-                e = details
-                traceback.print_exception(type(e), e, e.__traceback__)
-            details = details.__class__.__name__ + ': ' + str(details)
-        else:
-            details = str(details)
-        entry['details'] = details
-    state['log'][mode].append(entry)
-    if action == 'error':
-        log.warning('Plugin "%s:%s" failed: %s', kind, name, details)
 
 
-def _destroy_res(name, res_node, state, force):
-    def add_log(action: str, details: str = None):
-        _add_log(state, 'destroy', res_node['kind'], name, action, details)
 
-    def fn_destroy1(handler, res_data, res_state, fn_set_state):
+def _destroy_res(name, res_node, state, force):
+    def fn_destroy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
         if not res_state:
-            add_log('skipped', 'Not found')
+            kop.skip('Not found')
             return
         
-        add_log('start')
+        kop.id(res_state.get('id'))
+        kop.start(KOP.MODE.delete)
         try:
             ret = handler.destroy(res_data, res_state)
             state['destroy_output'][name] = deepcopy(ret)
             fn_set_state(None)
-            add_log('success', 'Deleted')
         except Exception as e:
             if force:
-                add_log('error', e)
+                kop.error(e)
                 pass
             else:
                 # add_log('error', e) will be handled by framework.
                 raise
+    _handle_resource(name, res_node, state, False, fn_destroy1)
 
-    _handle_resource(name, res_node, state, False, add_log, fn_destroy1)
-
-def destroy(data, force: bool, resource_name: str = None, concurrency: int = 4, additional_context: dict = None):
+def destroy(data, force: bool, resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4, additional_context: dict = None):
     
-    blueprint, state, state_file = _prepare_data(data, additional_context)
-    state['log']['destroy'] = []    # clear destroy log
+    blueprint, state, state_file = _prepare_data(data, additional_context, resource_name)
+    state['log']['delete'] = []    # clear destroy log
 
     def destroy_resource(node_name):
         # ignore functional nodes (defaults, providers)
         node = blueprint['resources'].get(node_name)
         if not node:
             return
         # skip runtime
         if node['kind'].startswith('runtime/'):
             return
         
         res_node = state['resources'].get(node_name)
         if not res_node:
             res_node = blueprint['resources'][node_name]
-        _destroy_res(node_name, res_node, state, force)
-        util.save_data_file(state, state_file)
-        if resource_name and resource_name == node_name:
-            return True
+
+        if resource_name:
+            if include_related_resources:
+                pass
+            else:
+                if resource_name != node_name:
+                    return
+            _destroy_res(node_name, res_node, state, force)
+            util.save_data_file(state, state_file)
+            if resource_name == node_name:
+                return True
+        else:
+            _destroy_res(node_name, res_node, state, force)
+            util.save_data_file(state, state_file)
 
     try:
-        dag.reverse_traverse(blueprint, destroy_resource)
+        dag.process_blueprint(blueprint, destroy_resource, True, concurrency)
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
         util.save_data_file(state, state_file)
 
 def graph(data: dict, additional_context: dict = None, simplify: bool = True):
-    blueprint, state, state_file = _prepare_data(data, additional_context)
+    blueprint, state, state_file = _prepare_data(data, additional_context, None)
     g = dag.graph(blueprint, state, simplify)
-    return g
+    return g
+
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/dag.py` & `hcs-cli-0.1.47/vhcs/plan/dag.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,35 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from copy import deepcopy
 import time
 import threading
 from graphlib import TopologicalSorter
 from graphviz import Digraph
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable
-from vhcs.common import util
+
 
 class Node:
     id: str
     dependencies: list[str] = []
     data: Any = None
 
 class DAG:
-    graph: dict[str, set[str]] = {}
-    data: dict[str, Any] = {}
+    graph: dict[str, set[str]]
+    data: dict[str, Any]
+
+    def __init__(self):
+        self.graph = {}
+        self.data = {}
 
     def add(self, id: str, data: Any, dependencies = None):
         if id in self.data:
             raise Exception('Node already added to graph: ' + id)
         self.data[id] = data
         self.graph[id] = set(dependencies) if dependencies else set()
 
@@ -40,44 +45,33 @@
     def validate(self):
         all_keys = self.data.keys()
         for k, v in self.graph.items():
             for d in v:
                 if d not in all_keys:
                     raise Exception(f"Blueprint error: target dpendency not found: from={k}, target={d}")
     
-def process_blueprint(blueprint, fn_process_node: Callable, concurrency: int = 3):
+def process_blueprint(blueprint, fn_process_node: Callable, reverse: bool, concurrency: int = 3):
     dag = _build_graph(blueprint)
-    return _walkthrough(dag, fn_process_node, concurrency)
 
-def reverse_traverse(blueprint, fn_process_node):
-    # TODO: this is sequential so far
-    dag = _build_graph(blueprint)
-    dag.validate()
-
-    topological_sorter = TopologicalSorter(dag.graph)
-    sequence = list(topological_sorter.static_order())
-    sequence.reverse()
+    if reverse:
+        _reverse_dag(dag)
 
-    for node_name in sequence:
-        stop = fn_process_node(node_name)
-        if stop == True:
-            break
+    return _walkthrough(dag, fn_process_node, concurrency)
 
 def _build_graph(blueprint):
     dag = DAG()
 
+    from vhcs.common import util
     def add_node(name, obj):
-        data = obj.get('data')
         dependencies = set()
-        if data:
-            variables = util.deep_find_variables(data)
-            for v in variables:
-                i = v.find('.')
-                resource_name = v if i < 0 else v[:i]
-                dependencies.add(resource_name)
+        variables = util.deep_find_variables(obj)
+        for v in variables:
+            i = v.find('.')
+            resource_name = v if i < 0 else v[:i]
+            dependencies.add(resource_name)
         after = obj.get('after')
         if after:
             def _add(t):
                 if t in dependencies:
                     raise Exception("Invalid blueprint: statement after contains a dependency that is already implicitly created. This is not necessary. Key: " + t)
                 dependencies.add(t)
             if isinstance(after, str):
@@ -88,14 +82,17 @@
         dag.add(name, obj, dependencies)
     
     for k,v in blueprint['resources'].items():
         add_node(k, v)
     defaults = blueprint.get('defaults')
     if defaults:
         add_node('defaults', defaults)
+    vars = blueprint.get('vars')
+    if vars:
+        add_node('vars', vars)
     providers = blueprint.get('providers')
     if providers:
         for p in providers:
             add_node(p['type'], p)
     
     dag.validate()
     return dag
@@ -135,15 +132,15 @@
                 time.sleep(1)
                 continue
             for node in read_nodes:
                 executor.submit(process_node, node)
         executor.shutdown(wait=True)
         if flags['err']:
             raise flags['err']
-
+        
 def _has_indirect_dependency(tree: dict, from_node: str, to_node: str):
     deps = list(tree[from_node])
     deps.remove(to_node)
     while deps:
         n = deps.pop()
         new_deps = tree[n]
         if to_node in new_deps:
@@ -206,21 +203,47 @@
         for dependency in dependencies:
             if simplify and _has_indirect_dependency(dag.graph, from_node=node, to_node=dependency):
                 continue    #simplify the diagram by removing ommitable 
             graph.edge(dependency, node)
 
     return graph
 
-# dag = DAG()
-# dag.add("b", "b")
-# dag.add("a", "a", {"b", "c"})
-# dag.add("c", "c")
-
-# def fn_proc(id, data):
-#     print("processing", id, data)
-#     import time
-#     import random
-#     time.sleep(random.randint(0, 2))
-#     raise Exception('demo error')
+def _reverse_dag(dag: DAG):
+    old_dep = deepcopy(dag.graph)
+    dag.graph = {}
+    for k, h in old_dep.items():
+        dag.graph[k] = set()
+
+    def add_dep(from_node: str, to_node: str):
+        holder = dag.graph[from_node]
+        holder.add(to_node)
+    
+    for k, h in old_dep.items():
+        for t in h:
+            add_dep(t, k)
 
-# _walkthrough(dag, fn_proc, 1)
-# print('exit')
+
+
+def _test(reverse):
+    print('reverse=', reverse)
+    dag = DAG()
+    dag.add("a", "a")
+    dag.add("b1", "b1", {"a"})
+    dag.add("b2", "b2", {"a"})
+    dag.add("c", "c", {"b1"})
+    dag.add("d", "d", {"b2", "c"})
+
+    if reverse:
+        _reverse_dag(dag)
+
+    def fn_proc(id):
+        print("-> ", id)
+        print('sleeping', id)
+        time.sleep(2)
+        print("<- ", id)
+
+    _walkthrough(dag, fn_proc, 3)
+    print('exit')
+
+if __name__ == '__main__':
+    _test(False)
+    _test(True)
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/helper.py` & `hcs-cli-0.1.47/vhcs/plan/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from typing import Tuple
 import os
 from vhcs.common.util import load_data_file, strict_dict_to_class, process_variables
 
 class PlanException(Exception):
     pass
 
+class PluginException(Exception):
+    pass
+
 class Blueprint:
     vars: dict
     defaults: dict = {}
     providers: list = []
     resources: list
 
     def __repr__(self):
@@ -38,25 +41,43 @@
         if data == None or isinstance(data, str):
             raise FileNotFoundError("Fail loading file: " + file)
         ret = _merge_dict_fail_on_dup(ret, _smart_load_file(file))
     return ret
 
 
 def process_template(template) -> Tuple[dict, dict]:
+    _validate_blueprint(template)
     bp, pending = _materialize_blueprint(template)
-    _validate_blueprint(bp)
     return bp, pending
 
 def _validate_blueprint(blueprint: dict):
+    _validate_resource_schema(blueprint)
     _validate_resource_id_no_dup(blueprint)
     _validate_resource_id_not_conflict_to_reserved_names(blueprint)
     _validate_resource_id_not_conflict_to_provider_types(blueprint)
     _validate_no_duplicate_provider_config(blueprint)
     _validate_statement_after(blueprint)
 
+def _validate_resource_schema(blueprint: dict):
+    resources = blueprint.get('resources')
+    if not resources:
+        return
+    required_keys = set(['kind'])
+    optional_keys = set(['data', 'conditions', 'for', 'after'])
+    for k, v in resources.items():
+        def _raise(reason):
+            raise PlanException(f"Invalid blueprint: {reason}. Resource: {k}")
+        actual_keys = set(v.keys())
+        missed_keys = required_keys - actual_keys
+        if missed_keys:
+            _raise(f'Missing required keys: {missed_keys}')
+        extra_keys = actual_keys - required_keys - optional_keys
+        if extra_keys:
+            _raise(f'Unknown extra keys: {extra_keys}')
+
 def _get_duplicates(lst):
     return [item for item in set(lst) if lst.count(item) > 1]
 
 def _validate_statement_after(blueprint: dict):
 
     def _raise(owner, reason):
         raise PlanException(f"Invalid statement: after. Owner={owner}, reason={reason}.")
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/_az_facade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 from . import _az_facade as az
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     display_name = data['displayName']
     mail_nickname = data['mailNickname']
     description = data.get('description')
     parent_group = data.get('parentGroup')
     ret = az.aad.group.create(display_name, mail_nickname, description)
     if parent_group:
         az.aad.group.member.add(parent_group, ret['id'])
     return ret
 
 
 def refresh(data: dict, state: dict) -> dict:
     display_name = data['displayName']
     return az.aad.group.get(display_name)
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     if state:
         id = state['id']
         return az.aad.group.delete(id)
     display_name = data['displayName']
     return az.aad.group.delete(display_name)
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 import random
 from . import _az_facade as az
 
-def deploy(data: dict) -> dict:
+def deploy(data: dic, state: dict) -> dict:
     group = data['group']
     email = data['email']
     domain_name = data['domainName']
 
     pname = _convert_email_to_principle(email, domain_name)
     display_name = pname
     password = _generate_password()
@@ -47,11 +48,14 @@
         if ret:
             return ret
     email = data['email']
     domain_name = data['domainName']
     pname = _convert_email_to_principle(email, domain_name)
     return az.aad.user.get(pname)
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     id = state['id']
     ret = az.aad.user.delete(id)
     return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/nsg.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 from . import _az_facade as az
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     name = data['name']
     location = data['location']
     resourceGroup = data['resourceGroup']
     tags = data.get('tags')
 
     return az.network.nsg.create(resourceGroup, name, location, tags)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     if state.get('NewNSG'):
         id = state.get('NewNSG')['id']
         return az.network.nsg.delete_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
     return az.network.nsg.delete(name, resourceGroup)
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/resource_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 from . import _az_facade as az
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     name = data['name']
     location = data['location']
     tags = data.get('tags')
     return az.resource_group.create(name, location, tags)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     name = data['name']
     return az.resource_group.delete(name)
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.47/vhcs/plan/provider/azure/subnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 from . import _az_facade as az
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     name = data['name']
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
     cidr = data['cidr']
     nsgName = data['nsgName']
 
     return az.network.subnet.create(resourceGroup, vNetName, name, cidr, nsgName)
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     id = state.get('id')
     if id:
         return az.network.subnet.delete_by_id(id)
     name = data['name']
     resourceGroup = data['resourceGroup']
     vNetName = data['vNetName']
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.47/vhcs/plan/provider/dev/dummy.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,35 +13,41 @@
 limitations under the License.
 """
 
 import time
 from copy import deepcopy
 from typing import Callable
 import vhcs.common.duration as duration
-from vhcs.plan import PlanException
+from vhcs.plan import actions
+from vhcs.plan import PluginException
 
-def deploy(data: dict, save_state: Callable) -> dict:
-
-    text = data.get('text')
-    error = data.get('error')
-    delay = data.get('delay')
-    error_before_save = data.get('error_before_save')
 
+def deploy(data: dict, state: dict, save_state: Callable) -> dict:
+    text = data.get("text")
+    error = data.get("error")
+    delay = data.get("delay")
+    error_before_save = data.get("error_before_save")
     delay_seconds = duration.to_seconds(delay)
     if delay_seconds:
         time.sleep(delay_seconds)
     ret = deepcopy(data)
-    ret['outputText'] = text
+    ret["outputText"] = text
 
     if not error_before_save:
         save_state(ret)
 
     if error:
-        raise PlanException(error)
-        
+        raise PluginException(error)
+
     return ret
 
+
 def refresh(data: dict, state: dict) -> dict:
     return state
 
+
+def decide(data: dict, state: dict):
+    return actions.skip
+
+
 def destroy(data: dict, state: dict) -> dict:
-    return {}
+    return {}
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/entitlement.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,27 @@
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
+from vhcs.plan import actions
 from vhcs.service import portal
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     return portal.entitlement.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
     if state:
         id = state.get('id')
         if id:
             return portal.entitlement.get(id, data['orgId'])
     
     # Fall back with smart find by users
     # TODO
 
+def decide(data: dict, state: dict):
+    return actions.skip
+    
 def destroy(data: dict, state: dict) -> dict:
     return portal.entitlement.delete(state['id'], data['orgId'])
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/launch_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from ulid import ULID
+from vhcs.plan import actions
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     users = data['users']
     entitlementId = data['entitlementId']
     domainName = data['domainName']
     stackUrl = data['stackUrl']
 
     launch_items = []
 
@@ -33,9 +34,12 @@
         
     return launch_items
     
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     return {}
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 import vhcs.service.portal as portal
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     return portal.pool.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
     if state:
         id = state.get('id')
         if id:
             return portal.pool.get(id, data['orgId'])
     
     # Fall back with smart find by name
     pools = portal.pool.list(search=f"name $eq {data['name']}")
     if pools and len(pools) == 1:
         return pools[0]
     return state
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     if state:
         id = state.get('id')
         if id:
             return portal.pool.delete(id, data['orgId'])
     return state
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/ad.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,44 +9,34 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Callable
-from vhcs.plan import PlanException
-import vhcs.service.admin as admin
+from vhcs.plan import actions
+from vhcs.service import admin
 
-def deploy(data: dict, save_state: Callable) -> dict:
-    ret = admin.template.create(data)
-    save_state(ret)
-    id = ret['id']
-    ready, template = admin.template.wait_for_template_ready(id, timeout_seconds=600)
-    if not ready:
-        save_state(template)
-        raise PlanException("Template deployment failed.")
-    return admin.template.get(id)
+def deploy(data: dict, state: dict) -> dict:
+    label = data['providerLabel']
+    return admin.ad.create(label, data)
 
 def refresh(data: dict, state: dict) -> dict:
+    org_id = data['orgId']
     if state:
-        id = state['id']
+        id = state.get('id')
         if id:
-            t = admin.template.get(id)
-            if t:
-                return t
+            return admin.ad.get(id, org_id)
     
     # Fall back with smart find by name
-    name = data['name']
-    search = 'name $eq ' + name
-    templates = admin.template.list(org_id=data['orgId'], search=search)
-    if templates:
-        return templates[0]
+    search = "name $eq " + data['name']
+    ads = admin.ad.list(org_id=org_id, search=search)
+    if ads:
+        return ads[0]
+
+def decide(data: dict, state: dict):
+    return actions.skip
 
 def destroy(data: dict, state: dict) -> dict:
-    if state:
-        id = state['id']
-        if id:
-            admin.template.delete(id)
-            admin.template.wait_for_template_deleted(id, 600)
-            return
-    
+    org_id = data['orgId']
+    id = state['id']
+    return admin.ad.delete(id, org_id)
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/provider.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/identity_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.service import admin
+from vhcs.plan import actions
+from vhcs.service import portal
 
-def deploy(data: dict) -> dict:
-    return admin.provider.create(data)
+def deploy(data: dict, state: dict) -> dict:
+    return portal.site.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
     org_id = data['orgId']
-    label = data['label']
     if state:
         id = state.get('id')
         if id:
-            return admin.provider.get(label, id)
+            ret = portal.site.get(id, org_id)
+            if ret:
+                return ret
     
     # Fall back with smart find by name
-    return admin.provider.find_by_name(data['name'], org_id)
+    return portal.site.find_by_name(data['name'], org_id)
+
+def decide(data: dict, state: dict):
+    return actions.skip
 
 def destroy(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    label = data['label']
-    id = state['id']
-    return admin.provider.delete(label, id, org_id)
+    return portal.site.delete(state['id'], data['orgId'])
```

### Comparing `hcs-cli-0.1.46/vhcs/plan/provider/hcs/site.py` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/site.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from vhcs.plan import actions
 from vhcs.service import portal
 
-def deploy(data: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     return portal.site.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
     org_id = data['orgId']
     if state:
         id = state.get('id')
         if id:
-            return portal.site.get(id, org_id)
+            ret = portal.site.get(id, org_id)
+            if ret:
+                return ret
     
     # Fall back with smart find by name
     return portal.site.find_by_name(data['name'], org_id)
 
+def decide(data: dict, state: dict):
+    return actions.skip
+
 def destroy(data: dict, state: dict) -> dict:
     return portal.site.delete(state['id'], data['orgId'])
```

### Comparing `hcs-cli-0.1.46/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.47/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/service/admin/edge.py` & `hcs-cli-0.1.47/vhcs/service/auth/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
+_client = hdc_service_client("auth")
 
-def get(id: str, **kwargs):
-    url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
+def get_org_idp_map(**kwargs):
+    url = with_query(f"/v1/admin/org-idp-map", **kwargs)
     return _client.get(url)
 
-def list(**kwargs):
-    def _get_page(query_string):
-        url = "/v2/edge-deployments?" + query_string
-        return _client.get(url)
-
-    return PageRequest(_get_page, **kwargs).get()
+#def create_org_idp_map():
```

### Comparing `hcs-cli-0.1.46/vhcs/service/admin/helper.py` & `hcs-cli-0.1.47/vhcs/service/admin/helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,22 +14,15 @@
 """
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
 
-def list(**kwargs):
-    def _get_page(query_string):
-        url = "/v2/templates?" + query_string
-        return _client.get(url)
-
-    return PageRequest(_get_page, **kwargs).get()
 
 def list_resources_by_provider(resource_type: str, provider_instance_id: str, limit: int = 10):
     def _get_page(query_string):
         url = f"/v2/{resource_type}?" + query_string
         return _client.get(url)
 
     search = f"providerInstanceId $eq {provider_instance_id}"
     return PageRequest(_get_page, search=search, limit=limit).get()
-
```

### Comparing `hcs-cli-0.1.46/vhcs/service/admin/provider.py` & `hcs-cli-0.1.47/vhcs/service/admin/provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 """
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
 
-def list(label: str, **kwargs):
+def list(label: str, org_id: str, **kwargs):
     def _get_page(query_string):
-        url = f"/v2/providers/{label}/instances?{query_string}"
+        url = f"/v2/providers/{label}/instances?{query_string}?org_id={org_id}"
         return _client.get(url)
 
     return PageRequest(_get_page, **kwargs).get()
 
-def get(label: str, id: str, **kwargs):
-    url = f"/v2/providers/{label}/instances/{id}"
+def get(label: str, id: str, org_id: str, **kwargs):
+    url = f"/v2/providers/{label}/instances/{id}?org_id={org_id}"
     url = with_query(url, **kwargs)
     return _client.get(url)
 
 def create(label: str, payload):
     return _client.post(f"/v2/providers/{label}/instances", json=payload)
 
 
-def delete(label: str, id: str):
-    return _client.delete(f"/v2/templates/{label}/instances/{id}") 
+def delete(label: str, id: str, org_id: str, **kwargs):
+    url = f"/v2/providers/{label}/instances/{id}?org_id={org_id}"
+    url = with_query(url, **kwargs)
+    return _client.delete(url)
```

### Comparing `hcs-cli-0.1.46/vhcs/service/auth/admin.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/ims/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
-from vhcs.util.query_util import with_query, PageRequest
+import click
+from vhcs.service import ims
+import vhcs.common.sglib.cli_options as cli
 
-_client = hdc_service_client("auth")
 
-def get_org_idp_map(**kwargs):
-    url = with_query(f"/v1/admin/org-idp-map", **kwargs)
-    return _client.get(url)
+@click.command()
+@click.option("--limit", "-l", type=int, required=False, default=20)
+@cli.org_id
+@cli.search
+def list(org: str, **kwargs):
+    """List images"""
+    org_id = cli.get_org_id(org)
+    return ims.images.list(org_id, **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,23 +9,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from . import images, image_copies
+import click
+from vhcs.service import admin
+import vhcs.common.sglib.cli_options as cli
 
-def get_images_by_provider_instance_with_asset_details(providerInstanceId: str):
-    all_images = images.list()
-    copies = image_copies.list(include_catalog_details=True,
-                      search=f"providerInstanceId $eq {providerInstanceId}")
-    ret = []
-    for copy in copies:
-        imageId = copy["catalogDetails"]["imageId"]
-        for image in all_images:
-            if image['id'] == imageId:
-                # add additional info
-                image['_assetDetails'] = copy['assetDetails']
-                ret.append(image)
-                break
-    return ret 
+
+@click.command()
+@click.argument('template-id', type=str, required=True)
+@cli.org_id
+def list(template_id: str, org: str, **kwargs):
+    """List template VMs"""
+    return admin.template.list_vms(template_id, org_id=cli.org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.46/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.47/vhcs/service/ims/image_copies.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import PageRequest
 
 _client = hdc_service_client("ims-catalog")
 
 
-def list(**kwargs):
+def list(org_id: str, **kwargs):
     def _get_page(query_string):
-        url = f"/v1/image-copies?{query_string}"
+        url = f"/v1/image-copies?org_id={org_id}&{query_string}"
         return _client.get(url)
     return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.46/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.47/vhcs/service/org_service/datacenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
-from vhcs.util.query_util import PageRequest
+from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("ims-catalog")
+_client = hdc_service_client("org-service")
 
 
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/datacenters/{id}", **kwargs)
+    return _client.get(url)
+
 def list(**kwargs):
-    def _get_page(query_string):
-        url = f"/v1/images?{query_string}"
-        return _client.get(url)
-    return PageRequest(_get_page, **kwargs).get()
+    url = with_query(f"/v1/datacenters", **kwargs)
+    return _client.get(url)
+
+def find_by_org(orgId, **kwargs):
+    url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
+    return _client.get(url)
+
```

### Comparing `hcs-cli-0.1.46/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.47/vhcs/service/inventory/vm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.47/vhcs/service/portal/site.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,42 +9,40 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import json
-from typing import Any
+import logging
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("lcm")
+log = logging.getLogger(__name__)
+_client = hdc_service_client("portal")
 
 
-def get(id: str, **kwargs: Any):
-    url = with_query(f"/v1/providers/{id}", **kwargs)
+def create(payload: dict):
+    url = "/v2/sites"
+    return _client.post(url, payload)
+
+def get(id: str, org_id: str):
+    url = f"/v2/sites/{id}?org_id={org_id}"
     return _client.get(url)
 
 def list(**kwargs):
-    def _get_page(query_string):
-        url = "/v1/providers?" + query_string
-        return _client.get(url)
-
-    return PageRequest(_get_page, **kwargs).get()
-
-def delete(id: str):
-    resp = _client.delete(f"/v1/providers/{id}")
-    return _convert_resp(resp)
-
-def create(data: dict):
-    url = "/v1/providers/" + data["type"].lower()
-    return _client.post(url, json=data)
-
-
-def _convert_resp(resp):
-    if resp:
-        resp.read()
-        try:
-            json.loads(resp.text)
-        except:
-            return resp.text
+    url = with_query(f"/v2/sites", **kwargs)
+    return _client.get(url)
+
+def delete(id: str, org_id: str):
+    url = f"/v2/sites/{id}?org_id={org_id}"
+    return _client.delete(url)
+
+def find_by_name(name: str, org_id: str):
+    sites = list(org_id=org_id)
+    for s in sites:
+        if s.get('name') == name:
+            return s
+    
+def set_edge(site_id: str, org_id: str, edge_deployment_id: str):
+    url = f"/v1/sites/{site_id}/edge/{edge_deployment_id}"
+    return _client.put(url, {})
```

### Comparing `hcs-cli-0.1.46/vhcs/service/lcm/template.py` & `hcs-cli-0.1.47/vhcs/service/lcm/template.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 import json
 from typing import Any
-from .._util import hdc_service_client
+from .._util import hdc_service_client, default_crud
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
+_crud = default_crud(_client, "/v1/templates", 'template')
 
-
-def get(id: str, **kwargs: Any):
-    url = with_query(f"/v1/templates/{id}", **kwargs)
-    return _client.get(url)
+get = _crud.get
 
 def list(name: str = None, **kwargs):
     def _get_page(query_string):
         url = "/v1/templates?" + query_string
         return _client.get(url)
 
     ret = PageRequest(_get_page, **kwargs).get()
@@ -47,16 +45,16 @@
 def create(template: dict):
     url = "/v1/templates"
     url += "/" + template["providerType"].lower()
     return _client.post(url=url, json=template)
 
 def wait(
     id: str,
-    expected_status: list,
     timeout_seconds: int,
+    expected_status: list = ["READY"],
     exclude_status: list = ["ERROR"],
     interval_seconds: int = 10,
 ):
     start = int(time.time())
     while True:
         t = get(id)
         if not t:
```

### Comparing `hcs-cli-0.1.46/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.47/vhcs/service/admin/ad.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,25 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
-from vhcs.util.query_util import with_query, PageRequest
-
-_client = hdc_service_client("org-service")
-
-
-def get(id: str, **kwargs):
-    url = with_query(f"/v1/datacenters/{id}", **kwargs)
-    return _client.get(url)
-
-def list(**kwargs):
-    url = with_query(f"/v1/datacenters", **kwargs)
-    return _client.get(url)
-
-def find_by_org(orgId, **kwargs):
-    url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
-    return _client.get(url)
+from .._util import hdc_service_client, default_crud, wait_for_res_status
 
+_client = hdc_service_client("admin")
+_crud = default_crud(_client, "/v2/active-directories", 'ad')
+get = _crud.get
+list = _crud.list
+create = _crud.create
+delete = _crud.delete
```

### Comparing `hcs-cli-0.1.46/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.47/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/service/portal/pool.py` & `hcs-cli-0.1.47/vhcs/service/admin/template.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,32 +9,45 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import logging
-from .._util import hdc_service_client
+from .._util import hdc_service_client, default_crud, wait_for_res_status
 from vhcs.util.query_util import with_query, PageRequest
 
-log = logging.getLogger(__name__)
-_client = hdc_service_client("portal")
+_client = hdc_service_client("admin")
+_crud = default_crud(_client, "/v2/templates", 'template')
+get = _crud.get
+list = _crud.list
+
+def create(payload):
+    return _crud.create(payload, ignore_warnings=True)
+
+def delete(id: str, org_id: str, force: bool = True):
+    return _crud.delete(id, org_id, force=force)
+
+def wait_for_ready(id: str, org_id: str, timeout_seconds: int = 600):
+    name = 'template/' + id
+    fn_get = lambda: get(id, org_id)
+    fn_get_status = lambda t: t['reportedStatus'].get('statusValue')
+    status_map = {
+        'ready': 'READY',
+        'error': 'ERROR',
+        'trasition': ['EXPANDING', 'SHRINKING', 'INIT']
+        # Unexpected:
+        # DELETING
+    }
+    return wait_for_res_status(name, fn_get, fn_get_status, status_map, timeout_seconds)
 
+wait_for_deleted = _crud.wait_for_deleted
 
-def create(payload: dict):
-    url = "/v2/pools"
-    return _client.post(url, payload)
-
-def get(id: str, org_id: str):
-    url = f"/v2/pools/{id}?org_id={org_id}"
-    return _client.get(url)
-
-def list(**kwargs):
+def list_vms(template_id: str, **kwargs):
     def _get_page(query_string):
-        url = "/v2/pools?" + query_string
+        url = f"/v2/templates/{template_id}/vms?" + query_string
         return _client.get(url)
     return PageRequest(_get_page, **kwargs).get()
 
-def delete(id: str, org_id: str):
-    url = f"/v2/pools/{id}?org_id={org_id}"
-    return _client.delete(url)
+def get_vm(template_id: str, vm_id: str, **kwargs):
+    url = with_query(f"/v2/templates/{template_id}/vms/{vm_id}", **kwargs)
+    return _client.get(url)
```

### Comparing `hcs-cli-0.1.46/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.47/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/cidr_util.py` & `hcs-cli-0.1.47/vhcs/support/daas/cidr_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/helper.py` & `hcs-cli-0.1.47/vhcs/support/daas/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     print('Subscription:', subscription_id)
     print('Directory:', directory_id)
     print('ApplicationId:', application_id)
     print('Region:', region)
     if application_id != provider['applicationId']:
         log.warning("Configured application ID for CLI does not match application ID for provider.")
     
-    az.login(provider['applicationId'], provider['applicationSecret'], directory_id)
+    az.login(provider['applicationId'], provider['applicationKey'], directory_id)
     az.set_subscription(subscription_id)
 
 def prepare_plan_file(deployment_id: str, blueprint_id: str, fn_collect_info: Callable):
     suffix = '.blueprint.yml'
 
     if blueprint_id.endswith(suffix):
         blueprint_id = blueprint_id[:-len(suffix)]
@@ -62,35 +62,43 @@
     # Add defaults from shared infra config, if anything missing
     data_util.deep_apply_defaults(input_data, infra.all())
     
     # Enforce key values
     input_data['deploymentId'] = deployment_id
     input_data['vars']['orgId'] = _get_org_id()
     
-    # Collect input from user
-    fn_collect_info(input_data)
+    def create_file(success):
+        # Combine and save
+        blueprint_file = blueprint_id + '.blueprint.yml'
+        blueprint = template.get(blueprint_file)
+        text = "\n".join([
+            yaml.safe_dump(input_data, sort_keys=False),
+            "",
+            "# ----------------------------------",
+            "# Blueprint: " + blueprint_file,
+            "",
+            yaml.safe_dump(blueprint, sort_keys=False)
+        ])
+        with open(file_name, "w") as file:
+            file.write(text)
+
+        if success:
+            print("Plan saved as file: " + file_name)
+            print(f"To view the plan:   'hcs plan graph -f {file_name}'")
+            print(f"To deploy the plan: 'hcs plan deploy -f {file_name}'")
+    success = False
+    try:
+        # Collect input from user
+        fn_collect_info(input_data)
+        success = True
+    except Exception:
+        raise
+    finally:
+        create_file(success)
 
-    # Combine and save
-    blueprint_file = blueprint_id + '.blueprint.yml'
-    blueprint = template.get(blueprint_file)
-    text = "\n".join([
-        yaml.safe_dump(input_data, sort_keys=False),
-        "",
-        "# ----------------------------------",
-        "# Blueprint: " + blueprint_file,
-        "",
-        yaml.safe_dump(blueprint, sort_keys=False)
-    ])
-
-    with open(file_name, "w") as file:
-        file.write(text)
-
-    print("Plan saved as file: " + file_name)
-    print(f"To view the plan:   'hcs plan graph -f {file_name}'")
-    print(f"To deploy the plan: 'hcs plan deploy -f {file_name}'")
 
 def _get_file_name(deployment_id: str) -> str:
     return deployment_id + '.plan.yml'
 
 def _get_org_id():
     from vhcs.common.sglib import auth
     auth_info = auth.details(get_org_details=False)
```

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/infra.py` & `hcs-cli-0.1.47/vhcs/support/daas/infra.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     ret.update(target)
     return ret
 
 _config_template = {
 	"provider": {
 		"id": "",
 		"applicationId": "",
-		"applicationSecret": ""
+		"applicationKey": ""
 	},
 	"network": {
 		"vNetId": "",
 		"tenantCIDRs": []
 	},
 	"desktop": {
 		"markerId": "",
```

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/infra_calc.py` & `hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,29 +8,25 @@
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import logging
-from vhcs.service import admin, auth
-from vhcs.plan.provider.azure import _az_facade as az
-from vhcs.plan import PlanException
 
-log = logging.getLogger(__name__)
+import click
+from vhcs.service.org_service import datacenter
+import vhcs.common.sglib.cli_options as cli
 
-def deploy(data: dict, save_state) -> dict:
-    provider = data['provider']
-    provider_id = provider['id']
-    log.info('Provider: %s', provider_id)
-    providerInstance = admin.provider.get('azure', provider_id)
-    if not providerInstance:
-        raise PlanException('Provider not found: ' + provider_id)
-    providerData = providerInstance['providerDetails']['data']
-    region = providerData['region']
-    return {
-        'location': region
-    }
 
-def destroy(data: dict, prev: dict):
-    return
+@click.command("list")
+@cli.org_id
+def list_datacenters(org: str):
+    """List all datacenters"""
+
+    if org == "" or org == "all":
+        ret = datacenter.list()
+    else:
+        org_id = cli.get_org_id(org)
+        return datacenter.find_by_org(org_id)
+
+    return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/tenant.py.xx` & `hcs-cli-0.1.47/vhcs/plan/provider/hcs/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,69 +9,36 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ulid import ULID
-import vhcs.common.ctxp as ctxp
+from vhcs.plan import actions
+from vhcs.service import admin
 
-def _store() -> ctxp.fstore:
-    return ctxp.profile_store('daas-tenant')
-
-_config_template = {
-    "id": "",
-    "customerName": "",
-    "applicationId": "",
-    "applicationSecret": "",
-    "desktopName": "",
-    "groupName": "",
-    "markerId": "",
-    "orgId": "",
-    "providerInstanceId": "",
-    "streamId": "",
-    "templateType": "",
-    "userEmails": "",
-    "vmSkuName": ""
-}
-
-def _with_default(target : dict, default : dict) -> dict:
-    ret = dict(default)
-    if target:
-        ret.update(target)
-    return ret
-
-def list():
-    return _store().values()
-
-def names():
-    ret = []
-    for v in list():
-        ret.append(v['customerName'])
-    return ret
-
-def ids():
-    return _store().keys()
-
-def get(id: str):
-    return _store().get(id)
-
-def find_by_customer_name(customer_name: str):
-    for doc in list():
-        if doc['customerName'] == customer_name:
-            return doc
-
-def save(id: str, data: dict):
-    return _store().save(id, data)
-
-def delete(id: str):
-    return _store().delete(id)
-
-def create(customer_name: str):
-    data = find_by_customer_name(customer_name)
-    if data:
-        raise ctxp.CtxpException("A tenant with that name already exists.")
-    data = _with_default(data, _config_template)
-    data['id'] = str(ULID())
-    data['customerName'] = customer_name
-    return data
+def deploy(data: dict, state: dict) -> dict:
+    label = data['providerLabel']
+    return admin.provider.create(label, data)
+
+def refresh(data: dict, state: dict) -> dict:
+    org_id = data['orgId']
+    label = data['providerLabel']
+    if state:
+        id = state.get('id')
+        if id:
+            return admin.provider.get(label, id, org_id)
+    
+    # Fall back with smart find by name
+    search = "name $eq " + data['name']
+    providers = admin.provider.list(label, org_id=org_id, search=search)
+    if providers:
+        return providers[0]
+
+def decide(data: dict, state: dict):
+    return actions.skip
+
+def destroy(data: dict, state: dict) -> dict:
+    org_id = data['orgId']
+    label = data['providerLabel']
+    id = state['id']
+    return admin.provider.delete(label, id, org_id)
```

### Comparing `hcs-cli-0.1.46/vhcs/support/daas/tenant_calc.py` & `hcs-cli-0.1.47/vhcs/support/daas/tenant_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from vhcs.service import admin, auth
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.plan import PlanException
 from .cidr_util import find_available_cidr_24
 
 log = logging.getLogger(__name__)
 
-def deploy(data: dict) -> dict:
+def process(data: dict, state: dict) -> dict:
     provider = data['provider']
     provider_id = provider['id']
     log.info('Provider: %s', provider_id)
     providerInstance = admin.provider.get('azure', provider_id)
     if not providerInstance:
         raise PlanException('Provider not found: ' + provider_id)
     providerData = providerInstance['providerDetails']['data']
```

### Comparing `hcs-cli-0.1.46/vhcs/support/plan_util.py` & `hcs-cli-0.1.47/vhcs/support/plan_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/support/profile.py` & `hcs-cli-0.1.47/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/util/check_license.py` & `hcs-cli-0.1.47/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/util/duration.py` & `hcs-cli-0.1.47/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/util/pki_util.py` & `hcs-cli-0.1.47/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.46/vhcs/util/query_util.py` & `hcs-cli-0.1.47/vhcs/util/query_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,10 +56,12 @@
             page = self.fn_get_page(query_string)
             if not page or not page.content:
                 break
             ret += page.content
             if len(ret) > self.limit:
                 ret = ret[:self.limit]
                 break
+            if len(page.content) < self.query['size']:
+                break
             page_index += 1
 
         return ret
```

### Comparing `hcs-cli-0.1.46/vhcs/util/versions.py` & `hcs-cli-0.1.47/vhcs/util/versions.py`

 * *Files identical despite different names*

