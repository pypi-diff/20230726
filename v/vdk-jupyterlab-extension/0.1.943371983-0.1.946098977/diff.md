# Comparing `tmp/vdk_jupyterlab_extension-0.1.943371983.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.946098977.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.943371983.tar` & `vdk_jupyterlab_extension-0.1.946098977.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/install.json
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jest.config.js
--rw-r--r--   0        0        0   637348 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/package-lock.json
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/tsconfig.json
--rw-r--r--   0        0        0   424494 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/schema/plugin.json
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/handler.ts
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/index.ts
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/jobData.ts
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/vdkTags.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/testutils/jest-file-mock.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/convert-job.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/convert_job.py
--rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    21604 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/remoteEntry.f9166f3ab54776548603.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_directory_archiver.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jest.config.js
+-rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/package-lock.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/tsconfig.json
+-rw-r--r--   0        0        0   425044 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/schema/plugin.json
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/handler.ts
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/index.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    21604 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/remoteEntry.c2eb77da248d9dc524fb.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.946098977/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/jest.config.js` & `vdk_jupyterlab_extension-0.1.946098977/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/package-lock.json` & `vdk_jupyterlab_extension-0.1.946098977/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999862881059471%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'word-wrap': '1.2.4'}}, 'node_modules/word-wrap': "*

 * *               "{'version': '1.2.4', 'resolved': "*

 * *               "'https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz', 'integrity': "*

 * *               "'sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA=='}}"}*

```diff
@@ -27,14 +27,15 @@
                 "@jupyterlab/statusbar": "3.6.3",
                 "@jupyterlab/testutils": "3.6.3",
                 "@jupyterlab/translation": "3.6.3",
                 "@jupyterlab/ui-components": "3.6.3",
                 "@lumino/widgets": "1.33.0",
                 "@types/react": "17.0.53",
                 "typescript": "4.1.3",
+                "word-wrap": "1.2.4",
                 "yjs": "^13.5.17"
             },
             "devDependencies": {
                 "@babel/core": "7.8.0",
                 "@babel/preset-env": "7.0.0",
                 "@testing-library/react": "12.1.5",
                 "@types/enzyme": "3.10.12",
@@ -16240,17 +16241,17 @@
             "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.1.tgz",
             "version": "2.0.1"
         },
         "node_modules/word-wrap": {
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==",
-            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz",
-            "version": "1.2.3"
+            "integrity": "sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA==",
+            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz",
+            "version": "1.2.4"
         },
         "node_modules/worker-loader": {
             "dependencies": {
                 "loader-utils": "^2.0.0",
                 "schema-utils": "^3.0.0"
             },
             "engines": {
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/package.json` & `vdk_jupyterlab_extension-0.1.946098977/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9764890282131661%*

 * *Differences: {"'dependencies'": "{'word-wrap': '1.2.4'}", "'version'": "'0.1.946098977'"}*

```diff
@@ -30,14 +30,15 @@
         "@jupyterlab/statusbar": "3.6.3",
         "@jupyterlab/testutils": "3.6.3",
         "@jupyterlab/translation": "3.6.3",
         "@jupyterlab/ui-components": "3.6.3",
         "@lumino/widgets": "1.33.0",
         "@types/react": "17.0.53",
         "typescript": "4.1.3",
+        "word-wrap": "1.2.4",
         "yjs": "^13.5.17"
     },
     "description": "A Jupyterlab extension for using VDK",
     "devDependencies": {
         "@babel/core": "7.8.0",
         "@babel/preset-env": "7.0.0",
         "@testing-library/react": "12.1.5",
@@ -146,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.943371983"
+    "version": "0.1.946098977"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/tsconfig.json` & `vdk_jupyterlab_extension-0.1.946098977/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/yarn.lock` & `vdk_jupyterlab_extension-0.1.946098977/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2401,17 +2401,17 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
   integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.44.0"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.44.0.tgz#55818eabb376e2272f77fbf5c96c43137c3c1e53"
-  integrity sha512-gsF+c/0XOguWgaOgvFs+xnnRqt9GwgTvIks36WpE6ueeI4KCEHHd8K/CKHqhOqrJKsYH8m27kRzQEvWXAwXUTw==
+  version "8.44.1"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.44.1.tgz#d1811559bb6bcd1a76009e3f7883034b78a0415e"
+  integrity sha512-XpNDc4Z5Tb4x+SW1MriMVeIsMoONHCkWFMkR/aPJbzEsxqHy+4Glu/BqTdPrApfDeMaXbtNh6bseNgl5KaWrSg==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*", "@types/estree@^1.0.0":
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
@@ -2458,17 +2458,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "20.4.4"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.4.tgz#c79c7cc22c9d0e97a7944954c9e663bcbd92b0cb"
-  integrity sha512-CukZhumInROvLq3+b5gLev+vgpsIqC2D0deQr/yS1WnxvmYLlJXZpaQrQiseMY+6xusl79E04UjWoqyr+t1/Ew==
+  version "20.4.5"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.5.tgz#9dc0a5cb1ccce4f7a731660935ab70b9c00a5d69"
+  integrity sha512-rt40Nk13II9JwQBdeYqmbn2Q6IVTA5uPhvSO+JVqdXw/6/4glI6oR9ezty/A9Hg5u7JH4OmYmuQ+XvjKm0Datg==
 
 "@types/normalize-package-data@^2.4.0":
   version "2.4.1"
   resolved "https://registry.yarnpkg.com/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz#d3357479a0fdfdd5907fe67e17e0a85c906e1301"
   integrity sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==
 
 "@types/parse-json@^4.0.0":
@@ -3896,17 +3896,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.468"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.468.tgz#3cbf64ad67d9f12bfe69fefe5eb1935ec4f6ab7a"
-  integrity sha512-6M1qyhaJOt7rQtNti1lBA0GwclPH+oKCmsra/hkcWs5INLxfXXD/dtdnaKUYQu/pjOBP/8Osoe4mAcNvvzoFag==
+  version "1.4.471"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.471.tgz#14cb056d0ce4bfa99df57946d57fe46c2330dac3"
+  integrity sha512-GpmGRC1vTl60w/k6YpQ18pSiqnmr0j3un//5TV1idPi6aheNfkT1Ye71tMEabWyNDO6sBMgAR+95Eb0eUUr1tA==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -5431,35 +5431,35 @@
     "@babel/core" "^7.12.3"
     "@babel/parser" "^7.14.7"
     "@istanbuljs/schema" "^0.1.2"
     istanbul-lib-coverage "^3.2.0"
     semver "^6.3.0"
 
 istanbul-lib-report@^3.0.0:
-  version "3.0.0"
-  resolved "https://registry.yarnpkg.com/istanbul-lib-report/-/istanbul-lib-report-3.0.0.tgz#7518fe52ea44de372f460a76b5ecda9ffb73d8a6"
-  integrity sha512-wcdi+uAKzfiGT2abPpKZ0hSU1rGQjUQnLvtY5MpQ7QCTahD3VODhcu4wcfY1YtkGaDD5yuydOLINXsfbus9ROw==
+  version "3.0.1"
+  resolved "https://registry.yarnpkg.com/istanbul-lib-report/-/istanbul-lib-report-3.0.1.tgz#908305bac9a5bd175ac6a74489eafd0fc2445a7d"
+  integrity sha512-GCfE1mtsHGOELCU8e/Z7YWzpmybrx/+dSTfLrvY8qRmaY6zXTKWn6WQIjaAFw069icm6GVMNkgu0NzI4iPZUNw==
   dependencies:
     istanbul-lib-coverage "^3.0.0"
-    make-dir "^3.0.0"
+    make-dir "^4.0.0"
     supports-color "^7.1.0"
 
 istanbul-lib-source-maps@^4.0.0:
   version "4.0.1"
   resolved "https://registry.yarnpkg.com/istanbul-lib-source-maps/-/istanbul-lib-source-maps-4.0.1.tgz#895f3a709fcfba34c6de5a42939022f3e4358551"
   integrity sha512-n3s8EwkdFIJCG3BPKBYvskgXGoy88ARzvegkitk60NxRdwltLOTaH7CUiMRXvwYorl0Q712iEjcWB+fK/MrWVw==
   dependencies:
     debug "^4.1.1"
     istanbul-lib-coverage "^3.0.0"
     source-map "^0.6.1"
 
 istanbul-reports@^3.0.2, istanbul-reports@^3.1.3:
-  version "3.1.5"
-  resolved "https://registry.yarnpkg.com/istanbul-reports/-/istanbul-reports-3.1.5.tgz#cc9a6ab25cb25659810e4785ed9d9fb742578bae"
-  integrity sha512-nUsEMa9pBt/NOHqbcbeJEgqIlY/K7rVWUX6Lql2orY5e9roQOthbR3vtY4zzf2orPELg80fnxxk9zUyPlgwD1w==
+  version "3.1.6"
+  resolved "https://registry.yarnpkg.com/istanbul-reports/-/istanbul-reports-3.1.6.tgz#2544bcab4768154281a2f0870471902704ccaa1a"
+  integrity sha512-TLgnMkKg3iTDsQ9PbPTdpfAK2DzjF9mqUG7RMgcQl8oFjad8ob4laGxv5XV5U9MAfx8D6tSJiUyuAwzLicaxlg==
   dependencies:
     html-escaper "^2.0.0"
     istanbul-lib-report "^3.0.0"
 
 jest-changed-files@^26.6.2:
   version "26.6.2"
   resolved "https://registry.yarnpkg.com/jest-changed-files/-/jest-changed-files-26.6.2.tgz#f6198479e1cc66f22f9ae1e22acaa0b429c042d0"
@@ -6642,21 +6642,28 @@
   integrity sha512-AI2r85+4MquTw9ZYqabu4nMwy9Oftlfa/e/52t9IjtfG+mGBbTNdAoZ3RQKLHR6r0wQnwZnPIEh/Ya6XTWAKNA==
 
 lz-string@^1.5.0:
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/lz-string/-/lz-string-1.5.0.tgz#c1ab50f77887b712621201ba9fd4e3a6ed099941"
   integrity sha512-h5bgJWpxJNswbU7qCrV0tIKQCaS3blPDrqKWx+QxzuzL1zGUzij9XCWLrSLsJPu5t+eWA/ycetzYAO5IOMcWAQ==
 
-make-dir@^3.0.0, make-dir@^3.0.2:
+make-dir@^3.0.2:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/make-dir/-/make-dir-3.1.0.tgz#415e967046b3a7f1d185277d84aa58203726a13f"
   integrity sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==
   dependencies:
     semver "^6.0.0"
 
+make-dir@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.yarnpkg.com/make-dir/-/make-dir-4.0.0.tgz#c3c2307a771277cd9638305f915c29ae741b614e"
+  integrity sha512-hXdUTZYIVOt1Ex//jAQi+wTZZpUpwBj/0QsOzqegb3rGMMeJiSEu5xLHnYfBrRV4RH2+OCSOO95Is/7x1WJ4bw==
+  dependencies:
+    semver "^7.5.3"
+
 make-error@1.x:
   version "1.3.6"
   resolved "https://registry.yarnpkg.com/make-error/-/make-error-1.3.6.tgz#2eb2e37ea9b67c4891f684a1394799af484cf7a2"
   integrity sha512-s8UhlNe7vPKomQhC1qFelMokr/Sc3AgNbso3n74mVPA5LTZwkB9NlXf4XPamLxJE8h0gh73rM94xvwRT2CVInw==
 
 makeerror@1.0.12:
   version "1.0.12"
@@ -7930,15 +7937,15 @@
     ajv-keywords "^3.5.2"
 
 "semver@2 || 3 || 4 || 5", semver@^5.3.0, semver@^5.4.1, semver@^5.5.0:
   version "5.7.2"
   resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.2.tgz#48d55db737c3287cd4835e17fa13feace1c41ef8"
   integrity sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==
 
-semver@7.x, semver@^7.2.1, semver@^7.3.2, semver@^7.3.4, semver@^7.3.5:
+semver@7.x, semver@^7.2.1, semver@^7.3.2, semver@^7.3.4, semver@^7.3.5, semver@^7.5.3:
   version "7.5.4"
   resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.4.tgz#483986ec4ed38e1c6c48c34894a9182dbff68a6e"
   integrity sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==
   dependencies:
     lru-cache "^6.0.0"
 
 semver@^6.0.0, semver@^6.3.0, semver@^6.3.1:
@@ -9227,14 +9234,19 @@
     isexe "^2.0.0"
 
 wildcard@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.1.tgz#5ab10d02487198954836b6349f74fff961e10f67"
   integrity sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==
 
+word-wrap@1.2.4:
+  version "1.2.4"
+  resolved "https://registry.yarnpkg.com/word-wrap/-/word-wrap-1.2.4.tgz#cb4b50ec9aca570abd1f52f33cd45b6c61739a9f"
+  integrity sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA==
+
 worker-loader@^3.0.2:
   version "3.0.8"
   resolved "https://registry.yarnpkg.com/worker-loader/-/worker-loader-3.0.8.tgz#5fc5cda4a3d3163d9c274a4e3a811ce8b60dbb37"
   integrity sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==
   dependencies:
     loader-utils "^2.0.0"
     schema-utils "^3.0.0"
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.946098977/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/handler.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/index.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/initVDKConfigCell.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.946098977/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.946098977/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/style/base.css` & `vdk_jupyterlab_extension-0.1.946098977/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.946098977/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.946098977/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.946098977/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.946098977/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/convert-job.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/convert-job.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py` & `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/convert_job.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/convert_job.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761102403343783%*

 * *Differences: {"'dependencies'": "{'word-wrap': '1.2.4'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c2eb77da248d9dc524fb.js'}}",*

 * * "'version'": "'0.1.946098977'"}*

```diff
@@ -30,14 +30,15 @@
         "@jupyterlab/statusbar": "3.6.3",
         "@jupyterlab/testutils": "3.6.3",
         "@jupyterlab/translation": "3.6.3",
         "@jupyterlab/ui-components": "3.6.3",
         "@lumino/widgets": "1.33.0",
         "@types/react": "17.0.53",
         "typescript": "4.1.3",
+        "word-wrap": "1.2.4",
         "yjs": "^13.5.17"
     },
     "description": "A Jupyterlab extension for using VDK",
     "devDependencies": {
         "@babel/core": "7.8.0",
         "@babel/preset-env": "7.0.0",
         "@testing-library/react": "12.1.5",
@@ -78,15 +79,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f9166f3ab54776548603.js",
+            "load": "static/remoteEntry.c2eb77da248d9dc524fb.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -151,9 +152,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.943371983"
+    "version": "0.1.946098977"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9764890282131661%*

 * *Differences: {"'dependencies'": "{'word-wrap': '1.2.4'}", "'version'": "'0.1.946098977'"}*

```diff
@@ -30,14 +30,15 @@
         "@jupyterlab/statusbar": "3.6.3",
         "@jupyterlab/testutils": "3.6.3",
         "@jupyterlab/translation": "3.6.3",
         "@jupyterlab/ui-components": "3.6.3",
         "@lumino/widgets": "1.33.0",
         "@types/react": "17.0.53",
         "typescript": "4.1.3",
+        "word-wrap": "1.2.4",
         "yjs": "^13.5.17"
     },
     "description": "A Jupyterlab extension for using VDK",
     "devDependencies": {
         "@babel/core": "7.8.0",
         "@babel/preset-env": "7.0.0",
         "@testing-library/react": "12.1.5",
@@ -146,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.943371983"
+    "version": "0.1.946098977"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/remoteEntry.f9166f3ab54776548603.js` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/remoteEntry.c2eb77da248d9dc524fb.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => y.e(161).then((() => () => y(161))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.943371983"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.946098977"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_directory_archiver.py` & `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_directory_archiver.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/.gitignore` & `vdk_jupyterlab_extension-0.1.946098977/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/README.md` & `vdk_jupyterlab_extension-0.1.946098977/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/pyproject.toml` & `vdk_jupyterlab_extension-0.1.946098977/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.943371983/PKG-INFO` & `vdk_jupyterlab_extension-0.1.946098977/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.943371983
+Version: 0.1.946098977
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

