# Comparing `tmp/chatgpt4-cli-1.5.4.tar.gz` & `tmp/chatgpt4-cli-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.4.tar", last modified: Mon Apr 24 16:05:42 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.5.tar", last modified: Wed Apr 26 10:55:23 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.4.tar` & `chatgpt4-cli-1.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.240313 chatgpt4-cli-1.5.4/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32351 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.240313 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32143 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/setup.py
```

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.5/GPTCLI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.4"
+__version__ = "1.5.5"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 __info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
```

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/addons.py` & `chatgpt4-cli-1.5.5/GPTCLI/addons.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import re
 from os import remove, system
 from time import sleep
-from . import logging, getExc
+from . import logging, getExc, __repo__, __author__, error_handler
 from threading import Thread as thr
 from sys import exit
+from fpdf import FPDF
+from json import loads
+import requests
 
 
 class file_parser:
     """Handles contents from text file"""
 
     def __init__(self, prompt):
         self.prompt = prompt
@@ -141,31 +144,92 @@
 
     @classmethod
     def stop_spinning(cls):
         """Stop displaying busy-bar"""
         if cls.querying:
             cls.querying = False
             sleep(cls.sleep_time)
-    
+
     @classmethod
     def run(cls):
-        """Handles GPT querying functions
-        """
+        """Handles GPT querying functions"""
+
         def decorator(func):
-            def main(*args,**kwargs):
+            def main(*args, **kwargs):
                 try:
-                    return func(*args,**kwargs)
+                    return func(*args, **kwargs)
                 except KeyboardInterrupt:
                     cls.stop_spinning()
-                    return 
+                    return
                 except EOFError:
                     cls.querying = False
                     exit(logging.info("Stopping program"))
                 except Exception as e:
                     cls.stop_spinning()
                     logging.error(getExc(e))
+
             return main
+
         return decorator
 
+
+class prompts_to_pdf:
+    def __init__(self):
+        self.contents = self.get_contents()
+        self.pdf = FPDF()
+        self.pdf.add_page()
+
+    @error_handler()
+    def get_contents(self):
+        resp = requests.get(__repo__ + "/raw/main/assets/all-acts.json", timeout=15)
+        if resp.ok:
+            return loads(resp.text)
+        raise Exception("Prompts NOT found in path.")
+
+    @error_handler()
+    def main(self) -> None:
+        if not self.contents:
+            return
+        x = 1
+        self.pdf.set_text_color(255, 0, 0)
+        self.pdf.set_font("Helvetica", size=18)
+        self.pdf.cell(
+            0,
+            10,
+            "Prompts for ChatGPT and Bard",
+            align="C",
+        )
+        self.pdf.ln()
+        for key, value in self.contents.items():
+            key = f"{x}. {key}"
+            value = f"  {value}"
+            self.pdf.set_text_color(0, 0, 255)
+            self.pdf.set_font("Arial", size=14)
+            text_width = self.pdf.get_string_width(key)
+            self.pdf.set_x((210 - text_width) / 2)
+            self.pdf.cell(0, 10, key)
+            self.pdf.cell(0, 10, "")
+            self.pdf.ln()
+            self.pdf.set_x(0)
+            self.pdf.set_font("Courier", size=12)
+            self.pdf.set_text_color(0, 0, 128)
+            self.pdf.multi_cell(0, 10, value.encode("utf-8").decode("latin-1"))
+            x += 1
+        self.pdf.ln()
+        self.pdf.set_author(__author__)
+        self.pdf.set_text_color(255, 0, 0)
+        msg = "Click here to visit project's official repo."
+        self.pdf.set_x((210 - self.pdf.get_string_width(msg)) / 2)
+        self.pdf.add_link()
+        self.pdf.cell(0, 10, msg, link=__repo__)
+
+        self.pdf.ln()
+        self.pdf.set_text_color(0, 0, 0)
+        self.pdf.set_x((210 - self.pdf.get_string_width(__repo__)) / 2)
+        self.pdf.cell(0, 10, __repo__)
+        self.pdf.output("all-acts.pdf")
+        logging.info("Contents saved to 'all-acts.pdf'")
+
+
 if __name__ == "__main__":
     st = file_parser("I want you to debug this python code {f.test.py}")
     print(st.parse)
```

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/bard.py` & `chatgpt4-cli-1.5.5/GPTCLI/bard.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/emage.py` & `chatgpt4-cli-1.5.5/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.5/GPTCLI/gptcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             default="yellow",
             metavar="[cyan|green|yellow|red]",
             choices=self.colors,
         )
         parser.add_argument(
             "--prompt",
             help="Customizes the prompt display",
-            default=f"┌─[{getlogin().capitalize()}@GPTs]─(%H:%M:%S)",
+            default=f"┌─[{getlogin().capitalize()}@GPT-CLI]─(%H:%M:%S)",
             dest="settings",
             nargs="*",
         )
         parser.add_argument(
             "-tm",
             "--timeout",
             help="Request timeout while making request - (Soon)",
@@ -460,25 +460,25 @@
 class intro_prompt_handler:
     """Fetches prompts"""
 
     def __init__(self, filename: str = path.join(app_dir, "awesome_prompts")):
         self.fnm = filename
         self.links = {
             "prompts": "https://raw.githubusercontent.com/f/awesome-chatgpt-prompts/main/prompts.csv",
-            "prompts1": "https://raw.githubusercontent.com/Simatwa/gpt-cli/main/prompts.csv",
+            "prompts1": "https://raw.githubusercontent.com/Simatwa/gpt-cli/main/assets/prompts.csv",
         }
 
     def update(self) -> list:
         from requests import get
 
         try:
             logging.info("Updating acts and prompts")
 
             for key, value in self.links.items():
-                resp = get(value)
+                resp = get(value, timeout=15)
                 if resp.status_code == 200:
                     with open(path.join(app_dir, key), "w", encoding="utf-8") as fh:
                         fh.write(resp.text)
                 else:
                     logging.error(
                         f'Failed to get prompts from "{value}" - [{resp.status_code} : {resp.reason}]'
                     )
@@ -523,14 +523,19 @@
             elif args.dump in ("show", "pretty", "prettify"):
                 for key, value in resp.items():
                     print(
                         f"{config_h.color_dict[args.input_color]}>>[{x}] {key} : {config_h.color_dict[args.output_color]}{value}{Fore.RESET}",
                         end="\n\n",
                     )
                     x += 1
+            elif args.dump in ("pdf"):
+                from .addons import prompts_to_pdf
+
+                prompts_to_pdf().main()
+
             else:
                 with open(args.dump, "w", encoding="utf-8") as fh:
                     from json import dumps
 
                     data = json.dumps(resp, indent=4)
                     fh.write(data)
                     print(data)
@@ -597,15 +602,15 @@
         if isinstance(prompt, list):
             if len(prompt) >= 2 and prompt[0:2] == ["I'm", "sorry"]:
                 resp = False
         else:
             if prompt.startswith("I'm sorry"):
                 resp = False
         return resp
-    
+
     @progress.run()
     def default(self, raw, return_fb=False, no_check=False):
         raw = self.parser(raw)
         run_against_system = False
         if not raw:
             self.do__prompt(self.prompt_disp)
             return
@@ -800,81 +805,71 @@
                 args.prompt_color = line[1]
                 self.do__prompt(self.prompt_disp)
         except Exception as e:
             logging.error(getExc(e))
         else:
             self.apply_color()
         self.do__prompt(self.prompt_disp)
-
+    
+    @error_handler()
     def do__background_color(self, line):
         """Sets background-color"""
-
-        try:
-            self.bcolor_dict[line.lower()]
-            args.background_color = line.lower()
-            self.apply_color()
-        except Exception as e:
-            logging.exception(e)
+        self.bcolor_dict[line.lower()]
+        args.background_color = line.lower()
+        self.apply_color()
         self.do__prompt(self.prompt_disp)
-
+    
+    @error_handler()
     def do__save(self, line):
-        try:
-            if gpt4:
-                all = (
-                    "engine",
-                    "session",
-                    "api_key",
-                    "system_prompt",
-                    "max_tokens",
-                    "temperature",
-                    "top_p",
-                    "presence_penalty",
-                    "frequency_penalty",
-                    "reply_count",
+        if gpt4:
+            all = (
+                "engine",
+                "session",
+                "api_key",
+                "system_prompt",
+                "max_tokens",
+                "temperature",
+                "top_p",
+                "presence_penalty",
+                "frequency_penalty",
+                "reply_count",
                 )
-                chatbot.save(join_list(line), *all)
-            else:
-                chatbot.save_conversation(join_list(line))
-        except Exception as e:
-            logging.error(getExc(e))
+            chatbot.save(join_list(line), *all)
+        else:
+            chatbot.save_conversation(join_list(line))
         self.do__prompt(self.prompt_disp)
-
+    
+    @error_handler()
     def do__load(self, line):
-        try:
-            if gpt4:
-                chatbot.load(join_list(line))
-            else:
-                chatbot.load_conversation(join_list(line))
-        except Exception as e:
-            logging.error(getExc(e))
-            # logging.exception(e)
+        if gpt4:
+            chatbot.load(join_list(line))
+        else:
+            chatbot.load_conversation(join_list(line))
         self.do__prompt(self.prompt_disp)
-
+    
+    @error_handler()
     def do__rollback(self, line):
-        try:
-            if line.isdigit():
-                chatbot.rollback(int(line))
-        except Exception as e:
-            logging.error(getExc(e))
+        if line.isdigit():
+            chatbot.rollback(int(line))
         self.do__prompt(self.prompt_disp)
-
+    
+    @error_handler()
     def do__reset(self, line):
-        try:
-            if gpt4:
-                chatbot.reset(system_prompt=args.system_prompt)
-            else:
-                chatbot.reset()
-        except Exception as e:
-            logging.error(getExc(e))
+        if gpt4:
+            chatbot.reset(system_prompt=args.system_prompt)
+        else:
+            chatbot.reset()
         self.do__prompt(self.prompt_disp)
 
     def do__help(self, line):
         from .helper import help
 
-        print(help)
+        rich_print(
+            Panel(Markdown(help),title='Help Info')
+            )
         self.do__prompt(self.prompt_disp)
 
     def do__exit(self, line):
         return True
 
 
 def get_api_key() -> str:
```

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/helper.py` & `chatgpt4-cli-1.5.5/GPTCLI/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from . import __version__, __repo__
 
 from os import getlogin
 
 help = f"""
-   gpt-cli {__version__}
- Repo : {__repo__}
 
 ╒═══════╤═══════════════════╤═════════════════════════════════════════════╕
 │   No. │ Command           │ Action                                      │
 ╞═══════╪═══════════════════╪═════════════════════════════════════════════╡
 │     0 │ ./{{command}}       │ Run command against system                  │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     1 │ img               │ Generate image ChatGPT based on prompt      │
@@ -19,68 +17,68 @@
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     4 │ _font_color       │ Modify font-color                           │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     5 │ _background_color │ Modify background_color                     │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     6 │ _prompt           │ Modify terminal prompt                      │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
-│     7 │ _save             │ Save current configurations to `.json` file │
+│     7 │ _save             │ Save current configurations to '.json' file │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     8 │ _load             │ Load configurations from file               │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │     9 │ _rollback         │ Rollback Chat by {{n}} times                  │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │    10 │ _reset            │ Reset current chat and start new            │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │    11 │ _help             │ Show this help info                         │
 ├───────┼───────────────────┼─────────────────────────────────────────────┤
 │    12 │ {{Any Other}}       │ Chat with ChatGPT                           │
 ╘═══════╧═══════════════════╧═════════════════════════════════════════════╛
 
-1.  img : Text-to-Image converter - (EXPERIMENTAL)
-    e.g 'img Toddler cartoon coding in Python'
+1.  `img` : Text-to-Image converter - *(EXPERIMENTAL)*
+    e.g *img Toddler cartoon coding in Python*
 
-2.  txt2img : Generate image based on GPT description
-    e.g 'txt2img Describe phenotype anatomy of ancient dinosaurs'
+2.  `txt2img` : Generate image based on GPT description
+    e.g *txt2img Describe phenotype anatomy of ancient dinosaurs*
 
-3. _font_color : modifies font-color
-    e.g 'font_color input red'
+3. `_font_color` : modifies font-color
+    e.g *font_color input red*
 
-4. _background_color : modifies background_color
-    e.g 'background_color cyan'
+4. `_background_color` : modifies background_color
+    e.g *background_color cyan*
 
-5. _prompt : Modify CMD prompt
-    e.g '_prompt ┌─[{getlogin().capitalize()}@ChatGPT4]─(%H:%M:%S)
+5. `_prompt` : Modify CMD prompt
+    e.g *_prompt ┌─[{getlogin().capitalize()}@ChatGPT4]─(%H:%M:%S)*
 
-6. _load : Load configurations from the json file
-    e.g '_load DAN.json'
+6. `_load` : Load configurations from the json file
+    e.g *_load DAN.json*
 
-7. _save : Save the current Chat Configurations
-    e.g '_load DAN.json'
+7. `_save` : Save the current Chat Configurations
+    e.g *_load DAN.json*
 
-8. _rollback : Rollback the Chat by  {{n}} time(s)
-    e.g '_rollback 2'
+8. `_rollback` : Rollback the Chat by  {{n}} time(s)
+    e.g *_rollback 2*
 
-9. _reset : Reset current chat and start new
-    e.g '_reset Chat as if you are a 10 year old child'
+9. `_reset` : Reset current chat and start new
+    e.g *_reset Chat as if you are a 10 year old child*
 
-11. bard : Specifies to use bard GPT
-    e.g bard Explain the composite concept in business.
+11. `bard` : Specifies to use bard GPT
+    e.g *bard Explain the composite concept in business.*
 
-12. gpt4 : Specifies to use ChatGPT in case `--bard` was made default
-    e.g gpt4 How do you make?
+12. `gpt4` : Specifies to use ChatGPT in case `--bard` was made default
+    e.g *gpt4 How do you make?*
 
-13. _help : Show this help info
+13. `_help` : Show this help info
 
 * You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
-* Use `_botchat` to let the 2 GPTs chat to each other
+* Use **_botchat** to let the 2 GPTs chat to each other
 
 * Use double `./` (fullstop and foward slash) to interact with system commands
-      e.g './ifconfig'
+      e.g *./ifconfig*
       
-* Use {{f.text-filename}} to issue prompt contained in  the 'text-filename'
+* Use `{{f.text-filename}}` to issue prompt contained in  the 'text-filename'
 
 * Use `CTRL+C` to cancel a request 
 
-* _exit or `CTRL+C` or `CTRL+Z` : Quits the program.
+* **_exit** or `CTRL+C` or `CTRL+Z` : Quits the program.
         """
```

### Comparing `chatgpt4-cli-1.5.4/GPTCLI/image.py` & `chatgpt4-cli-1.5.5/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.4/LICENSE` & `chatgpt4-cli-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.4/PKG-INFO` & `chatgpt4-cli-1.5.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.4
+Version: 1.5.5
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,35 +24,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
-## [Independencies](requirements.txt)
-
-* [Openai](https://github.com/openai/openai-python)
-* [Numpy](https://github.com/numpy/numpy)
-* [Colorama](https://github.com/tartley/colorama)
-* [revChatGPT](https://github.com/acheong08/ChatGPT)
-
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
 - Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
@@ -69,34 +62,35 @@
 - [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
+
 - From pypi
 
 ```sh
-$ sudo pip install chatgpt4-cli
+sudo pip install chatgpt4-cli
 ```
 
 - Installing from source
- 
- ```sh
- $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
+
+```sh
+ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
  ```
 
 2. Cloning locally and install
 
 ```sh
-$ git clone https://github.com/Simatwa/gpt-cli.git
-$ cd gpt-cli
-$ sudo python3 setup.py install
+git clone https://github.com/Simatwa/gpt-cli.git
+cd gpt-cli
+sudo python3 setup.py install
  #or
-$ python3 setup.py install
+python3 setup.py install
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
@@ -336,15 +330,15 @@
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
-> **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
+> `$ gpt-cli --dump pdf` will generate `all-acts.pdf` file containing latest acts and prompts as shown [here](https://chatgpt-prompts.tiiny.site). 
 
 Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
@@ -362,16 +356,17 @@
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
 - [x] Busy bar
+- [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-cli/edit/main/assets/prompts.csv)
 
-  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
+  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.4 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.5 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -14,48 +14,44 @@
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
 bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
 E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
-Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
-github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
-[Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
-conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
-description. - Stream or Non-stream responses. - Maintain record of the chats.
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily. - Fully customizable Commandline Interface. - Interact with system
-commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
-bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
-Installation Either of the following ways will get you ready. 1. Using pip -
-From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
-```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
-Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
-install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
-OPENAI_API_KEY=` After that you can launch the script with or without a prompt
-> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
-Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
-one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
-```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
-NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
-prompts) can be parsed to the script through the following ways: - Specifying
-the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
-index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+Screenshot1.png) ### Features - Chat with ChatGPT and Bard conversationally. -
+Let **ChatGPT** and **Bard** chat to each other. - Generate Images (DALL-E &
+BingImageCreator)- Based on your prompt or GPT generated description. - Stream
+or Non-stream responses. - Maintain record of the chats. - Parse [awesome-
+chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) - *optional* ## Installation Either of the following ways
+will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
+cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
+Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
+github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
+python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -136,22 +132,24 @@
 spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
 responses from ChatGPT --new-record Override previous chats under the filepath
 --disable-recording Disable saving prompts and responses --zero-show Specifies
 not to stdout prompt of the act parsed --bard Make Bard the default GPT --
 markdown Stdout responses in markdown-format - disables streaming --update
 Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
 system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
-*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
-fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
-info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
-`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
-shifting from one window to next in order to access ChatGPT even after trying
-out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
-(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
-[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
-github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
-[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
-dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
-(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
-1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
-github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
-prompts)
+*7000* tokens and others *3000*. > `$ gpt-cli --dump pdf` will generate `all-
+acts.pdf` file containing latest acts and prompts as shown [here](https://
+chatgpt-prompts.tiiny.site). Visit [acheong08/Bard](https://github.com/
+acheong08/Bard) for info on how to get the Bard's cookie file and Sessions. ##
+Motive   Love for `Terminal` â¤ï¸  As a `terminal guy` I used to find it
+uncomfortable to keep shifting from one window to next in order to access
+ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-
+login), the rest is [here.](https://github.com/Simatwa/gpt-cli)  ##
+Contributions - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/
+fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
+**guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
+cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
+Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
+cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
+Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
+(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
```

### Comparing `chatgpt4-cli-1.5.4/README.md` & `chatgpt4-cli-1.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
-## [Independencies](requirements.txt)
-
-* [Openai](https://github.com/openai/openai-python)
-* [Numpy](https://github.com/numpy/numpy)
-* [Colorama](https://github.com/tartley/colorama)
-* [revChatGPT](https://github.com/acheong08/ChatGPT)
-
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
 - Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
@@ -42,34 +35,35 @@
 - [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
+
 - From pypi
 
 ```sh
-$ sudo pip install chatgpt4-cli
+sudo pip install chatgpt4-cli
 ```
 
 - Installing from source
- 
- ```sh
- $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
+
+```sh
+ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
  ```
 
 2. Cloning locally and install
 
 ```sh
-$ git clone https://github.com/Simatwa/gpt-cli.git
-$ cd gpt-cli
-$ sudo python3 setup.py install
+git clone https://github.com/Simatwa/gpt-cli.git
+cd gpt-cli
+sudo python3 setup.py install
  #or
-$ python3 setup.py install
+python3 setup.py install
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
@@ -309,15 +303,15 @@
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
-> **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
+> `$ gpt-cli --dump pdf` will generate `all-acts.pdf` file containing latest acts and prompts as shown [here](https://chatgpt-prompts.tiiny.site). 
 
 Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
@@ -335,16 +329,17 @@
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
 - [x] Busy bar
+- [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-cli/edit/main/assets/prompts.csv)
 
-  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
+  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
```

#### html2text {}

```diff
@@ -1,47 +1,43 @@
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
 bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
 E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
-Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
-github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
-[Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
-conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
-description. - Stream or Non-stream responses. - Maintain record of the chats.
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily. - Fully customizable Commandline Interface. - Interact with system
-commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
-bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
-Installation Either of the following ways will get you ready. 1. Using pip -
-From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
-```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
-Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
-install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
-OPENAI_API_KEY=` After that you can launch the script with or without a prompt
-> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
-Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
-one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
-```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
-NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
-prompts) can be parsed to the script through the following ways: - Specifying
-the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
-index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+Screenshot1.png) ### Features - Chat with ChatGPT and Bard conversationally. -
+Let **ChatGPT** and **Bard** chat to each other. - Generate Images (DALL-E &
+BingImageCreator)- Based on your prompt or GPT generated description. - Stream
+or Non-stream responses. - Maintain record of the chats. - Parse [awesome-
+chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) - *optional* ## Installation Either of the following ways
+will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
+cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
+Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
+github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
+python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -122,22 +118,24 @@
 spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
 responses from ChatGPT --new-record Override previous chats under the filepath
 --disable-recording Disable saving prompts and responses --zero-show Specifies
 not to stdout prompt of the act parsed --bard Make Bard the default GPT --
 markdown Stdout responses in markdown-format - disables streaming --update
 Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
 system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
-*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
-fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
-info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
-`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
-shifting from one window to next in order to access ChatGPT even after trying
-out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
-(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
-[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
-github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
-[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
-dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
-(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
-1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
-github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
-prompts)
+*7000* tokens and others *3000*. > `$ gpt-cli --dump pdf` will generate `all-
+acts.pdf` file containing latest acts and prompts as shown [here](https://
+chatgpt-prompts.tiiny.site). Visit [acheong08/Bard](https://github.com/
+acheong08/Bard) for info on how to get the Bard's cookie file and Sessions. ##
+Motive   Love for `Terminal` â¤ï¸  As a `terminal guy` I used to find it
+uncomfortable to keep shifting from one window to next in order to access
+ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-
+login), the rest is [here.](https://github.com/Simatwa/gpt-cli)  ##
+Contributions - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/
+fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
+**guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
+cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
+Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
+cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
+Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
+(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
```

### Comparing `chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.4
+Version: 1.5.5
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,35 +24,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
 > Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
-## [Independencies](requirements.txt)
-
-* [Openai](https://github.com/openai/openai-python)
-* [Numpy](https://github.com/numpy/numpy)
-* [Colorama](https://github.com/tartley/colorama)
-* [revChatGPT](https://github.com/acheong08/ChatGPT)
-
 ### Features
 
 - Chat with ChatGPT and Bard conversationally.
 - Let **ChatGPT** and **Bard** chat to each other.
 - Generate Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated description.
 - Stream or Non-stream responses.
 - Maintain record of the chats.
@@ -69,34 +62,35 @@
 - [x] [Bing cookies](https://bing.com) - *optional*
 
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
+
 - From pypi
 
 ```sh
-$ sudo pip install chatgpt4-cli
+sudo pip install chatgpt4-cli
 ```
 
 - Installing from source
- 
- ```sh
- $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
+
+```sh
+ sudo pip install git+https://github.com/Simatwa/gpt-cli.git
  ```
 
 2. Cloning locally and install
 
 ```sh
-$ git clone https://github.com/Simatwa/gpt-cli.git
-$ cd gpt-cli
-$ sudo python3 setup.py install
+git clone https://github.com/Simatwa/gpt-cli.git
+cd gpt-cli
+sudo python3 setup.py install
  #or
-$ python3 setup.py install
+python3 setup.py install
 ```
 
 ## Usage 
 
 - Make OPENAI_API_KEY an environment variable.
 
 `$ export OPENAI_API_KEY=<openai-api-key>`
@@ -336,15 +330,15 @@
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
-> **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
+> `$ gpt-cli --dump pdf` will generate `all-acts.pdf` file containing latest acts and prompts as shown [here](https://chatgpt-prompts.tiiny.site). 
 
 Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
@@ -362,16 +356,17 @@
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
 - [x] Busy bar
+- [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-cli/edit/main/assets/prompts.csv)
 
-  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
+  > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.4 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.5 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -14,48 +14,44 @@
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
 bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
 E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
-Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
-github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
-[Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
-conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
-Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
-description. - Stream or Non-stream responses. - Maintain record of the chats.
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily. - Fully customizable Commandline Interface. - Interact with system
-commands on the fly. ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) - [x] [Bard Cookies](https://
-bard.google.com) - [x] [Bing cookies](https://bing.com) - *optional* ##
-Installation Either of the following ways will get you ready. 1. Using pip -
-From pypi ```sh $ sudo pip install chatgpt4-cli ``` - Installing from source
-```sh $ sudo pip install git+https://github.com/Simatwa/gpt-cli.git ``` 2.
-Cloning locally and install ```sh $ git clone https://github.com/Simatwa/gpt-
-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or $ python3 setup.py
-install ``` ## Usage - Make OPENAI_API_KEY an environment variable. `$ export
-OPENAI_API_KEY=` After that you can launch the script with or without a prompt
-> For instance : ```sh #Without a prompt $ gpt-cli # With a prompt $ gpt-cli
-Write a conversation between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as
-one of the arguments Run `$ gpt-cli -k  ` at the terminal. > For instance :
-```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using
-NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-
-prompts) can be parsed to the script through the following ways: - Specifying
-the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the
-index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+Screenshot1.png) ### Features - Chat with ChatGPT and Bard conversationally. -
+Let **ChatGPT** and **Bard** chat to each other. - Generate Images (DALL-E &
+BingImageCreator)- Based on your prompt or GPT generated description. - Stream
+or Non-stream responses. - Maintain record of the chats. - Parse [awesome-
+chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) - *optional* ## Installation Either of the following ways
+will get you ready. 1. Using pip - From pypi ```sh sudo pip install chatgpt4-
+cli ``` - Installing from source ```sh sudo pip install git+https://github.com/
+Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh git clone https://
+github.com/Simatwa/gpt-cli.git cd gpt-cli sudo python3 setup.py install #or
+python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -136,22 +132,24 @@
 spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
 responses from ChatGPT --new-record Override previous chats under the filepath
 --disable-recording Disable saving prompts and responses --zero-show Specifies
 not to stdout prompt of the act parsed --bard Make Bard the default GPT --
 markdown Stdout responses in markdown-format - disables streaming --update
 Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
 system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
-*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
-fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
-info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
-`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
-shifting from one window to next in order to access ChatGPT even after trying
-out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
-(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
-[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
-github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
-[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
-dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
-(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
-1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
-github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
-prompts)
+*7000* tokens and others *3000*. > `$ gpt-cli --dump pdf` will generate `all-
+acts.pdf` file containing latest acts and prompts as shown [here](https://
+chatgpt-prompts.tiiny.site). Visit [acheong08/Bard](https://github.com/
+acheong08/Bard) for info on how to get the Bard's cookie file and Sessions. ##
+Motive   Love for `Terminal` â¤ï¸  As a `terminal guy` I used to find it
+uncomfortable to keep shifting from one window to next in order to access
+ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-
+login), the rest is [here.](https://github.com/Simatwa/gpt-cli)  ##
+Contributions - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/
+fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
+**guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
+cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
+Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
+cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
+Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
+(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
```

### Comparing `chatgpt4-cli-1.5.4/setup.py` & `chatgpt4-cli-1.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
         "GoogleBard==0.0.7",
+        "fpdf==1.7.2",
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

