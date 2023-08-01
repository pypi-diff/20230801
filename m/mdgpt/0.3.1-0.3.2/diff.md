# Comparing `tmp/mdgpt-0.3.1.tar.gz` & `tmp/mdgpt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgpt-0.3.1.tar", max compression
+gzip compressed data, was "mdgpt-0.3.2.tar", max compression
```

## Comparing `mdgpt-0.3.1.tar` & `mdgpt-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.3.1/LICENSE
--rw-r--r--   0        0        0     5552 2023-07-27 21:10:00.673003 mdgpt-0.3.1/README.md
--rw-r--r--   0        0        0     8009 2023-07-30 00:39:42.717647 mdgpt-0.3.1/mdgpt/__init__.py
--rw-r--r--   0        0        0     4322 2023-07-29 21:00:05.927261 mdgpt-0.3.1/mdgpt/build.py
--rw-r--r--   0        0        0     1301 2023-07-29 20:35:09.844197 mdgpt-0.3.1/mdgpt/image.py
--rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.3.1/mdgpt/misc.py
--rw-r--r--   0        0        0     2715 2023-07-29 20:36:43.111687 mdgpt-0.3.1/mdgpt/models.py
--rw-r--r--   0        0        0    10989 2023-07-30 00:37:31.021435 mdgpt-0.3.1/mdgpt/translate.py
--rw-r--r--   0        0        0     5726 2023-07-29 14:25:42.495475 mdgpt-0.3.1/mdgpt/utils.py
--rw-r--r--   0        0        0      940 2023-07-30 00:44:32.624266 mdgpt-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6817 2023-07-30 00:45:53.837730 mdgpt-0.3.1/setup.py
--rw-r--r--   0        0        0     6531 2023-07-30 00:45:53.838303 mdgpt-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5552 2023-07-27 21:10:00.673003 mdgpt-0.3.2/README.md
+-rw-r--r--   0        0        0     7850 2023-08-01 10:02:40.355439 mdgpt-0.3.2/mdgpt/__init__.py
+-rw-r--r--   0        0        0     3926 2023-07-30 22:30:05.679933 mdgpt-0.3.2/mdgpt/build.py
+-rw-r--r--   0        0        0     1255 2023-07-30 20:59:20.461923 mdgpt-0.3.2/mdgpt/image.py
+-rw-r--r--   0        0        0     2778 2023-08-01 13:32:41.425798 mdgpt-0.3.2/mdgpt/models.py
+-rw-r--r--   0        0        0     6637 2023-08-01 21:25:38.501701 mdgpt-0.3.2/mdgpt/translate.py
+-rw-r--r--   0        0        0     5108 2023-08-01 21:25:58.313128 mdgpt-0.3.2/mdgpt/utils.py
+-rw-r--r--   0        0        0      971 2023-08-01 21:30:51.245211 mdgpt-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6817 2023-08-01 21:31:45.265616 mdgpt-0.3.2/setup.py
+-rw-r--r--   0        0        0     6531 2023-08-01 21:31:45.266048 mdgpt-0.3.2/PKG-INFO
```

### Comparing `mdgpt-0.3.1/LICENSE` & `mdgpt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.1/README.md` & `mdgpt-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.1/mdgpt/__init__.py` & `mdgpt-0.3.2/mdgpt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,61 +8,56 @@
 from rich.progress import track
 
 from mdgpt.utils import log_usage
 from mdgpt.models import PromptConfig
 from mdgpt.models import get_prompt_config
 from mdgpt.build import get_build_tasks
 from mdgpt.build import build_step
-from mdgpt.utils import get_json_to_translate
-from mdgpt.utils import get_url_map
-from mdgpt.utils import get_lang_dict
 from mdgpt.utils import get_markdown_files
+from mdgpt.utils import get_url_matrices
 from mdgpt.translate import save_json_translated
 from mdgpt.translate import translate_missing_json
 from mdgpt.translate import get_translation_tasks
 from mdgpt.translate import translate_markdown_file
 from mdgpt.translate import get_target_file
 from mdgpt.image import create_image
 
 
 load_dotenv()
 
 
 def cli():
-
     args = parse_args()
     cfg = get_prompt_config(args.prompt, **vars(args))
 
-    source_lang = get_lang_dict(cfg.LANGUAGE)
-    source_lang['dir'] = cfg.SOURCE_DIR if cfg.SOURCE_DIR else cfg.LANGUAGE
-
     funcs = {
         'build': _build,
         'translate': _translate,
         'debug': _debug,
         'image': _image,
     }
 
     func = funcs.get(args.action)
     if func is not None:
         func(cfg)
     else:
         print('[red]Unknown action')
+        raise SystemExit(1)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Build and translate markdown files from a prompt configuration file')
     parser.add_argument('action', type=str, help='Action to perform')
     parser.add_argument('prompt', type=str, help='Path to prompt configuration file without extension')
-    parser.add_argument('-d', '--dir', dest='dir', type=str, required=False, help='Root directory for language subdirectories and files')
+    parser.add_argument('-d', '--dir', dest='dir', type=str, required=False, help='Root directory for language files')
     parser.add_argument('-f', '--file', dest='file', type=str, required=False, help='Optional single file to translate')
-    parser.add_argument('-l', '--lang', dest='lang', type=str, required=False, help='Source language in ISO 639-1 two-letter code')
-    parser.add_argument('-s', '--source-dir', dest='source_dir', type=str, help='Optional Source directory. Defaults to lang')
-    parser.add_argument('-t', '--target', dest='target', type=str, required=False, help='Target language in ISO 639-1 two-letter code')
-
+    parser.add_argument('-l', '--lang', dest='lang', type=str, required=False, help='Src lang in ISO 639-1 2-letter code')
+    parser.add_argument('-s', '--source-dir', dest='source_dir', type=str, help='Optional src dir. Defaults to lang')
+    parser.add_argument('-t', '--target', dest='target', type=str, required=False, help='Target lang in ISO 639-1')
+    parser.add_argument('--no-cache', help='Flag to ignore cache', dest='ignore_cache', action='store_true')
     return parser.parse_args()
 
 
 def _build(cfg: PromptConfig):
     print(f'Building {cfg.ROOT_DIR} ...')
 
     prompt_tokens = completion_tokens = 0
@@ -72,15 +67,15 @@
     if wcfg is None:
         print('[red]No website builder config found.')
         exit(1)
 
     tasks = get_build_tasks(wcfg)
     total_tasks = len(tasks)
 
-    for i in track(range(total_tasks), description="Building ..."):
+    for i in track(range(total_tasks), description='Building ...'):
         step = tasks[i]
 
         print_details = f'({i+1}/{total_tasks}) Writing {step.destination} ...'
         print(print_details, end='', flush=True)
 
         usage, err = build_step(cfg, step)
         if err:
@@ -111,33 +106,37 @@
     tasks = get_translation_tasks(cfg)
     total_tasks = len(tasks)
 
     prompt_tokens = completion_tokens = 0
     errors = skips = oks = 0
 
     # Build url maps for each target language
-    lang_matrix, url_matrix, missing_matrix = {}, {}, {}
-    for target in cfg.TARGET_LANGUAGES:
-        url_hashes = get_url_map(cfg)
-        url_map, missing = get_json_to_translate(cfg, url_hashes, target)
-
-        url_matrix[target] = url_map
-        missing_matrix[target] = missing
-        lang_matrix[target] = get_lang_dict(target)
+    lang_matrix, url_matrix, missing_matrix = get_url_matrices(cfg)
+
+    exit_code = 0
+    exit_msg = ''
 
     # Execute translation tasks
     try:
-        for i in track(range(total_tasks), description="Translating ..."):
+        for i in track(range(total_tasks), description='Translating ...'):
             task = tasks[i]
             action, target, file = task.split(':')[:3]
 
             target_lang = lang_matrix[target]
 
             if action == 'js':
-                result, usage = _translate_js(cfg, i, target, total_tasks, url_matrix[target], missing_matrix[target], lang_matrix[target],)
+                result, usage = _translate_js(
+                    cfg,
+                    i,
+                    total_tasks,
+                    target,
+                    url_matrix[target],
+                    missing_matrix[target],
+                    lang_matrix[target],
+                )
             elif action == 'md':
                 result, usage = _translate_md(cfg, i, total_tasks, file, target, target_lang, url_matrix[target])
 
             if usage:
                 prompt_tokens += usage['prompt_tokens']
                 completion_tokens += usage['completion_tokens']
                 # log_usage(f'translate_{action}', target, file, usage['prompt_tokens'], usage['completion_tokens'])
@@ -146,29 +145,36 @@
                 oks += 1
             elif result == 'skip':
                 skips += 1
             elif result == 'error':
                 errors += 1
 
     except KeyboardInterrupt:
-        print('Interrupted!')
+        print('[red]Aborted!')
+
     except Exception as e:
-        print('An error occurred:', e)
+        errors += 1
+        exit_code = 1
+        exit_msg = f'An error occurred: {e}'
 
     print('---')
     print('prompt_tokens:', prompt_tokens)
     print('completion_tokens:', completion_tokens)
     print('---')
     print(f'[bold]Tasks: {total_tasks}')
     print(f'[yellow]skips: {skips}')
     print(f'[green]oks: {oks}')
     print(f'[red]errors: {errors}')
 
+    if exit_code > 0:
+        print(f'[red]{exit_msg}')
+        raise SystemExit(exit_code)
+
 
-def _translate_js(cfg: PromptConfig, i, target, total_tasks, url_map, missing, target_lang):
+def _translate_js(cfg: PromptConfig, i: int, total_tasks: int, target: str, url_map: dict, missing: dict, target_lang: dict):
     print_details = f'{i+1}/{total_tasks} Translating file urls {cfg.LANGUAGE} -> {target} ...'
     print(print_details, end='', flush=True)   # end='\r',
 
     if len(missing) == 0:
         print(f'[yellow]{print_details} Skip!')
         return 'skip', None
 
@@ -182,50 +188,43 @@
 
         # Save url_map ...
         save_json_translated(cfg, url_map, target)
         print(f'[green]{print_details} ok ;)')
         return 'ok', usage
 
 
-def _translate_md(cfg: PromptConfig, i, total_tasks, file, target, target_lang, url_map):
+def _translate_md(cfg: PromptConfig, i: int, total_tasks: int, file: str, target: str, target_lang: dict, url_map: dict):
     # Check if file exists
     root = Path(cfg.ROOT_DIR)
     target_path = get_target_file(file, root, target, url_map)
 
     print_details = f'{i+1}/{total_tasks} Translating {target_path} ...'
 
     print(print_details, end='', flush=True)   # end='\r',
     if target_path.exists():
-        skip = True
-        if cfg.FILE:
-            if cfg.FILE == file:
-                skip = False
-
+        skip = False if cfg.FILE and cfg.FILE == file else True
         if skip:
             print(f'[yellow]{print_details} Skip!')
             return 'skip', None
 
     if usage := translate_markdown_file(cfg, file, target_lang, url_map):
-        # prompt_tokens += usage['prompt_tokens']
-        # completion_tokens += usage['completion_tokens']
         log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
 
         print(f'[green]{print_details} ok!')
         return 'ok', usage
 
     else:
         print(f'[red]{print_details} error!')
         return 'error', None
 
 
 def _debug(cfg: PromptConfig):
-    print(f'cfg:', cfg)
+    print('cfg:', cfg)
 
     unique_matters = []
-    matters = []
     root_path = Path(cfg.ROOT_DIR, cfg.SOURCE_DIR or cfg.LANGUAGE)
     files = get_markdown_files(root_path)
     for file in files:
         content = Path(root_path, file).read_text()
         matter = frontmatter.loads(content)
         for k, v in matter.metadata.items():
             if k not in unique_matters:
```

### Comparing `mdgpt-0.3.1/mdgpt/build.py` & `mdgpt-0.3.2/mdgpt/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,157 +1,135 @@
-import argparse
 import frontmatter
 
 from pathlib import Path
 from rich import print
 
 from mdgpt.models import PromptConfig
 from mdgpt.models import WebsiteBuilder
 
 from mdgpt.utils import (
-    load_prompt,
     get_chat_response,
     get_gpt_options,
-    get_language_name,
     DefaultDictFormatter,
 )
 
 
 def build_step(prompt_cfg: PromptConfig, step):
     target_path = Path(prompt_cfg.ROOT_DIR, prompt_cfg.LANG.directory, step.destination)
     if target_path.exists():
-        skip = True
-        if prompt_cfg.FILE:
-            if prompt_cfg.FILE == step.destination:
-                skip = False
-
+        skip = False if prompt_cfg.FILE and prompt_cfg.FILE == step.destination else True
         if skip:
             return False, None
 
     wcfg = prompt_cfg.WEBSITE_BUILDER
 
-    # title = wcfg.title
-    # description = wcfg.description
-
     user_suffix = wcfg.user_suffix.strip()
     system_prompt = wcfg.system_prompt.strip()
 
-    step_prompt = '\n'.join([
-        step.prompt.strip(),
-        user_suffix,
-    ])
+    step_prompt = '\n'.join(
+        [
+            step.prompt.strip(),
+            user_suffix,
+        ]
+    )
 
     variables = wcfg.variables
 
     variables['lang_name'] = prompt_cfg.LANG.name
     variables['lang_code'] = prompt_cfg.LANG.code
 
     messages = [
         {
             'role': 'system',
-            # 'content': system_prompt.format(lang=source_lang, **variables)
-            'content': system_prompt.format_map(DefaultDictFormatter(variables)).strip()
+            'content': system_prompt.format_map(DefaultDictFormatter(variables)).strip(),
         },
-        {
-            'role': 'user',
-            'content': step_prompt.format_map(DefaultDictFormatter(variables))
-        }
+        {'role': 'user', 'content': step_prompt.format_map(DefaultDictFormatter(variables))},
     ]
 
     options = get_gpt_options(prompt_cfg.MODEL)
 
     try:
         response, usage = get_chat_response(messages, **options)
 
     except Exception as e:
         return None, e
 
     try:
         new_matter, new_content = frontmatter.parse(response)
     except Exception as e:
-        # raise Exception(f'Could not parse: {e}. response: {response}')
-        # print(f'Could not parse: {e}. response: {response}')
         return usage, e
 
     post = frontmatter.Post(new_content, **new_matter)
 
     target_path.parent.mkdir(parents=True, exist_ok=True)
     target_path.write_text(frontmatter.dumps(post))
 
     return usage, None
 
 
-def build(prompt_cfg: PromptConfig):
-    print(f'Building {prompt_cfg.ROOT_DIR} ...')
+# def build(prompt_cfg: PromptConfig):
+#     print(f'Building {prompt_cfg.ROOT_DIR} ...')
 
-    cfg = prompt_cfg.WEBSITE_BUILDER
-    if cfg is None:
-        print('No website builder config found.')
-        exit(1)
+#     cfg = prompt_cfg.WEBSITE_BUILDER
+#     if cfg is None:
+#         print('No website builder config found.')
+#         exit(1)
+
+#     source_lang = {
+#         'code': prompt_cfg.LANGUAGE,
+#         'name': get_language_name(prompt_cfg.LANGUAGE),
+#         'dir': prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE,
+#     }
+
+#     title = cfg.title
+#     description = cfg.description
+
+#     user_suffix = cfg.user_suffix.strip()
+#     system_prompt = cfg.system_prompt.strip()
+
+#     steps = cfg.steps
+#     for i, step in enumerate(steps):
+#         print(f'Building step {i+1}: {step.destination} ...')
+
+#         messages = [
+#             {'role': 'system', 'content': system_prompt.format(lang=source_lang, title=title, description=description)},
+#             {
+#                 'role': 'user',
+#                 'content': '\n'.join([step.prompt.format(lang=source_lang, title=title).strip(), user_suffix]),
+#             },
+#         ]
+
+#         target_path = Path(prompt_cfg.ROOT_DIR, source_lang['dir'], step.destination)
+#         if target_path.exists():
+#             print(f'File {target_path} exists. Skipping.')
+#             continue
+
+#         options = get_gpt_options(prompt_cfg.MODEL)
+
+#         try:
+#             response, usage = get_chat_response(messages, **options)
+#         except Exception as e:
+#             raise Exception(f'Could not get response: {e}')
+
+#         try:
+#             new_matter, new_content = frontmatter.parse(response)
+#         except Exception as e:
+#             raise Exception(f'Could not parse: {e}. response: {response}')
+
+#         post = frontmatter.Post('')
+#         post.content = new_content
+#         post.metadata = new_matter
 
-    source_lang = {
-        'code': prompt_cfg.LANGUAGE,
-        'name': get_language_name(prompt_cfg.LANGUAGE),
-        'dir': prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE,
-    }
-
-    title = cfg.title
-    description = cfg.description
-
-    user_suffix = cfg.user_suffix.strip()
-    system_prompt = cfg.system_prompt.strip()
-
-    steps = cfg.steps
-    for i, step in enumerate(steps):
-        print(f'Building step {i+1}: {step.destination} ...')
-
-        messages = [
-            {
-                'role': 'system',
-                'content': system_prompt.format(lang=source_lang, title=title, description=description)
-            },
-            {
-                'role': 'user',
-                'content': '\n'.join([
-                    step.prompt.format(lang=source_lang, title=title).strip(),
-                    user_suffix
-                ])
-            }
-        ]
-
-        target_path = Path(prompt_cfg.ROOT_DIR, source_lang['dir'], step.destination)
-        if target_path.exists():
-            print(f'File {target_path} exists. Skipping.')
-            continue
-
-        options = get_gpt_options(prompt_cfg.MODEL)
-
-        try:
-            response, usage = get_chat_response(messages, **options)
-        except Exception as e:
-            raise Exception(f'Could not get response: {e}')
-
-        try:
-            new_matter, new_content = frontmatter.parse(response)
-        except Exception as e:
-            raise Exception(f'Could not parse: {e}. response: {response}')
-
-        post = frontmatter.Post('')
-        post.content = new_content
-        post.metadata = new_matter
-
-        target_path.parent.mkdir(parents=True, exist_ok=True)
-        target_path.write_text(frontmatter.dumps(post))
+#         target_path.parent.mkdir(parents=True, exist_ok=True)
+#         target_path.write_text(frontmatter.dumps(post))
 
 
 def get_build_tasks(website_builder_cfg: WebsiteBuilder):
     # cfg = prompt_cfg.WEBSITE_BUILDER
     if website_builder_cfg is None:
         print('No website builder config found.')
         exit(1)
 
     steps = website_builder_cfg.steps
     return steps
     # for i, step in enumerate(steps):
     #     ...
-
-
```

### Comparing `mdgpt-0.3.1/mdgpt/image.py` & `mdgpt-0.3.2/mdgpt/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from PIL import Image
 
 from mdgpt.models import PromptConfig
 
 
 def create_image(prompt_cfg: PromptConfig):
-    prompt = "Photo realistic white male human in a suit with a tie and a hat."
+    prompt = 'Photo realistic white male human in a suit with a tie and a hat.'
     prompt_slug = slugify(prompt)
 
     response = openai.Image.create(
         prompt=prompt,
         n=3,
         size='256x256',
         api_key=os.getenv('OPENAI_API_KEY'),
@@ -26,19 +26,15 @@
 
     for i, item in enumerate(response['data']):
         url = item['url']
 
         hash_hex = _get_md5_hash(url)
         img_slug = f'{prompt_cfg.ROOT_DIR}/images/{prompt_slug}-{i}-{hash_hex}.jpg'
 
-        img_path = Path(
-            prompt_cfg.ROOT_DIR,
-            'images',
-            f'{prompt_slug}-{i}-{hash_hex}.jpg'
-        )
+        img_path = Path(prompt_cfg.ROOT_DIR, 'images', f'{prompt_slug}-{i}-{hash_hex}.jpg')
         img_path.parent.mkdir(parents=True, exist_ok=True)
 
         response = requests.get(url)
         image = Image.open(BytesIO(response.content))
         image.save(f'{img_path}', 'JPEG')
 
         print('img_slug:', img_slug)
```

### Comparing `mdgpt-0.3.1/mdgpt/models.py` & `mdgpt-0.3.2/mdgpt/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 import yaml
 import pycountry
 
-from pydantic_core.core_schema import FieldValidationInfo
 from pydantic import BaseModel, ValidationError, field_validator
-from typing import List, Optional
-
-from pathlib import Path
+from typing import List
 
 
 class LangModel(BaseModel):
     code: str
     name: str
     directory: str
 
 
 class ChatGPTModel(BaseModel):
-    temperature: float=0.2
-    engine: str='gpt-3.5-turbo'
-    max_tokens: int=1024*2
+    temperature: float = 0.2
+    engine: str = 'gpt-3.5-turbo'
+    max_tokens: int = 1024 * 2
 
 
 class ChatGPTPrompt(BaseModel):
-    role: str='user'
+    role: str = 'user'
     prompt: str
 
 
 class ChatGPTStepPrompt(BaseModel):
-    role: str='user'
+    role: str = 'user'
     prompt: str
     destination: str
 
 
 class WebsiteBuilder(BaseModel):
-    title: str=''
-    description: str=''
-    user_suffix: str=''
-    system_prompt: str=''
+    title: str = ''
+    description: str = ''
+    user_suffix: str = ''
+    system_prompt: str = ''
     steps: List[ChatGPTStepPrompt]
-    variables: dict={}
+    variables: dict = {}
 
 
 class PromptConfig(BaseModel):
-    LANGUAGE: str=None
-    ROOT_DIR: str=None
-    SOURCE_DIR: str=None
-    TARGET_LANGUAGES: List[str]=[]
-    MODEL: ChatGPTModel=None
-    WEBSITE_BUILDER: WebsiteBuilder=None
+    LANGUAGE: str = None
+    ROOT_DIR: str = None
+    SOURCE_DIR: str = None
+    TARGET_LANGUAGES: List[str] = []
+    MODEL: ChatGPTModel = None
+    WEBSITE_BUILDER: WebsiteBuilder = None
     URL_PROMPT: List[ChatGPTPrompt]
     MARKDOWN_PROMPT: List[ChatGPTPrompt]
-    ONLY_INDEXES: bool=False
-    FILE: str=None
-    FIELD_KEYS: List[str]=None
-    FIELD_KEYS_DELETE: List[str]=None
-    LANG: LangModel=None
+    ONLY_INDEXES: bool = False
+    FILE: str = None
+    FIELD_KEYS: List[str] = None
+    FIELD_KEYS_DELETE: List[str] = None
+    LANG: LangModel = None
+    IGNORE_CACHE: bool = False
 
     @field_validator('LANGUAGE')
     def language_must_be_iso(cls, v):
         if len(v) != 2:
             raise ValueError('LANGUAGE must be an ISO 639-1 two-letter language code')
         return v
 
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        if self.LANGUAGE is not None:
+            self.LANG = LangModel(
+                code=self.LANGUAGE,
+                name=get_language_name(self.LANGUAGE),
+                directory=self.SOURCE_DIR or self.LANGUAGE,
+            )
 
-def get_prompt_config(prompt_file: str, **kwargs) -> PromptConfig:
 
-    def get_language_name(lang_code):
-        lang = None
-        try:
-            lang = pycountry.languages.get(alpha_2=lang_code)
-        except Exception as e:
-            print(f'An error occurred: {e}')
-            exit(1)
-
-        if lang is None:
-            print(f'Language {lang_code} not found.', lang)
-            exit(1)
+def get_language_name(lang_code):
+    lang = pycountry.languages.get(alpha_2=lang_code)
+    if lang is None:
+        print(f'Language {lang_code} not found :/', lang)
+        exit(1)
+    return lang.name
 
-        return lang.name
 
+def get_prompt_config(prompt_file: str, **kwargs) -> PromptConfig:
     try:
         with open(f'{prompt_file}.yaml', 'r') as f:
             prompt = yaml.load(f, Loader=yaml.loader.SafeLoader)
 
     except FileNotFoundError:
         print(f'Prompt file {prompt_file} not found.')
         exit(1)
@@ -97,20 +98,18 @@
 
     if kwargs.get('target'):
         prompt['TARGET_LANGUAGES'] = [kwargs['target']]
 
     if kwargs.get('file'):
         prompt['FILE'] = kwargs['file']
 
+    if kwargs.get('ignore_cache'):
+        prompt['IGNORE_CACHE'] = True
+
     try:
         cfg = PromptConfig(**prompt)
 
     except ValidationError as e:
-        print(e)
+        print(f'[red]{e}')
         exit(1)
 
-    cfg.LANG = LangModel(
-        code=cfg.LANGUAGE,
-        name=get_language_name(cfg.LANGUAGE),
-        directory=cfg.SOURCE_DIR or cfg.LANGUAGE
-    )
     return cfg
```

### Comparing `mdgpt-0.3.1/mdgpt/utils.py` & `mdgpt-0.3.2/mdgpt/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
-import yaml
 import pycountry
 import openai
 import glob
 import json
 
 from pathlib import Path
 
 from mdgpt.models import PromptConfig
+from mdgpt.models import ChatGPTModel
 
 
 def urlize(text):
     if text.endswith('index.md'):
         text = text[:-9]
     return text
 
@@ -22,26 +22,15 @@
         logger.parent.mkdir(parents=True, exist_ok=True)
         logger.write_text('target;file;prompt_tokens;completion_tokens\n')
 
     with logger.open('a') as f:
         f.write(f'{target};{file};{prompt_tokens};{completion_tokens}\n')
 
 
-def load_prompt(prompt_file):
-    try:
-        with open(prompt_file, 'r') as f:
-            prompt = yaml.load(f, Loader=yaml.loader.SafeLoader)
-    except FileNotFoundError:
-        print(f'Prompt file {prompt_file} not found.')
-        exit(1)
-
-    return prompt
-
-
-def get_chat_response(messages, model='gpt-3.5-turbo', temperature=0.2, max_tokens=1024*2, n=1):
+def get_chat_response(messages, model='gpt-3.5-turbo', temperature=0.2, max_tokens=1024 * 2, n=1):
     if os.getenv('OPENAI_API_KEY') is None:
         print('Please set OPENAI_API_KEY and OPENAI_ORGANIZATION environment variables.')
         exit(1)
     openai.api_key = os.getenv('OPENAI_API_KEY')
     try:
         completions = openai.ChatCompletion.create(
             model=model,
@@ -69,54 +58,43 @@
 
     except Exception as e:
         print(f'An error occurred: {e}')
         # exit(1)
         raise e
 
 
-def get_gpt_options(gpt_model):
+def get_gpt_options(gpt_model: ChatGPTModel):
     options = {}
 
     if gpt_model is None:
         return options
 
-    if isinstance(gpt_model, dict):
-        if gpt_model.get('engine'):
-            options['model'] = gpt_model['engine']
-        if gpt_model.get('temperature'):
-            options['temperature'] = gpt_model['temperature']
-        if gpt_model.get('max_tokens'):
-            options['max_tokens'] = gpt_model['max_tokens']
-    else:
-        if gpt_model.engine:
-            options['model'] = gpt_model.engine
-        if gpt_model.temperature:
-            options['temperature'] = gpt_model.temperature
-        if gpt_model.max_tokens:
-            options['max_tokens'] = gpt_model.max_tokens
+    if gpt_model.engine:
+        options['model'] = gpt_model.engine
+    if gpt_model.temperature:
+        options['temperature'] = gpt_model.temperature
+    if gpt_model.max_tokens:
+        options['max_tokens'] = gpt_model.max_tokens
 
     return options
 
 
 def get_language_name(lang_code):
-    try:
-        lang = pycountry.languages.get(alpha_2=lang_code)
-    except Exception as e:
-        print(f'An error occurred: {e}')
-        exit(1)
-
+    lang = pycountry.languages.get(alpha_2=lang_code)
     if lang is None:
         print(f'Language {lang_code} not found.', lang)
         exit(1)
 
     return lang.name
 
 
 def get_url_map(prompt_cfg: PromptConfig):
-    files = get_markdown_files(Path(prompt_cfg.ROOT_DIR, prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE))
+    files = get_markdown_files(
+        Path(prompt_cfg.ROOT_DIR, prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE)
+    )
     # print('Files:', prompt_cfg.LANGUAGE, len(files))
 
     # Translate urls
     if prompt_cfg.ONLY_INDEXES:
         url_hash = {urlize(f): '' for f in files if f.endswith('index.md')}
     else:
         url_hash = {urlize(f): '' for f in files}
@@ -131,28 +109,29 @@
         url_hashes = get_url_map(cfg)
         url_map, missing = get_json_to_translate(cfg, url_hashes, target)
 
         url_matrix[target] = url_map
         missing_matrix[target] = missing
         lang_matrix[target] = get_lang_dict(target)
 
+    return lang_matrix, url_matrix, missing_matrix
+
 
 def get_json_to_translate(prompt_cfg: PromptConfig, json_dict, target):
     filename = f'{prompt_cfg.LANGUAGE}_{target}.json'
     src_file = Path(f'{prompt_cfg.ROOT_DIR}/.mdgpt-urls/{filename}')
 
     if src_file.exists():
         # print(f'Loading existing file {src_file}')
         src_json = json.loads(src_file.read_text())
 
         for k, v in json_dict.items():
             if src_json.get(k):
                 json_dict[k] = src_json.get(k)
 
-
     if json_dict.get(''):
         del json_dict['']
 
     missing = {}
     for k, v in json_dict.items():
         if k == '':
             # print('This is empty', k, v)
@@ -173,15 +152,15 @@
         'dir': lang,
     }
 
 
 def get_markdown_files(path: Path):
     files = []
     for filepath in glob.iglob(f'{path}/**/*.md', recursive=True):
-        relative_path = filepath[len(f'{path}'):]
+        relative_path = filepath[len(f'{path}') :]
         if relative_path.endswith('README.md'):
             continue
         files.append(relative_path.lstrip('/'))
     files.sort()
     return files
```

### Comparing `mdgpt-0.3.1/pyproject.toml` & `mdgpt-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.blue]
-line-length = 120
+line-length = 130
 exclude = '''
 /(
   | .git
   | .terraform
   | __pycache__
   | dist
   | venv
 )/
 '''
 
+[tool.ruff]
+line-length = 130
+
 [tool.poetry]
 name = "mdgpt"
-version = "0.3.1"
+version = "0.3.2"
 description = "Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file."
 authors = ["Jeppe Bårris <jeppe@barris.dk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Djarnis/mdGPT"
 repository = "https://github.com/Djarnis/mdGPT"
 keywords = ["markdown", "translation", "openai", "chatgpt", "gpt"]
```

### Comparing `mdgpt-0.3.1/setup.py` & `mdgpt-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'rich>=13.4.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['mdgpt = mdgpt:cli']}
 
 setup_kwargs = {
     'name': 'mdgpt',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.',
     'long_description': '# mdGPT - Mark Down General Purpose Transformer\n\nTranslate markdown files using OpenAI ChatGPT, and generate localized copies of each file.\n\n## Installation\n\n### Using pip\n\n```bash\npip install mdgpt\n```\n\nSet environment variable `OPENAI_API_KEY` or create it in a `.env` file\n\n```bash\nexport OPENAI_API_KEY=YOUR_API_KEY\n```\n\nDownload example prompts:\n\n```bash\ncurl -o example.yaml https://raw.githubusercontent.com/Djarnis/mdGPT/main/prompts.yaml\n```\n\nUse the example `WEBSITE_BUILDER` option from the prompts to build some example files;\n\n```bash\nmdgpt build example\n```\n\nTranslate these markdown files into Finish (fi) versions:\n\n```bash\nmdgpt translate example --target fi\n```\n\nor Danish (da):\n\n```bash\nmdgpt translate example --target da\n```\n\nor German (de):\n\n```bash\nmdgpt translate example --target de\n```\n\nOr whatever. Just make sure it is an ISO 639-1 two-letter language code, and all should be fine.\n\nAdjust the `example.yaml` prompts to suit your needs.\n\n#### MODEL\n\nYou can change the `MODEL` to any engine supported by OpenAI, change the default temperature, and adjust max tokens.\n\nDefault values are:\n\n```yaml\nMODEL:\n    temperature: 0.2\n    engine: gpt-3.5-turbo\n    max_tokens: 2048\n```\n\n#### WEBSITE_BUILDER\n\nThis option is used for building mark down documents, given the example instructions below:\n\n```yaml\nWEBSITE_BUILDER:\n    title: The AI Markdown Translator\n    description: Translate markdown files for websites\n    system_prompt: |\n        Only reply in valid markdown with frontmatter.\n        No explanations. No notes.\n        Language: {lang[name]}\n        Markdown Document:\n        ---\n        # Frontmatter attributes:\n        title: Title of webpage\n        description: Short meta description\n        ---\n        <!-- markdown content -->\n    user_suffix: |\n        Respond in valid markdown format including all provided frontmatter attributes.\n\n    steps:\n        - prompt: |\n              Write the homepage content for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: index.md\n        - prompt: |\n              Write the "About Us" page content for a fictive team behind the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: about.md\n        - prompt: |\n              Write the history for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}), starting in 2019 with 5 major milestones.\n          destination: history.md\n```\n\n#### URL_PROMPT\n\nThis prompt is used when translating file paths.\n\n#### MARKDOWN_PROMPT\n\nThis prompt is used when translating markdown files.\n\n#### ONLY_INDEXES\n\nOptional boolean value, if you only want `index.md` files translated.\n\n```yaml\nONLY_INDEXES: True\n```\n\n#### FIELD_KEYS\n\nOptional list of frontmatter keys you want to translate.\n\nPer default, all keys will be translated, but you can define selected ones here.\n\n```yaml\nFIELD_KEYS:\n    - title\n    - description\n    - keywords\n    - heading\n    - teaser\n```\n\n---\n\n### Using repo source and Poetry:\n\n#### Step 1: Install Poetry\n\nPoetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.\n\nOn Unix-based systems like Linux and MacOS, you can install Poetry by using the following command in your terminal:\n\n```bash\ncurl -sSL https://install.python-poetry.org | python -\n```\n\nOn Windows, you can use PowerShell to install Poetry with the following command:\n\n```powershell\n(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -\n```\n\nYou can check if Poetry was installed correctly by running:\n\n```bash\npoetry --version\n```\n\n#### Step 2: Rename .env.tpl to .env\n\nIn your project directory, you have a file named .env.tpl which serves as a template for environment variables. To use this file, you should rename it to .env.\n\nOn Unix-based systems, use the following command:\n\n```bash\nmv .env.tpl .env\n```\n\nOn Windows, use the following command:\n\n```powershell\nrename .env.tpl .env\n```\n\n#### Step 3: Add OPENAI_API_KEY value to .env\n\nOpen your .env file in a text editor. You should see a line that looks something like this:\n\n```bash\nOPENAI_API_KEY=\n```\n\nAfter the equal sign, add your OpenAI API key in quotes. It should look something like this:\n\n```bash\nOPENAI_API_KEY="your-api-key-goes-here"\n```\n\nSave the .env file and close it.\n\n_Please note:_\n\n-   Make sure to replace "your-api-key-goes-here" with your actual OpenAI API key.\n-   Do not share your .env file or post it online, as it contains sensitive information.\n\n#### Step 4: Install mdGPT\n\nFrom the project directory, install mdGPT and its dependencies:\n\n```bash\npoetry install\n```\n\nThis installs mdGPT and all its dependencies, and you can now follow the example below.\n\n## Example\n\n### Build Markdown files\n\nThe example website ([./example/en](example/en)) was created using the `WEBSITE_BUILDER` option included in the [prompts.yaml](prompts.yaml) file.\n\n```bash\npoetry run mdgpt build example\n```\n\nWhich will create these files in the ./example/en directory:\n\n-   index.md\n-   about.md\n-   contact.md\n-   history.md\n\n## Translate website\n\nTo translate the markdown files into Finish (fi) versions, run this command:\n\n```bash\npoetry run mdgot translate example --target fi\n```\n\nAnd you should get a `/fi` subdirectory ./example/fi/ containing these files, translated from their original English (en) source:\n\n-   index.md\n-   tietoja.md\n-   yhteystiedot.md\n-   historia.md\n',
     'author': 'Jeppe Bårris',
     'author_email': 'jeppe@barris.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Djarnis/mdGPT',
```

### Comparing `mdgpt-0.3.1/PKG-INFO` & `mdgpt-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdgpt
-Version: 0.3.1
+Version: 0.3.2
 Summary: Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.
 Home-page: https://github.com/Djarnis/mdGPT
 License: MIT
 Keywords: markdown,translation,openai,chatgpt,gpt
 Author: Jeppe Bårris
 Author-email: jeppe@barris.dk
 Requires-Python: >=3.10,<4.0
```

