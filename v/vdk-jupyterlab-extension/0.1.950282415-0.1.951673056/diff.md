# Comparing `tmp/vdk_jupyterlab_extension-0.1.950282415.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.951673056.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.950282415.tar` & `vdk_jupyterlab_extension-0.1.951673056.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/install.json
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jest.config.js
--rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/package-lock.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/tsconfig.json
--rw-r--r--   0        0        0   425098 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/schema/plugin.json
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/handler.ts
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/index.ts
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/jobData.ts
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/vdkTags.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/props.tsx
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/testutils/jest-file-mock.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/convert-job.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/convert_job.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    21084 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/remoteEntry.74be29b03cb2d5a0e3ab.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_directory_archiver.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jest.config.js
+-rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/package-lock.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/tsconfig.json
+-rw-r--r--   0        0        0   425098 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/schema/plugin.json
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/handler.ts
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/index.ts
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/props.tsx
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    21084 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/remoteEntry.c52cf3d95e66ca429f2e.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/LICENSE
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/pyproject.toml
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.951673056/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/jest.config.js` & `vdk_jupyterlab_extension-0.1.951673056/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/package-lock.json` & `vdk_jupyterlab_extension-0.1.951673056/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/package.json` & `vdk_jupyterlab_extension-0.1.951673056/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.951673056'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.950282415"
+    "version": "0.1.951673056"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/tsconfig.json` & `vdk_jupyterlab_extension-0.1.951673056/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/yarn.lock` & `vdk_jupyterlab_extension-0.1.951673056/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3304,17 +3304,17 @@
 
 camelcase@^6.0.0, camelcase@^6.2.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-6.3.0.tgz#5685b95eb209ac9c0c177467778c9c84df58ba9a"
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001517:
-  version "1.0.30001517"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz#90fabae294215c3495807eb24fc809e11dc2f0a8"
-  integrity sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==
+  version "1.0.30001518"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001518.tgz#b3ca93904cb4699c01218246c4d77a71dbe97150"
+  integrity sha512-rup09/e3I0BKjncL+FesTayKtPrdwKhUufQFd3riFw1hHg8JmIFoInYfB102cFcY/pPgGmdyl/iy+jgiDi2vdA==
 
 capture-exit@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/capture-exit/-/capture-exit-2.0.0.tgz#fb953bfaebeb781f62898239dabb426d08a509a4"
   integrity sha512-PiT/hQmTonHhl/HFGN+Lx3JJUznrVYJ3+AQsnthneZbvW7x+f08Tk7yLJTLEOUvBTbduLeeBkxEaYXUOUrRq6g==
   dependencies:
     rsvp "^4.8.4"
@@ -3896,17 +3896,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.477:
-  version "1.4.477"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.477.tgz#05669aa6f161ee9076a6805457e9bd9fe6d0dfd1"
-  integrity sha512-shUVy6Eawp33dFBFIoYbIwLHrX0IZ857AlH9ug2o4rvbWmpaCUdBpQ5Zw39HRrfzAFm4APJE9V+E2A/WB0YqJw==
+  version "1.4.479"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.479.tgz#ec9f676f23d3a0b0e429bc454d25e0b3253d2118"
+  integrity sha512-ABv1nHMIR8I5n3O3Een0gr6i0mfM+YcTZqjHy3pAYaOjgFG+BMquuKrSyfYf5CbEkLr9uM05RA3pOk4udNB/aQ==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.951673056/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/handler.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/index.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/initVDKConfigCell.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/handler.spec.ts`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import { ServerConnection } from '@jupyterlab/services';
 import { requestAPI } from '../handler';
 
 jest.mock('@jupyterlab/services', () => {
   const originalModule = jest.requireActual('@jupyterlab/services');
   const mockServerConnection = {
     makeSettings: jest.fn(
-      () => ({ baseUrl: 'https://example.com' } as ServerConnection.ISettings)
+      () => ({ baseUrl: 'https://example.com' }) as ServerConnection.ISettings
     ),
     makeRequest: jest.fn(() =>
       Promise.resolve(new Response(JSON.stringify({ message: 'OK' })))
     )
   };
   return {
     ...originalModule,
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.951673056/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.951673056/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/style/base.css` & `vdk_jupyterlab_extension-0.1.951673056/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.951673056/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.951673056/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.951673056/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.951673056/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/convert-job.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/convert-job.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py` & `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/convert_job.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/convert_job.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c52cf3d95e66ca429f2e.js'}}",*

 * * "'version'": "'0.1.951673056'"}*

```diff
@@ -79,15 +79,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.74be29b03cb2d5a0e3ab.js",
+            "load": "static/remoteEntry.c52cf3d95e66ca429f2e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -152,9 +152,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.950282415"
+    "version": "0.1.951673056"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.951673056'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.950282415"
+    "version": "0.1.951673056"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/remoteEntry.74be29b03cb2d5a0e3ab.js` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/remoteEntry.c52cf3d95e66ca429f2e.js`

 * *Files 0% similar despite different names*

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
-                })("vdk-jupyterlab-extension", "0.1.950282415"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.951673056"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_directory_archiver.py` & `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_directory_archiver.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/.gitignore` & `vdk_jupyterlab_extension-0.1.951673056/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/README.md` & `vdk_jupyterlab_extension-0.1.951673056/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # vdk-jupyterlab-extension
 
 A Jupyterlab extension for using VDK
 For more information see: https://github.com/vmware/versatile-data-kit/tree/main/specs/vep-994-jupyter-notebook-integration
 
 This extension is composed of a Python package named `vdk-jupyterlab-extension`
-for the server extension and a NPM package named `vdk-jupyterlab-extension`
-for the frontend extension.
+for the server extension and a NPM package named `vdk-jupyterlab-extension` for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 3.0
 - python ~=3.7
 - Versatile Data Kit
 - npm
@@ -44,43 +43,31 @@
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
 If you are struggling with a particular aspect of the JupyterLab API,
-you can contact the Jupyter team in the following way: go to their repo
-(https://github.com/jupyterlab/jupyterlab), go to Issues, go to New issue,
+you can contact the Jupyter team in the following way: go to their repo issues page at
+https://github.com/jupyterlab/jupyterlab/issues/new/choose
 then click on Open in the "Chat with the devs" section, which will send you
 to a Gitter channel where you can ask your question.
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
-# Clone the repo to your local environment
-# Change directory to the vdk-jupyterlab-extension directory
-# Once in the project directory, use the npm ci command to install
-# the exact versions of the dependencies specified in the package-lock.json
-npm ci
-# Install package in development mode
-pip install -e .
-# Link your development version of the extension with JupyterLab
-jupyter labextension develop . --overwrite
-# Server extension must be manually installed in develop mode
-jupyter server extension enable vdk-jupyterlab-extension
-# Rebuild extension Typescript source after making changes
-jlpm build
+../cicd/build.sh
 ```
 
 NB: If you're changing some dependencies of the project,
 meaning you're adding, removing, or updating packages, you'd use npm install.
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
```

### Comparing `vdk_jupyterlab_extension-0.1.950282415/pyproject.toml` & `vdk_jupyterlab_extension-0.1.951673056/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.950282415/PKG-INFO` & `vdk_jupyterlab_extension-0.1.951673056/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.950282415
+Version: 0.1.951673056
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
@@ -36,16 +36,15 @@
 
 # vdk-jupyterlab-extension
 
 A Jupyterlab extension for using VDK
 For more information see: https://github.com/vmware/versatile-data-kit/tree/main/specs/vep-994-jupyter-notebook-integration
 
 This extension is composed of a Python package named `vdk-jupyterlab-extension`
-for the server extension and a NPM package named `vdk-jupyterlab-extension`
-for the frontend extension.
+for the server extension and a NPM package named `vdk-jupyterlab-extension` for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 3.0
 - python ~=3.7
 - Versatile Data Kit
 - npm
@@ -80,43 +79,31 @@
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
 If you are struggling with a particular aspect of the JupyterLab API,
-you can contact the Jupyter team in the following way: go to their repo
-(https://github.com/jupyterlab/jupyterlab), go to Issues, go to New issue,
+you can contact the Jupyter team in the following way: go to their repo issues page at
+https://github.com/jupyterlab/jupyterlab/issues/new/choose
 then click on Open in the "Chat with the devs" section, which will send you
 to a Gitter channel where you can ask your question.
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
-# Clone the repo to your local environment
-# Change directory to the vdk-jupyterlab-extension directory
-# Once in the project directory, use the npm ci command to install
-# the exact versions of the dependencies specified in the package-lock.json
-npm ci
-# Install package in development mode
-pip install -e .
-# Link your development version of the extension with JupyterLab
-jupyter labextension develop . --overwrite
-# Server extension must be manually installed in develop mode
-jupyter server extension enable vdk-jupyterlab-extension
-# Rebuild extension Typescript source after making changes
-jlpm build
+../cicd/build.sh
 ```
 
 NB: If you're changing some dependencies of the project,
 meaning you're adding, removing, or updating packages, you'd use npm install.
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
```

