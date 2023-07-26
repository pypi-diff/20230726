# Comparing `tmp/python-semantic-release-8.0.3.tar.gz` & `tmp/python-semantic-release-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.3.tar", last modified: Fri Jul 21 16:21:41 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.4.tar", last modified: Wed Jul 26 20:43:33 2023, max compression
```

## Comparing `python-semantic-release-8.0.3.tar` & `python-semantic-release-8.0.4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/README.rst
--rw-r--r--   0 root         (0) root         (0)     4651 2023-07-21 16:21:34.000000 python-semantic-release-8.0.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.698726 python-semantic-release-8.0.3/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4266 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.698726 python-semantic-release-8.0.3/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1123 2023-07-21 16:21:34.000000 python-semantic-release-8.0.3/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18649 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    12975 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3753 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.694726 python-semantic-release-8.0.3/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      844 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10146 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14710 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    13967 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.694726 python-semantic-release-8.0.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     3631 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22533 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    23987 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13407 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9248 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9675 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.998366 python-semantic-release-8.0.4/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-26 20:43:32.998366 python-semantic-release-8.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4695 2023-07-26 20:43:25.000000 python-semantic-release-8.0.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.978366 python-semantic-release-8.0.4/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 20:43:32.000000 python-semantic-release-8.0.4/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.982366 python-semantic-release-8.0.4/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-26 20:43:25.000000 python-semantic-release-8.0.4/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.982366 python-semantic-release-8.0.4/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.982366 python-semantic-release-8.0.4/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.986366 python-semantic-release-8.0.4/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18649 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.986366 python-semantic-release-8.0.4/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.974366 python-semantic-release-8.0.4/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.986366 python-semantic-release-8.0.4/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      844 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.986366 python-semantic-release-8.0.4/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10146 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.990366 python-semantic-release-8.0.4/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14058 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 20:43:32.998366 python-semantic-release-8.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.978366 python-semantic-release-8.0.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.990366 python-semantic-release-8.0.4/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.990366 python-semantic-release-8.0.4/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    48642 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.990366 python-semantic-release-8.0.4/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.994366 python-semantic-release-8.0.4/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.994366 python-semantic-release-8.0.4/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.994366 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.994366 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.994366 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.998366 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22533 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    23987 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:43:32.998366 python-semantic-release-8.0.4/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9248 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9675 2023-07-26 20:42:44.000000 python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.3/LICENSE` & `python-semantic-release-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/PKG-INFO` & `python-semantic-release-8.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.3
+Version: 8.0.4
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
```

### Comparing `python-semantic-release-8.0.3/README.rst` & `python-semantic-release-8.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/pyproject.toml` & `python-semantic-release-8.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.3"
+version = "8.0.4"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 readme = "README.rst"
 authors = [{ name = "Rolf Erik Lekang", email = "me@rolflekang.com" }]
 dependencies = [
   "click>=8,<9",
   "gitpython>=3.0.8,<4",
   "requests>=2.25,<3",
```

### Comparing `python-semantic-release-8.0.3/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.4/python_semantic_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.3
+Version: 8.0.4
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
```

### Comparing `python-semantic-release-8.0.3/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.4/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.4/python_semantic_release.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/__init__.py` & `python-semantic-release-8.0.4/semantic_release/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.3"
+__version__ = "8.0.4"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.3/semantic_release/changelog/context.py` & `python-semantic-release-8.0.4/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.4/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/changelog/template.py` & `python-semantic-release-8.0.4/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.4/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.4/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.4/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.4/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.4/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/common.py` & `python-semantic-release-8.0.4/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/config.py` & `python-semantic-release-8.0.4/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.4/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.4/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/cli/util.py` & `python-semantic-release-8.0.4/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.4/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/const.py` & `python-semantic-release-8.0.4/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.4/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 {% for commit in commits %}{% if type_ != "unknown" %}
 * {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% else %}
 * {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% endif %}{% endfor %}{% endfor %}{% endif %}
 {% for version, release in context.history.released.items() %}
 {# RELEASED #}
-## {{ version.as_tag() }} ({{ release.tagged_date.strftime("%Y-%m-%d") }})
+## {{ version.as_semver_tag() }} ({{ release.tagged_date.strftime("%Y-%m-%d") }})
 {% for type_, commits in release["elements"] | dictsort %}
 ### {{ type_ | capitalize }}
 {% for commit in commits %}{% if type_ != "unknown" %}
 * {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% else %}
 * {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% endif %}{% endfor %}{% endfor %}{% endfor %}
```

### Comparing `python-semantic-release-8.0.3/semantic_release/enums.py` & `python-semantic-release-8.0.4/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/errors.py` & `python-semantic-release-8.0.4/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/helpers.py` & `python-semantic-release-8.0.4/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.4/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.4/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/version/declaration.py` & `python-semantic-release-8.0.4/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/version/translator.py` & `python-semantic-release-8.0.4/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/semantic_release/version/version.py` & `python-semantic-release-8.0.4/semantic_release/version/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,17 @@
             )
             + ")"
         )
 
     def as_tag(self) -> str:
         return self.tag_format.format(version=str(self))
 
+    def as_semver_tag(self) -> str:
+        return "v{version}".format(version=str(self))
+
     def bump(self, level: LevelBump) -> Version:
         """
         Return a new Version instance according to the level specified to bump.
         Note this will intentionally drop the build metadata - that should be added
         elsewhere for the specific build producing this version.
         """
         if type(level) != LevelBump:
```

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.4/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.4/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_help.py` & `python-semantic-release-8.0.4/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_main.py` & `python-semantic-release-8.0.4/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_publish.py` & `python-semantic-release-8.0.4/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/command_line/test_version.py` & `python-semantic-release-8.0.4/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.4/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/fixtures/example_project.py` & `python-semantic-release-8.0.4/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.4/tests/fixtures/git_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -938,14 +938,97 @@
     assert git_repo.commit("v1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
     assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
+def repo_with_git_flow_and_release_channels_angular_commits_using_tag_format(
+    git_repo_factory, file_in_repo
+):
+    git_repo = git_repo_factory()
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="Initial commit")
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.1.0"))
+    git_repo.git.tag("vpy0.1.0", m="vpy0.1.0")
+
+    # Do a prerelease
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="fix: add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.1.1-rc.1"))
+    git_repo.git.tag("vpy0.1.1-rc.1", m="vpy0.1.1-rc.1")
+
+    # Do a prerelease
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="feat!: add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.0.0-rc.1"))
+    git_repo.git.tag("vpy1.0.0-rc.1", m="vpy1.0.0-rc.1")
+
+    # Do a full release
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="feat: add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.0.0"))
+    git_repo.git.tag("vpy1.0.0", m="vpy1.0.0")
+
+    assert git_repo.commit("vpy1.0.0").hexsha == git_repo.head.commit.hexsha
+
+    # Suppose branch "dev" has prerelease suffix of "rc"
+    git_repo.create_head("dev")
+    git_repo.heads.dev.checkout()
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="feat: (dev) add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-rc.1"))
+    git_repo.git.tag("vpy1.1.0-rc.1", m="vpy1.1.0-rc.1")
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="fix: (dev) add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-rc.2"))
+    git_repo.git.tag("vpy1.1.0-rc.2", m="vpy1.1.0-rc.2")
+
+    assert git_repo.commit("vpy1.1.0-rc.2").hexsha == git_repo.head.commit.hexsha
+
+    # Suppose branch "feature" has prerelease suffix of "alpha"
+    git_repo.create_head("feature")
+    git_repo.heads.feature.checkout()
+
+    # Do a prerelease on the branch
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="feat: (feature) add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.1"))
+    git_repo.git.tag("vpy1.1.0-alpha.1", m="vpy1.1.0-alpha.1")
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="feat: (feature) add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.2"))
+    git_repo.git.tag("vpy1.1.0-alpha.2", m="vpy1.1.0-alpha.2")
+
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m="fix: (feature) add some more text")
+    add_text_to_file(git_repo, file_in_repo)
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.3"))
+    git_repo.git.tag("vpy1.1.0-alpha.3", m="vpy1.1.0-alpha.3")
+
+    assert git_repo.commit("vpy1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
+    yield git_repo
+    git_repo.close()
+
+
+@pytest.fixture
 def repo_with_git_flow_and_release_channels_emoji_commits(
     git_repo_factory, file_in_repo
 ):
     git_repo = git_repo_factory()
 
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="Initial commit")
```

### Comparing `python-semantic-release-8.0.3/tests/fixtures/scipy.py` & `python-semantic-release-8.0.4/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.4/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.4/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.4/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_util.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.4/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

