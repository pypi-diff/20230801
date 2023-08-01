# Comparing `tmp/wxai-langchain-0.0.2.tar.gz` & `tmp/wxai-langchain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxai-langchain-0.0.2.tar", last modified: Thu Jul 27 10:46:50 2023, max compression
+gzip compressed data, was "wxai-langchain-0.0.3.tar", last modified: Tue Aug  1 05:37:39 2023, max compression
```

## Comparing `wxai-langchain-0.0.2.tar` & `wxai-langchain-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.320000 wxai-langchain-0.0.2/
--rw-rw-rw-   0        0        0     3237 2023-07-27 10:11:54.000000 wxai-langchain-0.0.2/.gitignore
--rw-rw-rw-   0        0        0    11525 2023-07-27 09:46:48.000000 wxai-langchain-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      781 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-07-27 10:24:30.000000 wxai-langchain-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/examples/
--rw-rw-rw-   0        0        0    17233 2023-07-27 10:45:34.000000 wxai-langchain-0.0.2/examples/wxai_langchain_interface.ipynb
--rw-rw-rw-   0        0        0      798 2023-07-27 10:46:38.000000 wxai-langchain-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/wxai_langchain/
--rw-rw-rw-   0        0        0      157 2023-07-27 10:02:04.000000 wxai-langchain-0.0.2/src/wxai_langchain/__init__.py
--rw-rw-rw-   0        0        0     1204 2023-07-27 09:34:42.000000 wxai-langchain-0.0.2/src/wxai_langchain/credentials.py
--rw-rw-rw-   0        0        0     2316 2023-07-27 10:45:16.000000 wxai-langchain-0.0.2/src/wxai_langchain/llm.py
--rw-rw-rw-   0        0        0      875 2023-07-27 09:34:42.000000 wxai-langchain-0.0.2/src/wxai_langchain/prompt.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/
--rw-rw-rw-   0        0        0      781 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/top_level.txt
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-01 05:37:39.006442 wxai-langchain-0.0.3/
+-rw-r--r--   0 cong       (501) staff       (20)     3077 2023-08-01 04:34:29.000000 wxai-langchain-0.0.3/.gitignore
+-rw-r--r--   0 cong       (501) staff       (20)    11325 2023-08-01 04:34:29.000000 wxai-langchain-0.0.3/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)     1266 2023-08-01 05:37:39.005889 wxai-langchain-0.0.3/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      902 2023-08-01 05:36:25.000000 wxai-langchain-0.0.3/README.md
+-rw-r--r--   0 cong       (501) staff       (20)      902 2023-08-01 05:24:12.000000 wxai-langchain-0.0.3/pyproject.toml
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-08-01 05:37:39.006610 wxai-langchain-0.0.3/setup.cfg
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-01 05:37:38.998412 wxai-langchain-0.0.3/src/
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-01 05:37:39.002123 wxai-langchain-0.0.3/src/wxai_langchain/
+-rw-r--r--   0 cong       (501) staff       (20)      157 2023-08-01 04:34:29.000000 wxai-langchain-0.0.3/src/wxai_langchain/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1150 2023-08-01 05:09:45.000000 wxai-langchain-0.0.3/src/wxai_langchain/credentials.py
+-rw-r--r--   0 cong       (501) staff       (20)     2646 2023-08-01 05:10:27.000000 wxai-langchain-0.0.3/src/wxai_langchain/llm.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-08-01 05:37:39.005084 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)     1266 2023-08-01 05:37:38.000000 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      343 2023-08-01 05:37:38.000000 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-08-01 05:37:38.000000 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)      188 2023-08-01 05:37:38.000000 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       15 2023-08-01 05:37:38.000000 wxai-langchain-0.0.3/src/wxai_langchain.egg-info/top_level.txt
```

### Comparing `wxai-langchain-0.0.2/.gitignore` & `wxai-langchain-0.0.3/.gitignore`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-.idea/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+.idea/
```

### Comparing `wxai-langchain-0.0.2/LICENSE` & `wxai-langchain-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-  Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+  Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `wxai-langchain-0.0.2/PKG-INFO` & `wxai-langchain-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,54 @@
-Metadata-Version: 2.1
-Name: wxai-langchain
-Version: 0.0.2
-Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
-Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
-Keywords: watsonx.ai,wxai,langchain
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IBM watsonx.ai LangChain interface
-
-This is a Python library to add a LangChain interface to IBM watsonx.ai. This is not an IBM project and is not supported by IBM.
-
-To install,
-
-```shell
-pip install wxai-langchain
-```
-
-To use, see the examples folder. This LangChain interface is not compatible with IBM's GenAI GenerateParams schema object.
-Always use a JSON for the model's parameters as shown in the examples.
+Metadata-Version: 2.1
+Name: wxai-langchain
+Version: 0.0.3
+Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
+Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
+Keywords: watsonx.ai,wxai,langchain
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# IBM watsonx.ai LangChain interface
+
+This is a Python library to add a LangChain interface to IBM watsonx.ai. This is not an IBM project and is not supported by IBM.
+
+```shell
+pip install wxai-langchain==0.0.3
+```
+
+## v0.0.3
+
+Version 0.0.3 is a breaking change and uses ibm-watson-machine-learning SDK to use the syntatic sugars that comes with the SDK.
+
+```shell
+pip install -e '.[dev]'
+```
+
+Examples:
+
+1. Create a new `.env` file `examples/0.0.3` with contents
+
+```
+API_KEY=
+PROJECT_ID=
+```
+
+2. Run the examples with 
+
+```shell
+python examples/0.0.3/<example-file>.py
+```
+
+## v0.0.2
+
+Version 0.0.2 does not use ibm-watson-machine-learning SDK.
+
+To install,
+
+```shell
+pip install wxai-langchain==0.0.2
+```
+
+To use, see the examples folder. This LangChain interface is not compatible with IBM's GenAI GenerateParams schema object.
+Always use a JSON for the model's parameters as shown in the examples.
```

### Comparing `wxai-langchain-0.0.2/pyproject.toml` & `wxai-langchain-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-[build-system]
-requires = ["setuptools>=68.0.0", "wheel>=0.40.0", "setuptools_scm[toml]>=7.1.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "wxai-langchain"
-version = "0.0.2"
-authors = [
-  {name="Cong Nguyen", email="cong.nguyen@au1.ibm.com"}
-]
-keywords = ["watsonx.ai", "wxai", "langchain"]
-description = "wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM."
-readme = "README.md"
-dependencies = [
-    "urllib3<2", # https://github.com/psf/requests/issues/6432
-    "requests>=2.31.0",
-    "pydantic<=1.10.10",
-    "langchain>=0.0.200",
-    "ibm_cloud_sdk_core>=3.16.7",
-    "aiohttp>=3.8.4"
-]
-requires-python = ">=3.9"
-
-[options]
-package_dir=[
-  "src"
-]
-
-[options.packages.find]
-where=[
-  "src/genai"
+[build-system]
+requires = ["setuptools>=68.0.0", "wheel>=0.40.0", "setuptools_scm[toml]>=7.1.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "wxai-langchain"
+version = "0.0.3"
+authors = [
+  {name="Cong Nguyen", email="cong.nguyen@au1.ibm.com"}
+]
+keywords = ["watsonx.ai", "wxai", "langchain"]
+description = "wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM."
+readme = "README.md"
+dependencies = [
+    "urllib3<2", # https://github.com/psf/requests/issues/6432
+    "requests>=2.31.0",
+    "pydantic<=1.10.10",
+    "langchain>=0.0.200",
+    "ibm_cloud_sdk_core>=3.16.7",
+    "aiohttp>=3.8.4",
+    "ibm-watson-machine-learning>=1.0.311"
+]
+requires-python = ">=3.9"
+
+
+[project.optional-dependencies]
+dev = [
+  "python-dotenv>=1.0.0",
+  "datasets==2.11.0"
+]
+
+[options]
+package_dir=[
+  "src"
+]
+
+[options.packages.find]
+where=[
+  "src/genai"
 ]
```

### Comparing `wxai-langchain-0.0.2/src/wxai_langchain/credentials.py` & `wxai-langchain-0.0.3/src/wxai_langchain/credentials.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,13 @@
         self.api_key = api_key
         if api_endpoint is None:
             raise ValueError("api_endpoint must be provided")
         self.api_endpoint = api_endpoint
         if project_id is None:
             raise ValueError("project_id must be provided")
         self.project_id = project_id
-        
-    def get_access_token(self):
-        access_token = IAMTokenManager(
-            apikey = self.api_key,
-            url = "https://iam.cloud.ibm.com/identity/token"
-        ).get_token()
-        return access_token
+
+        # New dict for ibm-watson-machine-learning-sdk
+        self.wml_credentials = {
+            "apikey": self.api_key,
+            "url": self.api_endpoint
+        }
```

### Comparing `wxai-langchain-0.0.2/src/wxai_langchain/llm.py` & `wxai-langchain-0.0.3/src/wxai_langchain/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,43 +6,48 @@
 
 try:
     from langchain.llms.base import LLM
     from langchain.llms.utils import enforce_stop_tokens
 except ImportError:
     raise ImportError("Could not import langchain: Please install langchain.")
 
+from ibm_watson_machine_learning.foundation_models import Model
+from ibm_watson_machine_learning.metanames import GenTextParamsMetaNames as GenParams
+
 from wxai_langchain.credentials import Credentials
-from wxai_langchain.prompt import Prompt
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["LangChainInterface"]
 
 
 class LangChainInterface(LLM, BaseModel):
     """
     Wrapper around IBM watsonx.ai models.
 
         .. code-block:: python
-            llm = LangChainInterface(model="google/flan-ul2", credentials=creds)
+            from ibm_watson_machine_learning.foundation_models import Model
+            from ibm_watson_machine_learning.metanames import GenTextParamsMetaNames as GenParams
+
+            llm = LangChainInterface(model=ModelTypes.FLAN_UL2, params=generate_params, credentials=creds)
     """
 
     credentials: Credentials = None
     model: Optional[str] = None
     params: Optional[dict] = None
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         """Get the identifying parameters."""
-        _params = self.params or GenerateParams()
+        _params = self.params or GenParams()
         return {
             **{"model": self.model},
             **{"params": _params},
         }
 
     @property
     def _llm_type(self) -> str:
@@ -57,17 +62,21 @@
         Returns:
             The string generated by the model.
         Example:
             .. code-block:: python
                 llm = LangChainInterface(model_id="google/flan-ul2", credentials=creds)
                 response = llm("What is a molecule")
         """
-        params = self.params or GenerateParams()
+        params = self.params or GenParams()
+
+        wml_model = Model(
+            model_id=self.model,
+            params=params,
+            credentials=self.credentials.wml_credentials,
+            project_id=self.credentials.project_id
+        )
+        text = wml_model.generate_text(prompt, params)
 
-        access_token = self.credentials.get_access_token()
-        wml_prompt = Prompt(access_token, self.credentials.project_id, self.credentials.api_endpoint)
-        text = wml_prompt.generate(prompt, self.model, params)
-        
         logger.info("Output of watsonx.ai call: {}".format(text))
         if stop is not None:
             text = enforce_stop_tokens(text, stop)
         return text
```

### Comparing `wxai-langchain-0.0.2/src/wxai_langchain.egg-info/PKG-INFO` & `wxai-langchain-0.0.3/src/wxai_langchain.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,54 @@
-Metadata-Version: 2.1
-Name: wxai-langchain
-Version: 0.0.2
-Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
-Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
-Keywords: watsonx.ai,wxai,langchain
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IBM watsonx.ai LangChain interface
-
-This is a Python library to add a LangChain interface to IBM watsonx.ai. This is not an IBM project and is not supported by IBM.
-
-To install,
-
-```shell
-pip install wxai-langchain
-```
-
-To use, see the examples folder. This LangChain interface is not compatible with IBM's GenAI GenerateParams schema object.
-Always use a JSON for the model's parameters as shown in the examples.
+Metadata-Version: 2.1
+Name: wxai-langchain
+Version: 0.0.3
+Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
+Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
+Keywords: watsonx.ai,wxai,langchain
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# IBM watsonx.ai LangChain interface
+
+This is a Python library to add a LangChain interface to IBM watsonx.ai. This is not an IBM project and is not supported by IBM.
+
+```shell
+pip install wxai-langchain==0.0.3
+```
+
+## v0.0.3
+
+Version 0.0.3 is a breaking change and uses ibm-watson-machine-learning SDK to use the syntatic sugars that comes with the SDK.
+
+```shell
+pip install -e '.[dev]'
+```
+
+Examples:
+
+1. Create a new `.env` file `examples/0.0.3` with contents
+
+```
+API_KEY=
+PROJECT_ID=
+```
+
+2. Run the examples with 
+
+```shell
+python examples/0.0.3/<example-file>.py
+```
+
+## v0.0.2
+
+Version 0.0.2 does not use ibm-watson-machine-learning SDK.
+
+To install,
+
+```shell
+pip install wxai-langchain==0.0.2
+```
+
+To use, see the examples folder. This LangChain interface is not compatible with IBM's GenAI GenerateParams schema object.
+Always use a JSON for the model's parameters as shown in the examples.
```

