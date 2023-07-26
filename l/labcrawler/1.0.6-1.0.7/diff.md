# Comparing `tmp/labcrawler-1.0.6.tar.gz` & `tmp/labcrawler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-1.0.6.tar", last modified: Tue Jul  4 04:27:39 2023, max compression
+gzip compressed data, was "labcrawler-1.0.7.tar", last modified: Wed Jul 26 04:27:36 2023, max compression
```

## Comparing `labcrawler-1.0.6.tar` & `labcrawler-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-04 04:26:51.000000 labcrawler-1.0.6/.version
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-04 04:27:30.000000 labcrawler-1.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-04 04:27:30.000000 labcrawler-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15062 2023-07-04 04:27:39.232059 labcrawler-1.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14780 2023-07-04 04:27:30.000000 labcrawler-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.229059 labcrawler-1.0.6/labcrawler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     4288 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/_legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.231059 labcrawler-1.0.6/labcrawler/analyzers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/analyzers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/analyzers/gitlab_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     6271 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.231059 labcrawler-1.0.6/labcrawler/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/gitlab_ci_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/gitlab_repository_files_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/project_data_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab_ci_data_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/labcrawler/templates/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/labcrawler.json.template
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.230059 labcrawler-1.0.6/labcrawler.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15062 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-04 04:27:30.000000 labcrawler-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 04:27:39.232059 labcrawler-1.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/test/
--rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-04 04:27:30.000000 labcrawler-1.0.6/test/test_gitlab_ci_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.685319 labcrawler-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-26 04:26:45.000000 labcrawler-1.0.7/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-26 04:27:27.000000 labcrawler-1.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-26 04:27:27.000000 labcrawler-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15071 2023-07-26 04:27:36.685319 labcrawler-1.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14789 2023-07-26 04:27:27.000000 labcrawler-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.682319 labcrawler-1.0.7/labcrawler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/_legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.683319 labcrawler-1.0.7/labcrawler/analyzers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/analyzers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/analyzers/gitlab_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.684319 labcrawler-1.0.7/labcrawler/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/gitlab/gitlab_ci_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/gitlab/gitlab_repository_files_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/gitlab/project_data_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/gitlab_ci_data_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.684319 labcrawler-1.0.7/labcrawler/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/templates/labcrawler.json.template
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-07-26 04:27:27.000000 labcrawler-1.0.7/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.683319 labcrawler-1.0.7/labcrawler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15071 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 04:27:36.000000 labcrawler-1.0.7/labcrawler.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-26 04:27:27.000000 labcrawler-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 04:27:36.685319 labcrawler-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 04:27:36.684319 labcrawler-1.0.7/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-26 04:27:27.000000 labcrawler-1.0.7/test/test_gitlab_ci_config.py
```

### Comparing `labcrawler-1.0.6/LICENSE` & `labcrawler-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/PKG-INFO` & `labcrawler-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: labcrawler
-Version: 1.0.6
-Summary: Analysis tool for GitLab project and CI configurations
-Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 Summary
 -------
 
-*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
-
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
-Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
+Assumes the use of the GitLab "ultimate" paid tier, as it looks for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
 
 Installation
 ------------
 
 Install LabCrawler using `pipx`. [Install `pipx` first if necessary.](https://pypa.github.io/pipx/#install-pipx)
@@ -63,24 +51,22 @@
 
 The output from the `init` command includes the location of the LabCrawler config file (`labcrawler.json`). Edit the file with the following information:
 
 - `api_url` - URL to the root of the GitLab API, including `https://`.
 - `groups` - All the groups containing projects that you wish to examine. LabCrawler will not examine subgroups, so include them too.
 - `output_dir` - Directory to store the CSV files that are generated; the default is based on the OS and might be sufficient.
 
-*TODO: Note about the GitLab private token*
-
 Meltano loading
 ---------------
 
 LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in analyzer.
 
 Generating the CSV files requires two phases: `melt` and `load`.
 
-To run the Meltano load, issue the following command:
+To run Meltano, issue the following command:
 
 ```
 labcrawler melt
 ```
 
 The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation](https://docs.gitlab.com/ee/api/api_resources.html) to understand the fields. Data loaded includes:
     - `groups`
@@ -149,92 +135,93 @@
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
 # List the projects
-projects
+gitlab.projects
 
 # See what columns are available in any table
-projects.columns
+gitlab.projects.columns
 
 # View just certain columns from a table
-projects[['name','merge_method']]
+gitlab.projects[['name','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_method'])
+gitlab.projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
-len(branches.loc[~branches['merged']])
+len(gitlab.branches.loc[~gitlab.branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_name'])
+gitlab.branches.loc[~gitlab.branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
+gitlab.project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
-group_members.value_counts(['access_level_name'])
+gitlab.group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # Which projects use a non-default location for CI configuration?
-projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
+gitlab.projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
 
 # Which projects have CI configuration at all?
-ci_config_paths.query("main.notnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.notnull()")[['project_name']]
 
 # Projects without any CI configuration
-ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # Local CI configuration includes
-ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
+gitlab.ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
-ci_config_committers[['committer_name','project_name']]
+gitlab.ci_config_committers[['committer_name','project_name']]
 
 ```
 
 LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
->>> neat(projects[['name_with_namespace','merge_method']])
+>>> neat(gitlab.projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
 Steampunk Wizard / WizLib                                    merge
 Steampunk Wizard / FileWiz                                   merge
 Steampunk Wizard / LabCrawler                                merge
 Steampunk Wizard / Busy                                      merge
 ```
 
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
+- Redesign it to work within GitLab CI/CD
+- Undo the hack that allows for large group lists
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
 - Fix everything to use the `logger` instead of `print()`.
 - Add a command (`labcrawler info`?) to get e.g. locations of config and output files.
 - Load information about [external main CI configuration files](https://docs.gitlab.com/ee/ci/pipelines/settings.html#specify-a-custom-cicd-configuration-file)
 - Load information about external included CI configuration files
 - Load CI configuration includes recursively, so if an included CI config includes another one, it's loaded also
 - Pull committer information for included and external CI configuration files
 - "Crawl" through subgroups at the beginning, to get all the groups and projects within a portfolio
 - Add one command to combine `crawl`, `melt`, and `load`
 - Enable designation of groups and/or projects as options in the CLI
 - Provide a Dockerfile for easy deployment
-- Set it up to run inside GitLab CI
 - Integrate with Jupyter Notebook to make querying easier
 - Generate useful reports (in GitLab Pages? Conflucence?)
 - Read the CI configuration and smartly explain what it includes
 - Add (in reports, analysis, Jupyter, etc) clear explanations of what each field means (so users new to GitLab can understand more quickly)
 - Provide a test bed for LabCrawler itself, including a GitLab instance with test groups/projects
 - Contribute some or all of LabCrawler's custom queries back to tap-gitlab
 
@@ -279,15 +266,15 @@
 -----------
 
 1. Make sure you have Python 3.8+ and Pip installed
 2. Make a GitLab account and give it your SSH public key
 3. Follow the steps below (YMMV, from memory, please update if I missed anything)
 
 ```
-git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+git clone git@gitlab.com:steampunk-wizard/projects/labcrawler.git
 cd labcrawler
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements/freeze.txt
 ```
 
 Then to run it:
```

### Comparing `labcrawler-1.0.6/README.md` & `labcrawler-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+Metadata-Version: 2.1
+Name: labcrawler
+Version: 1.0.7
+Summary: Analysis tool for GitLab project and CI configurations
+Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 Summary
 -------
 
-*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
-
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
-Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
+Assumes the use of the GitLab "ultimate" paid tier, as it looks for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
 
 Installation
 ------------
 
 Install LabCrawler using `pipx`. [Install `pipx` first if necessary.](https://pypa.github.io/pipx/#install-pipx)
@@ -53,24 +61,22 @@
 
 The output from the `init` command includes the location of the LabCrawler config file (`labcrawler.json`). Edit the file with the following information:
 
 - `api_url` - URL to the root of the GitLab API, including `https://`.
 - `groups` - All the groups containing projects that you wish to examine. LabCrawler will not examine subgroups, so include them too.
 - `output_dir` - Directory to store the CSV files that are generated; the default is based on the OS and might be sufficient.
 
-*TODO: Note about the GitLab private token*
-
 Meltano loading
 ---------------
 
 LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in analyzer.
 
 Generating the CSV files requires two phases: `melt` and `load`.
 
-To run the Meltano load, issue the following command:
+To run Meltano, issue the following command:
 
 ```
 labcrawler melt
 ```
 
 The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation](https://docs.gitlab.com/ee/api/api_resources.html) to understand the fields. Data loaded includes:
     - `groups`
@@ -139,92 +145,93 @@
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
 # List the projects
-projects
+gitlab.projects
 
 # See what columns are available in any table
-projects.columns
+gitlab.projects.columns
 
 # View just certain columns from a table
-projects[['name','merge_method']]
+gitlab.projects[['name','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_method'])
+gitlab.projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
-len(branches.loc[~branches['merged']])
+len(gitlab.branches.loc[~gitlab.branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_name'])
+gitlab.branches.loc[~gitlab.branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
+gitlab.project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
-group_members.value_counts(['access_level_name'])
+gitlab.group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # Which projects use a non-default location for CI configuration?
-projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
+gitlab.projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
 
 # Which projects have CI configuration at all?
-ci_config_paths.query("main.notnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.notnull()")[['project_name']]
 
 # Projects without any CI configuration
-ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # Local CI configuration includes
-ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
+gitlab.ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
-ci_config_committers[['committer_name','project_name']]
+gitlab.ci_config_committers[['committer_name','project_name']]
 
 ```
 
 LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
->>> neat(projects[['name_with_namespace','merge_method']])
+>>> neat(gitlab.projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
 Steampunk Wizard / WizLib                                    merge
 Steampunk Wizard / FileWiz                                   merge
 Steampunk Wizard / LabCrawler                                merge
 Steampunk Wizard / Busy                                      merge
 ```
 
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
+- Redesign it to work within GitLab CI/CD
+- Undo the hack that allows for large group lists
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
 - Fix everything to use the `logger` instead of `print()`.
 - Add a command (`labcrawler info`?) to get e.g. locations of config and output files.
 - Load information about [external main CI configuration files](https://docs.gitlab.com/ee/ci/pipelines/settings.html#specify-a-custom-cicd-configuration-file)
 - Load information about external included CI configuration files
 - Load CI configuration includes recursively, so if an included CI config includes another one, it's loaded also
 - Pull committer information for included and external CI configuration files
 - "Crawl" through subgroups at the beginning, to get all the groups and projects within a portfolio
 - Add one command to combine `crawl`, `melt`, and `load`
 - Enable designation of groups and/or projects as options in the CLI
 - Provide a Dockerfile for easy deployment
-- Set it up to run inside GitLab CI
 - Integrate with Jupyter Notebook to make querying easier
 - Generate useful reports (in GitLab Pages? Conflucence?)
 - Read the CI configuration and smartly explain what it includes
 - Add (in reports, analysis, Jupyter, etc) clear explanations of what each field means (so users new to GitLab can understand more quickly)
 - Provide a test bed for LabCrawler itself, including a GitLab instance with test groups/projects
 - Contribute some or all of LabCrawler's custom queries back to tap-gitlab
 
@@ -269,15 +276,15 @@
 -----------
 
 1. Make sure you have Python 3.8+ and Pip installed
 2. Make a GitLab account and give it your SSH public key
 3. Follow the steps below (YMMV, from memory, please update if I missed anything)
 
 ```
-git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+git clone git@gitlab.com:steampunk-wizard/projects/labcrawler.git
 cd labcrawler
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements/freeze.txt
 ```
 
 Then to run it:
```

### Comparing `labcrawler-1.0.6/labcrawler/_legacy.py` & `labcrawler-1.0.7/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/labcrawler/analyzers/gitlab_analyzer.py` & `labcrawler-1.0.7/labcrawler/analyzers/gitlab_analyzer.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/labcrawler/cli.py` & `labcrawler-1.0.7/labcrawler/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import logging
 import sys
 import os
 
 from platformdirs import user_data_dir
 from platformdirs import user_documents_dir
 import pandas
+import yaml
 
 from labcrawler.analyzers.gitlab_analyzer import GitLabAnalyzer
 from labcrawler.gitlab_ci_data_loader import GitLabCIDataLoader
 from labcrawler.analyzers.gitlab_analyzer import output_neat
 
 APPNAME = "LabCrawler"
 APPAUTHOR = "SteampunkWizard"
@@ -128,21 +129,30 @@
     def melt(self, namespace):
         """Load all the data via meltano"""
         if not self.workspace.exists():
             raise RuntimeError("Use the init command first")
         output_dir = self.config['output_dir']
         self.clear_dir("previous output", Path(output_dir))
         chdir(self.workspace)
-        for source in SOURCES:
+        for source in SOURCES: # FAKE: we only really support 1 source
             csv_dir = Path(output_dir) / source
             csv_dir.mkdir()
             self.grab_token()
             environ['OUTPUT_DIR'] = str(csv_dir)
             environ['GITLAB_API_URL'] = self.config['api_url']
-            environ['GITLAB_GROUPS'] = ' '.join(self.config['groups'])
+
+            # HACK: Work with longer lists of groups - insert a list into the YAML
+            # environ['GITLAB_GROUPS'] = ' '.join(self.config['groups'])
+            groups = self.config['groups']
+            with open('meltano.yml') as file:
+                myaml = yaml.load(file, Loader=yaml.Loader)
+            myaml['plugins']['extractors'][0]['config']['groups'] = groups
+            with open('meltano.yml', 'w') as file:
+                file.write(yaml.dump(myaml))
+
             run(['meltano','run','tap-gitlab','target-csv'])
         print(f"Output is in {output_dir}")
 
     def load(self, namespace):
         """Load CI includes (and later blames), not covered by meltano"""
         # Cheap and easy cli argument: give me PROJECT_ID to limit scope
         self.grab_token()
```

### Comparing `labcrawler-1.0.6/labcrawler/gitlab/gitlab_ci_config.py` & `labcrawler-1.0.7/labcrawler/gitlab/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/labcrawler/gitlab/gitlab_repository_files_extractor.py` & `labcrawler-1.0.7/labcrawler/gitlab/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.7/labcrawler/gitlab_ci_data_loader.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/labcrawler/templates/meltano.yml` & `labcrawler-1.0.7/labcrawler/templates/meltano.yml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 default_environment: main
 environments:
   - name: main
 plugins:
   extractors:
   - name: tap-gitlab
     variant: meltanolabs
-    pip_url: git+https://github.com/MeltanoLabs/tap-gitlab.git
+    pip_url: git+https://gitlab.com/steampunk-wizard/forks/tap-gitlab.git
     config:
       api_url: $GITLAB_API_URL
       private_token: $GITLAB_PRIVATE_TOKEN
       groups: $GITLAB_GROUPS
       ultimate_license: true
       start_date: '2000-01-01T00:00:00Z'
     select:
```

### Comparing `labcrawler-1.0.6/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.7/labcrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Summary
 -------
 
-*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
-
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
-Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
+Assumes the use of the GitLab "ultimate" paid tier, as it looks for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
 
 Installation
 ------------
 
 Install LabCrawler using `pipx`. [Install `pipx` first if necessary.](https://pypa.github.io/pipx/#install-pipx)
@@ -63,24 +61,22 @@
 
 The output from the `init` command includes the location of the LabCrawler config file (`labcrawler.json`). Edit the file with the following information:
 
 - `api_url` - URL to the root of the GitLab API, including `https://`.
 - `groups` - All the groups containing projects that you wish to examine. LabCrawler will not examine subgroups, so include them too.
 - `output_dir` - Directory to store the CSV files that are generated; the default is based on the OS and might be sufficient.
 
-*TODO: Note about the GitLab private token*
-
 Meltano loading
 ---------------
 
 LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in analyzer.
 
 Generating the CSV files requires two phases: `melt` and `load`.
 
-To run the Meltano load, issue the following command:
+To run Meltano, issue the following command:
 
 ```
 labcrawler melt
 ```
 
 The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation](https://docs.gitlab.com/ee/api/api_resources.html) to understand the fields. Data loaded includes:
     - `groups`
@@ -149,92 +145,93 @@
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
 # List the projects
-projects
+gitlab.projects
 
 # See what columns are available in any table
-projects.columns
+gitlab.projects.columns
 
 # View just certain columns from a table
-projects[['name','merge_method']]
+gitlab.projects[['name','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_method'])
+gitlab.projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
-len(branches.loc[~branches['merged']])
+len(gitlab.branches.loc[~gitlab.branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_name'])
+gitlab.branches.loc[~gitlab.branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
+gitlab.project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
-group_members.value_counts(['access_level_name'])
+gitlab.group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
+gitlab.group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # Which projects use a non-default location for CI configuration?
-projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
+gitlab.projects.query("ci_config_path.notnull()")[['name','ci_config_path']]
 
 # Which projects have CI configuration at all?
-ci_config_paths.query("main.notnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.notnull()")[['project_name']]
 
 # Projects without any CI configuration
-ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
+gitlab.ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # Local CI configuration includes
-ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
+gitlab.ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
-ci_config_committers[['committer_name','project_name']]
+gitlab.ci_config_committers[['committer_name','project_name']]
 
 ```
 
 LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
->>> neat(projects[['name_with_namespace','merge_method']])
+>>> neat(gitlab.projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
 Steampunk Wizard / WizLib                                    merge
 Steampunk Wizard / FileWiz                                   merge
 Steampunk Wizard / LabCrawler                                merge
 Steampunk Wizard / Busy                                      merge
 ```
 
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
+- Redesign it to work within GitLab CI/CD
+- Undo the hack that allows for large group lists
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
 - Fix everything to use the `logger` instead of `print()`.
 - Add a command (`labcrawler info`?) to get e.g. locations of config and output files.
 - Load information about [external main CI configuration files](https://docs.gitlab.com/ee/ci/pipelines/settings.html#specify-a-custom-cicd-configuration-file)
 - Load information about external included CI configuration files
 - Load CI configuration includes recursively, so if an included CI config includes another one, it's loaded also
 - Pull committer information for included and external CI configuration files
 - "Crawl" through subgroups at the beginning, to get all the groups and projects within a portfolio
 - Add one command to combine `crawl`, `melt`, and `load`
 - Enable designation of groups and/or projects as options in the CLI
 - Provide a Dockerfile for easy deployment
-- Set it up to run inside GitLab CI
 - Integrate with Jupyter Notebook to make querying easier
 - Generate useful reports (in GitLab Pages? Conflucence?)
 - Read the CI configuration and smartly explain what it includes
 - Add (in reports, analysis, Jupyter, etc) clear explanations of what each field means (so users new to GitLab can understand more quickly)
 - Provide a test bed for LabCrawler itself, including a GitLab instance with test groups/projects
 - Contribute some or all of LabCrawler's custom queries back to tap-gitlab
 
@@ -279,15 +276,15 @@
 -----------
 
 1. Make sure you have Python 3.8+ and Pip installed
 2. Make a GitLab account and give it your SSH public key
 3. Follow the steps below (YMMV, from memory, please update if I missed anything)
 
 ```
-git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+git clone git@gitlab.com:steampunk-wizard/projects/labcrawler.git
 cd labcrawler
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements/freeze.txt
 ```
 
 Then to run it:
```

### Comparing `labcrawler-1.0.6/labcrawler.egg-info/SOURCES.txt` & `labcrawler-1.0.7/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/pyproject.toml` & `labcrawler-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.6/test/test_gitlab_ci_config.py` & `labcrawler-1.0.7/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*

