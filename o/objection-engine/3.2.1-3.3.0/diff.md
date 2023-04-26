# Comparing `tmp/objection_engine-3.2.1.tar.gz` & `tmp/objection_engine-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objection_engine-3.2.1.tar", max compression
+gzip compressed data, was "objection_engine-3.3.0.tar", max compression
```

## Comparing `objection_engine-3.2.1.tar` & `objection_engine-3.3.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1075 2021-10-15 10:08:59.067420 objection_engine-3.2.1/LICENSE
--rw-r--r--   0        0        0      132 2023-03-22 16:25:45.063760 objection_engine-3.2.1/objection_engine/__init__.py
--rw-r--r--   0        0        0    24178 2023-04-25 14:33:11.508614 objection_engine-3.2.1/objection_engine/anim.py
--rw-r--r--   0        0        0      914 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/comment.py
--rw-r--r--   0        0        0      404 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/comment_bridge.py
--rw-r--r--   0        0        0     1220 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/font_constants.py
--rw-r--r--   0        0        0     3077 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/font_tools.py
--rw-r--r--   0        0        0     3520 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/img.py
--rw-r--r--   0        0        0      743 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/scene.py
--rw-r--r--   0        0        0     5231 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/text.py
--rw-r--r--   0        0        0     1640 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/beans/video.py
--rw-r--r--   0        0        0     7008 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/constants.py
--rw-r--r--   0        0        0     6845 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/parse_tags.py
--rw-r--r--   0        0        0     2954 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/polarity_analysis.py
--rw-r--r--   0        0        0     4170 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/renderer.py
--rw-r--r--   0        0        0     4261 2023-04-23 08:29:00.793378 objection_engine-3.2.1/objection_engine/utils.py
--rw-r--r--   0        0        0      708 2023-04-25 15:06:12.111011 objection_engine-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 objection_engine-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-10-15 10:08:59.067420 objection_engine-3.3.0/LICENSE
+-rw-r--r--   0        0        0    19025 2023-04-06 23:37:25.489269 objection_engine-3.3.0/objection_engine/MovieKit.py
+-rw-r--r--   0        0        0      132 2023-03-22 16:25:45.063760 objection_engine-3.3.0/objection_engine/__init__.py
+-rw-r--r--   0        0        0    58533 2023-04-06 23:37:25.489269 objection_engine-3.3.0/objection_engine/ace_attorney_scene.py
+-rw-r--r--   0        0        0      837 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/beans/comment.py
+-rw-r--r--   0        0        0      388 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/beans/text.py
+-rw-r--r--   0        0        0     1406 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/font_constants.py
+-rw-r--r--   0        0        0     3077 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/font_tools.py
+-rw-r--r--   0        0        0    10021 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/loading.py
+-rw-r--r--   0        0        0     4344 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/make_movie.py
+-rw-r--r--   0        0        0      670 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/math_helpers.py
+-rw-r--r--   0        0        0     9008 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/parse_tags.py
+-rw-r--r--   0        0        0       43 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/renderer.py
+-rw-r--r--   0        0        0     1063 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/tag_macros.py
+-rw-r--r--   0        0        0     2784 2023-04-06 23:37:25.493269 objection_engine-3.3.0/objection_engine/utils.py
+-rw-r--r--   0        0        0     1048 2023-04-06 23:37:25.493269 objection_engine-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 objection_engine-3.3.0/PKG-INFO
```

### Comparing `objection_engine-3.2.1/LICENSE` & `objection_engine-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `objection_engine-3.2.1/objection_engine/beans/comment.py` & `objection_engine-3.3.0/objection_engine/beans/comment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from ..constants import Character
-
-
 class Comment:
     def __init__(self,
     user_id: str = None,
     user_name: str = 'Prosecutor',
     text_content: str = '...',
     evidence_path: str = None,
     score: float = 0
@@ -19,8 +16,7 @@
         """
         self.user_name = user_name
         self.user_id = user_id
         self.text_content = text_content
         self.score = score
         self.evidence_path = evidence_path
         self.effective_user_id = self.user_id or self.user_name
-        self.character: Character = None
```

### Comparing `objection_engine-3.2.1/objection_engine/beans/font_constants.py` & `objection_engine-3.3.0/objection_engine/font_constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from enum import IntEnum
+from objection_engine.loading import ASSETS_FOLDER
 
 class TextType(IntEnum):
     DIALOGUE = 0
     NAME = 1
 
 FONT_ARRAY = [
         # AA-Like > Pixel > Generic
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari-cyrillic/igiari-cyrillic.ttf'},
         # AA-like, Latin, hiragana, katakana, (part of) cyrillic
-        {'path': './assets/igiari/Igiari.ttf'},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/Igiari.ttf'},
         # AA-like, Latin, hiragana, katakana, (part of) cyrillic
-        {'path': './assets/igiari/Galmuri11.ttf'},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/Galmuri11.ttf'},
         # Pixel, Kanji, Hiragana, Katakana
-        {'path':'./assets/igiari/jackeyfont.ttf'},
-        # Better Arabic
-        {'path':'./assets/igiari/KawkabMono-Regular.ttf', 'size': 8, 'offset': {TextType.NAME: (0, -2)}, 'rtl': True},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/jackeyfont.ttf'},
         # Arabic
-        {'path':'./assets/igiari/arabic-1.ttf', 'size': 12, 'offset': {TextType.NAME: (0, -5)}, 'rtl': True},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/arabic-1.ttf', 'size': 12, 'offset': {TextType.NAME: (0, -5)}, 'rtl': True},
         # Pixel-font, Hebrew
-        {'path':'./assets/igiari/STANRG__.ttf'},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/STANRG__.ttf'},
         # Generic
-        {'path':'./assets/igiari/NotoSans-Regular.ttf'},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/NotoSans-Regular.ttf'},
         # Pixel font, Arabic
-        {'path':'./assets/igiari/bitsy-font-with-arabic.ttf', 'size': 10, 'rtl': True},
+        {'path': f'./{ASSETS_FOLDER}/textbox/font/igiari/bitsy-font-with-arabic.ttf', 'size': 10, 'rtl': True},
     ]
 
 NAMETAG_FONT_ARRAY = [
-    {'path': './assets/ace-name/ace-name.ttf', 'size': 8}
+    {'path': f'./{ASSETS_FOLDER}/textbox/font/ace-name/ace-name.ttf', 'size': 8}
 ] + FONT_ARRAY
 
 TEXT_COLORS = {
     "red": (240, 112, 56),
     "blue": (104, 192, 240),
     "green": (0, 240, 0)
 }
```

### Comparing `objection_engine-3.2.1/objection_engine/beans/font_tools.py` & `objection_engine-3.3.0/objection_engine/font_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from objection_engine.beans.font_constants import FONT_ARRAY
+from .font_constants import FONT_ARRAY
 from PIL import ImageFont
 from typing import List, Dict, Union
 from textwrap import wrap
 import spacy
 
 nlp = spacy.blank("xx")
 nlp.add_pipe('sentencizer')
@@ -32,15 +32,15 @@
                 valid_chars += 1
                 break
     return valid_chars
 
 def get_best_font(text, font_array):
     best_font = font_array[-1]
     best_font_points = 0
-    text = text.replace('\n', '').replace('\r', '').replace('\t', '')
+    text = text.replace('\n', '').replace('\r', '').replace('\t', '').replace('\u200B', '')
     for font in font_array:
         pts = get_font_score(font, text)
         if pts > best_font_points:
             best_font_points = pts
             best_font = font
         if best_font_points >= len(text):
             return font
```

### Comparing `objection_engine-3.2.1/objection_engine/parse_tags.py` & `objection_engine-3.3.0/objection_engine/parse_tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,101 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from re import compile
 from typing import Union
 from copy import deepcopy
-from objection_engine.beans.font_tools import get_best_font, split_str_into_newlines, split_with_joined_sentences
-from objection_engine.beans.font_constants import FONT_ARRAY
+from .font_tools import get_best_font, split_str_into_newlines, split_with_joined_sentences
+from .font_constants import FONT_ARRAY
 
 @dataclass
 class DialogueTag:
-    name: str
-    start: int
-    end: int
+    name: str = ""
+    start: int = 0
+    end: int = 0
 
     def range(self):
         return range(self.start, self.end)
 
-@dataclass
-class DialogueAction:
-    name: str
-    index: int
+class BaseDialogueItem:
+    completed: bool = False
 
-@dataclass
-class DialogueTextChunk:
-    text: str
-    tags: list[str]
+    def __repr__(self) -> str:
+        return f"BaseDialogueItem()"
+
+class DialogueAction(BaseDialogueItem):
+    name: str = ""
+    index: int = -1
+
+    def __init__(self, name: str, index: str):
+        self.name = name
+        self.index = index
+
+    def __repr__(self) -> str:
+        return f"DialogueAction(\'{self.name}\', {self.index})"
+
+class DialogueTextLineBreak(BaseDialogueItem):
+    def __repr__(self) -> str:
+        return f"DialogueTextLineBreak()"
+
+class DialogueTextChunk(BaseDialogueItem):
+    text: str = ""
+    tags: list[str] = field(default_factory=list)
+    position: int = 0
+
+    def __init__(self, text: str, tags: list[str]):
+        self.text = text
+        self.tags = tags
 
     def __len__(self) -> int:
         return len(self.text)
 
-@dataclass
+    def __repr__(self) -> str:
+        return f"DialogueTextChunk(\'{self.text}\', {self.tags}, {self.position})"
+
 class DialoguePage:
-    lines: list[list[DialogueTextChunk]]
+    commands: list[BaseDialogueItem]
+    current_item: int
+
+    def __init__(self, commands: list[BaseDialogueItem]):
+        self.commands = commands
+
+    def __repr__(self) -> str:
+        return f"DialoguePage({self.commands})"
+
+    def get_current_item(self):
+        for command in self.commands:
+            if (command is not None) and (not command.completed):
+                return command
+        return None
 
     def __len__(self) -> int:
         lens = []
-        for line in self.lines:
-            for chunk in line:
-                lens.append(len(chunk))
+        for command in self.commands:
+            if isinstance(command, DialogueTextChunk):
+                lens.append(len(command))
         return sum(lens)
 
     def get_raw_text(self) -> str:
         texts = []
-        for line in self.lines:
-            for chunk in line:
-                texts.append(chunk.text)
+        for command in self.commands:
+            if isinstance(command, DialogueTextChunk):
+                texts.append(command.text)
         return ''.join(texts)
 
     def get_visible_text(self, visible_chars: int = 10) -> 'DialoguePage':
         """
         Iterate through each line, and within each line, its chunks.
         Count the characters and keep adding to a variable.
         Once the variable hits visible_chars, stop counting.
         The chunks we read should be added to a list, and the chunk we're reading right now
         should be cut off to its correct length before being added.
         """
+        read_everything = True
         chars_remaining = visible_chars
         new_lines = []
-        for line in self.lines:
+        for line in self.commands:
             new_line = []
             for chunk in line:
                 if chars_remaining >= len(chunk):
                     new_line.append(deepcopy(chunk))
                     chars_remaining -= len(chunk)
                 elif chars_remaining > 0:
                     partial_copy = deepcopy(chunk)
@@ -69,131 +105,151 @@
                     break
                 else:
                     break
             new_lines.append(new_line)
             if chars_remaining <= 0:
                 break
 
-        return DialoguePage(new_lines)
+        d = DialoguePage(new_lines)
+        # print("output from get_visible_text", d)
+        return d
 
     def condense_chunks(self) -> 'DialoguePage':
-        lines_of_chunks = []
-        for line in self.lines:
-            current_string = ""
-            current_tags = None
-            chunks: list[DialogueTextChunk] = []
-            for chunk in line:
-                if current_tags is None or chunk.tags == current_tags:
-                    current_string += chunk.text
-                    if current_tags is None:
-                        current_tags = chunk.tags.copy()
-                else:
-                    chunks.append(DialogueTextChunk(current_string, current_tags))
-                    current_string = chunk.text
+        chunks = []
+        current_string = ""
+        current_tags = None
+        for chunk in self.commands:
+            if isinstance(chunk, DialogueTextChunk) and (current_tags is None or chunk.tags == current_tags):
+                current_string += chunk.text
+                if current_tags is None:
                     current_tags = chunk.tags.copy()
-            if len(current_string) > 0:
+            elif isinstance(chunk, DialogueTextChunk):
                 chunks.append(DialogueTextChunk(current_string, current_tags))
-            lines_of_chunks.append(chunks)
-        return DialoguePage(lines_of_chunks)
-
-    def use_rtl(self):
-        best_font = get_best_font(self.get_raw_text(), FONT_ARRAY)
-        return best_font.get("rtl", False)
+                current_string = chunk.text
+                current_tags = chunk.tags.copy()
+            elif isinstance(chunk, DialogueAction):
+                if len(current_string) > 0:
+                    chunks.append(DialogueTextChunk(current_string, current_tags))
+                chunks.append(chunk)
+                current_string = ""
+                current_tags = None
+            elif isinstance(chunk, DialogueTextLineBreak):
+                if len(current_string) > 0:
+                    chunks.append(DialogueTextChunk(current_string, current_tags))
+                chunks.append(chunk)
+                current_string = ""
+                current_tags = None
+        if len(current_string) > 0:
+            chunks.append(DialogueTextChunk(current_string, current_tags))
+
+        d = DialoguePage(chunks)
+        # print("condensed chunks:", d)
+        return d
 
 @dataclass
 class DialogueTextContent:
     cleaned_lines: str
-    tags: list[Union[DialogueTag, DialogueAction]]
+    tags: list[DialogueTag]
+    actions: list[DialogueAction]
 
     def get_text_chunks(self) -> list[DialoguePage]:
         pages = []
         current_position = 0
         for box_text in split_with_joined_sentences(self.cleaned_lines):
             splitter_font_path = get_best_font(box_text, FONT_ARRAY)['path']
             wrapped_box_lines = split_str_into_newlines(box_text, splitter_font_path, 15).split('\n')
-            lines: list[list[DialogueTextChunk]] = []
+            chunks: list[list[DialogueTextChunk]] = []
+
             for line in wrapped_box_lines:
-                chunks: list[DialogueTextChunk] = []
                 for char in line:
+                    # print(f"Processing char {char} at position {current_position}")
+                    # First, process actions
+                    for action in [a for a in self.actions if a.index == current_position]:
+                        # print(f"Action {action} takes place at this position, so insert it")
+                        chunks.append(action)
+
                     this_char_tags: list[str] = []
                     for tag in self.tags:
-                        if isinstance(tag, DialogueTag) and current_position in tag.range():
+                        if current_position in tag.range():
                             this_char_tags.append(tag.name)
                     chunks.append(DialogueTextChunk(char, this_char_tags))
                     current_position += 1
 
-                lines.append(chunks)
-
-            new_page = DialoguePage(lines).condense_chunks()
+                chunks.append(DialogueTextLineBreak())
+            new_page = DialoguePage(chunks).condense_chunks()
             pages.append(new_page)
             
         return pages
 
 
 # Group 1: Optional slash at the beginning (i.e. it's a closing tag)
 # Group 2: Tag name
 # Group 3: Arguments to tag
 # Group 4: Optional slash at end (i.e. it's self-closing, like an action)
-tag_re = compile(r"<(/??)([a-z]*?)(/??)>")
+tag_re = compile(r"(?<!\\)<(/?)(.+?)(/??)>")
 
 def parse_text(text: str) -> DialogueTextContent:
     tag_stack = []
     final_tags = []
-    stripped_text = text.replace('\n', ' ').replace('\r', ' ').replace('\t', ' ')
+    final_actions = []
+    stripped_text = text
     
     next_match = tag_re.search(stripped_text)
     while next_match is not None:
         start, end = next_match.span(0)
         stripped_text = stripped_text[:start] + stripped_text[end:]
 
         closing_slash, tag_name, self_closing_slash = next_match.group(1, 2, 3)
         is_closing_tag = closing_slash == "/"
         is_self_closing_tag = self_closing_slash == "/"
 
         if is_closing_tag and is_self_closing_tag:
             raise Exception(f"Tag at index {start} is both closing and self-closing")
 
         # Opening tag, like <red>
-        if not is_closing_tag:
+        if not is_closing_tag and not is_self_closing_tag:
             tag_stack.append({
                 "name": tag_name,
                 "start": start
             })
 
         # Closing tag, like </red>
         elif is_closing_tag:
             if len(tag_stack) == 0:
                 # Closing tag before opening tag
+                print(f"Error - tag stack is empty on closing tag {tag_name}")
                 return DialogueTextContent(text, [])
             tag = tag_stack.pop()
             if tag["name"] != tag_name:
                 # Tag mismatch
+                print(f"Error - tag mismatch (opening tag {tag['name']}, closing tag {tag_name})")
                 return DialogueTextContent(text, [])
 
             # I know it's confusing, sorry. This is the start index of the closing tag
             tag["end"] = start
             final_tags.append(tag)
 
         # Self-closing tag, like <shake/>
-        if is_self_closing_tag:
-            final_tags.append({
+        elif is_self_closing_tag:
+            final_actions.append({
                 "name": tag_name,
                 "index": start
             })
         next_match = tag_re.search(stripped_text)
 
     # Construct list of tags and actions
     tag_objects = []
     for tag in final_tags:
-        if "index" in tag:
-            tag_objects.append(DialogueAction(**tag))
-        else:
-            tag_objects.append(DialogueTag(**tag))
+        tag_objects.append(DialogueTag(**tag))
+
+    action_objects = []
+    for action in final_actions:
+        action_objects.append(DialogueAction(**action))
 
-    return DialogueTextContent(stripped_text, tag_objects)
+    return DialogueTextContent(stripped_text, tag_objects, action_objects)
 
 def get_rich_boxes(text: str):
     """
     Given input `text`, returns a list of `DialoguePage` objects. Each object
     represents a single dialogue box.
     """
     return parse_text(text).get_text_chunks()
```

