# Comparing `tmp/hpc-rocket-0.4.0.tar.gz` & `tmp/hpc-rocket-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc-rocket-0.4.0.tar", last modified: Tue Jan 17 16:40:56 2023, max compression
+gzip compressed data, was "hpc-rocket-0.5.0.tar", last modified: Wed Jul 26 15:27:57 2023, max compression
```

## Comparing `hpc-rocket-0.4.0.tar` & `hpc-rocket-0.5.0.tar`

### file list

```diff
@@ -1,117 +1,106 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.314103 hpc-rocket-0.4.0/
--rw-r--r--   0 marcus     (501) staff       (20)       11 2021-05-28 10:03:43.000000 hpc-rocket-0.4.0/AUTHORS
--rw-r--r--   0 marcus     (501) staff       (20)     1068 2021-04-16 16:44:20.000000 hpc-rocket-0.4.0/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)      751 2023-01-17 16:40:56.314213 hpc-rocket-0.4.0/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     3823 2022-12-13 08:24:18.000000 hpc-rocket-0.4.0/README.md
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.259881 hpc-rocket-0.4.0/docs/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.266386 hpc-rocket-0.4.0/docs/source/
--rw-r--r--   0 marcus     (501) staff       (20)     1999 2022-12-13 08:44:48.000000 hpc-rocket-0.4.0/docs/source/conf.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.268549 hpc-rocket-0.4.0/hpc_rocket.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)      751 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     3264 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       56 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/entry_points.txt
--rw-r--r--   0 marcus     (501) staff       (20)       77 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)       45 2023-01-17 16:40:56.000000 hpc-rocket-0.4.0/hpc_rocket.egg-info/top_level.txt
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.273760 hpc-rocket-0.4.0/hpcrocket/
--rw-r--r--   0 marcus     (501) staff       (20)     2939 2022-08-15 12:47:20.000000 hpc-rocket-0.4.0/hpcrocket/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)      111 2022-05-05 14:04:43.000000 hpc-rocket-0.4.0/hpcrocket/__main__.py
--rw-r--r--   0 marcus     (501) staff       (20)     6341 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/hpcrocket/cli.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.276828 hpc-rocket-0.4.0/hpcrocket/core/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2021-09-24 08:32:35.000000 hpc-rocket-0.4.0/hpcrocket/core/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     1441 2022-08-15 10:57:05.000000 hpc-rocket-0.4.0/hpcrocket/core/application.py
--rw-r--r--   0 marcus     (501) staff       (20)      403 2021-09-24 08:32:35.000000 hpc-rocket-0.4.0/hpcrocket/core/errors.py
--rw-r--r--   0 marcus     (501) staff       (20)      851 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/hpcrocket/core/executor.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.278505 hpc-rocket-0.4.0/hpcrocket/core/filesystem/
--rw-r--r--   0 marcus     (501) staff       (20)      102 2023-01-16 10:13:38.000000 hpc-rocket-0.4.0/hpcrocket/core/filesystem/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     2252 2023-01-16 10:13:38.000000 hpc-rocket-0.4.0/hpcrocket/core/filesystem/_filesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     1157 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/hpcrocket/core/filesystem/glob.py
--rw-r--r--   0 marcus     (501) staff       (20)     4044 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/hpcrocket/core/filesystem/progressive.py
--rw-r--r--   0 marcus     (501) staff       (20)     1560 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/hpcrocket/core/launchoptions.py
--rw-r--r--   0 marcus     (501) staff       (20)     2033 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/hpcrocket/core/slurmbatchjob.py
--rw-r--r--   0 marcus     (501) staff       (20)     1537 2022-05-05 13:46:20.000000 hpc-rocket-0.4.0/hpcrocket/core/slurmcontroller.py
--rw-r--r--   0 marcus     (501) staff       (20)     1686 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/hpcrocket/core/workflowfactory.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.279747 hpc-rocket-0.4.0/hpcrocket/core/workflows/
--rw-r--r--   0 marcus     (501) staff       (20)     2143 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/hpcrocket/core/workflows/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     7326 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/hpcrocket/core/workflows/stages.py
--rw-r--r--   0 marcus     (501) staff       (20)     2241 2022-08-15 12:45:48.000000 hpc-rocket-0.4.0/hpcrocket/core/workflows/workflow.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.281892 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2021-09-27 09:44:06.000000 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)      682 2022-10-26 08:37:21.000000 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/factory.py
--rw-r--r--   0 marcus     (501) staff       (20)      391 2022-06-10 09:45:35.000000 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/localfilesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     6984 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/pyfilesystembased.py
--rw-r--r--   0 marcus     (501) staff       (20)     1571 2023-01-17 10:48:47.000000 hpc-rocket-0.4.0/hpcrocket/pyfilesystem/sshfilesystem.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.284335 hpc-rocket-0.4.0/hpcrocket/ssh/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2021-09-24 08:32:35.000000 hpc-rocket-0.4.0/hpcrocket/ssh/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     3432 2023-01-17 10:48:47.000000 hpc-rocket-0.4.0/hpcrocket/ssh/chmodsshfs.py
--rw-r--r--   0 marcus     (501) staff       (20)      766 2022-01-03 08:51:25.000000 hpc-rocket-0.4.0/hpcrocket/ssh/connectiondata.py
--rw-r--r--   0 marcus     (501) staff       (20)       88 2022-03-28 15:59:34.000000 hpc-rocket-0.4.0/hpcrocket/ssh/errors.py
--rw-r--r--   0 marcus     (501) staff       (20)     4130 2023-01-17 10:48:47.000000 hpc-rocket-0.4.0/hpcrocket/ssh/sshexecutor.py
--rw-r--r--   0 marcus     (501) staff       (20)      253 2022-03-31 13:16:20.000000 hpc-rocket-0.4.0/hpcrocket/typesafety.py
--rw-r--r--   0 marcus     (501) staff       (20)     3701 2023-01-17 10:59:27.000000 hpc-rocket-0.4.0/hpcrocket/ui.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.286101 hpc-rocket-0.4.0/hpcrocket/watcher/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2021-09-24 08:32:35.000000 hpc-rocket-0.4.0/hpcrocket/watcher/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     2468 2022-08-15 12:47:48.000000 hpc-rocket-0.4.0/hpcrocket/watcher/jobwatcher.py
--rw-r--r--   0 marcus     (501) staff       (20)     1761 2022-08-15 12:47:58.000000 hpc-rocket-0.4.0/hpcrocket/watcher/watcherthread.py
--rw-r--r--   0 marcus     (501) staff       (20)      166 2022-06-10 12:20:56.000000 hpc-rocket-0.4.0/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)      872 2023-01-17 16:40:56.314884 hpc-rocket-0.4.0/setup.cfg
--rw-r--r--   0 marcus     (501) staff       (20)       38 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/setup.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.293721 hpc-rocket-0.4.0/test/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.294338 hpc-rocket-0.4.0/test/acceptance/
--rw-r--r--   0 marcus     (501) staff       (20)     1010 2022-06-10 12:53:58.000000 hpc-rocket-0.4.0/test/acceptance/test_launch_acceptance.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.299421 hpc-rocket-0.4.0/test/application/
--rw-r--r--   0 marcus     (501) staff       (20)     1159 2022-08-15 11:35:16.000000 hpc-rocket-0.4.0/test/application/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)      668 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/assertions.py
--rw-r--r--   0 marcus     (501) staff       (20)     1850 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/executor_filesystem_callorder.py
--rw-r--r--   0 marcus     (501) staff       (20)     4456 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/optionbuilders.py
--rw-r--r--   0 marcus     (501) staff       (20)      524 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_cancel_options.py
--rw-r--r--   0 marcus     (501) staff       (20)     1410 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_cancel_watching.py
--rw-r--r--   0 marcus     (501) staff       (20)     3627 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_collect_clean.py
--rw-r--r--   0 marcus     (501) staff       (20)      950 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_finalize_options.py
--rw-r--r--   0 marcus     (501) staff       (20)     8910 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_launch_options.py
--rw-r--r--   0 marcus     (501) staff       (20)     2175 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_status_options.py
--rw-r--r--   0 marcus     (501) staff       (20)     1706 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/application/test_application_watch_options.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.299843 hpc-rocket-0.4.0/test/integration/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/integration/__init__.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.301629 hpc-rocket-0.4.0/test/integration/application/
--rw-r--r--   0 marcus     (501) staff       (20)     1546 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/integration/application/fixtures.py
--rw-r--r--   0 marcus     (501) staff       (20)     7696 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/integration/application/test_application_with_filesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     3057 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/integration/application/test_application_with_paramiko.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.302787 hpc-rocket-0.4.0/test/integration/cli/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/integration/cli/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     4867 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/integration/cli/test_cli_app_integration.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.304381 hpc-rocket-0.4.0/test/integration/paramiko/
--rw-r--r--   0 marcus     (501) staff       (20)     1452 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/integration/paramiko/test_remotecommand.py
--rw-r--r--   0 marcus     (501) staff       (20)     2561 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/integration/paramiko/test_slurmrunner_with_sshexecutor.py
--rw-r--r--   0 marcus     (501) staff       (20)     5391 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/integration/paramiko/test_sshexecutor.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.307205 hpc-rocket-0.4.0/test/integration/pyfilesystem/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/integration/pyfilesystem/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     1506 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/integration/pyfilesystem/sshfilesystem_assertions.py
--rw-r--r--   0 marcus     (501) staff       (20)     3501 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/integration/pyfilesystem/test_pyfilesystembased.py
--rw-r--r--   0 marcus     (501) staff       (20)     1774 2022-06-15 15:22:11.000000 hpc-rocket-0.4.0/test/integration/pyfilesystem/test_sshfilesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     4470 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/test_cli.py
--rw-r--r--   0 marcus     (501) staff       (20)      651 2022-05-02 14:01:41.000000 hpc-rocket-0.4.0/test/test_executor.py
--rw-r--r--   0 marcus     (501) staff       (20)    16942 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/test_filesystem_abc.py
--rw-r--r--   0 marcus     (501) staff       (20)     3858 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_jobwatcher.py
--rw-r--r--   0 marcus     (501) staff       (20)     5068 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/test_progressive_fileoperations.py
--rw-r--r--   0 marcus     (501) staff       (20)     1903 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_slurmbatchjob.py
--rw-r--r--   0 marcus     (501) staff       (20)     3250 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_slurmcontroller.py
--rw-r--r--   0 marcus     (501) staff       (20)     1939 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_slurmjob.py
--rw-r--r--   0 marcus     (501) staff       (20)      552 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_typesafety.py
--rw-r--r--   0 marcus     (501) staff       (20)     5605 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/test_watcherthread.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.309817 hpc-rocket-0.4.0/test/testdoubles/
--rw-r--r--   0 marcus     (501) staff       (20)        0 2021-09-27 09:44:06.000000 hpc-rocket-0.4.0/test/testdoubles/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     5394 2022-05-02 13:52:12.000000 hpc-rocket-0.4.0/test/testdoubles/executor.py
--rw-r--r--   0 marcus     (501) staff       (20)    11705 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/testdoubles/filesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     1547 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/testdoubles/paramiko_sshclient_mockutil.py
--rw-r--r--   0 marcus     (501) staff       (20)      658 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/testdoubles/pyfilesystem.py
--rw-r--r--   0 marcus     (501) staff       (20)     6615 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/testdoubles/sshclient.py
--rw-r--r--   0 marcus     (501) staff       (20)     1871 2022-06-15 15:23:44.000000 hpc-rocket-0.4.0/test/testdoubles/test_memoryfilesystem.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-01-17 16:40:56.313549 hpc-rocket-0.4.0/test/workflows/
--rw-r--r--   0 marcus     (501) staff       (20)      732 2022-05-02 14:00:20.000000 hpc-rocket-0.4.0/test/workflows/test_cancelstage.py
--rw-r--r--   0 marcus     (501) staff       (20)     2970 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/workflows/test_finalizestage.py
--rw-r--r--   0 marcus     (501) staff       (20)     2393 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/workflows/test_launchstage.py
--rw-r--r--   0 marcus     (501) staff       (20)     2695 2023-01-16 10:13:39.000000 hpc-rocket-0.4.0/test/workflows/test_preparestage.py
--rw-r--r--   0 marcus     (501) staff       (20)      868 2022-08-16 09:19:11.000000 hpc-rocket-0.4.0/test/workflows/test_statusstage.py
--rw-r--r--   0 marcus     (501) staff       (20)     4997 2023-01-17 16:37:45.000000 hpc-rocket-0.4.0/test/workflows/test_watchstage.py
--rw-r--r--   0 marcus     (501) staff       (20)     3568 2022-05-31 14:42:02.000000 hpc-rocket-0.4.0/test/workflows/test_workflow.py
+-rw-r--r--   0        0        0       11 2022-04-28 07:48:09.807441 hpc-rocket-0.5.0/AUTHORS
+-rw-r--r--   0        0        0     1068 2022-04-28 07:48:09.807641 hpc-rocket-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3823 2022-12-21 09:27:31.477185 hpc-rocket-0.5.0/README.md
+-rw-r--r--   0        0        0     2569 2023-07-26 14:43:14.135596 hpc-rocket-0.5.0/hpcrocket/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-26 12:14:52.915595 hpc-rocket-0.5.0/hpcrocket/__main__.py
+-rw-r--r--   0        0        0      485 2023-07-26 14:43:05.119751 hpc-rocket-0.5.0/hpcrocket/cli/__init__.py
+-rw-r--r--   0        0        0     4614 2023-07-26 14:42:17.259236 hpc-rocket-0.5.0/hpcrocket/cli/_builders.py
+-rw-r--r--   0        0        0     2381 2023-07-26 14:27:37.031833 hpc-rocket-0.5.0/hpcrocket/cli/_parsers.py
+-rw-r--r--   0        0        0      604 2023-07-26 14:33:43.950390 hpc-rocket-0.5.0/hpcrocket/cli/_yaml.py
+-rw-r--r--   0        0        0        0 2022-04-28 07:48:09.816720 hpc-rocket-0.5.0/hpcrocket/core/__init__.py
+-rw-r--r--   0        0        0     1441 2022-12-21 12:27:51.880734 hpc-rocket-0.5.0/hpcrocket/core/application.py
+-rw-r--r--   0        0        0      403 2022-04-28 07:48:09.816996 hpc-rocket-0.5.0/hpcrocket/core/errors.py
+-rw-r--r--   0        0        0      851 2022-11-03 08:32:33.380541 hpc-rocket-0.5.0/hpcrocket/core/executor.py
+-rw-r--r--   0        0        0      102 2023-01-12 17:22:27.577869 hpc-rocket-0.5.0/hpcrocket/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     2252 2022-05-05 17:15:01.345821 hpc-rocket-0.5.0/hpcrocket/core/filesystem/_filesystem.py
+-rw-r--r--   0        0        0     1157 2023-01-13 16:41:37.297944 hpc-rocket-0.5.0/hpcrocket/core/filesystem/glob.py
+-rw-r--r--   0        0        0     4044 2023-01-13 16:41:36.849616 hpc-rocket-0.5.0/hpcrocket/core/filesystem/progressive.py
+-rw-r--r--   0        0        0     1592 2023-07-26 14:45:05.802103 hpc-rocket-0.5.0/hpcrocket/core/launchoptions.py
+-rw-r--r--   0        0        0     2033 2022-11-03 08:32:33.397750 hpc-rocket-0.5.0/hpcrocket/core/slurmbatchjob.py
+-rw-r--r--   0        0        0     1537 2022-05-03 17:10:58.195549 hpc-rocket-0.5.0/hpcrocket/core/slurmcontroller.py
+-rw-r--r--   0        0        0     1686 2023-07-26 09:38:38.799203 hpc-rocket-0.5.0/hpcrocket/core/workflowfactory.py
+-rw-r--r--   0        0        0     2331 2023-07-26 12:39:29.496811 hpc-rocket-0.5.0/hpcrocket/core/workflows/__init__.py
+-rw-r--r--   0        0        0     7897 2023-07-26 15:20:45.189526 hpc-rocket-0.5.0/hpcrocket/core/workflows/stages.py
+-rw-r--r--   0        0        0     2241 2022-11-03 08:32:33.423993 hpc-rocket-0.5.0/hpcrocket/core/workflows/workflow.py
+-rw-r--r--   0        0        0        0 2022-04-28 07:48:09.817999 hpc-rocket-0.5.0/hpcrocket/pyfilesystem/__init__.py
+-rw-r--r--   0        0        0      682 2022-11-03 08:32:33.430827 hpc-rocket-0.5.0/hpcrocket/pyfilesystem/factory.py
+-rw-r--r--   0        0        0      391 2022-11-03 08:32:33.436719 hpc-rocket-0.5.0/hpcrocket/pyfilesystem/localfilesystem.py
+-rw-r--r--   0        0        0     6984 2023-03-31 11:38:22.978881 hpc-rocket-0.5.0/hpcrocket/pyfilesystem/pyfilesystembased.py
+-rw-r--r--   0        0        0     1571 2022-11-03 08:32:33.449423 hpc-rocket-0.5.0/hpcrocket/pyfilesystem/sshfilesystem.py
+-rw-r--r--   0        0        0        0 2022-04-28 07:48:09.818487 hpc-rocket-0.5.0/hpcrocket/ssh/__init__.py
+-rw-r--r--   0        0        0     3432 2022-11-03 08:32:33.459483 hpc-rocket-0.5.0/hpcrocket/ssh/chmodsshfs.py
+-rw-r--r--   0        0        0      766 2022-04-28 07:48:09.818708 hpc-rocket-0.5.0/hpcrocket/ssh/connectiondata.py
+-rw-r--r--   0        0        0       88 2022-04-28 07:48:09.818816 hpc-rocket-0.5.0/hpcrocket/ssh/errors.py
+-rw-r--r--   0        0        0     4130 2022-11-03 08:32:33.466132 hpc-rocket-0.5.0/hpcrocket/ssh/sshexecutor.py
+-rw-r--r--   0        0        0      253 2022-04-28 07:48:09.819052 hpc-rocket-0.5.0/hpcrocket/typesafety.py
+-rw-r--r--   0        0        0     3701 2022-11-03 08:32:33.471443 hpc-rocket-0.5.0/hpcrocket/ui.py
+-rw-r--r--   0        0        0        0 2022-04-28 07:48:09.819222 hpc-rocket-0.5.0/hpcrocket/watcher/__init__.py
+-rw-r--r--   0        0        0     2468 2022-11-03 08:32:33.478873 hpc-rocket-0.5.0/hpcrocket/watcher/jobwatcher.py
+-rw-r--r--   0        0        0     1761 2022-11-03 08:32:33.484376 hpc-rocket-0.5.0/hpcrocket/watcher/watcherthread.py
+-rw-r--r--   0        0        0     1368 2023-07-26 15:21:46.774366 hpc-rocket-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      192 2022-11-03 08:32:33.516239 hpc-rocket-0.5.0/test/__init__.py
+-rw-r--r--   0        0        0     1010 2022-11-03 08:32:33.525709 hpc-rocket-0.5.0/test/acceptance/test_launch_acceptance.py
+-rw-r--r--   0        0        0     1159 2022-11-03 08:32:33.531965 hpc-rocket-0.5.0/test/application/__init__.py
+-rw-r--r--   0        0        0      668 2023-07-26 09:38:38.800552 hpc-rocket-0.5.0/test/application/assertions.py
+-rw-r--r--   0        0        0     1850 2023-07-26 09:38:38.801124 hpc-rocket-0.5.0/test/application/executor_filesystem_callorder.py
+-rw-r--r--   0        0        0     4456 2023-07-26 09:38:38.801260 hpc-rocket-0.5.0/test/application/optionbuilders.py
+-rw-r--r--   0        0        0      524 2023-07-26 09:38:38.801418 hpc-rocket-0.5.0/test/application/test_application_cancel_options.py
+-rw-r--r--   0        0        0     1410 2023-07-26 09:38:38.801555 hpc-rocket-0.5.0/test/application/test_application_cancel_watching.py
+-rw-r--r--   0        0        0     3627 2023-07-26 09:38:38.801658 hpc-rocket-0.5.0/test/application/test_application_collect_clean.py
+-rw-r--r--   0        0        0      950 2023-07-26 09:38:38.801773 hpc-rocket-0.5.0/test/application/test_application_finalize_options.py
+-rw-r--r--   0        0        0     9312 2023-07-26 12:39:24.305772 hpc-rocket-0.5.0/test/application/test_application_launch_options.py
+-rw-r--r--   0        0        0     2175 2023-07-26 09:38:38.802388 hpc-rocket-0.5.0/test/application/test_application_status_options.py
+-rw-r--r--   0        0        0     1706 2023-07-26 09:38:38.802518 hpc-rocket-0.5.0/test/application/test_application_watch_options.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:04:55.125595 hpc-rocket-0.5.0/test/integration/__init__.py
+-rw-r--r--   0        0        0     1546 2022-11-03 08:32:33.570145 hpc-rocket-0.5.0/test/integration/application/fixtures.py
+-rw-r--r--   0        0        0     7696 2023-07-26 09:38:38.802826 hpc-rocket-0.5.0/test/integration/application/test_application_with_filesystem.py
+-rw-r--r--   0        0        0     3057 2023-07-26 09:38:38.802997 hpc-rocket-0.5.0/test/integration/application/test_application_with_paramiko.py
+-rw-r--r--   0        0        0        0 2023-01-12 15:58:41.782420 hpc-rocket-0.5.0/test/integration/cli/__init__.py
+-rw-r--r--   0        0        0     4699 2023-07-26 12:16:00.035410 hpc-rocket-0.5.0/test/integration/cli/test_cli_app_integration.py
+-rw-r--r--   0        0        0     1452 2022-11-03 08:32:33.596170 hpc-rocket-0.5.0/test/integration/paramiko/test_remotecommand.py
+-rw-r--r--   0        0        0     2561 2023-07-26 09:38:38.803171 hpc-rocket-0.5.0/test/integration/paramiko/test_slurmrunner_with_sshexecutor.py
+-rw-r--r--   0        0        0     5391 2022-11-03 08:32:33.606602 hpc-rocket-0.5.0/test/integration/paramiko/test_sshexecutor.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:05:36.794630 hpc-rocket-0.5.0/test/integration/pyfilesystem/__init__.py
+-rw-r--r--   0        0        0     1506 2022-11-03 08:32:33.613530 hpc-rocket-0.5.0/test/integration/pyfilesystem/sshfilesystem_assertions.py
+-rw-r--r--   0        0        0     3501 2022-12-21 10:17:25.237957 hpc-rocket-0.5.0/test/integration/pyfilesystem/test_pyfilesystembased.py
+-rw-r--r--   0        0        0     1771 2023-07-26 09:38:38.803443 hpc-rocket-0.5.0/test/integration/pyfilesystem/test_sshfilesystem.py
+-rw-r--r--   0        0        0     1510 2022-05-05 17:15:01.347863 hpc-rocket-0.5.0/test/slurm_assertions.py
+-rw-r--r--   0        0        0      335 2022-04-28 07:48:09.822233 hpc-rocket-0.5.0/test/slurmoutput/sacct_canceled.txt
+-rw-r--r--   0        0        0      390 2022-04-28 07:48:09.822300 hpc-rocket-0.5.0/test/slurmoutput/sacct_completed.txt
+-rw-r--r--   0        0        0      279 2022-04-28 07:48:09.822365 hpc-rocket-0.5.0/test/slurmoutput/sacct_completed_failed.txt
+-rw-r--r--   0        0        0      279 2022-04-28 07:48:09.822423 hpc-rocket-0.5.0/test/slurmoutput/sacct_running.txt
+-rw-r--r--   0        0        0       27 2022-04-28 07:48:09.822482 hpc-rocket-0.5.0/test/slurmoutput/sbatch_submit.txt
+-rw-r--r--   0        0        0     1974 2022-05-03 17:10:58.197875 hpc-rocket-0.5.0/test/slurmoutput.py
+-rw-r--r--   0        0        0     5369 2023-07-26 14:05:42.869753 hpc-rocket-0.5.0/test/test_cli.py
+-rw-r--r--   0        0        0      651 2022-05-03 17:10:58.198176 hpc-rocket-0.5.0/test/test_executor.py
+-rw-r--r--   0        0        0    16972 2023-07-26 14:45:06.016434 hpc-rocket-0.5.0/test/test_filesystem_abc.py
+-rw-r--r--   0        0        0     3858 2022-11-03 08:32:33.640071 hpc-rocket-0.5.0/test/test_jobwatcher.py
+-rw-r--r--   0        0        0     5068 2023-01-12 17:23:32.193463 hpc-rocket-0.5.0/test/test_progressive_fileoperations.py
+-rw-r--r--   0        0        0     1903 2022-11-03 08:32:33.649575 hpc-rocket-0.5.0/test/test_slurmbatchjob.py
+-rw-r--r--   0        0        0     3250 2022-11-03 08:32:33.655109 hpc-rocket-0.5.0/test/test_slurmcontroller.py
+-rw-r--r--   0        0        0     1939 2022-11-03 08:32:33.660058 hpc-rocket-0.5.0/test/test_slurmjob.py
+-rw-r--r--   0        0        0      552 2022-11-03 08:32:33.664839 hpc-rocket-0.5.0/test/test_typesafety.py
+-rw-r--r--   0        0        0     5605 2022-11-03 08:32:33.670701 hpc-rocket-0.5.0/test/test_watcherthread.py
+-rw-r--r--   0        0        0      818 2022-11-03 08:32:33.677599 hpc-rocket-0.5.0/test/testconfig/config.yml
+-rw-r--r--   0        0        0        9 2022-05-05 17:15:01.348353 hpc-rocket-0.5.0/test/testconfig/dir/hello.txt
+-rw-r--r--   0        0        0       10 2023-01-12 15:06:09.593716 hpc-rocket-0.5.0/test/testconfig/dir/subdir/next.txt
+-rw-r--r--   0        0        0        8 2022-05-05 17:15:01.348530 hpc-rocket-0.5.0/test/testconfig/dir/test.txt
+-rw-r--r--   0        0        0      509 2023-01-12 15:07:11.154065 hpc-rocket-0.5.0/test/testconfig/integration_launch_config_fail_allowed.yml
+-rw-r--r--   0        0        0      280 2022-11-03 08:32:33.687289 hpc-rocket-0.5.0/test/testconfig/local_slurm.job
+-rw-r--r--   0        0        0        0 2022-04-28 07:48:09.823444 hpc-rocket-0.5.0/test/testdoubles/__init__.py
+-rw-r--r--   0        0        0     5394 2022-05-03 17:10:58.198488 hpc-rocket-0.5.0/test/testdoubles/executor.py
+-rw-r--r--   0        0        0    11705 2022-12-21 17:04:41.553605 hpc-rocket-0.5.0/test/testdoubles/filesystem.py
+-rw-r--r--   0        0        0     1547 2022-11-03 08:32:33.696424 hpc-rocket-0.5.0/test/testdoubles/paramiko_sshclient_mockutil.py
+-rw-r--r--   0        0        0      658 2022-11-03 08:32:33.700322 hpc-rocket-0.5.0/test/testdoubles/pyfilesystem.py
+-rw-r--r--   0        0        0     6615 2022-11-03 08:32:33.704588 hpc-rocket-0.5.0/test/testdoubles/sshclient.py
+-rw-r--r--   0        0        0     1871 2022-11-03 08:32:33.708746 hpc-rocket-0.5.0/test/testdoubles/test_memoryfilesystem.py
+-rw-r--r--   0        0        0      969 2022-11-03 08:32:33.712475 hpc-rocket-0.5.0/test/ui_testdoubles.py
+-rw-r--r--   0        0        0      732 2022-05-03 17:10:58.198781 hpc-rocket-0.5.0/test/workflows/test_cancelstage.py
+-rw-r--r--   0        0        0     2970 2023-01-12 17:23:32.193419 hpc-rocket-0.5.0/test/workflows/test_finalizestage.py
+-rw-r--r--   0        0        0      885 2023-07-26 12:21:58.500160 hpc-rocket-0.5.0/test/workflows/test_jobloggingstage.py
+-rw-r--r--   0        0        0     2393 2023-07-26 09:38:38.804223 hpc-rocket-0.5.0/test/workflows/test_launchstage.py
+-rw-r--r--   0        0        0     2695 2023-01-12 17:23:32.193039 hpc-rocket-0.5.0/test/workflows/test_preparestage.py
+-rw-r--r--   0        0        0      868 2022-11-03 08:32:33.727806 hpc-rocket-0.5.0/test/workflows/test_statusstage.py
+-rw-r--r--   0        0        0     5004 2023-07-26 12:01:52.379720 hpc-rocket-0.5.0/test/workflows/test_watchstage.py
+-rw-r--r--   0        0        0     3568 2022-11-03 08:32:33.732697 hpc-rocket-0.5.0/test/workflows/test_workflow.py
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 hpc-rocket-0.5.0/PKG-INFO
```

### Comparing `hpc-rocket-0.4.0/LICENSE` & `hpc-rocket-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/README.md` & `hpc-rocket-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/__init__.py` & `hpc-rocket-0.5.0/hpcrocket/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import signal
 import sys
 from typing import Any, List
-from hpcrocket.cli import parse_cli_args
+
+from hpcrocket.cli import ParseError, parse_cli_args
 from hpcrocket.core.application import Application
 from hpcrocket.core.executor import CommandExecutor
 from hpcrocket.core.filesystem import Filesystem, FilesystemFactory
 from hpcrocket.core.launchoptions import Options
 from hpcrocket.pyfilesystem.factory import PyFilesystemFactory
 from hpcrocket.pyfilesystem.localfilesystem import localfilesystem
 from hpcrocket.ssh.sshexecutor import SSHExecutor
@@ -61,34 +62,21 @@
     options: Options, service_registry: ServiceRegistry, ui: UI
 ) -> Application:
     executor = service_registry.get_executor(options)
     filesystem_factory = service_registry.get_filesystem_factory(options)
     return Application(executor, filesystem_factory, ui)
 
 
-class RuntimeContainer:
-    """
-    A container to run and cancel the HPC Rocket application. Created to decouple running/canceling from sys.exit commands
-    """
-
-    def __init__(
-        self, args: List[str], service_registry: ServiceRegistry, ui: UI
-    ) -> None:
-        self.options = parse_cli_args(args[1:], service_registry.local_filesystem())
-        self.app = create_application(self.options, service_registry, ui)
-
-    def run(self) -> int:
-        return self.app.run(self.options)
-
-    def cancel(self) -> int:
-        return self.app.cancel()
-
-
-def main(args: List[str], service_registry: ServiceRegistry) -> None:
+def main(args: List[str], service_registry: ServiceRegistry) -> int:
     with RichUI() as ui:
-        runtime = RuntimeContainer(args, service_registry, ui)
+        options = parse_cli_args(args[1:], service_registry.local_filesystem())
+        if isinstance(options, ParseError):
+            ui.error(str(options))
+            sys.exit(1)
+
+        app = create_application(options, service_registry, ui)
 
         def on_cancel(*args: Any, **kwargs: Any) -> None:
-            sys.exit(runtime.cancel())
+            sys.exit(app.cancel())
 
         signal.signal(signal.SIGINT, on_cancel)
-        sys.exit(runtime.run())
+        return app.run(options)
```

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/application.py` & `hpc-rocket-0.5.0/hpcrocket/core/application.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/executor.py` & `hpc-rocket-0.5.0/hpcrocket/core/executor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/filesystem/_filesystem.py` & `hpc-rocket-0.5.0/hpcrocket/core/filesystem/_filesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/filesystem/glob.py` & `hpc-rocket-0.5.0/hpcrocket/core/filesystem/glob.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/filesystem/progressive.py` & `hpc-rocket-0.5.0/hpcrocket/core/filesystem/progressive.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/launchoptions.py` & `hpc-rocket-0.5.0/hpcrocket/core/launchoptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from enum import Enum, auto
 from typing import List, Union
 
 from hpcrocket.core.filesystem.progressive import CopyInstruction
 from hpcrocket.ssh.connectiondata import ConnectionData
 
 
-Options = Union["LaunchOptions", "ImmediateCommandOptions", "WatchOptions", "FinalizeOptions"]
+Options = Union[
+    "LaunchOptions", "ImmediateCommandOptions", "WatchOptions", "FinalizeOptions"
+]
 JobBasedOptions = Union["ImmediateCommandOptions", "WatchOptions"]
 
 
 @dataclass
 class ImmediateCommandOptions:
     class Action(Enum):
         status = auto()
@@ -29,14 +31,15 @@
     proxyjumps: List[ConnectionData] = field(default_factory=lambda: [])
     copy_files: List[CopyInstruction] = field(default_factory=lambda: [])
     clean_files: List[str] = field(default_factory=lambda: [])
     collect_files: List[CopyInstruction] = field(default_factory=lambda: [])
     poll_interval: int = 5
     watch: bool = False
     continue_if_job_fails: bool = False
+    job_id_file: str = ""
 
 
 @dataclass
 class WatchOptions:
     jobid: str
     connection: ConnectionData
     proxyjumps: List[ConnectionData] = field(default_factory=lambda: [])
```

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/slurmbatchjob.py` & `hpc-rocket-0.5.0/hpcrocket/core/slurmbatchjob.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/slurmcontroller.py` & `hpc-rocket-0.5.0/hpcrocket/core/slurmcontroller.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/workflowfactory.py` & `hpc-rocket-0.5.0/hpcrocket/core/workflowfactory.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/workflows/__init__.py` & `hpc-rocket-0.5.0/hpcrocket/core/workflows/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+from pathlib import Path
 from typing import List
 
 from hpcrocket.core.filesystem import FilesystemFactory
-from hpcrocket.core.launchoptions import FinalizeOptions, ImmediateCommandOptions, LaunchOptions, WatchOptions
+from hpcrocket.core.launchoptions import (
+    FinalizeOptions,
+    ImmediateCommandOptions,
+    LaunchOptions,
+    WatchOptions,
+)
 from hpcrocket.core.slurmbatchjob import SlurmBatchJob
 from hpcrocket.core.slurmcontroller import SlurmController
 from hpcrocket.core.workflows.workflow import Stage, Workflow
 from hpcrocket.core.workflows.stages import (
     CancelStage,
     FinalizeStage,
+    JobLoggingStage,
     PrepareStage,
     LaunchStage,
     StatusStage,
     WatchStage,
 )
 from hpcrocket.ui import UI
 
@@ -23,14 +30,17 @@
 ) -> Workflow:
     launch_stage = LaunchStage(controller, options.sbatch)
     stages: List[Stage] = [
         PrepareStage(filesystem_factory, options.copy_files),
         launch_stage,
     ]
 
+    if options.job_id_file:
+        stages.append(JobLoggingStage(launch_stage, Path(options.job_id_file)))
+
     if options.watch:
         stages.append(
             WatchStage(
                 launch_stage, options.poll_interval, options.continue_if_job_fails
             )
         )
         stages.append(
@@ -38,19 +48,23 @@
                 filesystem_factory, options.collect_files, options.clean_files
             )
         )
 
     return Workflow(stages)
 
 
-def statusworkflow(controller: SlurmController, options: ImmediateCommandOptions) -> Workflow:
+def statusworkflow(
+    controller: SlurmController, options: ImmediateCommandOptions
+) -> Workflow:
     return Workflow([StatusStage(controller, options.jobid)])
 
 
-def cancelworkflow(controller: SlurmController, options: ImmediateCommandOptions) -> Workflow:
+def cancelworkflow(
+    controller: SlurmController, options: ImmediateCommandOptions
+) -> Workflow:
     return Workflow([CancelStage(controller, options.jobid)])
 
 
 def watchworkflow(controller: SlurmController, options: WatchOptions) -> Workflow:
     class SimpleBatchJobProvider:
         def get_batch_job(self) -> SlurmBatchJob:
             return SlurmBatchJob(controller, options.jobid)
```

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/workflows/stages.py` & `hpc-rocket-0.5.0/hpcrocket/core/workflows/stages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from pathlib import Path
 from typing import List, Optional, Tuple, cast
 
+from hpcrocket.core.errors import get_error_message
+from hpcrocket.core.filesystem import FilesystemFactory
 from hpcrocket.core.filesystem.progressive import (
     CopyInstruction,
-    progressive_copy,
     progressive_clean,
+    progressive_copy,
 )
-from hpcrocket.core.errors import get_error_message
-from hpcrocket.core.filesystem import FilesystemFactory
 from hpcrocket.core.slurmbatchjob import SlurmBatchJob, SlurmJobStatus
 from hpcrocket.core.slurmcontroller import SlurmController
 from hpcrocket.typesafety import get_or_raise
 from hpcrocket.ui import UI
 from hpcrocket.watcher.jobwatcher import (
     JobWatcher,
     NotWatchingError,
@@ -19,14 +20,34 @@
 
 try:
     from typing import Protocol
 except ImportError:  # pragma: no cover
     from typing_extensions import Protocol  # type: ignore
 
 
+class BatchJobProvider(Protocol):
+    def get_batch_job(self) -> SlurmBatchJob:
+        """
+        Provides the watch stage with a batch job to watch
+
+        Returns:
+            SlurmBatchJob
+        """
+        ...
+
+    def cancel(self, ui: UI) -> None:
+        """
+        Informs the BatchJobProvider that the WatchStage was canceled
+
+        Args:
+            ui (UI): The UI instance WatchStage was called with
+        """
+        ...
+
+
 class NoJobLaunchedError(Exception):
     pass
 
 
 def _log_errors(errors: List[Exception], ui: UI) -> None:
     for error in errors:
         ui.error(get_error_message(error))
@@ -62,38 +83,43 @@
     def _no_job_launched(self) -> NoJobLaunchedError:
         return NoJobLaunchedError("Canceled before a job was started")
 
     def get_batch_job(self) -> SlurmBatchJob:
         return cast(SlurmBatchJob, self._batch_job)
 
 
+class JobLoggingStage:
+    """
+    Logs the Slurm Job ID into a file
+    """
+
+    def __init__(
+        self, batch_job_provider: BatchJobProvider, log_file_path: Path
+    ) -> None:
+        self._provider = batch_job_provider
+        self._log_file = log_file_path
+
+    def allowed_to_fail(self) -> bool:
+        return False
+
+    def __call__(self, ui: UI) -> bool:
+        jobid = self._provider.get_batch_job().jobid
+        self._log_file.write_text(jobid)
+        ui.success(f"Wrote job ID {jobid} to file {self._log_file}")
+        return True
+
+    def cancel(self, ui: UI) -> None:
+        pass
+
+
 class WatchStage:
     """
     Watches a batch job until it completes
     """
 
-    class BatchJobProvider(Protocol):
-        def get_batch_job(self) -> SlurmBatchJob:
-            """
-            Provides the watch stage with a batch job to watch
-
-            Returns:
-                SlurmBatchJob
-            """
-            ...
-
-        def cancel(self, ui: UI) -> None:
-            """
-            Informs the BatchJobProvider that the WatchStage was canceled
-
-            Args:
-                ui (UI): The UI instance WatchStage was called with
-            """
-            ...
-
     def __init__(
         self,
         batch_job_provider: BatchJobProvider,
         poll_interval: int,
         allowed_to_fail: bool = False,
     ) -> None:
         self._poll_interval = poll_interval
```

### Comparing `hpc-rocket-0.4.0/hpcrocket/core/workflows/workflow.py` & `hpc-rocket-0.5.0/hpcrocket/core/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/pyfilesystem/factory.py` & `hpc-rocket-0.5.0/hpcrocket/pyfilesystem/factory.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/pyfilesystem/pyfilesystembased.py` & `hpc-rocket-0.5.0/hpcrocket/pyfilesystem/pyfilesystembased.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/pyfilesystem/sshfilesystem.py` & `hpc-rocket-0.5.0/hpcrocket/pyfilesystem/sshfilesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/ssh/chmodsshfs.py` & `hpc-rocket-0.5.0/hpcrocket/ssh/chmodsshfs.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/ssh/connectiondata.py` & `hpc-rocket-0.5.0/hpcrocket/ssh/connectiondata.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/ssh/sshexecutor.py` & `hpc-rocket-0.5.0/hpcrocket/ssh/sshexecutor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/ui.py` & `hpc-rocket-0.5.0/hpcrocket/ui.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/watcher/jobwatcher.py` & `hpc-rocket-0.5.0/hpcrocket/watcher/jobwatcher.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/hpcrocket/watcher/watcherthread.py` & `hpc-rocket-0.5.0/hpcrocket/watcher/watcherthread.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/acceptance/test_launch_acceptance.py` & `hpc-rocket-0.5.0/test/acceptance/test_launch_acceptance.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/__init__.py` & `hpc-rocket-0.5.0/test/application/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/assertions.py` & `hpc-rocket-0.5.0/test/application/assertions.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/executor_filesystem_callorder.py` & `hpc-rocket-0.5.0/test/application/executor_filesystem_callorder.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/optionbuilders.py` & `hpc-rocket-0.5.0/test/application/optionbuilders.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_cancel_options.py` & `hpc-rocket-0.5.0/test/application/test_application_cancel_options.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_cancel_watching.py` & `hpc-rocket-0.5.0/test/application/test_application_cancel_watching.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_collect_clean.py` & `hpc-rocket-0.5.0/test/application/test_application_collect_clean.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_finalize_options.py` & `hpc-rocket-0.5.0/test/application/test_application_finalize_options.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_launch_options.py` & `hpc-rocket-0.5.0/test/application/test_application_launch_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from typing import List, Tuple
 import unittest
+from pathlib import Path
 from test.application import make_application
 from test.application.assertions import (
     assert_does_not_exist_locally,
     assert_does_not_exist_on_remote,
     assert_exists_locally,
     assert_exists_on_remote,
 )
@@ -21,30 +21,31 @@
     REMOTE_DIR,
     REMOTE_FILE,
     launch_options,
     launch_options_copy_collect_clean,
     launch_options_with_copy,
     main_connection,
 )
-from test.slurmoutput import completed_slurm_job
+from test.slurmoutput import DEFAULT_JOB_ID, completed_slurm_job
 from test.testdoubles.executor import (
-    failed_slurm_job_command_stub,
     LoggingCommandExecutorSpy,
     SlurmJobExecutorSpy,
+    failed_slurm_job_command_stub,
     successful_slurm_job_command_stub,
 )
 from test.testdoubles.filesystem import (
     MemoryFilesystemFactoryStub,
     MemoryFilesystemFake,
 )
+from typing import List, Tuple
 from unittest.mock import Mock
 
 from hpcrocket.core.application import Application
-from hpcrocket.core.filesystem.progressive import CopyInstruction
 from hpcrocket.core.executor import RunningCommand
+from hpcrocket.core.filesystem.progressive import CopyInstruction
 from hpcrocket.ssh.errors import SSHError
 
 
 class ConnectionFailingCommandExecutor(LoggingCommandExecutorSpy):
     def connect(self) -> None:
         raise SSHError(main_connection().hostname)
 
@@ -67,19 +68,25 @@
     verifier = CallOrderVerification(expected_calls)
     factory = VerifierReturningFilesystemFactory(verifier)
     sut = Application(verifier, factory, Mock())
     return sut, verifier
 
 
 class Application_With_Launch_Options(unittest.TestCase):
+
+    LOG_FILE = "test.log"
+
     def setUp(self) -> None:
         self.executor = SlurmJobExecutorSpy()
         self.ui_spy = Mock()
         self.sut = make_application(self.executor, ui=self.ui_spy)
 
+    def tearDown(self) -> None:
+        Path(self.LOG_FILE).unlink(missing_ok=True)
+
     def test__when_running__it_runs_sbatch_with_executor(self) -> None:
         self.sut.run(launch_options())
 
         actual_sbatch = str(self.executor.command_log[0])
         assert actual_sbatch == f"sbatch {launch_options().sbatch}"
 
     def test__when_sbatch_job_succeeds__should_return_exit_code_zero(self) -> None:
@@ -107,14 +114,22 @@
         self.sut = make_application(executor, ui=self.ui_spy)
 
         actual = self.sut.run(launch_options(watch=True))
 
         self.assert_error_logged(f"SSHError: {main_connection().hostname}")
         self.assert_exited_without_running_commands(actual)
 
+    def test__when_adding_log_job_id__stores_job_id_in_logfile(self) -> None:
+        options = launch_options()
+        options.job_id_file = self.LOG_FILE
+
+        self.sut.run(options)
+
+        Path(self.LOG_FILE).read_text() == DEFAULT_JOB_ID
+
     def assert_error_logged(self, expected_message: str) -> None:
         self.ui_spy.error.assert_called_once_with(expected_message)
 
     def assert_exited_without_running_commands(self, actual: int) -> None:
         assert self.executor.command_log == []
         assert actual == 1
```

### Comparing `hpc-rocket-0.4.0/test/application/test_application_status_options.py` & `hpc-rocket-0.5.0/test/application/test_application_status_options.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/application/test_application_watch_options.py` & `hpc-rocket-0.5.0/test/application/test_application_watch_options.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/application/fixtures.py` & `hpc-rocket-0.5.0/test/integration/application/fixtures.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/application/test_application_with_filesystem.py` & `hpc-rocket-0.5.0/test/integration/application/test_application_with_filesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/application/test_application_with_paramiko.py` & `hpc-rocket-0.5.0/test/integration/application/test_application_with_paramiko.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/cli/test_cli_app_integration.py` & `hpc-rocket-0.5.0/test/integration/cli/test_cli_app_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
-from unittest.mock import patch
-
 from test.slurm_assertions import assert_job_submitted
 from test.testdoubles.executor import (
     LoggingCommandExecutorSpy,
     SlurmJobExecutorSpy,
     failed_slurm_job_command_stub,
     successful_slurm_job_command_stub,
 )
 from typing import Dict, List, Optional, cast
+from unittest.mock import patch
 
 import fs.base
 import pytest
 from fs.memoryfs import MemoryFS
-from hpcrocket import RuntimeContainer, ServiceRegistry
+
+from hpcrocket import ServiceRegistry, main
 from hpcrocket.core.executor import CommandExecutor, RunningCommand
 from hpcrocket.core.filesystem import Filesystem, FilesystemFactory
 from hpcrocket.core.launchoptions import Options
 from hpcrocket.pyfilesystem.pyfilesystembased import PyFilesystemBased
 from hpcrocket.ui import RichUI
 
 CONFIG_FILE_PATH = "test/testconfig/integration_launch_config_fail_allowed.yml"
@@ -117,16 +117,14 @@
     fs_factory = registry.fs_factory
 
     prepare_local_filesystem(fs_factory.local.internal_fs)
 
     args = ["hpc-rocket", "launch", "--watch", "config.yml"]
     run_with_args(registry, args)
 
-    print("\n")
-    fs_factory.remote.internal_fs.tree()
     assert fs_factory.local.exists("test.txt")
     assert fs_factory.local.exists("hello.txt")
     assert fs_factory.remote.exists("target/hello.txt")
     assert fs_factory.remote.exists("target/test.txt")
     assert fs_factory.remote.exists("target/subdir/next.txt")
     assert not fs_factory.remote.exists("my_slurm_job.job")
 
@@ -135,11 +133,8 @@
     job_result_command: Optional[RunningCommand] = None,
 ) -> _TestServiceRegistry:
     executor = SlurmJobExecutorSpy(job_result_command)
     return _TestServiceRegistry(executor, MemoryPyFilesystemFactory())
 
 
 def run_with_args(registry: ServiceRegistry, args: List[str]) -> int:
-    with RichUI() as ui:
-        sut = RuntimeContainer(args, registry, ui)
-        exit_code = sut.run()
-        return exit_code
+    return main(args, registry)
```

### Comparing `hpc-rocket-0.4.0/test/integration/paramiko/test_remotecommand.py` & `hpc-rocket-0.5.0/test/integration/paramiko/test_remotecommand.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/paramiko/test_slurmrunner_with_sshexecutor.py` & `hpc-rocket-0.5.0/test/integration/paramiko/test_slurmrunner_with_sshexecutor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/paramiko/test_sshexecutor.py` & `hpc-rocket-0.5.0/test/integration/paramiko/test_sshexecutor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/pyfilesystem/sshfilesystem_assertions.py` & `hpc-rocket-0.5.0/test/integration/pyfilesystem/sshfilesystem_assertions.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/integration/pyfilesystem/test_pyfilesystembased.py` & `hpc-rocket-0.5.0/test/integration/pyfilesystem/test_pyfilesystembased.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_cli.py` & `hpc-rocket-0.5.0/test/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
-from typing import Dict, Generator, List
+from pathlib import Path
+from typing import Dict, Generator, Iterator, List, Union, cast
 from unittest.mock import patch
 
 import pytest
-from hpcrocket.cli import parse_cli_args
+
+from hpcrocket.cli import ParseError, parse_cli_args
 from hpcrocket.core.filesystem.progressive import CopyInstruction
 from hpcrocket.core.launchoptions import (
     FinalizeOptions,
+    ImmediateCommandOptions,
     LaunchOptions,
     Options,
-    ImmediateCommandOptions,
     WatchOptions,
 )
 from hpcrocket.pyfilesystem.localfilesystem import localfilesystem
 from hpcrocket.ssh.connectiondata import ConnectionData
 
-
 HOME = "/home/user"
 REMOTE_USER = "the_user"
 REMOTE_HOST = "cluster.example.com"
 PROXY1_KEYFILE = "/home/user/.ssh/proxy1_keyfile"
 PROXY3_PASSWORD = "PROXY3_PASS"
 
 LOCAL_SLURM_SCRIPT_PATH = "slurm.job"
@@ -73,47 +74,45 @@
 
 @pytest.fixture(autouse=True)
 def setup_env() -> Generator[Dict[str, str], None, None]:
     with patch.dict(os.environ, ENV) as env:
         yield env
 
 
-def run_parser(args: List[str]) -> Options:
+def run_parser(args: List[str]) -> Union[Options, ParseError]:
     return parse_cli_args(args, localfilesystem(os.getcwd()))
 
 
 def test__given_valid_launch_args__should_return_matching_config() -> None:
     config = run_parser(
-        [
-            "launch",
-            "--watch",
-            "test/testconfig/config.yml",
-        ]
+        ["launch", "--watch", "test/testconfig/config.yml", "--save-jobid", "test.log"]
     )
 
     assert config == LaunchOptions(
         sbatch=REMOTE_SLURM_SCRIPT_PATH,
         connection=CONNECTION_DATA,
         proxyjumps=PROXYJUMPS,
         copy_files=[
             CopyInstruction("myfile.txt", "mycopy.txt"),
             CopyInstruction(LOCAL_SLURM_SCRIPT_PATH, REMOTE_SLURM_SCRIPT_PATH, True),
         ],
         clean_files=CLEAN_INSTRUCTIONS,
         collect_files=COLLECT_INSTRUCTIONS,
         continue_if_job_fails=True,
         watch=True,
+        job_id_file="test.log",
     )
 
 
 def test__given_status_args__when_parsing__should_return_matching_config() -> None:
     config = run_parser(
         [
             "status",
             "test/testconfig/config.yml",
+            "--jobid",
             "1234",
         ]
     )
 
     assert config == ImmediateCommandOptions(
         jobid="1234",
         action=ImmediateCommandOptions.Action.status,
@@ -123,14 +122,15 @@
 
 
 def test__given_watch_args__when_parsing__should_return_matching_config() -> None:
     config = run_parser(
         [
             "watch",
             "test/testconfig/config.yml",
+            "--jobid",
             "1234",
         ]
     )
 
     assert config == WatchOptions(
         jobid="1234",
         connection=CONNECTION_DATA,
@@ -139,14 +139,15 @@
 
 
 def test__given_cancel_args__when_parsing__should_return_matching_config() -> None:
     config = run_parser(
         [
             "cancel",
             "test/testconfig/config.yml",
+            "--jobid",
             "1234",
         ]
     )
 
     assert config == ImmediateCommandOptions(
         jobid="1234",
         action=ImmediateCommandOptions.Action.cancel,
@@ -165,7 +166,34 @@
 
     assert config == FinalizeOptions(
         connection=CONNECTION_DATA,
         proxyjumps=PROXYJUMPS,
         clean_files=CLEAN_INSTRUCTIONS,
         collect_files=COLLECT_INSTRUCTIONS,
     )
+
+
+@pytest.fixture
+def log_file() -> Iterator[None]:
+    log_file = Path("test.log")
+    log_file.write_text("1234")
+    yield
+    log_file.unlink(missing_ok=True)
+
+
+@pytest.mark.usefixtures("log_file")
+@pytest.mark.parametrize("command", ("status", "watch", "cancel"))
+def test__specified_option_to_read_jobid_from_log__when_parsing__options_contain_jobid(
+    command: str,
+) -> None:
+    config = run_parser(
+        [command, "test/testconfig/config.yml", "--read-jobid-from", "test.log"]
+    )
+
+    config = cast(ImmediateCommandOptions, config)
+    assert config.jobid == "1234"
+
+
+def test__given_non_existing_config_file__returns_parse_error() -> None:
+    config = run_parser(["launch"])
+
+    assert isinstance(config, ParseError)
```

### Comparing `hpc-rocket-0.4.0/test/test_executor.py` & `hpc-rocket-0.5.0/test/test_executor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_filesystem_abc.py` & `hpc-rocket-0.5.0/test/test_filesystem_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,17 @@
 
         sut.copy("*.txt", "newdir/")
 
         assert sut.exists("newdir/hello.txt")
         assert sut.exists("newdir/world.txt")
         assert not sut.exists("newdir/nope.gif")
 
-    def test__when_copying_with_trailing_glob__it_copies_subtree_into_target(self) -> None:
+    def test__when_copying_with_trailing_glob__it_copies_subtree_into_target(
+        self,
+    ) -> None:
         sut = self.create_filesystem()
         self.create_file(sut, "dir/first.txt")
         self.create_file(sut, "dir/subdir/second.txt")
 
         sut.copy("dir/*", "target")
 
         assert sut.exists("target/first.txt")
@@ -325,15 +327,17 @@
 
         sut.delete("*.txt")
 
         assert not sut.exists("hello.txt")
         assert not sut.exists("world.txt")
         assert sut.exists("nope.gif")
 
-    def test__when_deleteting_with_glob_in_dir__it_deletes_matching_files_but_not_dir(self) -> None:
+    def test__when_deleteting_with_glob_in_dir__it_deletes_matching_files_but_not_dir(
+        self,
+    ) -> None:
         sut = self.create_filesystem()
         self.create_file(sut, "directory/hello.txt")
         self.create_file(sut, "directory/subdir/file.txt")
 
         sut.delete("directory/*")
 
         assert sut.exists("directory")
```

### Comparing `hpc-rocket-0.4.0/test/test_jobwatcher.py` & `hpc-rocket-0.5.0/test/test_jobwatcher.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_progressive_fileoperations.py` & `hpc-rocket-0.5.0/test/test_progressive_fileoperations.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_slurmbatchjob.py` & `hpc-rocket-0.5.0/test/test_slurmbatchjob.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_slurmcontroller.py` & `hpc-rocket-0.5.0/test/test_slurmcontroller.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_slurmjob.py` & `hpc-rocket-0.5.0/test/test_slurmjob.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_typesafety.py` & `hpc-rocket-0.5.0/test/test_typesafety.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/test_watcherthread.py` & `hpc-rocket-0.5.0/test/test_watcherthread.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/executor.py` & `hpc-rocket-0.5.0/test/testdoubles/executor.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/filesystem.py` & `hpc-rocket-0.5.0/test/testdoubles/filesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/paramiko_sshclient_mockutil.py` & `hpc-rocket-0.5.0/test/testdoubles/paramiko_sshclient_mockutil.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/pyfilesystem.py` & `hpc-rocket-0.5.0/test/testdoubles/pyfilesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/sshclient.py` & `hpc-rocket-0.5.0/test/testdoubles/sshclient.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/testdoubles/test_memoryfilesystem.py` & `hpc-rocket-0.5.0/test/testdoubles/test_memoryfilesystem.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_cancelstage.py` & `hpc-rocket-0.5.0/test/workflows/test_cancelstage.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_finalizestage.py` & `hpc-rocket-0.5.0/test/workflows/test_finalizestage.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_launchstage.py` & `hpc-rocket-0.5.0/test/workflows/test_launchstage.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_preparestage.py` & `hpc-rocket-0.5.0/test/workflows/test_preparestage.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_statusstage.py` & `hpc-rocket-0.5.0/test/workflows/test_statusstage.py`

 * *Files identical despite different names*

### Comparing `hpc-rocket-0.4.0/test/workflows/test_watchstage.py` & `hpc-rocket-0.5.0/test/workflows/test_watchstage.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class BatchJobProviderSpy:
     def __init__(
         self,
         controller: SlurmController,
         jobid: str,
-        factory: Optional[JobWatcherFactory],
+        factory: Optional[JobWatcherFactory] = None,
     ) -> None:
         self.controller = controller
         self.jobid = jobid
         self.factory = factory
 
         self.was_canceled = False
```

### Comparing `hpc-rocket-0.4.0/test/workflows/test_workflow.py` & `hpc-rocket-0.5.0/test/workflows/test_workflow.py`

 * *Files identical despite different names*

