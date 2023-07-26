# Comparing `tmp/pdm-2.8.0a2.tar.gz` & `tmp/pdm-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.8.0a2.tar", last modified: Fri Jun 30 01:46:07 2023, max compression
+gzip compressed data, was "pdm-2.8.1.tar", last modified: Wed Jul 26 05:34:15 2023, max compression
```

## Comparing `pdm-2.8.0a2.tar` & `pdm-2.8.1.tar`

### file list

```diff
@@ -1,280 +1,281 @@
--rw-r--r--   0        0        0   126958 2023-06-30 01:45:58.402574 pdm-2.8.0a2/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-30 01:45:58.402574 pdm-2.8.0a2/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-30 01:45:58.402574 pdm-2.8.0a2/LICENSE
--rw-r--r--   0        0        0     7937 2023-06-30 01:45:58.402574 pdm-2.8.0a2/README.md
--rw-r--r--   0        0        0     7937 2023-06-30 01:45:58.402574 pdm-2.8.0a2/README.md
--rw-r--r--   0        0        0     4559 2023-06-30 01:46:06.994550 pdm-2.8.0a2/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    16246 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7104 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2857 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     7165 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3689 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0    10543 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3638 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8112 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4284 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15489 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9370 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     7260 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6489 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1723 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-30 01:45:58.406574 pdm-2.8.0a2/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5137 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    50498 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18629 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25397 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/options.py
--rw-r--r--   0        0        0     6539 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/__init__.py
--rw-r--r--   0        0        0     3102 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/.gitignore
--rw-r--r--   0        0        0       18 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/README.md
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/__init__.py
--rw-r--r--   0        0        0      278 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/src/example_package/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/templates/default/tests/__init__.py
--rw-r--r--   0        0        0    25152 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2373 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/compat.py
--rw-r--r--   0        0        0    10667 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/base.py
--rw-r--r--   0        0        0     4255 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2614 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7502 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1367 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18219 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4698 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/backends.py
--rw-r--r--   0        0        0    12115 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26580 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1845 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18792 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/search.py
--rw-r--r--   0        0        0     3363 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2766 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-30 01:45:58.410574 pdm-2.8.0a2/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16757 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/config.py
--rw-r--r--   0        0        0    27068 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/py.typed
--rw-r--r--   0        0        0    20067 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     2001 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13176 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/termui.py
--rw-r--r--   0        0        0    14101 2023-06-30 01:45:58.414574 pdm-2.8.0a2/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_add.py
--rw-r--r--   0        0        0     5795 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4950 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     2778 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_template.py
--rw-r--r--   0        0        0     8876 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_use.py
--rw-r--r--   0        0        0    10808 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-30 01:45:58.414574 pdm-2.8.0a2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-30 01:45:58.418574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-30 01:45:58.422574 pdm-2.8.0a2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-30 01:45:58.426574 pdm-2.8.0a2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       13 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      572 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      726 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-30 01:45:58.430574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      344 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_signals.py
--rw-r--r--   0        0        0     4409 2023-06-30 01:45:58.434574 pdm-2.8.0a2/tests/test_utils.py
--rw-r--r--   0        0        0     9838 1970-01-01 00:00:00.000000 pdm-2.8.0a2/PKG-INFO
+-rw-r--r--   0        0        0   129793 2023-07-26 05:34:05.032076 pdm-2.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-07-26 05:34:05.032076 pdm-2.8.1/LICENSE
+-rw-r--r--   0        0        0     1075 2023-07-26 05:34:05.032076 pdm-2.8.1/LICENSE
+-rw-r--r--   0        0        0     7937 2023-07-26 05:34:05.032076 pdm-2.8.1/README.md
+-rw-r--r--   0        0        0     7937 2023-07-26 05:34:05.032076 pdm-2.8.1/README.md
+-rw-r--r--   0        0        0     4715 2023-07-26 05:34:15.188673 pdm-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3413 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11906 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1791 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16569 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.036077 pdm-2.8.1/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7084 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2871 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1275 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7537 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3679 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0    10561 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3982 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2645 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4284 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15489 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2437 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9371 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     7276 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6484 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1720 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2427 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2156 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      820 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2196 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1280 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2652 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5168 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    50740 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18666 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25535 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10529 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6539 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    26365 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2373 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/compat.py
+-rw-r--r--   0        0        0    10620 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     9734 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4255 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-26 05:34:05.040077 pdm-2.8.1/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7513 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    11127 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2092 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18219 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    11150 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        6 2023-07-26 05:34:15.160672 pdm-2.8.1/src/pdm/models/VERSION
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4916 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    12115 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26687 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     2114 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2202 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    22707 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18772 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3292 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16725 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2858 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    17114 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26872 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2194 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/py.typed
+-rw-r--r--   0        0        0    20073 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     2001 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13381 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1577 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/termui.py
+-rw-r--r--   0        0        0    14109 2023-07-26 05:34:05.044077 pdm-2.8.1/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-07-26 05:34:05.044077 pdm-2.8.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.044077 pdm-2.8.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5795 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11242 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6975 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29463 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2778 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_template.py
+-rw-r--r--   0        0        0     8876 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10808 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-07-26 05:34:05.048077 pdm-2.8.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    94569 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-07-26 05:34:05.052077 pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-07-26 05:34:05.056078 pdm-2.8.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-07-26 05:34:05.056078 pdm-2.8.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    13807 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      572 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-26 05:34:05.064078 pdm-2.8.1/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13397 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2936 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3590 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_signals.py
+-rw-r--r--   0        0        0     4409 2023-07-26 05:34:05.068078 pdm-2.8.1/tests/test_utils.py
+-rw-r--r--   0        0        0    10122 1970-01-01 00:00:00.000000 pdm-2.8.1/PKG-INFO
```

### Comparing `pdm-2.8.0a2/CHANGELOG.md` & `pdm-2.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,53 @@
+Release v2.8.1 (2023-07-26)
+---------------------------
+
+### Features & Improvements
+
+- Add `keyring`, `copier`, `cookiecutter`, `template`, `truststore` dependency groups. [#2109](https://github.com/pdm-project/pdm/issues/2109)
+- Ignore wheels for python versions not in range. [#2113](https://github.com/pdm-project/pdm/issues/2113)
+- Read default value from env var `PDM_PROJECT` for `-p/--project` option. [#2126](https://github.com/pdm-project/pdm/issues/2126)
+
+### Bug Fixes
+
+- Fix the comparison of the candidate keys in the lockfile. [#2120](https://github.com/pdm-project/pdm/issues/2120)
+- Don't update `pyproject.toml` if both `--unconstrained` and `--dry-run` are passed to `pdm update`. [#2125](https://github.com/pdm-project/pdm/issues/2125)
+- Overwrite the `build-system` table when importing from other package manager. [#2126](https://github.com/pdm-project/pdm/issues/2126)
+- Skip sources with empty URL when merging sources. [#2130](https://github.com/pdm-project/pdm/issues/2130)
+- Fix the invalid requirement converted from poetry metadata. [#2133](https://github.com/pdm-project/pdm/issues/2133)
+
+### Dependencies
+
+- Update `unearth` to 0.10.0 [#2113](https://github.com/pdm-project/pdm/issues/2113)
+
+
+Release v2.8.0 (2023-07-15)
+---------------------------
+
+### Features & Improvements
+
+- Support target python with other architectures. [#2078](https://github.com/pdm-project/pdm/issues/2078)
+- Display the help information when running pdm directly. [#2081](https://github.com/pdm-project/pdm/issues/2081)
+- Allow to change the python providers from the config. Support finding pythons from Rye installation location with the new findpython. [#2099](https://github.com/pdm-project/pdm/issues/2099)
+- Option to save static URLs in the lockfile. By default only filenames are saved. [#2101](https://github.com/pdm-project/pdm/issues/2101)
+
+### Bug Fixes
+
+- Fix a bug that egg-info directories are not removed completely, leading to incomplete distribution. [#2027](https://github.com/pdm-project/pdm/issues/2027)
+- Skip distributions with wrong package meta information and duplicate path. [#2075](https://github.com/pdm-project/pdm/issues/2075)
+- Avoid mistakenly passing command-line arguments while testing. [#2083](https://github.com/pdm-project/pdm/issues/2083)
+- Fix a bug that lockfile groups are overwritten when running locking in a preceding step of `pdm install`. [#2086](https://github.com/pdm-project/pdm/issues/2086)
+- Tolerate and actually ignore the local versions in version specifiers. [#2102](https://github.com/pdm-project/pdm/issues/2102)
+- Fix a bug that shared cache cannot support overlapping namespace packages. [#2105](https://github.com/pdm-project/pdm/issues/2105)
+
+### Documentation
+
+- Add notes about using custom venv path. [#2096](https://github.com/pdm-project/pdm/issues/2096)
+
+
 Release v2.8.0a2 (2023-06-30)
 -----------------------------
 
 ### Bug Fixes
 
 - Fix a bug that dependencies can't be updated when the table is separated by another table. [#2056](https://github.com/pdm-project/pdm/issues/2056)
 - Fix a bug that `*_lock` hooks are always emitted with dry_run=True in `pdm update`. [#2060](https://github.com/pdm-project/pdm/issues/2060)
```

### Comparing `pdm-2.8.0a2/LICENSE` & `pdm-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/README.md` & `pdm-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/pyproject.toml` & `pdm-2.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     "certifi",
     "packaging>=20.9,!=22.0",
     "platformdirs",
     "rich>=12.3.0",
     "virtualenv>=20",
     "pyproject-hooks",
     "requests-toolbelt",
-    "unearth>=0.9.0",
-    "findpython>=0.2.2",
+    "unearth>=0.10.0",
+    "findpython>=0.3.0,<1.0.0a0",
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
     "cachecontrol[filecache]>=0.13.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.8.0a2"
+version = "2.8.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
@@ -54,20 +54,32 @@
 Changelog = "https://pdm.fming.dev/latest/dev/changelog/"
 
 [project.optional-dependencies]
 pytest = [
     "pytest",
     "pytest-mock",
 ]
-all = [
+copier = [
     "copier",
+]
+cookiecutter = [
     "cookiecutter",
+]
+keyring = [
     "keyring",
+]
+template = [
+    "pdm[copier,cookiecutter]",
+]
+truststore = [
     "truststore; python_version >= \"3.10\"",
 ]
+all = [
+    "pdm[keyring,template,truststore]",
+]
 
 [project.scripts]
 pdm = "pdm.core:main"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "pdm/models/VERSION"
@@ -138,19 +150,18 @@
     "py38",
     "py39",
     "py310",
 ]
 
 [tool.ruff]
 line-length = 120
-select = [
+extend-select = [
+    "I",
     "B",
     "C4",
-    "E",
-    "F",
     "PGH",
     "RUF",
     "W",
     "YTT",
 ]
 extend-ignore = [
     "B018",
```

### Comparing `pdm-2.8.0a2/src/pdm/_types.py` & `pdm-2.8.1/src/pdm/_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     summary: str
 
 
 SearchResult = List[Package]
 
 
 if TYPE_CHECKING:
+    from typing import TypedDict
 
     class Comparable(Protocol):
         def __lt__(self, __other: Any) -> bool:
             ...
 
     SpinnerT = TypeVar("SpinnerT", bound="Spinner")
 
@@ -101,7 +102,12 @@
 
         def __exit__(self, *args: Any) -> None:
             ...
 
     class RichProtocol(Protocol):
         def __rich__(self) -> str:
             ...
+
+    class FileHash(TypedDict, total=False):
+        url: str
+        hash: str
+        file: str
```

### Comparing `pdm-2.8.0a2/src/pdm/builders/base.py` & `pdm-2.8.1/src/pdm/builders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import shutil
 import subprocess
 import textwrap
 import threading
 from logging import Logger
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, cast
+from typing import TYPE_CHECKING, Any, ClassVar, Iterable, Mapping, cast
 
 from pyproject_hooks import BuildBackendHookCaller
 
 from pdm.compat import tomllib
 from pdm.environments import PythonEnvironment
 from pdm.exceptions import BuildError
 from pdm.models.in_process import get_sys_config_paths
@@ -145,21 +145,21 @@
         self.shared = shared
         self.overlay = overlay
 
 
 class EnvBuilder:
     """A simple PEP 517 builder for an isolated environment"""
 
-    DEFAULT_BACKEND = {
+    DEFAULT_BACKEND: ClassVar[dict[str, Any]] = {
         "build-backend": "setuptools.build_meta:__legacy__",
         "requires": ["setuptools >= 40.8.0", "wheel"],
     }
 
-    _shared_envs: dict[int, str] = {}
-    _overlay_envs: dict[str, str] = {}
+    _shared_envs: ClassVar[dict[int, str]] = {}
+    _overlay_envs: ClassVar[dict[str, str]] = {}
 
     if TYPE_CHECKING:
         _hook: BuildBackendHookCaller
         _requires: list[str]
         _prefix: _Prefix
 
     @classmethod
```

### Comparing `pdm-2.8.0a2/src/pdm/builders/editable.py` & `pdm-2.8.1/src/pdm/builders/editable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import os
-from typing import Any, Mapping
+from typing import Any, ClassVar, Mapping
 
 from pyproject_hooks import HookMissing
 
 from pdm.builders.base import EnvBuilder
 from pdm.termui import logger
 
 
 class EditableBuilder(EnvBuilder):
     """Build egg-info in isolated env with managed Python."""
 
-    FALLBACK_BACKEND = {
+    FALLBACK_BACKEND: ClassVar[dict[str, Any]] = {
         "build-backend": "setuptools_pep660",
         "requires": ["setuptools_pep660"],
     }
 
     def prepare_metadata(self, out_dir: str, config_settings: Mapping[str, Any] | None = None) -> str:
         self.install(self._requires, shared=True)
         try:
```

### Comparing `pdm-2.8.0a2/src/pdm/builders/sdist.py` & `pdm-2.8.1/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/builders/wheel.py` & `pdm-2.8.1/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/actions.py` & `pdm-2.8.1/src/pdm/cli/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,35 +39,42 @@
     strategy: str = "all",
     tracked_names: Iterable[str] | None = None,
     requirements: list[Requirement] | None = None,
     dry_run: bool = False,
     refresh: bool = False,
     groups: list[str] | None = None,
     cross_platform: bool | None = None,
+    static_urls: bool | None = None,
     hooks: HookManager | None = None,
 ) -> dict[str, Candidate]:
     """Performs the locking process and update lockfile."""
     hooks = hooks or HookManager(project)
     check_project_file(project)
+    if static_urls is None:
+        static_urls = project.lockfile.static_urls
     if refresh:
         locked_repo = project.locked_repository
         repo = project.get_repository()
         mapping: dict[str, Candidate] = {}
         dependencies: dict[tuple[str, str | None], list[Requirement]] = {}
         with project.core.ui.open_spinner("Re-calculating hashes..."):
             for key, candidate in locked_repo.packages.items():
                 reqs, python_requires, summary = locked_repo.candidate_info[key]
                 candidate.summary = summary
                 candidate.requires_python = python_requires
                 mapping[candidate.identify()] = candidate
                 dependencies[candidate.dep_key] = list(map(parse_requirement, reqs))
             with project.core.ui.logging("lock"):
+                for c in mapping.values():
+                    c.hashes.clear()
                 fetch_hashes(repo, mapping)
-            lockfile = format_lockfile(project, mapping, dependencies)
-        project.write_lockfile(lockfile, groups=groups)
+            lockfile = format_lockfile(
+                project, mapping, dependencies, groups=project.lockfile.groups, static_urls=static_urls
+            )
+        project.write_lockfile(lockfile)
         return mapping
     # TODO: multiple dependency definitions for the same package.
     if cross_platform is None:
         cross_platform = project.lockfile.cross_platform
     provider = project.get_provider(strategy, tracked_names, ignore_compatibility=cross_platform)
     if not requirements:
         requirements = [
@@ -105,17 +112,19 @@
             )
             raise
         except ResolutionImpossible as err:
             ui.echo(f"{termui.Emoji.LOCK} Lock failed", err=True)
             ui.echo(format_resolution_impossible(err), err=True)
             raise ResolutionImpossible("Unable to find a resolution") from None
         else:
-            data = format_lockfile(project, mapping, dependencies)
+            data = format_lockfile(
+                project, mapping, dependencies, groups=groups, cross_platform=cross_platform, static_urls=static_urls
+            )
             ui.echo(f"{termui.Emoji.LOCK} Lock successful")
-            project.write_lockfile(data, write=not dry_run, groups=groups, cross_platform=cross_platform)
+            project.write_lockfile(data, write=not dry_run)
             hooks.try_emit("post_lock", resolution=mapping, dry_run=dry_run)
 
     return mapping
 
 
 def resolve_candidates_from_lockfile(project: Project, requirements: Iterable[Requirement]) -> dict[str, Candidate]:
     ui = project.core.ui
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/add.py` & `pdm-2.8.1/src/pdm/cli/commands/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     from pdm.models.requirements import Requirement
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Add package(s) to pyproject.toml and install them"""
 
-    arguments = [
+    arguments = (
         *BaseCommand.arguments,
         lockfile_option,
         save_strategy_group,
         update_strategy_group,
         prerelease_option,
         unconstrained_option,
         packages_group,
         install_group,
         dry_run_option,
         venv_option,
         skip_option,
-    ]
+    )
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-d",
             "--dev",
             default=False,
             action="store_true",
@@ -167,15 +167,15 @@
             )
 
         # Update dependency specifiers and lockfile hash.
         deps_to_update = group_deps if unconstrained else requirements
         save_version_specifiers({group: deps_to_update}, resolved, save)
         if not dry_run:
             project.add_dependencies(deps_to_update, group, selection.dev or False)
-            project.write_lockfile(project.lockfile._data, False, groups=lock_groups)
+            project.write_lockfile(project.lockfile._data, False)
             hooks.try_emit("post_lock", resolution=resolved, dry_run=dry_run)
         populate_requirement_names(group_deps)
         if sync:
             do_sync(
                 project,
                 selection=GroupSelection(project, groups=[group], default=False),
                 no_editable=no_editable and tracked_names,
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/base.py` & `pdm-2.8.1/src/pdm/cli/commands/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import argparse
 import inspect
 from argparse import _SubParsersAction
-from typing import Any, TypeVar
+from typing import Any, Sequence, TypeVar
 
 from pdm.cli.options import Option, global_option, project_option, verbose_option
 from pdm.project import Project
 from pdm.utils import deprecation_warning
 
 C = TypeVar("C", bound="BaseCommand")
 
@@ -17,15 +17,15 @@
 
     # The subcommand's name
     name: str | None = None
     # The subcommand's help string, if not given, __doc__ will be used.
     description: str | None = None
     # A list of pre-defined options which will be loaded on initializing
     # Rewrite this if you don't want the default ones
-    arguments: list[Option] = [verbose_option, global_option, project_option]
+    arguments: Sequence[Option] = (verbose_option, global_option, project_option)
 
     def __init__(self, parser: argparse.ArgumentParser | None = None) -> None:
         """For compatibility, the parser is optional and won't be used."""
 
     @classmethod
     def init_parser(cls: type[C], parser: argparse.ArgumentParser) -> C:
         args = inspect.signature(cls).parameters
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/build.py` & `pdm-2.8.1/src/pdm/cli/commands/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pdm.exceptions import ProjectError
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Build artifacts for distribution"""
 
-    arguments = [verbose_option, project_option, no_isolation_option, skip_option]
+    arguments = (verbose_option, project_option, no_isolation_option, skip_option)
 
     @staticmethod
     def do_build(
         project: Project,
         sdist: bool = True,
         wheel: bool = True,
         dest: str = "dist",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/cache.py` & `pdm-2.8.1/src/pdm/cli/commands/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Control the caches of PDM"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        subparsers = parser.add_subparsers(title="commands", metavar="cache")
+        subparsers = parser.add_subparsers(title="commands", metavar="")
         ClearCommand.register_to(subparsers, "clear")
         RemoveCommand.register_to(subparsers, "remove")
         ListCommand.register_to(subparsers, "list")
         InfoCommand.register_to(subparsers, "info")
         parser.set_defaults(search_parent=False)
         self.parser = parser
 
@@ -70,15 +70,15 @@
         project.core.ui.echo(f"Removed {file}", verbosity=termui.Verbosity.DETAIL)
     project.core.ui.echo(f"{len(files)} file{'s' if len(files) > 1 else ''} removed")
 
 
 class ClearCommand(BaseCommand):
     """Clean all the files under cache directory"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     CACHE_TYPES = ("hashes", "http", "wheels", "metadata", "packages")
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "type",
             nargs="?",
             help="Clear the given type of caches",
@@ -136,42 +136,42 @@
                 text = f"{' and '.join(message)} are removed"
         project.core.ui.echo(text)
 
 
 class RemoveCommand(BaseCommand):
     """Remove files matching the given pattern"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("pattern", help="The pattern to remove")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         return remove_cache_files(project, options.pattern)
 
 
 class ListCommand(BaseCommand):
     """List the built wheels stored in the cache"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("pattern", nargs="?", default="*", help="The pattern to list")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         rows = [
             (format_size(file_size(file)), file.name) for file in find_files(project.cache("wheels"), options.pattern)
         ]
         project.core.ui.display_columns(rows, [">Size", "Filename"])
 
 
 class InfoCommand(BaseCommand):
     """Show the info and current size of caches"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         with project.core.ui.open_spinner("Calculating cache files"):
             output = [
                 f"[primary]Cache Root[/]: {project.cache_dir}, "
                 f"Total size: {format_size(directory_size(project.cache_dir))}"
             ]
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/completion.py` & `pdm-2.8.1/src/pdm/cli/commands/completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 import argparse
 import sys
 
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.options import Option
 from pdm.compat import resources_read_text
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Generate completion scripts for the given shell"""
 
-    arguments: list[Option] = []
+    arguments = ()
     SUPPORTED_SHELLS = ("bash", "zsh", "fish", "powershell", "pwsh")
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "shell",
             nargs="?",
             help="The shell to generate the scripts for. "
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/config.py` & `pdm-2.8.1/src/pdm/cli/commands/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,40 +70,46 @@
             self._set_config(project, options)
         elif options.key:
             self._get_config(project, options)
         else:
             self._list_config(project, options)
 
     def _get_config(self, project: Project, options: argparse.Namespace) -> None:
+        from findpython import ALL_PROVIDERS
+
         if options.key in project.project_config.deprecated:  # pragma: no cover
             project.core.ui.echo(
                 f"DEPRECATED: the config has been renamed to {project.project_config.deprecated[options.key]}",
                 style="warning",
                 err=True,
             )
             options.key = project.project_config.deprecated[options.key]
         try:
             value = project.project_config[options.key]
         except KeyError:
             value = project.global_config[options.key]
         if options.key.endswith(".password"):
             value = "[i]<hidden>[/i]"
+        elif options.key == "python.providers" and not value:
+            value = ["venv", *ALL_PROVIDERS]
         project.core.ui.echo(value)
 
     def _set_config(self, project: Project, options: argparse.Namespace) -> None:
         config = project.project_config if options.local else project.global_config
         if options.key in config.deprecated:  # pragma: no cover
             project.core.ui.echo(
                 f"DEPRECATED: the config has been renamed to {config.deprecated[options.key]}",
                 style="warning",
                 err=True,
             )
         config[options.key] = options.value
 
     def _show_config(self, config: Mapping[str, Any], supersedes: Mapping[str, Any]) -> None:
+        from findpython import ALL_PROVIDERS
+
         assert Config.site is not None
         for key in sorted(config):
             deprecated = ""
             canonical_key = key
             superseded = key in supersedes
             if key in Config.site.deprecated:  # pragma: no cover
                 canonical_key = Config.site.deprecated[key]
@@ -129,15 +135,20 @@
                 continue
             config_item = Config._config_map[canonical_key]
             self.ui.echo(
                 f"[warning]# {config_item.description}",
                 style=extra_style,
                 verbosity=termui.Verbosity.DETAIL,
             )
-            value = "[i]<hidden>[/]" if key.endswith("password") else config[key]
+            if key.endswith("password"):
+                value: Any = "[i]<hidden>[/i]"
+            else:
+                value = config[key]
+                if key == "python.providers" and not value:
+                    value = ["venv", *ALL_PROVIDERS]
             self.ui.echo(
                 f"[primary]{canonical_key}[/]{deprecated} = {value}",
                 style=extra_style,
             )
 
     def _list_config(self, project: Project, options: argparse.Namespace) -> None:
         assert Config.site is not None
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/export.py` & `pdm-2.8.1/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.8.1/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.8.1/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/import_cmd.py` & `pdm-2.8.1/src/pdm/cli/commands/import_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         if "project" not in pyproject:
             pyproject.add("project", tomlkit.table())
             pyproject["project"].add(tomlkit.comment("PEP 621 project metadata"))
             pyproject["project"].add(tomlkit.comment("See https://www.python.org/dev/peps/pep-0621/"))
 
         merge_dictionary(pyproject["project"], project_data)
         merge_dictionary(pyproject["tool"]["pdm"], settings)
-        pyproject.setdefault("build-system", DEFAULT_BACKEND.build_system())
+        pyproject["build-system"] = DEFAULT_BACKEND.build_system()
 
         if "requires-python" not in pyproject["project"]:
             python_version = f"{project.python.major}.{project.python.minor}"
             pyproject["project"]["requires-python"] = f">={python_version}"
             project.core.ui.echo(
                 "The project's [primary]requires-python[/] has been set to [primary]>="
                 f"{python_version}[/]. You can change it later if necessary."
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/info.py` & `pdm-2.8.1/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/init.py` & `pdm-2.8.1/src/pdm/cli/commands/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import argparse
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, cast
 
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option
 from pdm.cli.templates import ProjectTemplate
@@ -141,15 +141,15 @@
             },
         }
 
         if python_requires and python_requires != "*":
             get_specifier(python_requires)
             data["project"]["requires-python"] = python_requires
         if build_backend is not None:
-            data["build-system"] = build_backend.build_system()
+            data["build-system"] = cast(dict, build_backend.build_system())
 
         return data
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         skip_option.add_to_parser(parser)
 
         status = {
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/install.py` & `pdm-2.8.1/src/pdm/cli/commands/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from pdm.cli.options import dry_run_option, groups_group, install_group, lockfile_option, skip_option, venv_option
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Install dependencies from lock file"""
 
-    arguments = [
+    arguments = (
         *BaseCommand.arguments,
         groups_group,
         install_group,
         dry_run_option,
         lockfile_option,
         skip_option,
         venv_option,
-    ]
+    )
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--no-lock",
             dest="lock",
             action="store_false",
             default=True,
@@ -77,17 +77,23 @@
                 project.core.ui.echo(
                     "Please run [success]`pdm lock`[/] to update the lock file",
                     err=True,
                 )
                 sys.exit(1)
             if options.lock:
                 project.core.ui.echo("Updating the lock file...", style="success", err=True)
-
+                unseleted = GroupSelection(project)
                 actions.do_lock(
-                    project, strategy=strategy, dry_run=options.dry_run, hooks=hooks, groups=selection.all()
+                    project,
+                    strategy=strategy,
+                    dry_run=options.dry_run,
+                    hooks=hooks,
+                    # We would like to keep the selected groups when the lockfile exists
+                    # but use the groups passed-in when creating a new lockfile.
+                    groups=unseleted.all() if strategy != "all" else selection.all(),
                 )
 
         actions.do_sync(
             project,
             selection=selection,
             no_editable=options.no_editable,
             no_self=options.no_self,
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/list.py` & `pdm-2.8.1/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/lock.py` & `pdm-2.8.1/src/pdm/cli/commands/lock.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Resolve and lock dependencies"""
 
-    arguments = [*BaseCommand.arguments, lockfile_option, no_isolation_option, skip_option, groups_group]
+    arguments = (*BaseCommand.arguments, lockfile_option, no_isolation_option, skip_option, groups_group)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--refresh",
             action="store_true",
             help="Don't update pinned versions, only refresh the lock file",
         )
@@ -35,14 +35,24 @@
         parser.add_argument(
             "--no-cross-platform",
             action="store_false",
             default=True,
             dest="cross_platform",
             help="Only lock packages for the current platform",
         )
+        group = parser.add_mutually_exclusive_group()
+        group.add_argument(
+            "--static-urls", action="store_true", help="Store static file URLs in the lockfile", default=None
+        )
+        group.add_argument(
+            "--no-static-urls",
+            action="store_false",
+            dest="static_urls",
+            help="Do not store static file URLs in the lockfile",
+        )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.check:
             strategy = actions.check_lockfile(project, False)
             if strategy:
                 project.core.ui.echo(
                     f"[error]{termui.Emoji.FAIL}[/] Lockfile is [error]out of date[/].",
@@ -59,9 +69,10 @@
                 sys.exit(0)
         selection = GroupSelection.from_options(project, options)
         actions.do_lock(
             project,
             refresh=options.refresh,
             groups=selection.all(),
             cross_platform=options.cross_platform,
+            static_urls=options.static_urls,
             hooks=HookManager(project, options.skip),
         )
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.8.1/src/pdm/cli/commands/publish/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Build and publish the project to PyPI"""
 
-    arguments = [verbose_option, project_option, skip_option]
+    arguments = (verbose_option, project_option, skip_option)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-r",
             "--repository",
             help="The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]",
         )
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/publish/package.py` & `pdm-2.8.1/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/publish/repository.py` & `pdm-2.8.1/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/remove.py` & `pdm-2.8.1/src/pdm/cli/commands/remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Remove packages from pyproject.toml"""
 
-    arguments = [*BaseCommand.arguments, install_group, dry_run_option, lockfile_option, skip_option, venv_option]
+    arguments = (*BaseCommand.arguments, install_group, dry_run_option, lockfile_option, skip_option, venv_option)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-d",
             "--dev",
             default=False,
             action="store_true",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/run.py` & `pdm-2.8.1/src/pdm/cli/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
             fallback = f"{lines[0]}{termui.Emoji.ELLIPSIS}" if len(lines) > 1 else lines[0]
         return self.options.get("help", fallback)
 
 
 class TaskRunner:
     """The task runner for pdm project"""
 
-    TYPES = ["cmd", "shell", "call", "composite"]
-    OPTIONS = ["env", "env_file", "help", "site_packages"]
+    TYPES = ("cmd", "shell", "call", "composite")
+    OPTIONS = ("env", "env_file", "help", "site_packages")
 
     def __init__(self, project: Project, hooks: HookManager) -> None:
         self.project = project
         global_options = cast(
             "TaskOptions",
             self.project.scripts.get("_", {}) if self.project.scripts else {},
         )
@@ -332,15 +332,15 @@
     return data
 
 
 class Command(BaseCommand):
     """Run commands or scripts with local packages loaded"""
 
     runner_cls: type[TaskRunner] = TaskRunner
-    arguments = [*BaseCommand.arguments, skip_option, venv_option]
+    arguments = (*BaseCommand.arguments, skip_option, venv_option)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         action = parser.add_mutually_exclusive_group()
         action.add_argument(
             "-l",
             "--list",
             action="store_true",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/search.py` & `pdm-2.8.1/src/pdm/cli/commands/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         except UnicodeEncodeError:
             pass
 
 
 class Command(BaseCommand):
     """Search for PyPI packages"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("query", help="Query string to search")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project.environment = BareEnvironment(project)
         result = project.get_repository().search(options.query)
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/self_cmd.py` & `pdm-2.8.1/src/pdm/cli/commands/self_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,28 @@
         text=True,
     )
 
 
 class Command(BaseCommand):
     """Manage the PDM program itself (previously known as plugin)"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     name = "self"
 
     @classmethod
     def register_to(
         cls,
         subparsers: argparse._SubParsersAction,
         name: str | None = None,
         **kwargs: Any,
     ) -> None:
         return super().register_to(subparsers, name, aliases=["plugin"], **kwargs)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        subparsers = parser.add_subparsers(title="commands", metavar="self")
+        subparsers = parser.add_subparsers(title="commands", metavar="")
         ListCommand.register_to(subparsers)
         if not is_in_zipapp():
             AddCommand.register_to(subparsers)
             RemoveCommand.register_to(subparsers)
             UpdateCommand.register_to(subparsers)
         parser.set_defaults(search_parent=False)
         self.parser = parser
@@ -77,15 +77,15 @@
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         self.parser.print_help()
 
 
 class ListCommand(BaseCommand):
     """List all packages installed with PDM"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     name = "list"
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("--plugins", action="store_true", help="List plugins only")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         distributions = list_distributions(plugin_only=options.plugins)
@@ -107,15 +107,15 @@
             )
         project.core.ui.display_columns(rows)
 
 
 class AddCommand(BaseCommand):
     """Install packages to the PDM's environment"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     name = "add"
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--pip-args",
             help="Arguments that will be passed to pip install",
             default="",
@@ -139,15 +139,15 @@
         else:
             project.core.ui.echo("[success]Installation succeeds.[/]")
 
 
 class RemoveCommand(BaseCommand):
     """Remove packages from PDM's environment"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     name = "remove"
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--pip-args",
             help="Arguments that will be passed to pip uninstall",
             default="",
@@ -201,15 +201,15 @@
         else:
             project.core.ui.echo("[success]Uninstallation succeeds.[/]")
 
 
 class UpdateCommand(BaseCommand):
     """Update PDM itself"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
     name = "update"
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--head",
             action="store_true",
             help="Update to the latest commit on the main branch",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/show.py` & `pdm-2.8.1/src/pdm/cli/commands/show.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     assert candidate.version
     return not Version(candidate.version).is_prerelease
 
 
 class Command(BaseCommand):
     """Show the package information"""
 
-    metadata_keys = ["name", "version", "summary", "license", "platform", "keywords"]
+    metadata_keys = ("name", "version", "summary", "license", "platform", "keywords")
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         venv_option.add_to_parser(parser)
         parser.add_argument(
             "package",
             type=normalize_name,
             nargs=argparse.OPTIONAL,
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/sync.py` & `pdm-2.8.1/src/pdm/cli/commands/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 )
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Synchronize the current working set with lock file"""
 
-    arguments = [
+    arguments = (
         *BaseCommand.arguments,
         groups_group,
         dry_run_option,
         lockfile_option,
         skip_option,
         clean_group,
         install_group,
         venv_option,
-    ]
+    )
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-r",
             "--reinstall",
             action="store_true",
             help="Force reinstall existing dependencies",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/update.py` & `pdm-2.8.1/src/pdm/cli/commands/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     from pdm.models.requirements import Requirement
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Update package(s) in pyproject.toml"""
 
-    arguments = [
+    arguments = (
         *BaseCommand.arguments,
         groups_group,
         install_group,
         lockfile_option,
         save_strategy_group,
         update_strategy_group,
         prerelease_option,
         unconstrained_option,
         skip_option,
         venv_option,
-    ]
+    )
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-t",
             "--top",
             action="store_true",
             help="Only update those listed in pyproject.toml",
@@ -169,18 +169,19 @@
             )
         hooks.try_emit("post_lock", resolution=resolved, dry_run=dry_run)
         for deps in updated_deps.values():
             populate_requirement_names(deps)
         if unconstrained:
             # Need to update version constraints
             save_version_specifiers(updated_deps, resolved, save)
-            for group, deps in updated_deps.items():
-                project.add_dependencies(deps, group, selection.dev or False)
         if not dry_run:
-            project.write_lockfile(project.lockfile._data, False, groups=locked_groups)
+            if unconstrained:
+                for group, deps in updated_deps.items():
+                    project.add_dependencies(deps, group, selection.dev or False)
+            project.write_lockfile(project.lockfile._data, False)
         if sync or dry_run:
             do_sync(
                 project,
                 selection=selection,
                 clean=False,
                 dry_run=dry_run,
                 requirements=[r for deps in updated_deps.values() for r in deps.values()],
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/use.py` & `pdm-2.8.1/src/pdm/cli/commands/use.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         venv: str | None,
         first: bool,
     ) -> PythonInfo:
         from pdm.cli.commands.venv.utils import get_venv_with_name
 
         def version_matcher(py_version: PythonInfo) -> bool:
             return py_version.valid and (
-                ignore_requires_python or project.python_requires.contains(str(py_version.version), True)
+                ignore_requires_python or project.python_requires.contains(py_version.version, True)
             )
 
         if venv:
             virtualenv = get_venv_with_name(project, venv)
             return PythonInfo.from_path(virtualenv.interpreter)
 
         if not project.cache_dir.exists():
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Virtualenv management"""
 
     name = "venv"
-    arguments = [project_option]
+    arguments = (project_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         group.add_argument("--path", help="Show the path to the given virtualenv")
         group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
-        subparser = parser.add_subparsers(metavar="venv", title="commands")
+        subparser = parser.add_subparsers(title="commands", metavar="")
         CreateCommand.register_to(subparser, "create")
         ListCommand.register_to(subparser, "list")
         RemoveCommand.register_to(subparser, "remove")
         ActivateCommand.register_to(subparser, "activate")
         PurgeCommand.register_to(subparser, "purge")
         self.parser = parser
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/activate.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/activate.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pdm.models.venv import VirtualEnv
 from pdm.project import Project
 
 
 class ActivateCommand(BaseCommand):
     """Activate the virtualenv with the given name"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("env", nargs="?", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.env:
             venv = get_venv_with_name(project, options.env)
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/backends.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/create.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class CreateCommand(BaseCommand):
     """Create a virtualenv
 
     pdm venv create <python> [-other args]
     """
 
     description = "Create a virtualenv"
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-w",
             "--with",
             dest="backend",
             choices=BACKENDS.keys(),
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/list.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pdm.cli.options import verbose_option
 from pdm.project import Project
 
 
 class ListCommand(BaseCommand):
     """List all virtualenvs associated with this project"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project.core.ui.echo("Virtualenvs created with this project:\n")
         for ident, venv in iter_venvs(project):
             saved_python = project._saved_python
             if saved_python and Path(saved_python).parent.parent == venv.root:
                 mark = "*"
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/purge.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/purge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 import shutil
 
-from pdm.project import Project
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.venv.utils import iter_central_venvs
 from pdm.cli.options import verbose_option
+from pdm.project import Project
 
 
 class PurgeCommand(BaseCommand):
     """Purge selected/all created Virtualenvs"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-f",
             "--force",
             action="store_true",
             help="Force purging without prompting for confirmation",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/remove.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/remove.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pdm.cli.options import verbose_option
 from pdm.project import Project
 
 
 class RemoveCommand(BaseCommand):
     """Remove the virtualenv with the given name"""
 
-    arguments = [verbose_option]
+    arguments = (verbose_option,)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-y",
             "--yes",
             action="store_true",
             help="Answer yes on the following question",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/commands/venv/utils.py` & `pdm-2.8.1/src/pdm/cli/commands/venv/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import base64
 import hashlib
+import typing as t
 from pathlib import Path
-from typing import Iterable, TypeVar
 
-from findpython import PythonVersion
-from findpython.providers import BaseProvider
+from findpython import BaseProvider, PythonVersion
 
 from pdm.exceptions import PdmUsageError
 from pdm.models.venv import VirtualEnv
 from pdm.project import Project
 
 
 def hash_path(path: str) -> str:
@@ -30,50 +29,47 @@
 def get_venv_prefix(project: Project) -> str:
     """Get the venv prefix for the project"""
     path = project.root
     name_hash = hash_path(path.as_posix())
     return f"{path.name}-{name_hash}-"
 
 
-def iter_venvs(project: Project) -> Iterable[tuple[str, VirtualEnv]]:
+def iter_venvs(project: Project) -> t.Iterable[tuple[str, VirtualEnv]]:
     """Return an iterable of venv paths associated with the project"""
     in_project_venv = get_in_project_venv(project.root)
     if in_project_venv is not None:
         yield "in-project", in_project_venv
     venv_prefix = get_venv_prefix(project)
     venv_parent = Path(project.config["venv.location"])
     for path in venv_parent.glob(f"{venv_prefix}*"):
         ident = path.name[len(venv_prefix) :]
         venv = VirtualEnv.get(path)
         if venv is not None:
             yield ident, venv
 
 
-def iter_central_venvs(project: Project) -> Iterable[tuple[str, Path]]:
+def iter_central_venvs(project: Project) -> t.Iterable[tuple[str, Path]]:
     """Return an iterable of all managed venvs and their paths."""
     venv_parent = Path(project.config["venv.location"])
     for venv in venv_parent.glob("*"):
         ident = venv.name
         yield ident, venv
 
 
-T = TypeVar("T", bound=BaseProvider)
-
-
 class VenvProvider(BaseProvider):
     """A Python provider for project venv pythons"""
 
     def __init__(self, project: Project) -> None:
         self.project = project
 
     @classmethod
-    def create(cls: type[T]) -> T | None:  # pragma: no cover
+    def create(cls) -> t.Self | None:
         return None
 
-    def find_pythons(self) -> Iterable[PythonVersion]:
+    def find_pythons(self) -> t.Iterable[PythonVersion]:
         for _, venv in iter_venvs(self.project):
             yield PythonVersion(venv.interpreter, _interpreter=venv.interpreter, keep_symlink=True)
 
 
 def get_venv_with_name(project: Project, name: str) -> VirtualEnv:
     all_venvs = dict(iter_venvs(project))
     try:
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/completions/pdm.bash` & `pdm-2.8.1/src/pdm/cli/completions/pdm.bash`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             ;;
 
             (list)
             opts="--csv --exclude --fields --freeze --global --graph --help --include --json --markdown --project --resolve --reverse --sort --venv --verbose"
             ;;
 
             (lock)
-            opts="--check --dev --global --group --help --lockfile --no-cross-platform --no-default --no-isolation --production --project --refresh --skip --verbose"
+            opts="--check --dev --global --group --help --lockfile --no-cross-platform --no-default --no-isolation --no-static-urls --production --project --refresh --skip --static-urls --verbose"
             ;;
 
             (plugin)
             opts="--help --verbose"
             ;;
 
             (publish)
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/completions/pdm.fish` & `pdm-2.8.1/src/pdm/cli/completions/pdm.fish`

 * *Files 0% similar despite different names*

```diff
@@ -210,18 +210,20 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-cross-platform -d 'Only lock packages for the current platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-isolation -d 'Do not isolate the build in a clean environment'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-static-urls -d 'Do not store static file URLs in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l refresh -d 'Don\'t update pinned versions, only refresh the lock file'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l static-urls -d 'Store static file URLs in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # plugin
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a plugin -d 'Manage the PDM program itself (previously known as plugin)'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 # plugin subcommands
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/completions/pdm.ps1` & `pdm-2.8.1/src/pdm/cli/completions/pdm.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
                         $projectOption
                     ))
                 break
             }
             "lock" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("--global", "-g", "--no-isolation", "--refresh", "-L", "--lockfile", "--check", "--dev", "--prod", "--production", "-d", "--no-default", "--no-cross-platform")),
+                        [Option]::new(@("--global", "-g", "--no-isolation", "--refresh", "-L", "--lockfile", "--check", "--dev", "--prod", "--production", "-d", "--no-default", "--no-cross-platform", "--static-urls", "--no-static-urls")),
                         $skipOption,
                         $sectionOption,
                         $projectOption
                     ))
                 break
             }
             "self" {
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/completions/pdm.zsh` & `pdm-2.8.1/src/pdm/cli/completions/pdm.zsh`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,16 @@
         "--no-isolation[Do not isolate the build in a clean environment]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         "--refresh[Don't update pinned versions, only refresh the lock file]"
         "--check[Check if the lock file is up to date and quit]"
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-d,--dev}"[Select dev dependencies]"
         {--prod,--production}"[Unselect dev dependencies]"
+        "--static-urls[Store static file URLs in the lockfile]"
+        "--no-static-urls[Do not store static file URLs in the lockfile]"
         "--no-default[Don\'t include dependencies from the default group]"
         "--no-cross-platform[Only lock packages for the current platform]"
       )
       ;;
     self)
       _arguments -C \
         $arguments \
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/filters.py` & `pdm-2.8.1/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/hooks.py` & `pdm-2.8.1/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/options.py` & `pdm-2.8.1/src/pdm/cli/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,17 @@
     help="Update all dependencies and sub-dependencies",
 )
 
 project_option = Option(
     "-p",
     "--project",
     dest="project_path",
-    help="Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__",
+    help="Specify another path as the project root, which changes the base of pyproject.toml "
+    "and __pypackages__ [env var: PDM_PROJECT]",
+    default=os.getenv("PDM_PROJECT"),
 )
 
 
 global_option = Option(
     "-g",
     "--global",
     dest="global_project",
```

### Comparing `pdm-2.8.0a2/src/pdm/cli/templates/__init__.py` & `pdm-2.8.1/src/pdm/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/templates/default/.gitignore` & `pdm-2.8.1/src/pdm/cli/templates/default/.gitignore`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/cli/utils.py` & `pdm-2.8.1/src/pdm/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import argparse
 import dataclasses as dc
 import json
 import os
+import re
 import sys
 from collections import ChainMap, OrderedDict
 from concurrent.futures import ThreadPoolExecutor
 from json import dumps
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
@@ -63,15 +64,17 @@
         usage: str | None,
         actions: Iterable[Action],
         groups: Iterable[_ArgumentGroup],
         prefix: str | None,
     ) -> str:
         if prefix is None:
             prefix = "Usage: "
-        result = super()._format_usage(usage, actions, groups, prefix)
+        result = super()._format_usage(usage, actions, groups, prefix)  # type: ignore[arg-type]
+        # Remove continuous spaces
+        result = re.sub(r" +", " ", result)
         if prefix:
             return result.replace(prefix, termui.style(prefix, style="warning"))
         return result
 
     def _format_action(self, action: Action) -> str:
         # determine the required width and the entry label
         help_position = min(self._action_max_length + 2, self._max_help_position)
@@ -92,32 +95,47 @@
 
         # long action name; start on the next line
         else:
             tup = self._current_indent, "", action_header
             action_header = "%*s%s\n" % tup
             indent_first = help_position
 
+        # Special format for empty action_header
+        # - No extra indent block
+        # - Help info in the same indent level as subactions
+        if not action_header.strip():
+            action_header = ""
+            help_position = self._current_indent
+            indent_first = self._current_indent
+
         # collect the pieces of the action help
         parts = [termui.style(action_header, style="primary")]
 
         # if there was help for the action, add lines of help text
         if action.help:
             help_text = self._expand_help(action)
             help_lines = self._split_lines(help_text, help_width)
             parts.append("%*s%s\n" % (indent_first, "", help_lines[0]))
             for line in help_lines[1:]:
                 parts.append("%*s%s\n" % (help_position, "", line))
 
         # or add a newline if the description doesn't end with one
         elif not action_header.endswith("\n"):
-            parts.append("\n")
+            if action_header:
+                parts.append("\n")
 
+        # cancel out extra indent when action_header is empty
+        if not action_header:
+            self._dedent()
         # if there are any sub-actions, add their help as well
         for subaction in self._iter_indented_subactions(action):
             parts.append(self._format_action(subaction))
+        # cancel out extra dedent when action_header is empty
+        if not action_header:
+            self._indent()
 
         # return a single string
         return self._join_parts(parts)
 
 
 class ArgumentParser(argparse.ArgumentParser):
     """A standard argument parser but with title-cased help."""
@@ -125,14 +143,15 @@
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["formatter_class"] = PdmFormatter
         kwargs["add_help"] = False
         super().__init__(*args, **kwargs)
         self.add_argument(
             "-h", "--help", action="help", default=argparse.SUPPRESS, help="Show this help message and exit."
         )
+        self._optionals.title = "options"
 
 
 class ErrorArgumentParser(ArgumentParser):
     """A subclass of argparse.ArgumentParser that raises
     parsing error rather than exiting.
 
     This does the same as passing exit_on_error=False on Python 3.9+
@@ -429,45 +448,57 @@
     echo(tree)
 
 
 def format_lockfile(
     project: Project,
     mapping: dict[str, Candidate],
     fetched_dependencies: dict[tuple[str, str | None], list[Requirement]],
+    groups: list[str] | None = None,
+    cross_platform: bool | None = None,
+    static_urls: bool | None = None,
 ) -> dict:
     """Format lock file from a dict of resolved candidates, a mapping of dependencies
     and a collection of package summaries.
     """
     from pdm.formats.base import make_array, make_inline_table
 
     packages = tomlkit.aot()
-    file_hashes = tomlkit.table()
-    for k, v in sorted(mapping.items()):
+    for _k, v in sorted(mapping.items()):
         base = tomlkit.table()
         base.update(v.as_lockfile_entry(project.root))
         base.add("summary", v.summary or "")
         deps = make_array(sorted(r.as_line() for r in fetched_dependencies[v.dep_key]), True)
         if len(deps) > 0:
             base.add("dependencies", deps)
-        packages.append(base)
         if v.hashes:
-            key = f"{strip_extras(k)[0]} {v.version}"
-            if key in file_hashes:
-                continue
-            array = tomlkit.array().multiline(True)
-            for link, hash_value in sorted(v.hashes.items(), key=lambda l_h: (l_h[0].url_without_fragment, l_h[1])):
-                inline = make_inline_table({"url": link.url_without_fragment, "hash": hash_value})
-                array.append(inline)
-            if array:
-                file_hashes.add(key, array)
+            collected = {}
+            for item in v.hashes:
+                if static_urls:
+                    row = {"url": item["url"], "hash": item["hash"]}
+                else:
+                    row = {"file": item["file"], "hash": item["hash"]}
+                inline = make_inline_table(row)
+                # deduplicate and sort
+                collected[tuple(row.values())] = inline
+            if collected:
+                base.add("files", make_array([collected[k] for k in sorted(collected)], True))
+        packages.append(base)
     doc = tomlkit.document()
-    doc.add("package", packages)
     metadata = tomlkit.table()
-    metadata.add("files", file_hashes)
+    if groups is None:
+        groups = list(project.iter_groups())
+    metadata.update(
+        {
+            "groups": sorted(groups, key=lambda k: k != "default"),
+            "cross_platform": cross_platform if cross_platform is not None else project.lockfile.cross_platform,
+            "static_urls": static_urls if static_urls is not None else project.lockfile.static_urls,
+        }
+    )
     doc.add("metadata", metadata)
+    doc.add("package", packages)
     return cast(dict, doc)
 
 
 def save_version_specifiers(
     requirements: dict[str, dict[str, Requirement]],
     resolved: dict[str, Candidate],
     save_strategy: str,
```

### Comparing `pdm-2.8.0a2/src/pdm/compat.py` & `pdm-2.8.1/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/core.py` & `pdm-2.8.1/src/pdm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,20 +74,19 @@
             help="Show the version and exit",
         )
         self.parser.add_argument(
             "-c",
             "--config",
             help="Specify another config file path [env var: PDM_CONFIG_FILE] ",
         )
-        self.parser._positionals.title = "Commands"
         verbose_option.add_to_parser(self.parser)
         ignore_python_option.add_to_parser(self.parser)
         pep582_option.add_to_parser(self.parser)
 
-        self.subparsers = self.parser.add_subparsers(parser_class=ArgumentParser, metavar="__root__")
+        self.subparsers = self.parser.add_subparsers(parser_class=ArgumentParser, title="commands", metavar="")
         for _, name, _ in pkgutil.iter_modules(COMMANDS_MODULE_PATH):
             module = importlib.import_module(f"pdm.cli.commands.{name}", __name__)
             try:
                 klass = module.Command
             except AttributeError:
                 continue
             self.register_command(klass, klass.name or name)
@@ -149,15 +148,16 @@
         if getattr(options, "lockfile", None):
             project.set_lockfile(cast(str, options.lockfile))
 
         if getattr(options, "use_venv", None):
             use_venv(project, cast(str, options.use_venv))
 
         if command is None:
-            self.parser.error("No command given")
+            self.parser.print_help()
+            sys.exit(0)
         command.handle(project, options)
 
     def _get_cli_args(self, args: list[str], obj: Project | None) -> list[str]:
         project = self.create_project(is_global=False) if obj is None else obj
         if project.is_global:
             return args
         config = project.pyproject.settings.get("options", {})
@@ -172,16 +172,17 @@
         args: list[str] | None = None,
         prog_name: str | None = None,
         obj: Project | None = None,
         **extra: Any,
     ) -> None:
         """The main entry function"""
 
-        # Ensure same behavior while testing and using the CLI
-        args = self._get_cli_args(args or sys.argv[1:], obj)
+        if args is None:
+            args = []
+        args = self._get_cli_args(args, obj)
         # Keep it for after project parsing to check if its a defined script
         root_script = None
         try:
             options = self.parser.parse_args(args)
         except PdmArgumentError as e:
             # Failed to parse, try to give all to `run` command as shortcut
             # and keep to root script (first non-dashed param) to check existence
@@ -282,8 +283,8 @@
                     style="error",
                     err=True,
                 )
 
 
 def main(args: list[str] | None = None) -> None:
     """The CLI entry function"""
-    return Core().main(args)
+    return Core().main(args or sys.argv[1:])
```

### Comparing `pdm-2.8.0a2/src/pdm/environments/__init__.py` & `pdm-2.8.1/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/environments/base.py` & `pdm-2.8.1/src/pdm/environments/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Generator
 
 from pdm.compat import cached_property
 from pdm.exceptions import BuildError, PdmUsageError
-from pdm.models.in_process import get_pep508_environment, get_python_abi_tag
+from pdm.models.in_process import get_pep508_environment, get_python_abi_tag, get_uname
 from pdm.models.python import PythonInfo
 from pdm.models.working_set import WorkingSet
 from pdm.utils import get_trusted_hosts, is_pip_compatible_with_python
 
 if TYPE_CHECKING:
     import unearth
 
@@ -90,14 +90,36 @@
             keyfn = self.project.config.get("pypi.client_key")
             session.cert = (Path(certfn), Path(keyfn) if keyfn else None)
 
         session.auth = self.auth
         return session
 
     @contextmanager
+    def _patch_target_python(self) -> Generator[None, None, None]:
+        """Patch the packaging modules to respect the arch of target python."""
+        import packaging.tags
+
+        old_32bit = packaging.tags._32_BIT_INTERPRETER
+        old_os_uname = getattr(os, "uname", None)
+
+        if old_os_uname is not None:
+
+            def uname() -> os.uname_result:
+                return get_uname(str(self.interpreter.executable))
+
+            os.uname = uname
+        packaging.tags._32_BIT_INTERPRETER = self.interpreter.is_32bit
+        try:
+            yield
+        finally:
+            packaging.tags._32_BIT_INTERPRETER = old_32bit
+            if old_os_uname is not None:
+                os.uname = old_os_uname
+
+    @contextmanager
     def get_finder(
         self,
         sources: list[RepositoryConfig] | None = None,
         ignore_compatibility: bool = False,
     ) -> Generator[unearth.PackageFinder, None, None]:
         """Return the package finder of given index sources.
 
@@ -115,36 +137,37 @@
                 "The 'pypi.ignore_stored_index' config value is "
                 f"{self.project.config['pypi.ignore_stored_index']}"
             )
 
         trusted_hosts = get_trusted_hosts(sources)
 
         session = self._build_session(trusted_hosts)
-        finder = PackageFinder(
-            session=session,
-            target_python=self.target_python,
-            ignore_compatibility=ignore_compatibility,
-            no_binary=os.getenv("PDM_NO_BINARY", "").split(","),
-            only_binary=os.getenv("PDM_ONLY_BINARY", "").split(","),
-            prefer_binary=os.getenv("PDM_PREFER_BINARY", "").split(","),
-            respect_source_order=self.project.pyproject.settings.get("resolution", {}).get(
-                "respect-source-order", False
-            ),
-            verbosity=self.project.core.ui.verbosity,
-        )
-        for source in sources:
-            assert source.url
-            if source.type == "find_links":
-                finder.add_find_links(source.url)
-            else:
-                finder.add_index_url(source.url)
-        try:
-            yield finder
-        finally:
-            session.close()
+        with self._patch_target_python():
+            finder = PackageFinder(
+                session=session,
+                target_python=self.target_python,
+                ignore_compatibility=ignore_compatibility,
+                no_binary=os.getenv("PDM_NO_BINARY", "").split(","),
+                only_binary=os.getenv("PDM_ONLY_BINARY", "").split(","),
+                prefer_binary=os.getenv("PDM_PREFER_BINARY", "").split(","),
+                respect_source_order=self.project.pyproject.settings.get("resolution", {}).get(
+                    "respect-source-order", False
+                ),
+                verbosity=self.project.core.ui.verbosity,
+            )
+            for source in sources:
+                assert source.url
+                if source.type == "find_links":
+                    finder.add_find_links(source.url)
+                else:
+                    finder.add_index_url(source.url)
+            try:
+                yield finder
+            finally:
+                session.close()
 
     def get_working_set(self) -> WorkingSet:
         """Get the working set based on local packages directory."""
         paths = self.get_paths()
         return WorkingSet([paths["platlib"], paths["purelib"]])
 
     @cached_property
```

### Comparing `pdm-2.8.0a2/src/pdm/environments/local.py` & `pdm-2.8.1/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/environments/python.py` & `pdm-2.8.1/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/exceptions.py` & `pdm-2.8.1/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/__init__.py` & `pdm-2.8.1/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/base.py` & `pdm-2.8.1/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/flit.py` & `pdm-2.8.1/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/pipfile.py` & `pdm-2.8.1/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/poetry.py` & `pdm-2.8.1/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/formats/requirements.py` & `pdm-2.8.1/src/pdm/formats/requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         if isinstance(candidate, Candidate):
             req = dataclasses.replace(candidate.req, specifier=f"=={candidate.version}", marker=None)
         else:
             assert isinstance(candidate, Requirement)
             req = candidate
         lines.append(project.backend.expand_line(req.as_line(), options.expandvars))
         if options.hashes and getattr(candidate, "hashes", None):
-            for item in sorted(set(candidate.hashes.values())):  # type: ignore[attr-defined]
+            for item in sorted({row["hash"] for row in candidate.hashes}):  # type: ignore[attr-defined]
                 lines.append(f" \\\n    --hash={item}")
         lines.append("\n")
     sources = project.pyproject.settings.get("source", [])
     for source in sources:
         url = source["url"]
         if options.expandvars:
             url = expand_env_vars_in_auth(url)
```

### Comparing `pdm-2.8.0a2/src/pdm/formats/setup_py.py` & `pdm-2.8.1/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/installers/core.py` & `pdm-2.8.1/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/installers/installers.py` & `pdm-2.8.1/src/pdm/installers/installers.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,31 +40,36 @@
             or child.is_dir()
             and _is_python_package(child)
         ):
             return True
     return False
 
 
+_namespace_package_lines = frozenset(
+    [
+        # pkg_resources style
+        "__import__('pkg_resources').declare_namespace(__name__)",
+        "pkg_resources.declare_namespace(__name__)",
+        # pkgutil style
+        "__path__ = __import__('pkgutil').extend_path(__path__, __name__)",
+        "__path__ = pkgutil.extend_path(__path__, __name__)",
+    ]
+)
+_namespace_package_lines = _namespace_package_lines.union(line.replace("'", '"') for line in _namespace_package_lines)
+
+
 @lru_cache()
 def _is_namespace_package(root: str) -> bool:
     if not _is_python_package(root):
         return False
     if not os.path.exists(os.path.join(root, "__init__.py")):  # PEP 420 style
         return True
     with Path(root, "__init__.py").open(encoding="utf-8") as f:
         init_py_lines = [line.strip() for line in f if line.strip() and not line.strip().startswith("#")]
-    namespace_identifiers = [
-        # pkg_resources style
-        "__import__('pkg_resources').declare_namespace(__name__)",
-        # pkgutil style
-        "__path__ = __import__('pkgutil').extend_path(__path__, __name__)",
-    ]
-    checker = namespace_identifiers[:]
-    checker.extend(item.replace("'", '"') for item in namespace_identifiers)
-    return any(line in checker for line in init_py_lines)
+    return not _namespace_package_lines.isdisjoint(init_py_lines)
 
 
 def _create_symlinks_recursively(source: str, destination: str) -> Iterable[str]:
     """Create symlinks recursively from source to destination.
     Caveats: This don't work for pkgutil or pkg_resources namespace packages.
     package  <-- link
         __init__.py
@@ -144,19 +149,19 @@
         self,
         scheme: Scheme,
         record_file_path: str | Path,
         records: Iterable[tuple[Scheme, RecordEntry]],
     ) -> None:
         if self.symlink_to:
             # Create symlinks to the cached location
-            for relpath in _create_symlinks_recursively(self.symlink_to, self.scheme_dict[scheme]):
-                records = itertools.chain(
-                    records,
-                    [(scheme, RecordEntry(relpath.replace("\\", "/"), None, None))],
-                )
+            def _symlink_files(symlink_to: str) -> Iterator[tuple[Scheme, RecordEntry]]:
+                for relpath in _create_symlinks_recursively(symlink_to, self.scheme_dict[scheme]):
+                    yield (scheme, RecordEntry(relpath.replace("\\", "/"), None, None))
+
+            records = itertools.chain(records, _symlink_files(self.symlink_to))
         return super().finalize_installation(scheme, record_file_path, records)
 
 
 def install_wheel(wheel: str, environment: BaseEnvironment, direct_url: dict[str, Any] | None = None) -> None:
     """Install a normal wheel file into the environment."""
     additional_metadata = None
     if direct_url is not None:
```

### Comparing `pdm-2.8.0a2/src/pdm/installers/manager.py` & `pdm-2.8.1/src/pdm/installers/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from pdm.models.candidates import Candidate
 
 
 class InstallManager:
     """The manager that performs the installation and uninstallation actions."""
 
     # The packages below are needed to load paths and thus should not be cached.
-    NO_CACHE_PACKAGES = ["editables"]
+    NO_CACHE_PACKAGES = ("editables",)
 
     def __init__(self, environment: BaseEnvironment, *, use_install_cache: bool = False) -> None:
         self.environment = environment
         self.use_install_cache = use_install_cache
 
     def install(self, candidate: Candidate) -> None:
         if self.use_install_cache and candidate.req.is_named and candidate.name not in self.NO_CACHE_PACKAGES:
```

### Comparing `pdm-2.8.0a2/src/pdm/installers/packages.py` & `pdm-2.8.1/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/installers/synchronizers.py` & `pdm-2.8.1/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/installers/uninstallers.py` & `pdm-2.8.1/src/pdm/installers/uninstallers.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,17 @@
                 location = dist.locate_file(file)
                 instance.add_path(str(location))
                 bare_name, ext = os.path.splitext(location)
                 if ext == ".py":
                     # .pyc files are added by add_path()
                     instance.add_path(bare_name + ".pyo")
 
+            # installed-files.txt isn't recorded in SOURCES.txt for egg-info
+            instance.add_path(os.path.join(meta_location, "installed-files.txt"))
+
         bin_dir = scheme["scripts"]
 
         if os.path.isdir(os.path.join(meta_location, "scripts")):  # pragma: no cover
             for script in os.listdir(os.path.join(meta_location, "scripts")):
                 instance.add_path(os.path.join(bin_dir, script))
                 if os.name == "nt":
                     instance.add_path(os.path.join(bin_dir, script) + ".bat")
```

### Comparing `pdm-2.8.0a2/src/pdm/models/auth.py` & `pdm-2.8.1/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/backends.py` & `pdm-2.8.1/src/pdm/models/backends.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from __future__ import annotations
 
 import abc
 import os
 import urllib.parse
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from pdm.utils import expand_env_vars, path_to_url
 
+if TYPE_CHECKING:
+    from typing import TypedDict
+
+    BuildSystem = TypedDict("BuildSystem", {"requires": list[str], "build-backend": str})
+
 
 class BuildBackend(metaclass=abc.ABCMeta):
     """A build backend that does not support dynamic values in dependencies"""
 
     def __init__(self, root: Path) -> None:
         self.root = root
 
@@ -18,30 +24,30 @@
         return line
 
     def relative_path_to_url(self, path: str) -> str:
         return path_to_url(os.path.join(self.root, path))
 
     @classmethod
     @abc.abstractmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         pass
 
 
 class FlitBackend(BuildBackend):
     @classmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         return {
             "requires": ["flit_core>=3.2,<4"],
             "build-backend": "flit_core.buildapi",
         }
 
 
 class SetuptoolsBackend(BuildBackend):
     @classmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         return {
             "requires": ["setuptools>=61", "wheel"],
             "build-backend": "setuptools.build_meta",
         }
 
 
 class PDMBackend(BuildBackend):
@@ -53,24 +59,24 @@
 
     def relative_path_to_url(self, path: str) -> str:
         if os.path.isabs(path):
             return path_to_url(path)
         return f"file:///${{PROJECT_ROOT}}/{urllib.parse.quote(path)}"
 
     @classmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         return {
             "requires": ["pdm-backend"],
             "build-backend": "pdm.backend",
         }
 
 
 class PDMLegacyBackend(PDMBackend):
     @classmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         return {
             "requires": ["pdm-pep517>=1.0"],
             "build-backend": "pdm.pep517.api",
         }
 
 
 # Context formatting helpers for hatch
@@ -113,15 +119,15 @@
 
     def relative_path_to_url(self, path: str) -> str:
         if os.path.isabs(path):
             return path_to_url(path)
         return f"{{root:uri}}/{urllib.parse.quote(path)}"
 
     @classmethod
-    def build_system(cls) -> dict:
+    def build_system(cls) -> BuildSystem:
         return {
             "requires": ["hatchling"],
             "build-backend": "hatchling.build",
         }
 
 
 _BACKENDS: dict[str, type[BuildBackend]] = {
```

### Comparing `pdm-2.8.0a2/src/pdm/models/caches.py` & `pdm-2.8.1/src/pdm/models/caches.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     Hashes are only cached when the URL appears to contain a hash in it and the
     cache key includes the hash value returned from the server). This ought to
     avoid issues where the location on the server changes.
     """
 
     FAVORITE_HASH = "sha256"
-    STRONG_HASHES = ["sha256", "sha384", "sha512"]
+    STRONG_HASHES = ("sha256", "sha384", "sha512")
 
     def __init__(self, directory: Path) -> None:
         self.directory = directory
 
     def _read_from_link(self, link: Link, session: Session) -> Iterable[bytes]:
         if link.is_file:
             with open(link.file_path, "rb") as f:
```

### Comparing `pdm-2.8.0a2/src/pdm/models/candidates.py` & `pdm-2.8.1/src/pdm/models/candidates.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hashlib
 import os
 import re
 import warnings
 from functools import lru_cache
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Any, Iterable, cast, no_type_check
+from typing import TYPE_CHECKING, Any, cast, no_type_check
 from zipfile import ZipFile
 
 from packaging.utils import parse_wheel_filename
 
 from pdm import termui
 from pdm.builders import EditableBuilder, WheelBuilder
 from pdm.compat import cached_property
@@ -37,14 +37,15 @@
     path_to_url,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
     from unearth import Link, Package, PackageFinder
 
+    from pdm._types import FileHash
     from pdm.environments import BaseEnvironment
 
 
 def _dist_info_files(whl_zip: ZipFile) -> list[str]:
     """Identify the .dist-info folder inside a wheel ZipFile."""
     res = []
     for path in whl_zip.namelist():
@@ -71,26 +72,29 @@
     """Return a new dict without None values"""
     return {k: v for k, v in data.items() if v is not None}
 
 
 def _find_best_match_link(
     finder: PackageFinder,
     req: Requirement,
-    links: Iterable[Link] | None = None,
+    files: list[FileHash],
     ignore_compatibility: bool = False,
 ) -> Link | None:
     """Get the best matching link for a requirement"""
 
     # This function is called when a lock file candidate is given or incompatible wheel
     # In this case, the requirement must be pinned, so no need to pass allow_prereleases
     # If links are not empty, find the best match from the links, otherwise find from
     # the package sources.
+    links = [Link(f["url"]) for f in files if "url" in f]
+    hashes = convert_hashes(files)
+
     def attempt_to_find() -> Link | None:
-        if links is None:
-            best = finder.find_best_match(req.as_line()).best
+        if not links:
+            best = finder.find_best_match(req.as_line(), hashes=hashes).best
         else:
             # this branch won't be executed twice if ignore_compatibility is True
             evaluator = finder.build_evaluator(req.name)
             packages = finder._evaluate_links(links, evaluator)
             best = max(packages, key=finder._sort_key, default=None)
         return best.link if best is not None else None
 
@@ -156,15 +160,15 @@
         self.req = req
         self.name = name or self.req.project_name
         self.version = version
         if link is None and not req.is_named:
             link = cast("Link", req.as_file_link())  # type: ignore[attr-defined]
         self.link = link
         self.summary = ""
-        self.hashes: dict[Link, str] | None = None
+        self.hashes: list[FileHash] = []
 
         self._requires_python: str | None = None
         self._prepared: PreparedCandidate | None = None
 
     def identify(self) -> str:
         return self.req.identify()
```

### Comparing `pdm-2.8.0a2/src/pdm/models/in_process/__init__.py` & `pdm-2.8.1/src/pdm/models/in_process/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with resources_path(__name__, name) as script:
         yield str(script)
 
 
 @functools.lru_cache()
 def get_python_abi_tag(executable: str) -> str:
     with _in_process_script("get_abi_tag.py") as script:
-        return json.loads(subprocess.check_output(args=[executable, "-Es", script]))
+        return json.loads(subprocess.check_output(args=[executable, "-EsS", script]))
 
 
 def get_sys_config_paths(executable: str, vars: dict[str, str] | None = None, kind: str = "default") -> dict[str, str]:
     """Return the sys_config.get_paths() result for the python interpreter"""
     env = os.environ.copy()
     env.pop("__PYVENV_LAUNCHER__", None)
     if vars is not None:
@@ -37,19 +37,26 @@
         cmd = [executable, "-Es", script, kind]
         return json.loads(subprocess.check_output(cmd, env=env))
 
 
 def get_pep508_environment(executable: str) -> dict[str, str]:
     """Get PEP 508 environment markers dict."""
     with _in_process_script("pep508.py") as script:
-        args = [executable, "-Es", script]
+        args = [executable, "-EsS", script]
         return json.loads(subprocess.check_output(args))
 
 
 def parse_setup_py(executable: str, path: str) -> dict[str, Any]:
     """Parse setup.py and return the kwargs"""
     with _in_process_script("parse_setup.py") as script:
         _, outfile = tempfile.mkstemp(suffix=".json")
         cmd = [executable, "-Es", script, path, outfile]
         subprocess.check_call(cmd)
         with open(outfile, "rb") as fp:
             return json.load(fp)
+
+
+@functools.lru_cache()
+def get_uname(executable: str) -> os.uname_result:
+    """Get uname of the system"""
+    script = "import os, json; print(json.dumps(os.uname()))"
+    return os.uname_result(json.loads(subprocess.check_output([executable, "-EsSc", script])))
```

### Comparing `pdm-2.8.0a2/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.8.1/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/in_process/parse_setup.py` & `pdm-2.8.1/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/in_process/pep508.py` & `pdm-2.8.1/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.8.1/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/markers.py` & `pdm-2.8.1/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/project_info.py` & `pdm-2.8.1/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/python.py` & `pdm-2.8.1/src/pdm/models/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,29 +44,29 @@
     def path(self) -> Path:
         return self._py_ver.executable
 
     @property
     def executable(self) -> Path:
         return self._py_ver.interpreter
 
-    @property
+    @cached_property
     def version(self) -> Version:
         return self._py_ver.version
 
     @property
     def major(self) -> int:
-        return self._py_ver.major
+        return self.version.major
 
     @property
     def minor(self) -> int:
-        return self._py_ver.minor
+        return self.version.minor
 
     @property
     def micro(self) -> int:
-        return self._py_ver.patch
+        return self.version.micro
 
     @property
     def version_tuple(self) -> tuple[int, ...]:
         return (self.major, self.minor, self.micro)
 
     @property
     def is_32bit(self) -> bool:
```

### Comparing `pdm-2.8.0a2/src/pdm/models/repositories.py` & `pdm-2.8.1/src/pdm/models/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Iterable, Mapping
 
     from unearth import Link
 
-    from pdm._types import CandidateInfo, RepositoryConfig, SearchResult
+    from pdm._types import CandidateInfo, FileHash, RepositoryConfig, SearchResult
     from pdm.environments import BaseEnvironment
 
     CandidateKey = tuple[str, str | None, str | None, bool]
 
 ALLOW_ALL_PYTHON = PySpecSet()
 T = TypeVar("T", bound="BaseRepository")
 
@@ -239,52 +239,94 @@
 
         return (
             reqs,
             str(self.environment.python_requires),
             project.pyproject.metadata.get("description", "UNKNOWN"),
         )
 
-    def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
+    def _is_python_match(self, link: Link) -> bool:
+        from packaging.tags import Tag
+        from packaging.utils import parse_wheel_filename
+
+        def is_tag_match(tag: Tag, python_requires: PySpecSet) -> bool:
+            if tag.interpreter.startswith(("cp", "py")):
+                major, minor = tag.interpreter[2], tag.interpreter[3:]
+                if not minor:
+                    version = f"{major}.0"
+                else:
+                    version = f"{major}.{minor}.0"
+                if tag.abi == "abi3":
+                    spec = PySpecSet(f">={version}")  # cp37-abi3 is compatible with >=3.7
+                else:
+                    spec = PySpecSet(f"~={version}")  # cp37-cp37 is only compatible with 3.7.*
+                return not (spec & python_requires).is_impossible
+            else:
+                # we don't know about compatility for non-cpython implementations
+                # assume it is compatible
+                return True
+
+        if not link.is_wheel:
+            return True
+        python_requires = self.environment.python_requires
+        tags = parse_wheel_filename(link.filename)[-1]
+        result = any(is_tag_match(tag, python_requires) for tag in tags)
+        if not result:
+            termui.logger.debug(
+                "Skipping %r because it is not compatible with %r",
+                link,
+                python_requires,
+            )
+        return result
+
+    def get_hashes(self, candidate: Candidate) -> list[FileHash]:
         """Get hashes of all possible installable candidates
         of a given package version.
         """
         if (
             candidate.req.is_vcs
             or candidate.req.is_file_or_url
             and candidate.req.is_local_dir  # type: ignore[attr-defined]
         ):
-            return None
+            return []
         if candidate.hashes:
             return candidate.hashes
         req = candidate.req.as_pinned_version(candidate.version)
         comes_from = candidate.link.comes_from if candidate.link else None
-        result: dict[Link, str] = {}
+        result: list[FileHash] = []
         logged = False
         respect_source_order = self.environment.project.pyproject.settings.get("resolution", {}).get(
             "respect-source-order", False
         )
         if req.is_named and respect_source_order and comes_from:
             sources = [s for s in self.sources if comes_from.startswith(s.url)]
         else:
             sources = self.sources
         with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
             if req.is_file_or_url:
                 this_link = cast("Link", candidate.prepare(self.environment).link)
                 links: list[Link] = [this_link]
             else:  # the req must be a named requirement
                 links = [package.link for package in finder.find_matches(req.as_line())]
+                if self.ignore_compatibility:
+                    links = [link for link in links if self._is_python_match(link)]
             for link in links:
                 if not link or link.is_vcs or link.is_file and link.file_path.is_dir():
                     # The links found can still be a local directory or vcs, skippping it.
                     continue
                 if not logged:
                     termui.logger.info("Fetching hashes for %s", candidate)
                     logged = True
-                result[link] = self._hash_cache.get_hash(link, finder.session)
-        return result or None
+                result.append(
+                    {
+                        "url": link.url_without_fragment,
+                        "file": link.filename,
+                        "hash": self._hash_cache.get_hash(link, finder.session),
+                    }
+                )
+        return result
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         """Return an iterable of getter functions to get dependencies, which will be
         called one by one.
         """
         raise NotImplementedError
 
@@ -391,56 +433,51 @@
         self,
         lockfile: Mapping[str, Any],
         sources: list[RepositoryConfig],
         environment: BaseEnvironment,
     ) -> None:
         super().__init__(sources, environment, ignore_compatibility=False)
         self.packages: dict[CandidateKey, Candidate] = {}
-        self.file_hashes: dict[tuple[str, str], dict[Link, str]] = {}
         self.candidate_info: dict[CandidateKey, CandidateInfo] = {}
         self._read_lockfile(lockfile)
 
     @property
     def all_candidates(self) -> dict[str, Candidate]:
         return {can.req.identify(): can for can in self.packages.values()}
 
     def _read_lockfile(self, lockfile: Mapping[str, Any]) -> None:
-        from unearth import Link
-
         root = self.environment.project.root
         with cd(root):
             for package in lockfile.get("package", []):
                 version = package.get("version")
                 if version:
                     package["version"] = f"=={version}"
                 package_name = package.pop("name")
-                req_dict = {k: v for k, v in package.items() if k not in ("dependencies", "requires_python", "summary")}
+                req_dict = {
+                    k: v for k, v in package.items() if k not in ("dependencies", "requires_python", "summary", "files")
+                }
                 req = Requirement.from_req_dict(package_name, req_dict)
                 if req.is_file_or_url and req.path and not req.url:  # type: ignore[attr-defined]
                     req.url = path_to_url(posixpath.join(root, req.path))  # type: ignore[attr-defined]
                 can = make_candidate(req, name=package_name, version=version)
+                can.hashes = package.get("files", [])
                 can_id = self._identify_candidate(can)
                 self.packages[can_id] = can
                 candidate_info: CandidateInfo = (
                     package.get("dependencies", []),
                     package.get("requires_python", ""),
                     package.get("summary", ""),
                 )
                 self.candidate_info[can_id] = candidate_info
 
-        for key, hashes in lockfile.get("metadata", {}).get("files", {}).items():
-            self.file_hashes[tuple(key.split(None, 1))] = {  # type: ignore[index]
-                Link(item["url"]): item["hash"] for item in hashes if "url" in item
-            }
-
     def _identify_candidate(self, candidate: Candidate) -> CandidateKey:
-        url = getattr(candidate.req, "url", None)
-        if url is not None:
-            url = url_without_fragments(url)
-            url = self.environment.project.backend.expand_line(url)
+        url: str | None = None
+        if candidate.link is not None:
+            url = candidate.link.url_without_fragment
+            url = self.environment.project.backend.expand_line(cast(str, url))
             if url.startswith("file://"):
                 path = posixpath.normpath(url_to_path(url))
                 url = path_to_url(path)
         return (
             candidate.identify(),
             candidate.version if not url else None,
             url,
@@ -492,13 +529,11 @@
             if not PySpecSet(info[1]).contains(str(self.environment.interpreter.version), True):
                 continue
             can = self.packages[key]
             can.requires_python = info[1]
             if not requirement.name:
                 # make sure can.identify() won't return a randomly-generated name
                 requirement.name = can.name
-            can.req = requirement
             yield can
 
-    def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
-        assert candidate.name
-        return self.file_hashes.get((normalize_name(candidate.name), candidate.version or ""))
+    def get_hashes(self, candidate: Candidate) -> list[FileHash]:
+        return candidate.hashes
```

### Comparing `pdm-2.8.0a2/src/pdm/models/requirements.py` & `pdm-2.8.1/src/pdm/models/requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,16 @@
         if "marker" in kwargs:
             try:
                 kwargs["marker"] = get_marker(kwargs["marker"])
             except InvalidMarker as e:
                 raise RequirementError("Invalid marker: %s" % str(e)) from None
         if "extras" in kwargs and isinstance(kwargs["extras"], str):
             kwargs["extras"] = tuple(e.strip() for e in kwargs["extras"][1:-1].split(","))
-        version = kwargs.pop("version", None)
-        if version:
-            kwargs["specifier"] = get_specifier(version)
+        version = kwargs.pop("version", "")
+        kwargs["specifier"] = get_specifier(version)
         return cls(**{k: v for k, v in kwargs.items() if k in inspect.signature(cls).parameters})
 
     @classmethod
     def from_dist(cls, dist: Distribution) -> Requirement:
         direct_url_json = dist.read_text("direct_url.json")
         if direct_url_json is not None:
             direct_url = json.loads(direct_url_json)
@@ -236,15 +235,15 @@
         return ""
 
 
 @dataclasses.dataclass(eq=False)
 class NamedRequirement(Requirement):
     def as_line(self) -> str:
         extras = f"[{','.join(sorted(self.extras))}]" if self.extras else ""
-        return f"{self.project_name}{extras}{self.specifier}{self._format_marker()}"
+        return f"{self.project_name}{extras}{self.specifier or ''}{self._format_marker()}"
 
 
 @dataclasses.dataclass(eq=False)
 class FileRequirement(Requirement):
     url: str = ""
     path: Path | None = None
     subdirectory: str | None = None
```

### Comparing `pdm-2.8.0a2/src/pdm/models/search.py` & `pdm-2.8.1/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/session.py` & `pdm-2.8.1/src/pdm/models/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     from ssl import SSLContext
 
     from urllib3 import HTTPResponse
 
 
 def _create_truststore_ssl_context() -> SSLContext | None:
     if sys.version_info < (3, 10):
-        logger.warning("truststore is not available on Python < 3.10")
         return None
 
     try:
         import ssl
     except ImportError:
         logger.warning("Disabling truststore since ssl support is missing")
         return None
```

### Comparing `pdm-2.8.0a2/src/pdm/models/setup.py` & `pdm-2.8.1/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/specifiers.py` & `pdm-2.8.1/src/pdm/models/specifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,30 @@
 
 
 @lru_cache()
 def fix_legacy_specifier(specifier: str) -> str:
     """Since packaging 22.0, legacy specifiers like '>=4.*' are no longer
     supported. We try to normalize them to the new format.
     """
+    from pdm.utils import deprecation_warning
 
     def fix_wildcard(match: Match[str]) -> str:
         operator, _, version = match.groups()
-        if ".*" not in version or operator in ("==", "!="):
+        if operator in ("==", "!="):
             return match.group(0)
-        version = version.replace(".*", ".0")
-        if operator in ("<", "<="):  # <4.* and <=4.* are equivalent to <4.0
-            operator = "<"
-        elif operator in (">", ">="):  # >4.* and >=4.* are equivalent to >=4.0
-            operator = ">="
+        if ".*" in version:
+            deprecation_warning(".* suffix can only be used with `==` or `!=` operators", stacklevel=4)
+            version = version.replace(".*", ".0")
+            if operator in ("<", "<="):  # <4.* and <=4.* are equivalent to <4.0
+                operator = "<"
+            elif operator in (">", ">="):  # >4.* and >=4.* are equivalent to >=4.0
+                operator = ">="
+        elif "+" in version:  # Drop the local version
+            deprecation_warning("Local version label can only be used with `==` or `!=` operators", stacklevel=4)
+            version = version.split("+")[0]
         return f"{operator}{version}"
 
     return _legacy_specifier_re.sub(fix_wildcard, specifier)
 
 
 def _normalize_op_specifier(op: str, version_str: str) -> tuple[str, Version]:
     version = Version(version_str)
```

### Comparing `pdm-2.8.0a2/src/pdm/models/venv.py` & `pdm-2.8.1/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/versions.py` & `pdm-2.8.1/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/models/working_set.py` & `pdm-2.8.1/src/pdm/models/working_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,19 @@
 
 class WorkingSet(Mapping[str, im.Distribution]):
     """A dictionary of currently installed distributions"""
 
     def __init__(self, paths: list[str] | None = None):
         if paths is None:
             paths = sys.path
-        self._dist_map = {normalize_name(dist.metadata["Name"]): dist for dist in distributions(path=paths)}
+        self._dist_map = {
+            normalize_name(dist.metadata["Name"]): dist
+            for dist in distributions(path=list(dict.fromkeys(paths)))
+            if dist.metadata["Name"]
+        }
 
     def __getitem__(self, key: str) -> im.Distribution:
         return self._dist_map[key]
 
     def __len__(self) -> int:
         return len(self._dist_map)
```

### Comparing `pdm-2.8.0a2/src/pdm/pep582/sitecustomize.py` & `pdm-2.8.1/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/project/config.py` & `pdm-2.8.1/src/pdm/project/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import collections
 import dataclasses
 import os
 from pathlib import Path
-from typing import Any, Callable, Iterator, Mapping, MutableMapping, cast
+from typing import Any, Callable, ClassVar, Iterator, Mapping, MutableMapping, cast
 
 import platformdirs
 import rich.theme
 import tomlkit
 
 from pdm import termui
 from pdm._types import RepositoryConfig
@@ -51,14 +51,21 @@
     """Coerce a string value to a boolean value"""
     if not isinstance(val, str):
         return val
 
     return bool(val) and val.lower() not in ("false", "no", "0")
 
 
+def split_by_comma(val: list[str] | str) -> list[str]:
+    """Split a string value by comma"""
+    if isinstance(val, str):
+        return [v.strip() for v in val.split(",")]
+    return val
+
+
 DEFAULT_PYPI_INDEX = "https://pypi.org/simple"
 
 
 @dataclasses.dataclass
 class ConfigItem:
     """An item of configuration, with following attributes:
 
@@ -83,15 +90,15 @@
     def should_show(self) -> bool:
         return self.default is not self._NOT_SET
 
 
 class Config(MutableMapping[str, str]):
     """A dict-like object for configuration key and values"""
 
-    _config_map: dict[str, ConfigItem] = {
+    _config_map: ClassVar[dict[str, ConfigItem]] = {
         "cache_dir": ConfigItem(
             "The root directory of cached files",
             platformdirs.user_cache_dir("pdm"),
             True,
         ),
         "check_update": ConfigItem(
             "Check if there is any newer version available",
@@ -151,14 +158,17 @@
             False,
             coerce=ensure_boolean,
         ),
         "install.cache_method": ConfigItem(
             "`symlink` or `pth` to create links to the cached installation",
             "symlink",
         ),
+        "python.providers": ConfigItem(
+            "List of python provider names for findpython", default=[], coerce=split_by_comma
+        ),
         "python.use_pyenv": ConfigItem("Use the pyenv interpreter", True, coerce=ensure_boolean),
         "python.use_venv": ConfigItem(
             "Use virtual environments when available", True, env_var="PDM_USE_VENV", coerce=ensure_boolean
         ),
         "pypi.url": ConfigItem(
             "The URL of PyPI mirror, defaults to https://pypi.org/simple",
             DEFAULT_PYPI_INDEX,
```

### Comparing `pdm-2.8.0a2/src/pdm/project/core.py` & `pdm-2.8.1/src/pdm/project/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -375,18 +375,21 @@
         if not self.config.get("pypi.ignore_stored_index", False):
             if "pypi" not in result:  # put pypi source at the beginning
                 result = {"pypi": self.default_source, **result}
             else:
                 result["pypi"].passive_update(self.default_source)
             merge_sources(self.project_config.iter_sources())
             merge_sources(self.global_config.iter_sources())
+        sources: list[RepositoryConfig] = []
         for source in result.values():
-            assert source.url, f"Source URL must not be empty for {source.name}"
+            if not source.url:
+                continue
             source.url = expand_env_vars_in_auth(source.url)
-        return list(result.values())
+            sources.append(source)
+        return sources
 
     def get_repository(
         self, cls: type[BaseRepository] | None = None, ignore_compatibility: bool = True
     ) -> BaseRepository:
         """Get the repository object"""
         if cls is None:
             cls = self.core.repository_class
@@ -469,40 +472,23 @@
         from pdm.resolver.reporters import SpinnerReporter
 
         if spinner is None:
             spinner = termui.SilentSpinner("")
 
         return SpinnerReporter(spinner, requirements)
 
-    def get_lock_metadata(
-        self, groups: Iterable[str] | None = None, cross_platform: bool | None = None
-    ) -> dict[str, Any]:
-        content_hash = tomlkit.string("sha256:" + self.pyproject.content_hash("sha256"))
-        content_hash.trivia.trail = "\n\n"
-        if groups is None:
-            groups = self.iter_groups()
-        if cross_platform is None:
-            cross_platform = self.lockfile.cross_platform
-        return {
-            "lock_version": self.lockfile.spec_version,
-            "cross_platform": cross_platform,
-            "groups": sorted(groups, key=lambda x: (x != "default", x)),
-            "content_hash": content_hash,
-        }
+    def get_lock_metadata(self) -> dict[str, Any]:
+        content_hash = "sha256:" + self.pyproject.content_hash("sha256")
+        return {"lock_version": self.lockfile.spec_version, "content_hash": content_hash}
 
-    def write_lockfile(
-        self,
-        toml_data: dict,
-        show_message: bool = True,
-        write: bool = True,
-        groups: Iterable[str] | None = None,
-        cross_platform: bool | None = None,
-    ) -> None:
+    def write_lockfile(self, toml_data: dict, show_message: bool = True, write: bool = True, **_kwds: Any) -> None:
         """Write the lock file to disk."""
-        toml_data["metadata"].update(self.get_lock_metadata(groups, cross_platform=cross_platform))
+        if _kwds:
+            deprecation_warning("Extra arguments have been moved to `format_lockfile` function", stacklevel=2)
+        toml_data["metadata"].update(self.get_lock_metadata())
         self.lockfile.set_data(toml_data)
 
         if write:
             self.lockfile.write(show_message)
 
     def make_self_candidate(self, editable: bool = True) -> Candidate:
         from unearth import Link
@@ -637,15 +623,15 @@
                 pyenv_shim = os.path.join(PYENV_ROOT, "shims", "python3")
                 if os.name == "nt":
                     pyenv_shim += ".bat"
                 if os.path.exists(pyenv_shim):
                     yield PythonInfo.from_path(pyenv_shim)
                 elif os.path.exists(pyenv_shim.replace("python3", "python")):
                     yield PythonInfo.from_path(pyenv_shim.replace("python3", "python"))
-            python = shutil.which("python")
+            python = shutil.which("python") or shutil.which("python3")
             if python:
                 yield PythonInfo.from_path(python)
             args = []
         else:
             if not all(c.isdigit() for c in python_spec.split(".")):
                 path = Path(python_spec)
                 if path.exists():
@@ -667,17 +653,19 @@
             yield PythonInfo.from_path(this_python)
 
     def _get_python_finder(self) -> Finder:
         from findpython import Finder
 
         from pdm.cli.commands.venv.utils import VenvProvider
 
-        finder = Finder(resolve_symlinks=True)
-        if self.config["python.use_venv"]:
-            finder.add_provider(VenvProvider(self), 0)
+        providers: list[str] = self.config["python.providers"]
+        finder = Finder(resolve_symlinks=True, selected_providers=providers or None)
+        if self.config["python.use_venv"] and (not providers or "venv" in providers):
+            venv_pos = providers.index("venv") if providers else 0
+            finder.add_provider(VenvProvider(self), venv_pos)
         return finder
 
     # compatibility, shouldn't be used directly
     @property
     def meta(self) -> dict[str, Any]:
         deprecation_warning("project.meta is deprecated, use project.pyproject.metadata instead", stacklevel=2)
         return self.pyproject.metadata
```

### Comparing `pdm-2.8.0a2/src/pdm/project/lockfile.py` & `pdm-2.8.1/src/pdm/project/lockfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 GENERATED_COMMENTS = [
     "This file is @generated by PDM.",
     "It is not intended for manual editing.",
 ]
 
 
 class Lockfile(TOMLBase):
-    spec_version = "4.2"
+    spec_version = "4.3"
 
     @property
     def hash(self) -> str:
         return self._data.get("metadata", {}).get("content_hash", "")
 
     @property
     def file_version(self) -> str:
@@ -30,14 +30,18 @@
 
     @property
     def cross_platform(self) -> bool:
         if self.empty():
             return True
         return self._data.get("metadata", {}).get("cross_platform", True)
 
+    @property
+    def static_urls(self) -> bool:
+        return self._data.get("metadata", {}).get("static_urls", False)
+
     def compare_groups(self, groups: Iterable[str]) -> list[str]:
         if not self.groups:
             return []
         return list(set(groups).difference(self.groups))
 
     def set_data(self, data: Mapping[str, Any]) -> None:
         self._data = tomlkit.document()
@@ -60,9 +64,9 @@
         if not self.exists():
             return True
         lockfile_version = str(self.file_version)
         if not lockfile_version:
             return False
         if "." not in lockfile_version:
             lockfile_version += ".0"
-        accepted = get_specifier(f"~={lockfile_version},>={lockfile_version}")
+        accepted = get_specifier(f"~={lockfile_version}")
         return accepted.contains(self.spec_version)
```

### Comparing `pdm-2.8.0a2/src/pdm/project/project_file.py` & `pdm-2.8.1/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/project/toml_file.py` & `pdm-2.8.1/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/pytest.py` & `pdm-2.8.1/src/pdm/pytest.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "pdm.pytest",
     ...
 ]
 ```
 """
 from __future__ import annotations
 
-import collections
+import collections.abc
 import json
 import os
 import shutil
 import sys
 from dataclasses import dataclass
 from io import BufferedReader, BytesIO, StringIO
 from pathlib import Path
@@ -67,15 +67,15 @@
 from pdm.utils import find_python_in_path, normalize_name, path_to_url
 
 if TYPE_CHECKING:
     from typing import Protocol
 
     from _pytest.fixtures import SubRequest
 
-    from pdm._types import CandidateInfo, RepositoryConfig
+    from pdm._types import CandidateInfo, FileHash, RepositoryConfig
 
 
 class LocalFileAdapter(requests.adapters.BaseAdapter):
     """
     A local file adapter for request.
 
     Allows to mock some HTTP requests with some local files
@@ -187,16 +187,16 @@
         return (
             self._get_dependencies_from_cache,
             self._get_dependency_from_local_package,
             self._get_dependencies_from_fixture,
             self._get_dependencies_from_metadata,
         )
 
-    def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
-        return {}
+    def get_hashes(self, candidate: Candidate) -> list[FileHash]:
+        return []
 
     def _find_candidates(self, requirement: Requirement) -> Iterable[Candidate]:
         for version, candidate in sorted(
             self._pypi_data.get(cast(str, requirement.key), {}).items(),
             key=lambda item: parse_version(item[0]),
             reverse=True,
         ):
```

### Comparing `pdm-2.8.0a2/src/pdm/resolver/core.py` & `pdm-2.8.1/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/resolver/providers.py` & `pdm-2.8.1/src/pdm/resolver/providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,15 +162,18 @@
         if isinstance(requirement, PythonRequirement):
             return is_python_satisfied_by(requirement, candidate)
         elif candidate.identify() in self.overrides:
             return True
         if not requirement.is_named:
             if candidate.req.is_named:
                 return False
-            return self._compare_file_reqs(requirement, candidate.req)  # type: ignore[arg-type]
+            can_req = candidate.req
+            if requirement.is_vcs and can_req.is_vcs:
+                return can_req.vcs == requirement.vcs and can_req.repo == requirement.repo  # type: ignore[attr-defined]
+            return self._compare_file_reqs(requirement, can_req)  # type: ignore[arg-type]
         version = candidate.version
         this_name = self.repository.environment.project.name
         if version is None or candidate.name == this_name:
             # This should be a URL candidate or self package, consider it to be matching
             return True
         # Allow prereleases if: 1) it is not specified in the tool settings or
         # 2) the candidate doesn't come from PyPI index.
```

### Comparing `pdm-2.8.0a2/src/pdm/resolver/python.py` & `pdm-2.8.1/src/pdm/resolver/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pdm.models.candidates import Candidate
 from pdm.models.requirements import NamedRequirement, Requirement
 from pdm.models.specifiers import PySpecSet
 
 
 class PythonCandidate(Candidate):
     def format(self) -> str:
-        return f"[req]{self.name}[/][warning]{str(self.req.specifier)}[/]"
+        return f"[req]{self.name}[/][warning]{self.req.specifier!s}[/]"
 
 
 class PythonRequirement(NamedRequirement):
     @classmethod
     def from_pyspec_set(cls, spec: PySpecSet) -> PythonRequirement:
         return cls(name="python", specifier=spec)
```

### Comparing `pdm-2.8.0a2/src/pdm/resolver/reporters.py` & `pdm-2.8.1/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/signals.py` & `pdm-2.8.1/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/termui.py` & `pdm-2.8.1/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/src/pdm/utils.py` & `pdm-2.8.1/src/pdm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
 from pdm.compat import importlib_metadata
 
 if TYPE_CHECKING:
     from re import Match
     from typing import IO, Any, Iterator
 
-    from unearth import Link
-
-    from pdm._types import RepositoryConfig
+    from pdm._types import FileHash, RepositoryConfig
     from pdm.compat import Distribution
 
 _egg_fragment_re = re.compile(r"(.*)[#&]egg=[^&]*")
 
 try:
     _packaging_version = importlib_metadata.version("packaging")
 except Exception:
@@ -90,26 +88,26 @@
         if path.parent == path:
             # Root path is reached
             break
         path = path.parent
     return None
 
 
-def convert_hashes(hashes: dict[Link, str]) -> dict[str, list[str]]:
+def convert_hashes(files: list[FileHash]) -> dict[str, list[str]]:
     """Convert Pipfile.lock hash lines into InstallRequirement option format.
 
     The option format uses a str-list mapping. Keys are hash algorithms, and
     the list contains all values of that algorithm.
     """
     result: dict[str, list[str]] = {}
-    for hash_value in hashes.values():
-        try:
-            name, hash_value = hash_value.split(":", 1)
-        except ValueError:
-            name = "sha256"
+    for f in files:
+        hash_value = f.get("hash", "")
+        name, has_name, hash_value = hash_value.partition(":")
+        if not has_name:
+            name, hash_value = "sha256", name
         result.setdefault(name, []).append(hash_value)
     return result
 
 
 def get_user_email_from_git() -> tuple[str, str]:
     """Get username and email from git config.
     Return empty if not configured or git is not found.
```

### Comparing `pdm-2.8.0a2/tests/cli/conftest.py` & `pdm-2.8.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_add.py` & `pdm-2.8.1/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_build.py` & `pdm-2.8.1/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_cache.py` & `pdm-2.8.1/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_config.py` & `pdm-2.8.1/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_fix.py` & `pdm-2.8.1/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_hooks.py` & `pdm-2.8.1/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_init.py` & `pdm-2.8.1/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_install.py` & `pdm-2.8.1/tests/cli/test_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 .whl#sha256=90e49598b553d8746c4dc7d9442e0359d038c3039d802c91c0a55505da318c63">
         future_fstrings-1.2.0.tar.gz
         </a>
     </body>
     </html>
     """
     pdm(["lock"], obj=project, strict=True)
-    file_hashes = project.lockfile["metadata"]["files"]["future-fstrings 1.2.0"]
+    file_hashes = project.lockfile["package"][0]["files"]
     assert [e["hash"] for e in file_hashes] == [
         "sha256:90e49598b553d8746c4dc7d9442e0359d038c3039d802c91c0a55505da318c63"
     ]
     # Mimic the CDN inconsistences of PyPI simple index. See issues/596.
     del index["/simple/future-fstrings/"]
     pdm(["sync", "--no-self"], obj=project, strict=True)
```

### Comparing `pdm-2.8.0a2/tests/cli/test_list.py` & `pdm-2.8.1/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_lock.py` & `pdm-2.8.1/tests/cli/test_lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pdm.models.requirements import parse_requirement
 from pdm.models.specifiers import PySpecSet
 
 
 def test_lock_command(project, pdm, mocker):
     m = mocker.patch.object(actions, "do_lock")
     pdm(["lock"], obj=project)
-    m.assert_called_with(project, refresh=False, groups=["default"], hooks=ANY, cross_platform=True)
+    m.assert_called_with(project, refresh=False, groups=["default"], hooks=ANY, cross_platform=True, static_urls=None)
 
 
 @pytest.mark.usefixtures("repository")
 def test_lock_dependencies(project):
     project.add_dependencies({"requests": parse_requirement("requests")})
     actions.do_lock(project)
     assert project.lockfile.exists
@@ -26,31 +26,40 @@
 
 
 def test_lock_refresh(pdm, project, repository):
     project.add_dependencies({"requests": parse_requirement("requests")})
     result = pdm(["lock"], obj=project)
     assert result.exit_code == 0
     assert project.is_lockfile_hash_match()
-    assert not project.lockfile["metadata"]["files"].get("requests 2.19.1")
+    package = next(p for p in project.lockfile["package"] if p["name"] == "requests")
+    assert not package.get("files")
     project.add_dependencies({"requests": parse_requirement("requests>=2.0")})
     url_hashes = {
         "http://example.com/requests-2.19.1-py3-none-any.whl": "sha256:abcdef123456",
         "http://example2.com/requests-2.19.1-py3-none-AMD64.whl": "sha256:abcdef123456",
         "http://example1.com/requests-2.19.1-py3-none-any.whl": "sha256:abcdef123456",
     }
-    repository.get_hashes = lambda c: (
-        {Link(url): hash for url, hash in url_hashes.items()} if c.identify() == "requests" else {}
+    repository.get_hashes = (
+        lambda c: [{"url": url, "file": Link(url).filename, "hash": hash} for url, hash in url_hashes.items()]
+        if c.identify() == "requests"
+        else []
     )
     assert not project.is_lockfile_hash_match()
     result = pdm(["lock", "--refresh", "-v"], obj=project)
     assert result.exit_code == 0
-    assert project.is_lockfile_hash_match()
-    assert project.lockfile["metadata"]["files"]["requests 2.19.1"] == [
-        {"url": url, "hash": hash} for url, hash in sorted(url_hashes.items())
+    package = next(p for p in project.lockfile["package"] if p["name"] == "requests")
+    assert package["files"] == [
+        {"file": "requests-2.19.1-py3-none-AMD64.whl", "hash": "sha256:abcdef123456"},
+        {"file": "requests-2.19.1-py3-none-any.whl", "hash": "sha256:abcdef123456"},
     ]
+    assert project.is_lockfile_hash_match()
+    result = pdm(["lock", "--refresh", "--static-urls", "-v"], obj=project)
+    assert result.exit_code == 0
+    package = next(p for p in project.lockfile["package"] if p["name"] == "requests")
+    assert package["files"] == [{"url": url, "hash": hash} for url, hash in sorted(url_hashes.items())]
 
 
 def test_lock_refresh_keep_consistent(pdm, project, repository):
     project.add_dependencies({"requests": parse_requirement("requests")})
     result = pdm(["lock"], obj=project)
     assert result.exit_code == 0
     assert project.is_lockfile_hash_match()
@@ -132,20 +141,22 @@
 
 @pytest.mark.usefixtures("local_finder")
 def test_lock_multiple_platform_wheels(project, pdm):
     project.environment.python_requires = PySpecSet(">=3.7")
     project.add_dependencies({"pdm-hello": parse_requirement("pdm-hello")})
     pdm(["lock"], obj=project, strict=True)
     assert project.lockfile.cross_platform
-    file_hashes = project.lockfile["metadata"]["files"]["pdm-hello 0.1.0"]
+    package = next(p for p in project.lockfile["package"] if p["name"] == "pdm-hello")
+    file_hashes = package["files"]
     assert len(file_hashes) == 2
 
 
 @pytest.mark.usefixtures("local_finder")
 def test_lock_current_platform_wheels(project, pdm):
     project.environment.python_requires = PySpecSet(">=3.7")
     project.add_dependencies({"pdm-hello": parse_requirement("pdm-hello")})
     pdm(["lock", "--no-cross-platform"], obj=project, strict=True)
     assert project.lockfile.cross_platform is False
-    file_hashes = project.lockfile["metadata"]["files"]["pdm-hello 0.1.0"]
+    package = next(p for p in project.lockfile["package"] if p["name"] == "pdm-hello")
+    file_hashes = package["files"]
     wheels_num = 2 if sys.platform == "win32" and not project.python.is_32bit else 1
     assert len(file_hashes) == wheels_num
```

### Comparing `pdm-2.8.0a2/tests/cli/test_others.py` & `pdm-2.8.1/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_publish.py` & `pdm-2.8.1/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_remove.py` & `pdm-2.8.1/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_run.py` & `pdm-2.8.1/tests/cli/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,16 +802,23 @@
     assert "Script unknown: whatever" in result.stderr
     assert "Usage" in result.stderr
 
 
 @pytest.mark.parametrize(
     "args",
     [
-        pytest.param([], id="no args"),
         pytest.param(["-ko"], id="unknown param"),
         pytest.param(["pip", "--version"], id="not an user script"),
     ],
 )
 def test_empty_positionnal_args_still_display_usage(project, pdm, args):
     result = pdm(args, obj=project)
     assert result.exit_code != 0
     assert "Usage" in result.stderr
+
+
+def test_empty_positional_args_display_help(project, pdm):
+    result = pdm([], obj=project)
+    assert result.exit_code == 0
+    assert "Usage:" in result.output
+    assert "Commands:" in result.output
+    assert "Options:" in result.output
```

### Comparing `pdm-2.8.0a2/tests/cli/test_self_command.py` & `pdm-2.8.1/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_template.py` & `pdm-2.8.1/tests/cli/test_template.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_update.py` & `pdm-2.8.1/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_use.py` & `pdm-2.8.1/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/cli/test_venv.py` & `pdm-2.8.1/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/conftest.py` & `pdm-2.8.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         FIXTURES / "artifacts" / wheel_name
         for wheel_name in (
             "pdm_pep517-1.0.0-py3-none-any.whl",
             "poetry_core-1.3.2-py3-none-any.whl",
             "setuptools-65.4.1-py3-none-any.whl",
             "wheel-0.37.1-py2.py3-none-any.whl",
             "flit_core-3.6.0-py3-none-any.whl",
-            "pdm_backend-2.0.2-py3-none-any.whl",
+            "pdm_backend-2.1.4-py3-none-any.whl",
             "importlib_metadata-4.8.3-py3-none-any.whl",
             "zipp-3.7.0-py3-none-any.whl",
             "typing_extensions-4.4.0-py3-none-any.whl",
         )
     ]
```

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.8.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.8.1/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.8.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.8.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.8.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.8.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.8.1/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.8.1/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     --hash=sha256:0fbeb6180d383a9186d0d6ed954e0042ad9f18e0e8de088b2b419d526927d196 \
     --hash=sha256:c34f04500f2cbbea882b1acb02002ad6fe6b7ffa64a6164577995657f50aed22
 itsdangerous==1.1.0 \
     --hash=sha256:321b033d07f2a4136d3ec762eac9f16a10ccd60f53c0c91af90217ace7ba1f19 \
     --hash=sha256:72a1252c0b2cc2bcc351acf2cfe2ec0159d8578c54767d5c2aa67fd869346e55 \
     --hash=sha256:ac4c9f590d59c36b7d2953f97fda415f2461280e5279650aafe1e593f129c4f7 \
     --hash=sha256:b12271b2047cb23eeb98c8b5622e2e5c5e9abd9784a153e9d8ef9cb4dd09d749
-Jinja2==2.11.3 \
+jinja2==2.11.3 \
     --hash=sha256:03e47ad063331dd6a3f04a43eddca8a966a26ba0c5b7207a9a9e4e08f1b29419 \
     --hash=sha256:a6d58433de0ae800347cab1fa3043cebbabe8baa9d29e668f1c768cb87a333c6
-MarkupSafe==1.1.1 \
+markupsafe==1.1.1 \
     --hash=sha256:00bc623926325b26bb9605ae9eae8a215691f33cae5df11ca5424f06f2d1f473 \
     --hash=sha256:09027a7803a62ca78792ad89403b1b7a73a01c8cb65909cd876f7fcebd79b161 \
     --hash=sha256:09c4b7f37d6c648cb13f9230d847adf22f8171b1ccc4d5682398e77f40309235 \
     --hash=sha256:0db2ff381c2218c1ba7192f75e5c5cf180efa023ddfc6914ffe9a38b2bd303dd \
     --hash=sha256:1027c282dad077d0bae18be6794e6b6b8c91d58ed8a8d89a89d59693b9131db5 \
     --hash=sha256:13d3144e1e340870b25e7b10b98d779608c02016d5184cfb9927a9f10c689f42 \
     --hash=sha256:195d7d2c4fbb0ee8139a6cf67194f3973a6b3042d742ebe0a9ed36d8b6f0c07f \
@@ -86,11 +86,11 @@
     --hash=sha256:d73a845f227b0bfe8a7455ee623525ee656a9e2e749e4742706d80a6065d5e2c \
     --hash=sha256:d9be0ba6c527163cbed5e0857c451fcd092ce83947944d6c14bc95441203f032 \
     --hash=sha256:dbc6ee2241abe4f518685f603e427a94ceb73c08b6d15d85c6c5c4a71bde9c3e \
     --hash=sha256:de603df0d005177f7ef7faa56578d2d47fc93aaef165cdef91d64959176edb15 \
     --hash=sha256:e249096428b3ae81b08327a63a485ad0878de3fb939049038579ac0ef61e17e7 \
     --hash=sha256:e8313f01ba26fbbe36c7be1966a7b7424942f670f38e666995b88d012765b9be \
     --hash=sha256:feb7b34d6325451ef96bc0e36e1a6c0c1c64bc1fbec4b854f4529e51887b1621
-Werkzeug==1.0.1 \
+werkzeug==1.0.1 \
     --hash=sha256:2de2a5db0baeae7b2d2664949077c2ac63fbd16d98da0ff71837f7d1dea3fd43 \
     --hash=sha256:6c80b1e5ad3665290ea39320b91e1be1e0d5f60652b964a3070216de83d2e47c
 --extra-index-url https://test.pypi.org/simple
```

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.8.1/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.8.1/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.8.1/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/pypi.json` & `pdm-2.8.1/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/fixtures/pyproject.toml` & `pdm-2.8.1/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/models/test_backends.py` & `pdm-2.8.1/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/models/test_candidates.py` & `pdm-2.8.1/tests/models/test_candidates.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,15 @@
     project.project_config["pypi.url"] = "https://my.pypi.org/simple"
     req = parse_requirement("pep345-legacy")
     repo = project.get_repository()
     candidate = next(iter(repo.find_candidates(req)))
     assert candidate.requires_python == ">=3,<4"
 
 
+@pytest.mark.filterwarnings("ignore::FutureWarning")
 def test_ignore_invalid_py_version(project):
     project.project_config["pypi.url"] = "https://my.pypi.org/simple"
     req = parse_requirement("wheel")
     repo = project.get_repository()
     candidate = next(iter(repo.find_candidates(req)))
     assert not candidate.requires_python
```

### Comparing `pdm-2.8.0a2/tests/models/test_marker.py` & `pdm-2.8.1/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/models/test_requirements.py` & `pdm-2.8.1/tests/models/test_requirements.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,17 +57,23 @@
         marks=pytest.mark.skipif(not PACKAGING_22, reason="packaging 22+ required"),
     ),
     pytest.param(
         "foo (>=4.*, <=5.*)",
         "foo<5.0,>=4.0",
         marks=pytest.mark.skipif(not PACKAGING_22, reason="packaging 22+ required"),
     ),
+    pytest.param(
+        "foo>=3.0+g1234; python_version>='3.6'",
+        'foo>=3.0; python_version >= "3.6"',
+        marks=pytest.mark.skipif(not PACKAGING_22, reason="packaging 22+ required"),
+    ),
 ]
 
 
+@pytest.mark.filterwarnings("ignore::FutureWarning")
 @pytest.mark.parametrize("req, result", REQUIREMENTS)
 def test_convert_req_dict_to_req_line(req, result):
     r = parse_requirement(req)
     result = result or req
     assert r.as_line() == result
```

### Comparing `pdm-2.8.0a2/tests/models/test_setup_parsing.py` & `pdm-2.8.1/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/models/test_specifiers.py` & `pdm-2.8.1/tests/models/test_specifiers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from pdm.models.specifiers import PySpecSet
 
 
+@pytest.mark.filterwarnings("ignore::FutureWarning")
 @pytest.mark.parametrize(
     "original,normalized",
     [
         (">=3.6", ">=3.6"),
         ("<3.8", "<3.8"),
         ("~=2.7.0", ">=2.7,<2.8"),
         ("", ""),
@@ -19,14 +20,16 @@
         (">=3.6,<3.8,!=3.8.*", ">=3.6,<3.8"),
         (">=2.7,<3.2,!=3.0.*,!=3.1.*", ">=2.7,<3.0"),
         ("!=3.0.*,!=3.0.2", "!=3.0.*"),
         (">=3.4.*", ">=3.4"),
         (">3.4.*", ">=3.4"),
         ("<=3.4.*", "<3.4"),
         ("<3.4.*", "<3.4"),
+        (">=3.0+g1234", ">=3.0"),
+        ("<3.0+g1234", "<3.0"),
         ("<3.10.0a6", "<3.10.0a6"),
         ("<3.10.2a3", "<3.10.2a3"),
     ],
 )
 def test_normalize_pyspec(original, normalized):
     spec = PySpecSet(original)
     assert str(spec) == normalized
@@ -75,14 +78,15 @@
     assert (spec & a).is_impossible
     assert spec | a == a
     spec_copy = spec.copy()
     assert spec_copy.is_impossible
     assert str(spec_copy) == "impossible"
 
 
+@pytest.mark.filterwarnings("ignore::FutureWarning")
 @pytest.mark.parametrize(
     "left,right",
     [
         ("~=2.7", ">=2.7"),
         (">=3.6", ""),
         (">=3.7", ">=3.6,<4.0"),
         (">=2.7,<3.0", ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*"),
```

### Comparing `pdm-2.8.0a2/tests/models/test_versions.py` & `pdm-2.8.1/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/resolver/test_resolve.py` & `pdm-2.8.1/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_formats.py` & `pdm-2.8.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_installer.py` & `pdm-2.8.1/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_integration.py` & `pdm-2.8.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_plugin.py` & `pdm-2.8.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_project.py` & `pdm-2.8.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_signals.py` & `pdm-2.8.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/tests/test_utils.py` & `pdm-2.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a2/PKG-INFO` & `pdm-2.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.8.0a2
+Version: 2.8.1
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,32 +21,39 @@
 Requires-Dist: certifi
 Requires-Dist: packaging!=22.0,>=20.9
 Requires-Dist: platformdirs
 Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20
 Requires-Dist: pyproject-hooks
 Requires-Dist: requests-toolbelt
-Requires-Dist: unearth>=0.9.0
-Requires-Dist: findpython>=0.2.2
+Requires-Dist: unearth>=0.10.0
+Requires-Dist: findpython<1.0.0a0,>=0.3.0
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
 Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: importlib-resources>=5; python_version < "3.9"
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest"
-Requires-Dist: copier; extra == "all"
-Requires-Dist: cookiecutter; extra == "all"
-Requires-Dist: keyring; extra == "all"
-Requires-Dist: truststore; python_version >= "3.10" and extra == "all"
+Requires-Dist: copier; extra == "copier"
+Requires-Dist: cookiecutter; extra == "cookiecutter"
+Requires-Dist: keyring; extra == "keyring"
+Requires-Dist: pdm[cookiecutter,copier]; extra == "template"
+Requires-Dist: truststore; python_version >= "3.10" and extra == "truststore"
+Requires-Dist: pdm[keyring,template,truststore]; extra == "all"
 Provides-Extra: pytest
+Provides-Extra: copier
+Provides-Extra: cookiecutter
+Provides-Extra: keyring
+Provides-Extra: template
+Provides-Extra: truststore
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # PDM
```

#### html2text {}

```diff
@@ -1,33 +1,37 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.8.0a2 Summary: A modern Python
-package and dependency manager supporting the latest PEP standards Keywords:
-packaging dependency workflow Author-Email: Frost Ming
+Metadata-Version: 2.1 Name: pdm Version: 2.8.1 Summary: A modern Python package
+and dependency manager supporting the latest PEP standards Keywords: packaging
+dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://pdm.fming.dev Project-URL: Repository, https://
 github.com/pdm-project/pdm Project-URL: Documentation, https://pdm.fming.dev
 Project-URL: Changelog, https://pdm.fming.dev/latest/dev/changelog/ Requires-
 Python: >=3.7 Requires-Dist: blinker Requires-Dist: certifi Requires-Dist:
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
-requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
-findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
+requests-toolbelt Requires-Dist: unearth>=0.10.0 Requires-Dist:
+findpython<1.0.0a0,>=0.3.0 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
 resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
 cachecontrol[filecache]>=0.13.0 Requires-Dist: tomli>=1.1.0; python_version <
 "3.11" Requires-Dist: importlib-resources>=5; python_version < "3.9" Requires-
 Dist: importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest;
 extra == "pytest" Requires-Dist: pytest-mock; extra == "pytest" Requires-Dist:
-copier; extra == "all" Requires-Dist: cookiecutter; extra == "all" Requires-
-Dist: keyring; extra == "all" Requires-Dist: truststore; python_version >=
-"3.10" and extra == "all" Provides-Extra: pytest Provides-Extra: all
-Description-Content-Type: text/markdown
+copier; extra == "copier" Requires-Dist: cookiecutter; extra == "cookiecutter"
+Requires-Dist: keyring; extra == "keyring" Requires-Dist: pdm
+[cookiecutter,copier]; extra == "template" Requires-Dist: truststore;
+python_version >= "3.10" and extra == "truststore" Requires-Dist: pdm
+[keyring,template,truststore]; extra == "all" Provides-Extra: pytest Provides-
+Extra: copier Provides-Extra: cookiecutter Provides-Extra: keyring Provides-
+Extra: template Provides-Extra: truststore Provides-Extra: all Description-
+Content-Type: text/markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
   (https://pdm.fming.dev) [![Twitter Follow](https://img.shields.io/twitter/
    follow/pdm_project?label=get%20updates&logo=twitter&style=for-the-badge)]
  (https://twitter.com/pdm_project) [![Discord](https://img.shields.io/discord/
```

