# Comparing `tmp/mdgpt-0.2.0.tar.gz` & `tmp/mdgpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgpt-0.2.0.tar", max compression
+gzip compressed data, was "mdgpt-0.2.1.tar", max compression
```

## Comparing `mdgpt-0.2.0.tar` & `mdgpt-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.2.0/LICENSE
--rw-r--r--   0        0        0     5552 2023-07-24 21:22:25.841195 mdgpt-0.2.0/README.md
--rw-r--r--   0        0        0     2110 2023-07-24 19:52:45.844735 mdgpt-0.2.0/mdgpt/__init__.py
--rw-r--r--   0        0        0     2380 2023-07-24 20:23:09.758292 mdgpt-0.2.0/mdgpt/build.py
--rw-r--r--   0        0        0      448 2023-07-24 10:56:16.849596 mdgpt-0.2.0/mdgpt/misc.py
--rw-r--r--   0        0        0     9710 2023-07-24 20:42:46.086327 mdgpt-0.2.0/mdgpt/translate.py
--rw-r--r--   0        0        0     2486 2023-07-24 20:44:39.997881 mdgpt-0.2.0/mdgpt/utils.py
--rw-r--r--   0        0        0      875 2023-07-24 20:38:27.733840 mdgpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6730 2023-07-24 21:28:40.787186 mdgpt-0.2.0/setup.py
--rw-r--r--   0        0        0     6402 2023-07-24 21:28:40.787602 mdgpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5552 2023-07-24 21:22:25.841195 mdgpt-0.2.1/README.md
+-rw-r--r--   0        0        0     7685 2023-07-26 19:28:45.661699 mdgpt-0.2.1/mdgpt/__init__.py
+-rw-r--r--   0        0        0     4229 2023-07-26 12:21:16.040964 mdgpt-0.2.1/mdgpt/build.py
+-rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.2.1/mdgpt/misc.py
+-rw-r--r--   0        0        0     2027 2023-07-26 19:33:53.466171 mdgpt-0.2.1/mdgpt/models.py
+-rw-r--r--   0        0        0     9952 2023-07-26 19:34:15.975350 mdgpt-0.2.1/mdgpt/translate.py
+-rw-r--r--   0        0        0     4964 2023-07-26 19:36:05.278406 mdgpt-0.2.1/mdgpt/utils.py
+-rw-r--r--   0        0        0      895 2023-07-26 19:53:57.285323 mdgpt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6757 2023-07-26 19:55:17.052047 mdgpt-0.2.1/setup.py
+-rw-r--r--   0        0        0     6443 2023-07-26 19:55:17.052469 mdgpt-0.2.1/PKG-INFO
```

### Comparing `mdgpt-0.2.0/LICENSE` & `mdgpt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgpt-0.2.0/README.md` & `mdgpt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mdgpt-0.2.0/mdgpt/translate.py` & `mdgpt-0.2.1/mdgpt/translate.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,120 +3,111 @@
 import json
 import frontmatter
 import yaml
 
 from pathlib import Path
 from rich import print
 
+from mdgpt.models import PromptConfig
+from mdgpt.utils import get_lang_dict
+from mdgpt.utils import get_url_map
 from mdgpt.utils import (
     urlize,
     log_usage,
     load_prompt,
     get_chat_response,
     get_gpt_options,
     get_language_name
 )
 
 
-def _translate():
-    args = get_args()
-    translate(
-        prompt=args.pfile,
-        language=args.lang,
-        target=args.target,
-        source_dir=args.source_dir,
-        root_dir=args.dir,
-        single_file=args.file,
-    )
+def get_translation_tasks(prompt_cfg: PromptConfig):
+    source_lang = get_lang_dict(prompt_cfg.LANGUAGE)
+    source_lang['dir'] = prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE
 
-def translate(prompt: str, language: str=None, target: str=None, source_dir: str=None, root_dir: str=None, single_file: str=None):
-    prompt_cfg = load_prompt(f'{prompt}.yaml')
+    tasks = []
+    for target in prompt_cfg.TARGET_LANGUAGES:
+        # target_lang = get_lang_dict(target)
 
-    if language is None:
-        language = prompt_cfg['LANGUAGE']
+        url_hash = get_url_map(prompt_cfg)
 
-    if root_dir is None:
-        root_dir = prompt_cfg['ROOT_DIR']
+        tasks.append(f'js:{target}:{prompt_cfg.LANGUAGE}_{target}')
 
-    source_lang = {
-        'code': language,
-        'name': get_language_name(language),
-        'dir': source_dir if source_dir else language,
-    }
+        if prompt_cfg.FILE:
+            tasks.append(f'md:{target}:{prompt_cfg.FILE}' )
+        else:
+            for k, v in url_hash.items():
+                if not k.endswith('.md'):
+                    if len(k) > 0:
+                        k = f'{k}/index.md'
+                    else:
+                        k = f'{k}index.md'
+                tasks.append(f'md:{target}:{k}')
+            # tasks.extend([f'md:{target}:{k}' for k, v in url_hash.items()])
 
-    if target is None:
-        targets = prompt_cfg.get('TARGET_LANGUAGES')
-        print('targets', targets)
-    else:
-        targets = [target]
+    return tasks
 
-    for target in targets:
 
+def translate(prompt_cfg: PromptConfig):
+    source_lang = {
+        'code': prompt_cfg.LANGUAGE,
+        'name': get_language_name(prompt_cfg.LANGUAGE),
+        'dir': prompt_cfg.SOURCE_DIR if prompt_cfg.SOURCE_DIR else prompt_cfg.LANGUAGE,
+    }
+
+    tasks = []
+    for target in prompt_cfg.TARGET_LANGUAGES:
         target_lang = {
             'code': target,
             'name': get_language_name(target),
-            # 'dir': args.target_dir if args.target_dir else target,
             'dir': target,
         }
 
-        print(f'Translating {source_lang["name"]} ({source_lang["code"]}) to {target_lang["name"]} ({target_lang["code"]})')
+        print(f'Translating {source_lang["name"]} ({source_lang["code"]}) to {target_lang["name"]} ({target_lang["code"]}) ...')
 
-        files = get_markdown_files(Path(root_dir, source_lang['dir']))
+        files = get_markdown_files(Path(prompt_cfg.ROOT_DIR, source_lang['dir']))
         print('Files:', len(files))
 
         # Translate urls
-        if prompt_cfg.get('ONLY_INDEXES'):
+        if prompt_cfg.ONLY_INDEXES:
             url_hash = {urlize(f): '' for f in files if f.endswith('index.md')}
         else:
             url_hash = {urlize(f): '' for f in files}
 
-        url_map, err = translate_json(prompt_cfg['URL_PROMPT'], url_hash, source_lang, target_lang, prompt_cfg.get('MODEL'), root_dir)
+        url_map, err = translate_json(prompt_cfg, url_hash, source_lang, target_lang)
 
-        if single_file:
-            print('Translating single file', single_file)
-            filtered_files = [single_file]
+        if prompt_cfg.FILE:
+            print('Translating single file', prompt_cfg.FILE)
+            filtered_files = [prompt_cfg.FILE]
         else:
-            filtered_files = filter_markdown_files(files, root_dir, target_lang['dir'], url_map)
+            filtered_files = filter_markdown_files(files, prompt_cfg.ROOT_DIR, target_lang['dir'], url_map)
             print('filtered_files', len(filtered_files))
 
         counter = 0
         prompt_tokens = 0
         completion_tokens = 0
 
         for file in filtered_files:
             print(f'Translating {file} ...', flush=True)   # end='\r',
-            if usage := translate_markdown_file(file, root_dir, source_lang, target_lang, url_map, prompt_cfg['MARKDOWN_PROMPT'], prompt_cfg.get('FIELD_KEYS'), prompt_cfg.get('MODEL')):
+            # if usage := translate_markdown_file(file, prompt_cfg.ROOT_DIR, source_lang, target_lang, url_map, prompt_cfg.MARKDOWN_PROMPT, prompt_cfg.FIELD_KEYS, prompt_cfg.MODEL):
+            if usage := translate_markdown_file(prompt_cfg, file, source_lang, target_lang, url_map):
                 prompt_tokens += usage['prompt_tokens']
                 completion_tokens += usage['completion_tokens']
-                log_usage('translate', target, file, usage['prompt_tokens'], usage['completion_tokens'])
+                log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
                 counter += 1
 
             else:
                 print(f'Could not translate {file} ...')
 
         print('')
         print('counter', counter)
         print('prompt_tokens', prompt_tokens)
         print('completion_tokens', completion_tokens)
 
 
-def get_args():
-    parser = argparse.ArgumentParser(description='')
-    parser.add_argument('prompt')
-    parser.add_argument('-d', '--dir', dest='dir', type=str, required=True, help='Root directory for language subdirectories and files')
-    parser.add_argument('-p', '--prompts', dest='pfile', type=str, required=True, help='Path to prompt configuration file without extension')
-    parser.add_argument('-f', '--file', dest='file', type=str, required=False, help='Optional single file to translate')
-    parser.add_argument('-sl', '--lang', dest='lang', type=str, required=True, help='Source language in ISO 639-1 two-letter code')
-    parser.add_argument('-sd', '--source-dir', dest='source_dir', type=str, help='Optional Source directory. Defaults to lang')
-    parser.add_argument('-tl', '--target', dest='target', type=str, required=True, help='Target language in ISO 639-1 two-letter code')
-    parser.add_argument('-td', '--target-dir', dest='target_dir', type=str, help='Optional Target directory. Defaults to target language')
-
-    return parser.parse_args()
-
-
 def generate_frontmatter(post, field_keys):
     field_dict = {}
     if field_keys is not None and len(field_keys) > 0:
         for field in field_keys:
             if field in post.keys():
                 if post[field] is not None:
                     field_value = post[field]
@@ -127,26 +118,26 @@
     return frontmatter
 
 
 def generate_md_promt(prompt_messages, post, lang, target_lang, field_keys):
     frontmatter = generate_frontmatter(post, field_keys)
     return [
         {
-            'role': msg.get('role', 'user'),
-            'content': msg['prompt'].format(
+            'role': msg.role,
+            'content': msg.prompt.format(
                 lang=lang,
                 target_lang=target_lang,
                 frontmatter=frontmatter,
                 content=post.content
             )
         } for msg in prompt_messages
     ]
 
 
-def get_target_file(file, root, target_dir, url_map):
+def get_target_file(file, root, target_dir, url_map) -> Path:
     file_dirs = file.split('/')
     # If file is in a "special" directory, look up best match in url_map ...
     if len(file_dirs) > 1:
         if file_dirs[-2] in ['__sections', '__process']:
             parent_dir = '/'.join(file_dirs[:-2])
             parent_dir_translated = url_map.get(parent_dir)
             if parent_dir_translated:
@@ -186,68 +177,92 @@
         if target_file.exists():
             continue
 
         filtered_files.append(file)
     return filtered_files
 
 
-def get_markdown_files(path: Path):
-    files = []
-    for filepath in glob.iglob(f'{path}/**/*.md', recursive=True):
-        relative_path = filepath[len(f'{path}'):]
-        files.append(relative_path.lstrip('/'))
-    files.sort()
-    return files
 
 
-def translate_markdown_file(file, root_dir, src, target, url_map, prompt_messages, field_keys, gpt_model, ignore_existing=True):
-    root = Path(root_dir)
+def translate_markdown_file(prompt_cfg: PromptConfig, file, src, target, url_map, ignore_existing=True):
+    root = Path(prompt_cfg.ROOT_DIR)
 
     src_code, src_name, src_dir = src['code'], src['name'], src['dir']
     trg_code, trg_name, trg_dir = target['code'], target['name'], target['dir']
 
     with open(root / src_dir / file) as f:
         post = frontmatter.load(f)
 
     target_path = get_target_file(file, root, trg_dir, url_map)
-    messages = generate_md_promt(prompt_messages, post, src, target, field_keys)
-    options = get_gpt_options(gpt_model)
+    messages = generate_md_promt(prompt_cfg.MARKDOWN_PROMPT, post, src, target, prompt_cfg.FIELD_KEYS)
+    options = get_gpt_options(prompt_cfg.MODEL)
 
     try:
         response, usage = get_chat_response(messages, **options)
     except Exception as e:
-        raise Exception(f'Could not get response for {file}: {e}')
+        # raise Exception(f'Could not get response for {file}: {e}')
+        print(f'Could not get response for {file}: {e}')
+        return
+
 
     try:
         new_matter, new_content = frontmatter.parse(response)
     except Exception as e:
-        raise Exception(f'Could not parse {file}: {e}. response: {response}')
+        # raise Exception(f'Could not parse {file}: {e}. response: {response}')
+        print(f'Could not parse {file}: {e}. response: {response}')
+        return
 
     post.content = new_content
 
-    if field_keys is not None and len(field_keys) > 0:
-        for field in field_keys:
+    if prompt_cfg.FIELD_KEYS is not None and len(prompt_cfg.FIELD_KEYS) > 0:
+        for field in prompt_cfg.FIELD_KEYS:
             if new_matter.get(field):
                 post[field] = new_matter[field]
     else:
         post.metadata = new_matter
 
     target_path.parent.mkdir(parents=True, exist_ok=True)
     target_path.write_text(frontmatter.dumps(post))
 
     return usage
 
 
-def translate_json(prompt_messages, json_dict, src, target, gpt_model, root_dir, ignore_existing=True):
 
-    filename = f'translater_urls_{src["code"]}_{target["code"]}.json'
-    src_file = Path(f'{root_dir}/.mdgpt-urls/{filename}')
+
+def save_json_translated(prompt_cfg: PromptConfig, json_dict, target):
+    filename = f'{prompt_cfg.LANGUAGE}_{target}.json'
+    src_file = Path(f'{prompt_cfg.ROOT_DIR}/.mdgpt-urls/{filename}')
+
+    src_file.parent.mkdir(parents=True, exist_ok=True)
+    src_file.write_text(json.dumps(json_dict, indent=2))
+
+
+def translate_missing_json(prompt_cfg: PromptConfig, json_dict, src, target):
+    messages = [
+        {
+            'role': msg.role,
+            'content': msg.prompt.format(lang=src, target_lang=target, content=json.dumps(json_dict, indent=2))
+        }
+        for msg in prompt_cfg.URL_PROMPT
+    ]
+    options = get_gpt_options(prompt_cfg.MODEL)
+    response, usage = get_chat_response(messages, **options)
+    log_usage('translate_json', target['code'], f'{src["code"]}_{target["code"]}', usage['prompt_tokens'], usage['completion_tokens'])
+
+    response_json = json.loads(response)
+
+    return response_json
+
+def translate_json(prompt_cfg: PromptConfig, json_dict, src, target, ignore_existing=True):
+
+    filename = f'{src["code"]}_{target["code"]}.json'
+    src_file = Path(f'{prompt_cfg.ROOT_DIR}/.mdgpt-urls/{filename}')
 
     if src_file.exists():
-        print(f'Loading existing file {src_file}')
+        # print(f'Loading existing file {src_file}')
         src_json = json.loads(src_file.read_text())
 
         for k, v in json_dict.items():
             if src_json.get(k):
                 json_dict[k] = src_json.get(k)
 
     if json_dict.get(''):
@@ -265,20 +280,20 @@
 
     print('missing', len(missing), missing)
     if len(missing) == 0:
         return json_dict, None
 
     messages = [
         {
-            'role': msg.get('role', 'user'),
-            'content': msg.get('prompt').format(lang=src, target_lang=target, content=json.dumps(json_dict, indent=2))
+            'role': msg.role,
+            'content': msg.prompt.format(lang=src, target_lang=target, content=json.dumps(json_dict, indent=2))
         }
-        for msg in prompt_messages
+        for msg in prompt_cfg.URL_PROMPT
     ]
-    options = get_gpt_options(gpt_model)
+    options = get_gpt_options(prompt_cfg.MODEL)
     response, usage = get_chat_response(messages, **options)
     log_usage('translate_json', target['code'], '', usage['prompt_tokens'], usage['completion_tokens'])
 
     response_json = json.loads(response)
     # Backfill missing values
     for k, v in response_json.items():
         json_dict[k] = v
```

### Comparing `mdgpt-0.2.0/pyproject.toml` & `mdgpt-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   | dist
   | venv
 )/
 '''
 
 [tool.poetry]
 name = "mdgpt"
-version = "0.2.0"
+version = "0.2.1"
 description = "Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file."
 authors = ["Jeppe Bårris <jeppe@barris.dk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Djarnis/mdGPT"
 repository = "https://github.com/Djarnis/mdGPT"
 keywords = ["markdown", "translation", "openai", "chatgpt", "gpt"]
@@ -25,14 +25,15 @@
 python = "^3.10"
 python-frontmatter = "^1.0.0"
 requests = "^2.31.0"
 pycountry = "^22.3.5"
 openai = "^0.27.8"
 rich = "^13.4.2"
 python-dotenv = "^1.0.0"
+pydantic = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mdgpt-0.2.0/setup.py` & `mdgpt-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.8,<0.28.0',
  'pycountry>=22.3.5,<23.0.0',
+ 'pydantic>=2.0.3,<3.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'python-frontmatter>=1.0.0,<2.0.0',
  'requests>=2.31.0,<3.0.0',
  'rich>=13.4.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['mdgpt = mdgpt:cli']}
 
 setup_kwargs = {
     'name': 'mdgpt',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.',
     'long_description': '# mdGPT - Mark Down General Purpose Transformer\n\nTranslate markdown files using OpenAI ChatGPT, and generate localized copies of each file.\n\n## Installation\n\n### Using pip\n\n```bash\npip install mdgpt\n```\n\nSet environment variable `OPENAI_API_KEY` or create it in a `.env` file\n\n```bash\nexport OPENAI_API_KEY=YOUR_API_KEY\n```\n\nDownload example prompts:\n\n```bash\ncurl -o example.yaml https://raw.githubusercontent.com/Djarnis/mdGPT/main/prompts.yaml\n```\n\nUse the example `WEBSITE_BUILDER` option from the prompts to build some example files;\n\n```bash\nmdgpt build example\n```\n\nTranslate these markdown files into Finish (fi) versions:\n\n```bash\nmdgpt translate example --target fi\n```\n\nor Danish (da):\n\n```bash\nmdgpt translate example --target da\n```\n\nor German (de):\n\n```bash\nmdgpt translate example --target de\n```\n\nOr whatever. Just make sure it is an ISO 639-1 two-letter language code, and all should be fine.\n\nAdjust the `example.yaml` prompts to suit your needs.\n\n#### MODEL\n\nYou can change the `MODEL` to any engine supported by OpenAI, change the default temperature, and adjust max tokens.\n\nDefault values are:\n\n```yaml\nMODEL:\n    temperature: 0.2\n    engine: gpt-3.5-turbo\n    max_tokens: 2048\n```\n\n#### WEBSITE_BUILDER\n\nThis option is used for building mark down documents, given the example instructions below:\n\n```yaml\nWEBSITE_BUILDER:\n    title: The AI Markdown Translator\n    description: Translate markdown files for websites\n    system_prompt: |\n        Only reply in valid markdown with frontmatter.\n        No explanations. No notes.\n        Language: {lang[name]}\n        Markdown Document:\n        ---\n        # Frontmatter attributes:\n        title: Title of webpage\n        description: Short meta description\n        ---\n        <!-- markdown content -->\n    user_suffix: |\n        Respond in valid markdown format including all provided frontmatter attributes.\n\n    steps:\n        - prompt: |\n              Write the homepage content for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: index.md\n        - prompt: |\n              Write the "About Us" page content for a fictive team behind the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: about.md\n        - prompt: |\n              Write the history for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}), starting in 2019 with 5 major milestones.\n          destination: history.md\n```\n\n#### URL_PROMPT\n\nThis prompt is used when translating file paths.\n\n#### MARKDOWN_PROMPT\n\nThis prompt is used when translating markdown files.\n\n#### ONLY_INDEXES\n\nOptional boolean value, if you only want `index.md` files translated.\n\n```yaml\nONLY_INDEXES: True\n```\n\n#### FIELD_KEYS\n\nOptional list of frontmatter keys you want to translate.\n\nPer default, all keys will be translated, but you can define selected ones here.\n\n```yaml\nFIELD_KEYS:\n    - title\n    - description\n    - keywords\n    - heading\n    - teaser\n```\n\n---\n\n### Using repo source and Poetry:\n\n#### Step 1: Install Poetry\n\nPoetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.\n\nOn Unix-based systems like Linux and MacOS, you can install Poetry by using the following command in your terminal:\n\n```bash\ncurl -sSL https://install.python-poetry.org | python -\n```\n\nOn Windows, you can use PowerShell to install Poetry with the following command:\n\n```powershell\n(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -\n```\n\nYou can check if Poetry was installed correctly by running:\n\n```bash\npoetry --version\n```\n\n#### Step 2: Rename .env.tpl to .env\n\nIn your project directory, you have a file named .env.tpl which serves as a template for environment variables. To use this file, you should rename it to .env.\n\nOn Unix-based systems, use the following command:\n\n```bash\nmv .env.tpl .env\n```\n\nOn Windows, use the following command:\n\n```powershell\nrename .env.tpl .env\n```\n\n#### Step 3: Add OPENAI_API_KEY value to .env\n\nOpen your .env file in a text editor. You should see a line that looks something like this:\n\n```bash\nOPENAI_API_KEY=\n```\n\nAfter the equal sign, add your OpenAI API key in quotes. It should look something like this:\n\n```bash\nOPENAI_API_KEY="your-api-key-goes-here"\n```\n\nSave the .env file and close it.\n\n_Please note:_\n\n-   Make sure to replace "your-api-key-goes-here" with your actual OpenAI API key.\n-   Do not share your .env file or post it online, as it contains sensitive information.\n\n#### Step 4: Install mdGPT\n\nFrom the project directory, install mdGPT and its dependencies:\n\n```bash\npoetry install\n```\n\nThis installs mdGPT and all its dependencies, and you can now follow the example below.\n\n## Example\n\n### Build Markdown files\n\nThe example website ([./example/en](example/en)) was created using the `WEBSITE_BUILDER` option included in the [prompts.yaml](prompts.yaml) file.\n\n```bash\npoetry run mdgpt build example\n```\n\nWhich will create these files in the ./example/en directory:\n\n-   index.md\n-   about.md\n-   contact.md\n-   history.md\n\n## Translate website\n\nTo translate the markdown files into Finish (fi) versions, run this command:\n\n```bash\npoetry run mdgot translate example --target fi\n```\n\nAnd you should get a `/fi` subdirectory ./example/fi/ containing these files, translated from their original English (en) source:\n\n-   index.md\n-   tietoja.md\n-   yhteystiedot.md\n-   historia.md\n',
     'author': 'Jeppe Bårris',
     'author_email': 'jeppe@barris.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Djarnis/mdGPT',
```

### Comparing `mdgpt-0.2.0/PKG-INFO` & `mdgpt-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mdgpt
-Version: 0.2.0
+Version: 0.2.1
 Summary: Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.
 Home-page: https://github.com/Djarnis/mdGPT
 License: MIT
 Keywords: markdown,translation,openai,chatgpt,gpt
 Author: Jeppe Bårris
 Author-email: jeppe@barris.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/Djarnis/mdGPT
 Description-Content-Type: text/markdown
```

