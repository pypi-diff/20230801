# Comparing `tmp/create_dara_app-1.0.0a1-py3-none-any.whl.zip` & `tmp/create_dara_app-1.0.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 266464 bytes, number of entries: 20
+Zip file size: 267584 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      658 b- defN 80-Jan-01 00:00 create_dara_app/__init__.py
--rw-r--r--  2.0 unx     2385 b- defN 80-Jan-01 00:00 create_dara_app/cli.py
+-rw-r--r--  2.0 unx     3129 b- defN 80-Jan-01 00:00 create_dara_app/cli.py
 -rw-r--r--  2.0 unx     3182 b- defN 80-Jan-01 00:00 create_dara_app/default_command_group.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 create_dara_app/templates/__init__.py
--rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/cookiecutter.json
--rw-r--r--  2.0 unx      705 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/hooks/post_gen_project.py
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/cookiecutter.json
+-rw-r--r--  2.0 unx     1245 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/hooks/post_gen_project.py
 -rw-r--r--  2.0 unx      294 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/hooks/pre_gen_project.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/.gitignore
--rw-r--r--  2.0 unx      635 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/README.md
--rw-r--r--  2.0 unx      695 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml
+-rw-r--r--  2.0 unx     1275 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/README.md
+-rw-r--r--  2.0 unx     1323 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml
 -rw-r--r--  2.0 unx   318043 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/static/dara_light.svg
--rw-r--r--  2.0 unx     1348 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py
+-rw-r--r--  2.0 unx      734 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py
 -rw-r--r--  2.0 unx     5011 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/components_page.py
 -rw-r--r--  2.0 unx     1590 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/intro_page.py
 -rw-r--r--  2.0 unx    64564 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2384 b- defN 16-Jan-01 00:00 create_dara_app-1.0.0a1.dist-info/RECORD
-20 files, 413883 bytes uncompressed, 262304 bytes compressed:  36.6%
+-rw-r--r--  2.0 unx      735 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 create_dara_app-1.0.0a2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2561 b- defN 16-Jan-01 00:00 create_dara_app-1.0.0a2.dist-info/RECORD
+21 files, 416828 bytes uncompressed, 263110 bytes compressed:  36.9%
```

## zipnote {}

```diff
@@ -39,23 +39,26 @@
 
 Filename: create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/intro_page.py
 Comment: 
 
 Filename: create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py
 Comment: 
 
-Filename: create_dara_app-1.0.0a1.dist-info/LICENSE
+Filename: create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py
 Comment: 
 
-Filename: create_dara_app-1.0.0a1.dist-info/METADATA
+Filename: create_dara_app-1.0.0a2.dist-info/LICENSE
 Comment: 
 
-Filename: create_dara_app-1.0.0a1.dist-info/WHEEL
+Filename: create_dara_app-1.0.0a2.dist-info/METADATA
 Comment: 
 
-Filename: create_dara_app-1.0.0a1.dist-info/entry_points.txt
+Filename: create_dara_app-1.0.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: create_dara_app-1.0.0a1.dist-info/RECORD
+Filename: create_dara_app-1.0.0a2.dist-info/entry_points.txt
+Comment: 
+
+Filename: create_dara_app-1.0.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## create_dara_app/cli.py

```diff
@@ -12,16 +12,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 import pathlib
+import shutil
 import sys
 from importlib.metadata import version
+from typing import Literal
 
 import click
 from cookiecutter.exceptions import FailedHookException, OutputDirExistsException
 from cookiecutter.main import cookiecutter
 
 from create_dara_app.default_command_group import DefaultCommandGroup
 
@@ -38,29 +40,46 @@
     """
 
 
 @cli.command(default=True)
 @click.argument('directory', type=click.Path(exists=False), default='.')
 @click.option('--debug', help='Enable debug logging', is_flag=True, default=False)
 @click.option('--no-install', help='Skip installing dependencies', is_flag=True, default=False)
-def bootstrap(directory: str, debug: bool, no_install: bool):
+@click.option(
+    '--packaging', help='Whether to use pip or poetry', type=click.Choice(['pip', 'poetry']), default='poetry'
+)
+@click.option('--pre', help='Accept prereleases', is_flag=True, default=False)
+def bootstrap(directory: str, debug: bool, no_install: bool, packaging: Literal['pip', 'poetry'], pre: bool):
     """
     Creates a new Decision App project under specified parent DIRECTORY with the default template.
     Uses the Dara version matching the CLI's version.
     """
     logging.basicConfig(level=logging.DEBUG if debug else logging.INFO)
 
     dara_version = version('create-dara-app')
     logger.debug(f'Using create-dara-app version {dara_version}')
+
+    if packaging == 'poetry':
+        # Check if poetry is available
+        poetry_path = shutil.which('poetry')
+        if poetry_path is None:
+            logger.warn('Poetry not found. Falling back to pip.')
+            packaging = 'pip'
+
     try:
         cookiecutter(
             TEMPLATE_DIRECTORY,
             output_dir=directory,
-            extra_context={'dara_version': dara_version},
-            accept_hooks=not no_install,
+            extra_context={
+                '__dara_version': dara_version,
+                '__install': not no_install,
+                '__packaging': packaging,
+                '__pip_args': '--pre' if pre else '',
+                '__poetry_args': '--allow-prereleases' if pre else '',
+            },
         )
     except OutputDirExistsException as e:
         click.echo(
             f'Error: {e}. Please remove it or pick a different project name and try again.',
             err=True,
         )
         sys.exit(1)
```

## create_dara_app/templates/default/cookiecutter.json

### Pretty-printed

 * *Similarity: 0.4%*

 * *Differences: {"'__dara_version'": "'*'",*

 * * "'__install'": "'true'",*

 * * "'__packaging'": "'poetry'",*

 * * "'__pip_args'": "''",*

 * * "'__poetry_args'": "''",*

 * * 'delete': "['dara_version']"}*

```diff
@@ -1,7 +1,11 @@
 {
+    "__dara_version": "*",
+    "__install": "true",
     "__package_name": "{{ cookiecutter.project_name|lower|replace(' ', '_') }}",
+    "__packaging": "poetry",
+    "__pip_args": "",
+    "__poetry_args": "",
     "__project_slug": "{{ cookiecutter.project_name|lower|replace(' ', '-') }}",
     "author_name": "Author <author@example.com>",
-    "dara_version": "*",
     "project_name": "Decision App"
 }
```

## create_dara_app/templates/default/hooks/post_gen_project.py

```diff
@@ -1,27 +1,48 @@
 import os
+import subprocess
 import sys
+import venv
 
 import click
 
+packaging = '{{ cookiecutter.__packaging }}'
+
+pip_args = '{{ cookiecutter.__pip_args }}'.split(' ')
+# Filter out empty
+pip_args = list(filter(None, pip_args))
+
+poetry_args = '{{ cookiecutter.__poetry_args }}'
+
 click.echo('\nProject generated. Running post-generation hooks...')
+click.echo(os.getcwd())
+
+{% if cookiecutter.__install %}
+
+if packaging == 'poetry':
+    click.echo('Installing dependencies...')
+    exit_code = os.system(f'poetry install {poetry_args}')
+
+    if exit_code > 0:
+        click.echo('Error: Poetry install failed', err=True)
+        sys.exit(1)
+
+    click.echo('Generating .env...')
+    os.system('poetry run dara generate-env')
+
+if packaging == 'pip':
+    click.echo('Creating a venv...')
+
+    venv.create('.venv', with_pip=True)
+    pip_path = os.path.join('.venv', 'bin', 'pip') if sys.platform != 'win32' else os.path.join('.venv', 'Scripts', 'pip.exe')
+
+    click.echo('Upgrading pip...')
+    subprocess.run([pip_path, 'install', '--upgrade', 'pip'])
+
+    click.echo('Installing dependencies...')
+    subprocess.run([pip_path, 'install', '-e', '.', *pip_args ])
 
-python_version = sys.version_info
-python_ver_string = f'{python_version.major}.{python_version.minor}'
+    click.echo('Generating .env...')
+    os.system('dara generate-env')
 
-click.echo('Creating a venv...')
-# This explicitly creates a new venv for the project
-exit_code = os.system(f'poetry env use {python_ver_string}')
-
-if exit_code > 0:
-    click.echo('Error: failed to create a new .venv', err=True)
-    sys.exit(1)
-
-click.echo('Installing dependencies...')
-exit_code = os.system('poetry install')
-
-if exit_code > 0:
-    click.echo('Error: Poetry install failed', err=True)
-    sys.exit(1)
 
-click.echo('Generating .env...')
-os.system('poetry run dara generate-env')
+{% endif %}
```

## create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/README.md

```diff
@@ -1,9 +1,11 @@
 # {{ cookiecutter.project_name }}
 
+{% if cookiecutter.__packaging == 'poetry' %}
+
 ## How to run the app
 
 To run the application you can use the following command:
 
 ```bash
 poetry run dara start
 ```
@@ -18,7 +20,34 @@
 ```
 
 To see other available commands you can run:
 
 ```bash
 poetry run dara
 ```
+
+{% else %}
+
+## How to run the app
+
+To run the application you can use the following command:
+
+```bash
+dara start
+```
+
+For development purposes it is often useful to add the `--reload` flag which will automatically reload the application when changes are made to any of the Python files.
+
+By default this will load the config from the `config` variable in `./{{ cookiecutter.__package_name }}/main.py` module.
+To see the list of available config options you can use the `--help` flag:
+
+```bash
+dara start --help
+```
+
+To see other available commands you can run:
+
+```bash
+dara
+```
+
+{% endif %}
```

## create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml

```diff
@@ -1,31 +1,57 @@
+{% if cookiecutter.__packaging == 'poetry' %}
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "{{ cookiecutter.project_name }}"
+name = "{{ cookiecutter.__package_name }}"
 version = "0.1.0"
-description = ""
+description = "{{ cookiecutter.project_name }}"
 authors = ["{{ cookiecutter.author_name }}"]
 
-[tool.blue]
-line-length = 120
-
-[tool.isort]
-known_causalens = ["dara"]
-profile = "black"
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "CAUSALENS", "FIRSTPARTY", "LOCALFOLDER"]
-
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.12.0"
-dara-core = "^{{ cookiecutter.dara_version }}"
-dara-components = "^{{ cookiecutter.dara_version }}"
-seaborn = ">=0.11.0"
+dara-core = "^{{ cookiecutter.__dara_version }}"
+dara-components = "^{{ cookiecutter.__dara_version }}"
 
 [tool.poetry.dev-dependencies]
 blue = "^0.9.0"
 isort = "^5.10.1"
 
 [virtualenvs]
 in-project = true
 create = true
+
+{% else %}
+
+[build-system]
+requires = ["setuptools>=64.0.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "{{ cookiecutter.__package_name }}"
+version = "0.1.0"
+dependencies = [
+    "dara-core == {{ cookiecutter.__dara_version }}",
+    "dara-components == {{ cookiecutter.__dara_version }}",
+    "blue >= 0.9.0",
+    "isort >= 5.10.1"
+]
+authors = [
+    { name = "{{ cookiecutter.author_name }}" }
+]
+description = "{{ cookiecutter.project_name }}"
+requires-python = ">=3.8, <3.12.0"
+
+[tool.setuptools]
+packages = ["{{ cookiecutter.__package_name }}"]
+
+{% endif %}
+
+[tool.blue]
+line-length = 120
+
+[tool.isort]
+known_dara = ["dara"]
+profile = "black"
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "DARA", "FIRSTPARTY", "LOCALFOLDER"]
```

## create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py

```diff
@@ -1,34 +1,18 @@
 from {{cookiecutter.__package_name}}.pages.components_page import components_page
 from {{cookiecutter.__package_name}}.pages.intro_page import intro_page
+from {{cookiecutter.__package_name}}.utils.template import template_renderer
 
 from dara.core import ConfigurationBuilder
-from dara.core.configuration import Configuration
 from dara.core.css import get_icon
-from dara.core.visual.components import Menu, RouterContent
-from dara.core.visual.components.sidebar_frame import SideBarFrame
-from dara.core.visual.template import TemplateBuilder
-from dara.core.visual.themes import Light
+
 
 # Create the configuration builder
 config = ConfigurationBuilder()
 
-def template_renderer(config: Configuration):
-    builder = TemplateBuilder(name='side-bar')
-
-    # Using the TemplateBuilder's helper method - add_router_from_pages
-    # to construct a router of page definitions
-    router = builder.add_router_from_pages(list(config.pages.values()))
-
-    builder.layout = SideBarFrame(
-        content=RouterContent(routes=router.content),
-        side_bar=Menu(routes=router.links),
-        logo_path='/static/dara_light.svg',
-    )
-
-    return builder.to_template()
-
+# Add the template renderer to the configuration
 config.add_template_renderer('side-bar', template_renderer)
 config.template = 'side-bar'
 
+# Add the pages to the configuration
 config.add_page(name='Welcome', content=intro_page(), icon=get_icon('newspaper'))
 config.add_page(name='A-Z Components', content=components_page(), icon=get_icon('spell-check'))
```

## Comparing `create_dara_app-1.0.0a1.dist-info/LICENSE` & `create_dara_app-1.0.0a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `create_dara_app-1.0.0a1.dist-info/METADATA` & `create_dara_app-1.0.0a2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-dara-app
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: CLI to quickly bootstrap a Dara app
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Krzysztof Bielikowicz
 Author-email: krzysztof@causalens.com
 Requires-Python: >=3.8,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `create_dara_app-1.0.0a1.dist-info/RECORD` & `create_dara_app-1.0.0a2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 create_dara_app/__init__.py,sha256=2GNh4sAYBaYZFs7Wz7eHNi-gSibZzksuSl8FKiqEB9A,658
-create_dara_app/cli.py,sha256=yC2HWPAMFFdsckEktHjh_-YY7BjC7twIZQj3EuvEY54,2385
+create_dara_app/cli.py,sha256=t-nDlY8alI4zmL7RkVq6VjoUKWmcL2JtSgNBzEUHGas,3129
 create_dara_app/default_command_group.py,sha256=W0dSVj0HK4sXbeA_UchuwybxGBLsZxexwL0S6wF3PLM,3182
 create_dara_app/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-create_dara_app/templates/default/cookiecutter.json,sha256=Zi66POiqNZoVZwhyqnIl3d7pDQ2iVeKAVxGYcOi9jcw,266
-create_dara_app/templates/default/hooks/post_gen_project.py,sha256=s2BtsR_Ahf_GrYnRHNEjDeKKULWrQEs2FaZ4T-mS8jg,705
+create_dara_app/templates/default/cookiecutter.json,sha256=PLw7utVnsh9aKN2U-9245GQ2rZpCpWRazt6K7ss4OGQ,361
+create_dara_app/templates/default/hooks/post_gen_project.py,sha256=_umZI9cJPpkb7wxvJBYyOjp6MBxeCg4UTy_HXZKijxg,1245
 create_dara_app/templates/default/hooks/pre_gen_project.py,sha256=BxX3zCGrexzGK9g8MOXUV_5Gl-gYY8mwrOMudNwGQYc,294
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/.gitignore,sha256=XoVjpt3wLLuaaB7LF04TxtWZ3wonQtKKO-pZCDzMMx8,320
-create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/README.md,sha256=uMhzjo1HHpbYD-ol5OFWzoPYnMCRvEQLc0MYfrRCD-4,635
-create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml,sha256=IDBv8mSEF2LD0TPgv4bynyoRsmrQ8DZc3E2Pu8MZa84,695
+create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/README.md,sha256=Vi3dSoNz6rJxVjZTWDaS4_qnzp8L2DxwhIjcLzWqqkQ,1275
+create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml,sha256=3fAg3TY4tu1o5KD9gxutmycPp02OocZNTiKuCG-l52w,1323
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/static/dara_light.svg,sha256=rX8oRQ3Uhcm7yQPO6NXsgRydcz4-mXkkChpZqEY8dOU,318043
-create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py,sha256=1BUqVc9Yg2coiFD_QZBYTG2MQgh-v0W_WdgYe7DNzNk,1348
+create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py,sha256=Z5Hc2AzEkqUyJsev0QeT3puI9Prrc_LyESi6MdzTVU0,734
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/components_page.py,sha256=4lFcasT5BAHyBw6WuKufG2yDANKMsWfqonsylvIzfn4,5011
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/intro_page.py,sha256=_G4z_9N66t6eMhIenzIFbIM-p_EzJM8LPGiJ_emRI8k,1590
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py,sha256=Bjx22aaBprvxifizEzTvfdRevtvwTFMOG_xtW6EqNWo,64564
-create_dara_app-1.0.0a1.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-create_dara_app-1.0.0a1.dist-info/METADATA,sha256=bczPvbOszMM52COmVNb9LLUwiPaFHvG6pg7N2nTt21g,712
-create_dara_app-1.0.0a1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-create_dara_app-1.0.0a1.dist-info/entry_points.txt,sha256=RZETW6Q9lb0vM1gptGnobZGlD2qvU-0ZgztNoboRRTk,59
-create_dara_app-1.0.0a1.dist-info/RECORD,,
+create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py,sha256=QzOQKLyC3BSFDnRDGilH1S8ceuqLgMSG4fsjeM4Hskg,735
+create_dara_app-1.0.0a2.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+create_dara_app-1.0.0a2.dist-info/METADATA,sha256=YC0gVIismxQxXbL_E4Jzjp5pcnHrJb2KscSxAvjXXic,712
+create_dara_app-1.0.0a2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+create_dara_app-1.0.0a2.dist-info/entry_points.txt,sha256=RZETW6Q9lb0vM1gptGnobZGlD2qvU-0ZgztNoboRRTk,59
+create_dara_app-1.0.0a2.dist-info/RECORD,,
```

