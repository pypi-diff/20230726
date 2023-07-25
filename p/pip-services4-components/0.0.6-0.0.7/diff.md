# Comparing `tmp/pip_services4_components-0.0.6.tar.gz` & `tmp/pip_services4_components-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_components-0.0.6.tar", last modified: Tue Jul 25 19:29:24 2023, max compression
+gzip compressed data, was "pip_services4_components-0.0.7.tar", last modified: Tue Jul 25 23:00:46 2023, max compression
```

## Comparing `pip_services4_components-0.0.6.tar` & `pip_services4_components-0.0.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.081045 pip_services4_components-0.0.6/
--rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5480 2023-07-25 19:29:24.081045 pip_services4_components-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:23.995423 pip_services4_components-0.0.6/pip_services4_components/
--rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.6/pip_services4_components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.012811 pip_services4_components-0.0.6/pip_services4_components/build/
--rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.6/pip_services4_components/build/CompositeFactory.py
--rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.6/pip_services4_components/build/CreateException.py
--rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.6/pip_services4_components/build/Factory.py
--rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.6/pip_services4_components/build/IFactory.py
--rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.6/pip_services4_components/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.023317 pip_services4_components-0.0.6/pip_services4_components/config/
--rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.6/pip_services4_components/config/ConfigParams.py
--rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.6/pip_services4_components/config/IConfigurable.py
--rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.6/pip_services4_components/config/IReconfigurable.py
--rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.6/pip_services4_components/config/NameResolver.py
--rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.6/pip_services4_components/config/OptionsResolver.py
--rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.6/pip_services4_components/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.035331 pip_services4_components-0.0.6/pip_services4_components/context/
--rw-rw-rw-   0        0        0     2488 2023-07-24 11:24:52.000000 pip_services4_components-0.0.6/pip_services4_components/context/Context.py
--rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.6/pip_services4_components/context/ContextInfo.py
--rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.6/pip_services4_components/context/ContextResolver.py
--rw-rw-rw-   0        0        0     1214 2023-07-25 18:21:26.000000 pip_services4_components-0.0.6/pip_services4_components/context/DefaultContextFactory.py
--rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.6/pip_services4_components/context/IContext.py
--rw-rw-rw-   0        0        0      773 2023-07-25 18:16:24.000000 pip_services4_components-0.0.6/pip_services4_components/context/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.048045 pip_services4_components-0.0.6/pip_services4_components/exec/
--rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/Executor.py
--rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/FixedRateTimer.py
--rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/IExecutable.py
--rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/INotifiable.py
--rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/IParameterized.py
--rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/Notifier.py
--rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/Parameters.py
--rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/exec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.062046 pip_services4_components-0.0.6/pip_services4_components/refer/
--rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/DependencyResolver.py
--rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.6/pip_services4_components/refer/Descriptor.py
--rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/IReferenceable.py
--rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/IReferences.py
--rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/IUnreferenceable.py
--rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/Reference.py
--rw-rw-rw-   0        0        0     1196 2023-07-24 07:50:07.000000 pip_services4_components-0.0.6/pip_services4_components/refer/ReferenceException.py
--rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/Referencer.py
--rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/References.py
--rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/refer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.072044 pip_services4_components-0.0.6/pip_services4_components/run/
--rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/Cleaner.py
--rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/Closer.py
--rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/ICleanable.py
--rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/IClosable.py
--rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/IOpenable.py
--rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/Opener.py
--rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.6/pip_services4_components/run/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.005806 pip_services4_components-0.0.6/pip_services4_components.egg-info/
--rw-rw-rw-   0        0        0     5480 2023-07-25 19:29:23.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2473 2023-07-25 19:29:23.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:29:23.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-25 19:29:23.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-07-25 19:29:23.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.6/pip_services4_components.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-25 19:29:24.082045 pip_services4_components-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-07-25 19:28:43.000000 pip_services4_components-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:23.986422 pip_services4_components-0.0.6/test/
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.075044 pip_services4_components-0.0.6/test/context/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.6/test/context/__init__.py
--rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.6/test/context/test_ContextInfo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:29:24.080046 pip_services4_components-0.0.6/test/exec/
--rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.6/test/exec/ClassTest.py
--rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.6/test/exec/__init__.py
--rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.6/test/exec/test_FixedRateTimer.py
--rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.6/test/exec/test_Parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.260993 pip_services4_components-0.0.7/
+-rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5480 2023-07-25 23:00:46.261991 pip_services4_components-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.198299 pip_services4_components-0.0.7/pip_services4_components/
+-rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.7/pip_services4_components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.213298 pip_services4_components-0.0.7/pip_services4_components/build/
+-rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.7/pip_services4_components/build/CompositeFactory.py
+-rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.7/pip_services4_components/build/CreateException.py
+-rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.7/pip_services4_components/build/Factory.py
+-rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.7/pip_services4_components/build/IFactory.py
+-rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.7/pip_services4_components/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.219297 pip_services4_components-0.0.7/pip_services4_components/config/
+-rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.7/pip_services4_components/config/ConfigParams.py
+-rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.7/pip_services4_components/config/IConfigurable.py
+-rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.7/pip_services4_components/config/IReconfigurable.py
+-rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.7/pip_services4_components/config/NameResolver.py
+-rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.7/pip_services4_components/config/OptionsResolver.py
+-rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.7/pip_services4_components/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.226413 pip_services4_components-0.0.7/pip_services4_components/context/
+-rw-rw-rw-   0        0        0     2488 2023-07-24 11:24:52.000000 pip_services4_components-0.0.7/pip_services4_components/context/Context.py
+-rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.7/pip_services4_components/context/ContextInfo.py
+-rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.7/pip_services4_components/context/ContextResolver.py
+-rw-rw-rw-   0        0        0     1214 2023-07-25 18:21:26.000000 pip_services4_components-0.0.7/pip_services4_components/context/DefaultContextFactory.py
+-rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.7/pip_services4_components/context/IContext.py
+-rw-rw-rw-   0        0        0      773 2023-07-25 18:16:24.000000 pip_services4_components-0.0.7/pip_services4_components/context/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.235417 pip_services4_components-0.0.7/pip_services4_components/exec/
+-rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/Executor.py
+-rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/FixedRateTimer.py
+-rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/IExecutable.py
+-rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/INotifiable.py
+-rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/IParameterized.py
+-rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/Notifier.py
+-rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/Parameters.py
+-rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/exec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.246601 pip_services4_components-0.0.7/pip_services4_components/refer/
+-rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/DependencyResolver.py
+-rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.7/pip_services4_components/refer/Descriptor.py
+-rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/IReferenceable.py
+-rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/IReferences.py
+-rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/IUnreferenceable.py
+-rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/Reference.py
+-rw-rw-rw-   0        0        0     1173 2023-07-25 23:00:12.000000 pip_services4_components-0.0.7/pip_services4_components/refer/ReferenceException.py
+-rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/Referencer.py
+-rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/References.py
+-rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/refer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.253597 pip_services4_components-0.0.7/pip_services4_components/run/
+-rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/Cleaner.py
+-rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/Closer.py
+-rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/ICleanable.py
+-rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/IClosable.py
+-rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/IOpenable.py
+-rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/Opener.py
+-rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.7/pip_services4_components/run/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.207297 pip_services4_components-0.0.7/pip_services4_components.egg-info/
+-rw-rw-rw-   0        0        0     5480 2023-07-25 23:00:46.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2473 2023-07-25 23:00:46.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 23:00:46.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-25 23:00:46.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-07-25 23:00:46.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.7/pip_services4_components.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 23:00:46.262995 pip_services4_components-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-25 23:00:21.000000 pip_services4_components-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.189296 pip_services4_components-0.0.7/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.255596 pip_services4_components-0.0.7/test/context/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.7/test/context/__init__.py
+-rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.7/test/context/test_ContextInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:00:46.259992 pip_services4_components-0.0.7/test/exec/
+-rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.7/test/exec/ClassTest.py
+-rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.7/test/exec/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.7/test/exec/test_FixedRateTimer.py
+-rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.7/test/exec/test_Parameters.py
```

### Comparing `pip_services4_components-0.0.6/LICENSE` & `pip_services4_components-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/PKG-INFO` & `pip_services4_components-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_components
-Version: 0.0.6
+Version: 0.0.7
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.6/README.md` & `pip_services4_components-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/build/CompositeFactory.py` & `pip_services4_components-0.0.7/pip_services4_components/build/CompositeFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/build/CreateException.py` & `pip_services4_components-0.0.7/pip_services4_components/build/CreateException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/build/Factory.py` & `pip_services4_components-0.0.7/pip_services4_components/build/Factory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/build/IFactory.py` & `pip_services4_components-0.0.7/pip_services4_components/build/IFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/build/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/ConfigParams.py` & `pip_services4_components-0.0.7/pip_services4_components/config/ConfigParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/IConfigurable.py` & `pip_services4_components-0.0.7/pip_services4_components/config/IConfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/IReconfigurable.py` & `pip_services4_components-0.0.7/pip_services4_components/config/IReconfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/NameResolver.py` & `pip_services4_components-0.0.7/pip_services4_components/config/NameResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/OptionsResolver.py` & `pip_services4_components-0.0.7/pip_services4_components/config/OptionsResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/config/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/context/Context.py` & `pip_services4_components-0.0.7/pip_services4_components/context/Context.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/context/ContextInfo.py` & `pip_services4_components-0.0.7/pip_services4_components/context/ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/context/ContextResolver.py` & `pip_services4_components-0.0.7/pip_services4_components/context/ContextResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/context/DefaultContextFactory.py` & `pip_services4_components-0.0.7/pip_services4_components/context/DefaultContextFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/context/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/context/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/Executor.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/Executor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/FixedRateTimer.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/IExecutable.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/IExecutable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/INotifiable.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/INotifiable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/IParameterized.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/IParameterized.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/Notifier.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/Notifier.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/Parameters.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/Parameters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/exec/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/DependencyResolver.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/DependencyResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/Descriptor.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/Descriptor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/IReferenceable.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/IReferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/IReferences.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/IReferences.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/IUnreferenceable.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/IUnreferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/Reference.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/Reference.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/ReferenceException.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/ReferenceException.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from typing import Any, Optional
 
 from pip_services4_commons.errors import InternalException
 
-from pip_services4_components.context import ContextResolver, IContext
+from ..context import ContextResolver, IContext
 
 
 class ReferenceException(InternalException):
     """
     Error when __required component dependency cannot be found.
     """
```

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/Referencer.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/Referencer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/References.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/References.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/refer/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/refer/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/Cleaner.py` & `pip_services4_components-0.0.7/pip_services4_components/run/Cleaner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/Closer.py` & `pip_services4_components-0.0.7/pip_services4_components/run/Closer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/ICleanable.py` & `pip_services4_components-0.0.7/pip_services4_components/run/ICleanable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/IClosable.py` & `pip_services4_components-0.0.7/pip_services4_components/run/IClosable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/IOpenable.py` & `pip_services4_components-0.0.7/pip_services4_components/run/IOpenable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/Opener.py` & `pip_services4_components-0.0.7/pip_services4_components/run/Opener.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components/run/__init__.py` & `pip_services4_components-0.0.7/pip_services4_components/run/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/pip_services4_components.egg-info/PKG-INFO` & `pip_services4_components-0.0.7/pip_services4_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-components
-Version: 0.0.6
+Version: 0.0.7
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.6/pip_services4_components.egg-info/SOURCES.txt` & `pip_services4_components-0.0.7/pip_services4_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/setup.py` & `pip_services4_components-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_components',
-    version='0.0.6',
+    version='0.0.7',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-components-python',
     license='MIT',
     description='Component definitions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `pip_services4_components-0.0.6/test/context/test_ContextInfo.py` & `pip_services4_components-0.0.7/test/context/test_ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/test/exec/test_FixedRateTimer.py` & `pip_services4_components-0.0.7/test/exec/test_FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.6/test/exec/test_Parameters.py` & `pip_services4_components-0.0.7/test/exec/test_Parameters.py`

 * *Files identical despite different names*

