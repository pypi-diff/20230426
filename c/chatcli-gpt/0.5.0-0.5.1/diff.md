# Comparing `tmp/chatcli_gpt-0.5.0.tar.gz` & `tmp/chatcli_gpt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcli_gpt-0.5.0.tar", max compression
+gzip compressed data, was "chatcli_gpt-0.5.1.tar", max compression
```

## Comparing `chatcli_gpt-0.5.0.tar` & `chatcli_gpt-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.5.0/LICENSE
--rw-r--r--   0        0        0     3498 2023-04-10 16:46:32.407744 chatcli_gpt-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.5.0/chatcli_gpt/__init__.py
--rw-r--r--   0        0        0       34 2023-03-26 16:42:54.474450 chatcli_gpt-0.5.0/chatcli_gpt/__main__.py
--rw-r--r--   0        0        0    16466 2023-04-14 14:50:08.474830 chatcli_gpt-0.5.0/chatcli_gpt/chatcli.py
--rw-r--r--   0        0        0      757 2023-04-14 10:35:38.365222 chatcli_gpt-0.5.0/chatcli_gpt/conversation.py
--rw-r--r--   0        0        0     7661 2023-04-14 14:27:59.909325 chatcli_gpt-0.5.0/chatcli_gpt/log.py
--rw-r--r--   0        0        0     3997 2023-04-14 14:39:01.261820 chatcli_gpt-0.5.0/chatcli_gpt/plugins.py
--rw-r--r--   0        0        0      961 2023-04-14 14:56:06.525301 chatcli_gpt-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 chatcli_gpt-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3497 2023-04-26 14:21:31.185327 chatcli_gpt-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.5.1/chatcli_gpt/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-15 05:23:10.942580 chatcli_gpt-0.5.1/chatcli_gpt/__main__.py
+-rw-r--r--   0        0        0    13883 2023-04-26 14:53:43.773831 chatcli_gpt-0.5.1/chatcli_gpt/cli.py
+-rw-r--r--   0        0        0     3380 2023-04-25 15:59:19.286886 chatcli_gpt-0.5.1/chatcli_gpt/conversation.py
+-rw-r--r--   0        0        0     8092 2023-04-26 15:08:09.711600 chatcli_gpt-0.5.1/chatcli_gpt/log.py
+-rw-r--r--   0        0        0     4638 2023-04-26 13:47:15.250569 chatcli_gpt-0.5.1/chatcli_gpt/plugins.py
+-rw-r--r--   0        0        0     1328 2023-04-26 15:10:50.708465 chatcli_gpt-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 chatcli_gpt-0.5.1/PKG-INFO
```

### Comparing `chatcli_gpt-0.5.0/LICENSE` & `chatcli_gpt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.5.0/README.md` & `chatcli_gpt-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 This will start a conversation with the chat bot, which will prompt you for a question. You can also include a text file as context for your question by using the `-f` or `--file` option:
 ```
 chatcli --file myfile.txt
 ```
 
 You can also specify the personality that the chat bot should use with the `-p` or `--personality` option:
 ```
-chatcli --personality concise
+chatcli --personality pyeval
 ```
 
 ### Continue a conversation
 
 To continue a previous conversation, use the `chat` command with the `--continue` option:
 ```
 chatcli --continue
```

### Comparing `chatcli_gpt-0.5.0/chatcli_gpt/chatcli.py` & `chatcli_gpt-0.5.1/chatcli_gpt/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import os.path
 import os
 import sys
 import itertools
 import functools
-import datetime
+from datetime import datetime, timezone
 import dateutil.parser
+from pathlib import Path
 import click
 from click_default_group import DefaultGroup
-import openai
 import prompt_toolkit
-import tiktoken
 
 from .log import (
     write_log,
     search_conversations,
     conversation_log,
     create_initial_log,
 )
@@ -39,50 +37,47 @@
 
 @click.group(cls=DefaultGroup, default="chat", default_if_no_args=True)
 @click.version_option()
 def cli():
     pass
 
 
-def cli_search_options(command):
-    @click.argument("offset", type=int, required=False)
-    @click.option("-s", "--search", help="Select by search term")
-    @click.option("-t", "--tag", help="Select by tag")
-    @functools.wraps(command)
-    def wrapper(*args, offset=None, search=None, tag=None, **kwargs):
-        return command(
-            *args,
-            search_options={"offset": offset, "search": search, "tag": tag},
-            **kwargs,
-        )
-
-    return wrapper
-
-
 def select_conversation(command):
     @click.argument("offset", type=int, required=False)
     @click.option("-s", "--search", help="Select by search term")
     @click.option("-t", "--tag", help="Select by tag")
     @functools.wraps(command)
     def wrapper(*args, offset=None, search=None, tag=None, **kwargs):
+        if (kwargs.get("continue_conversation") or kwargs.get("retry")) and not offset:
+            offset = 1
+        if kwargs.get("select_personality") and not (tag or search or offset):
+            tag = "^" + kwargs["select_personality"]
+        kwargs.pop("select_personality", None)
+        if kwargs.get("new") and not (tag or search or offset):
+            conversation = Conversation({})
+        else:
+            conversation = get_logged_conversation(offset=offset, search=search, tag=tag)
         return command(
             *args,
-            conversation=get_logged_conversation(offset=offset, search=search, tag=tag),
+            conversation=conversation,
             **kwargs,
         )
 
     return wrapper
 
 
 def filter_conversations(command):
     @click.argument("offsets", type=int, nargs=-1)
     @click.option("-s", "--search", help="Select by search term")
     @click.option("-t", "--tag", help="Select by tag")
     @functools.wraps(command)
     def wrapper(*args, offsets=None, search=None, tag=None, **kwargs):
+        if kwargs.get("select_personality") and not (tag or search):
+            tag = "^" + kwargs["select_personality"]
+        kwargs.pop("select_personality", None)
         return command(
             *args,
             conversations=search_conversations(offsets=offsets, search=search, tag=tag),
             **kwargs,
         )
 
     return wrapper
@@ -93,56 +88,36 @@
 @click.option(
     "-c",
     "--continue_conversation",
     "--continue",
     is_flag=True,
     help="Continue previous conversation.",
 )
-@click.option("-p", "--personality", default="concise")
+@click.option("-p", "--personality", "select_personality", default="default", help="Personality to use.")
 @click.option(
     "-f",
     "--file",
     type=click.Path(exists=True),
     multiple=True,
     help="Add a file to the conversation for context.",
 )
 @click.option("-r", "--retry", is_flag=True, help="Retry previous question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
 @click.option("--model", type=click.Choice(MODELS))
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
-@cli_search_options
-def chat(search_options, **kwargs):
-    if (kwargs["continue_conversation"] or kwargs["retry"]) and not search_options["offset"]:
-        search_options["offset"] = 1
-    elif (
-        kwargs["personality"]
-        and not search_options["tag"]
-        and not search_options["search"]
-        and not search_options["offset"]
-    ):
-        search_options["tag"] = "^" + kwargs["personality"]
-
-    conversation = get_logged_conversation(**search_options)
-
+@select_conversation
+def chat(conversation, **kwargs):
     for filename in kwargs["file"]:
-        with open(filename, encoding="utf-8") as fh:
+        with Path(filename).open(encoding="utf-8") as fh:
             file_contents = fh.read()
 
-        conversation.append(
-            {
-                "role": "user",
-                "content": f"The file {filename!r} contains:\n```\n{file_contents}```",
-            }
-        )
+        conversation.append("user", f"The file {filename!r} contains:\n```\n{file_contents}```")
 
     tags = conversation.tags
-    if tags and not is_personality(tags[-1]):
-        tags_to_apply = [tags[-1]]
-    else:
-        tags_to_apply = []
+    tags_to_apply = [tags[-1]] if tags and not is_personality(tags[-1]) else []
 
     conversation.plugins.extend(kwargs["additional_plugins"])
     conversation.tags = tags_to_apply
     conversation.model = kwargs["model"] or conversation.model or "gpt-3.5-turbo"
 
     quick = kwargs["quick"] or not os.isatty(0)
     multiline = not quick
@@ -164,43 +139,36 @@
     except FileExistsError as error:
         click.echo(f"{error}: Conversation log already exists.", file=sys.stderr)
         sys.exit(1)
 
 
 @cli.command(help="Add a message to a new or existing conversation.")
 @click.option("--multiline/--singleline", default=True)
-@click.option("-p", "--personality")
+@click.option("-p", "--personality", help="")
 @click.option("--role", type=click.Choice(["system", "user", "assistant"]), default="system")
 @click.option("--plugin", multiple="True", help="Activate plugins.")
-@click.option("--model", type=click.Choice(MODELS), default="gpt-3.5-turbo")
+@click.option("--model", type=click.Choice(MODELS))
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
-@cli_search_options
-def add(personality, role, plugin, multiline, search_options, **kwargs):
-    if any(search_options.values()):
-        conversation = get_logged_conversation(**search_options)
-    else:
-        conversation = Conversation()
-
+@click.option("--new/--continue", "-n/-c", default=True, help="Create a new conversation or continue.")
+@select_conversation
+def add(conversation, personality, role, multiline, **kwargs):
     tags = conversation.tags
-    if tags and not is_personality(tags[-1]):
-        tags_to_apply = [tags[-1]]
-    else:
-        tags_to_apply = []
+    tags_to_apply = [tags[-1]] if tags and not is_personality(tags[-1]) else []
 
     conversation.plugins.extend(kwargs["additional_plugins"])
     conversation.tags = tags_to_apply
     conversation.model = kwargs["model"] or conversation.model or "gpt-3.5-turbo"
 
     if personality:
         conversation.tags.append("^" + personality)
 
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
-    description = prompt(multiline=True)
-    conversation.append({"role": role, "content": description})
+    content = prompt(multiline=True)
+    conversation.append(role, content)
     write_log(conversation)
 
 
 def merge_list(input_list, additions):
     for item in additions:
         if item not in input_list:
             input_list.append(item)
@@ -221,27 +189,38 @@
 
     for _, item in reversed(list(conversations)):
         merge_list(merged_conversation["messages"], item.messages)
         merge_list(merged_conversation["tags"], (tag for tag in item.tags if not is_personality(tag)))
         merge_list(merged_conversation["plugins"], item.plugins)
         merged_conversation["model"] = item.model or merged_conversation["model"]
 
-    write_log(Conversation(**merged_conversation))
+    write_log(Conversation(merged_conversation))
 
 
 @cli.command(help="List tags.", name="tags")
 def list_tags():
     tags = set()
     for conversation in conversation_log():
         for tag in conversation.tags:
             tags.add(tag)
     for tag in sorted(tags):
         click.echo(tag)
 
 
+@cli.command(help="List personalities.", name="personalities")
+def list_personalities():
+    personalities = set()
+    for conversation in conversation_log():
+        for tag in conversation.tags:
+            if is_personality(tag):
+                personalities.add(tag[1:])
+    for personality in sorted(personalities):
+        click.echo(personality)
+
+
 @cli.command(help="Add tags to an conversation.", name="tag")
 @click.argument("new_tag")
 @select_conversation
 def add_tag(new_tag, conversation):
     new_tags = [tag for tag in conversation.tags if tag != new_tag]
     new_tags.append(new_tag)
     conversation.tags = new_tags
@@ -261,189 +240,120 @@
 @select_conversation
 def show_tag(conversation):
     if conversation.tags:
         click.echo(conversation.tags[-1])
 
 
 @cli.command(help="Show a conversation.")
+@click.option("-p", "--personality", "select_personality", help="Select conversation by personality.")
 @select_conversation
 @click.option(
     "-l/-s",
     "--long/--short",
     help="Show full conversation or just the most recent message.",
 )
 @click.option("--format-json", "--json", is_flag=True, help="Output conversation in JSON format.")
 def show(long, conversation, format_json):
     if format_json:
         click.echo(conversation.to_json())
         return
 
-    if long:
-        messages = conversation.messages
-    else:
-        messages = conversation.messages[-1:]
+    messages = conversation.messages if long else conversation.messages[-1:]
 
     for message in messages:
         prefix = ""
         if message["role"] == "user":
             prefix = ">> "
         click.echo(click.style(prefix + message["content"], fg=MESSAGE_COLORS[message["role"]]))
 
 
-@cli.command(help="List all the questions we've asked")
+@cli.command(help="Display conversation log.")
+@click.option("-p", "--personality", "select_personality", help="Select conversation by personality.")
 @filter_conversations
-@click.option("-l", "--limit", type=int, help="Limit number of results")
-@click.option("-u", "--usage", is_flag=True, help="Show token usage")
+@click.option("--limit", "-l", type=int, help="Limit number of results")
+@click.option("--usage", "-u", is_flag=True, help="Show token usage")
 @click.option("--cost", is_flag=True, help="Show token cost")
 @click.option("--plugins", is_flag=True, help="Show enabled plugins")
 @click.option("--model", is_flag=True, help="Show model")
-@click.option("--format-json", "--json", is_flag=True, help="Output conversation in JSON format.")
-def log(conversations, limit, usage, cost, plugins, model, format_json):
+@click.option("--json", "format_json", is_flag=True, help="Output conversation in JSON format.")
+def log(conversations, limit, format_json, **kwargs):
     for offset, conversation in reversed(list(itertools.islice(conversations, limit))):
         if format_json:
             click.echo(conversation.to_json())
             continue
         try:
-            question = find_recent_message(lambda message: message["role"] != "assistant", conversation)["content"]
+            question = conversation.find(lambda message: message["role"] != "assistant")["content"]
         except ValueError:
             question = conversation.messages[-1]["content"]
         trimmed_message = question.strip().split("\n", 1)[0][:80]
 
         fields = []
-        offset = click.style(f"{offset: 4d}:", fg="blue")
-        fields.append(offset)
+        fields.append(click.style(f"{offset: 4d}:", fg="blue"))
 
-        if usage:
-            if conversation.usage:
-                total_tokens = conversation.usage["total_tokens"]
-            else:
-                total_tokens = 0
+        if kwargs["usage"]:
+            total_tokens = conversation.usage["total_tokens"] if conversation.usage else 0
             fields.append(f"{total_tokens: 5d}")
 
-        if cost:
+        if kwargs["cost"]:
             fields.append(f"${conversation_cost(conversation): 2.3f}")
 
         fields.append(trimmed_message)
         if conversation.tags:
             fields.append(click.style(",".join(conversation.tags), fg="green"))
 
-        if plugins:
+        if kwargs["plugins"]:
             fields.append(",".join(conversation.plugins))
 
-        if model:
+        if kwargs["model"]:
             fields.append(click.style(conversation.model, fg="yellow"))
 
         click.echo(" ".join(fields))
 
 
-def run_conversation(conversation, stream=True, multiline=True, quick=False):
+def run_conversation(conversation, *, stream=True, multiline=True, quick=False):
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
 
     while True:
         question = prompt(multiline=multiline)
         if not question:
             break
-        conversation.append({"role": "user", "content": question})
+        conversation.append("user", question)
         add_answer(conversation, stream=stream)
 
         if quick:
             break
 
 
-def prompt(multiline=True):
+def prompt(*, multiline=True):
     if os.isatty(0):
         try:
             return prompt_toolkit.prompt(">> ", multiline=multiline, prompt_continuation=".. ").strip()
         except EOFError:
             return None
-        click.echo("....")
     else:
         return sys.stdin.read().strip()
 
 
-def synchroneous_request(request_messages, model):
-    completion = openai.ChatCompletion.create(model=model, messages=request_messages)
-    click.echo(completion["choices"][0]["message"]["content"])
-    return completion
-
-
-def stream_request(request_messages, model):
-    completion = {}
-    for chunk in openai.ChatCompletion.create(model=model, messages=request_messages, stream=True):
-        if not completion:
-            for key, value in chunk.items():
-                completion[key] = value
-            completion["choices"] = [{"message": {}} for choice in chunk["choices"]]
-
-        for choice in chunk["choices"]:
-            if choice.get("delta"):
-                for key, value in choice["delta"].items():
-                    message = completion["choices"][choice["index"]]["message"]
-                    if key not in message:
-                        message[key] = ""
-                    message[key] += value
-
-        content_chunk = chunk["choices"][0]["delta"].get("content")
-        if content_chunk:
-            click.echo(content_chunk, nl=False)
-
-    click.echo()
-    return completion
-
-
-def completion_usage(request_messages, model, completion):
-    if "usage" in completion:
-        return completion["usage"]
-
-    encoding = tiktoken.encoding_for_model(model)
-    request_text = " ".join("role: " + x["role"] + " content: " + x["content"] + "\n" for x in request_messages)
-    request_tokens = len(encoding.encode(request_text))
-    completion_tokens = len(encoding.encode(completion["choices"][0]["message"]["content"]))
-    return {
-        "prompt_tokens": request_tokens,
-        "completion_tokens": completion_tokens,
-        "total_tokens": request_tokens + completion_tokens,
-    }
-
-
 @cli.command(help="Add an answer to a question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
 @select_conversation
 def answer(conversation, stream):
     add_answer(conversation, stream=stream)
 
 
-def add_answer(conversation, stream=True):
-    if stream:
-        completion = stream_request(conversation.messages, conversation.model)
-    else:
-        completion = synchroneous_request(conversation.messages, conversation.model)
-
-    # TODO: handle multiple choices
-    response_message = completion["choices"][0]["message"]
-    conversation.append(response_message)
-    write_log(
-        conversation,
-        completion=completion,
-        usage=completion_usage(conversation.messages[:-1], conversation.model, completion),
-    )
-
-    # TODO:
-    # - [ ] wrote more plugins and see what's good interface for plugins
-    # - [ ] middleware pattern for plugins
-    if conversation.plugins:
-        plugin_response = evaluate_plugins(response_message["content"], conversation.plugins)
-
-        if plugin_response:
-            conversation.append({"role": "user", "content": plugin_response})
-            click.echo(click.style(plugin_response, fg=(200, 180, 90)))
-            return add_answer(conversation, stream=stream)
-
-    return response_message
+def add_answer(conversation, *, stream=True):
+    while True:
+        response = conversation.complete(stream=stream, callback=click.echo)
+        write_log(conversation, completion=conversation.completion, usage=conversation.usage)
+        plugin_response = evaluate_plugins(response["content"], conversation.plugins)
+        if not plugin_response:
+            break
+        click.echo(click.style(plugin_response, fg=(200, 180, 90)))
+        conversation.append("user", plugin_response)
 
 
 def conversation_cost(conversation):
     if not conversation.usage:
         return 0
     model = conversation.completion["model"]
     if model not in USAGE_COSTS:
@@ -453,28 +363,21 @@
     usage = conversation.usage
     return (
         model_price["prompt_tokens"] * usage["prompt_tokens"] / 1000
         + model_price["completion_tokens"] * usage["completion_tokens"] / 1000
     )
 
 
-def find_recent_message(predicate, conversation):
-    for message in reversed(conversation.messages):
-        if predicate(message):
-            return message
-    raise ValueError("No matching message found")
-
-
 @cli.command(help="Display number of tokens and token cost.", name="usage")
 @click.option("--today", is_flag=True, help="Show usage for today only.")
 def show_usage(today):
     conversations = conversation_log()
 
     def is_today(conversation):
-        return dateutil.parser.parse(conversation.timestamp).date() == datetime.date.today()
+        return dateutil.parser.parse(conversation.timestamp).date() == datetime.now(tz=timezone.utc).date()
 
     if today:
         conversations = [c for c in conversations if is_today(c)]
     tokens = sum(conversation.usage["total_tokens"] for conversation in conversations if conversation.usage)
 
     total_cost = sum(conversation_cost(conversation) for conversation in conversations)
     click.echo(f"Tokens: {tokens}")
```

### Comparing `chatcli_gpt-0.5.0/chatcli_gpt/log.py` & `chatcli_gpt-0.5.1/chatcli_gpt/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import os
 import os.path
 import sys
 import shutil
 from pathlib import Path
-import datetime
+from datetime import datetime, timezone
 import json
 from textwrap import dedent
 
 from .conversation import Conversation
 
 INITIAL_PERSONALITIES = {
-    "concise": {
-        "content": "You are a helpful, expert linux user and programmer. You give concise answers, providing code where possible.",
+    "default": {
+        "content": """
+            You are a helpful, expert linux user and programmer. You give concise answers. Provide code where possible.
+            """,
     },
     "code": {"content": "You only answer questions with a single example code block only, and no other explanations."},
     "commit": {
         "content": """
-                You generate commit messages from diffs. Every line of commit message should be less than eighty characters.
-                You never output anything that does not belong in the commit message.
-                """,
+            You generate commit messages from diffs. Every line of commit message should be less than eighty characters.
+            You never output anything that does not belong in the commit message.
+            """,
     },
     "pyeval": {
         "plugins": ["pyeval"],
         "model": "gpt-4",
         "content": """
-                You can evaluate code by returning any python code in a code block with the line "EVALUATE:" before it.
-                Do you not attempt to compute expressions, or the results of python code yourself, instead use an EVALUATE block.
-                You will get the result of running the code you provide in a result block.
-
-                For example:
-
-                EVALUATE:
-                ```
-                print(4 + 5)
-                ```
-
-                And you would then receive
-
-                RESULT:
-                ```
-                9
-                ```
-                as the next message.
+            You can evaluate code by returning any python code in a code block with the line "EVALUATE:" before it.
+            Do not compute expressions, or the results of python code yourself, instead use an EVALUATE block.
+            You will get the result of running the code you provide in a result block.
 
-                Use the result to help you answer the question.
-            """,
+            For example:
+
+            EVALUATE:
+            ```
+            print(4 + 5)
+            ```
+
+            And you would then receive
+
+            RESULT:
+            ```
+            9
+            ```
+            as the next message.
+
+            Use the result to help you answer the question.
+        """,
     },
     "search": {
         "plugins": ["search"],
         "model": "gpt-4",
         "content": """
             You can search the internet by returning query in the form SEARCH("query")
             Whenever you are asked a question, you should first search the internet for an answer.
@@ -110,54 +112,71 @@
 
             SAVE("hello.py")
             ```
             print("hello, world!")
             ```
         """,
     },
+    "image": {
+        "plugins": ["image"],
+        "model": "gpt-4",
+        "content": """
+            You can generate images by using an image block.
+
+            For example:
+
+            IMAGE("filename.png")
+            ```
+            A cartoon of a cute dog
+            ```
+        """,
+    },
 }
 
 CHAT_LOG = os.environ.get("CHATCLI_LOGFILE", ".chatcli.log")
 LOG_FILE_VERSION = "0.4"
 
 
 def write_log(conversation, usage=None, completion=None, path=None):
     path = path or find_log()
-    timestamp = datetime.datetime.now().isoformat()
-    with open(path, "a", buffering=1, encoding="utf-8") as fh:
+    timestamp = datetime.now(timezone.utc).isoformat()
+    with Path(path).open("a", buffering=1, encoding="utf-8") as fh:
         fh.write(
             json.dumps(
                 {
                     "messages": conversation.messages,
                     "completion": completion,
                     "usage": usage,
                     "tags": conversation.tags or [],
                     "timestamp": timestamp,
                     "plugins": conversation.plugins or [],
                     "model": conversation.model,
-                }
+                },
             )
-            + "\n"
+            + "\n",
         )
 
 
 def create_initial_log(reinit):
     if not reinit and Path(CHAT_LOG).exists():
         raise FileExistsError(CHAT_LOG)
 
-    with Path(CHAT_LOG).open("w", encoding="utf-8") as fh:
-        fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
+    if not Path(CHAT_LOG).exists():
+        with Path(CHAT_LOG).open("w", encoding="utf-8") as fh:
+            fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
 
     for key, value in INITIAL_PERSONALITIES.items():
         write_log(
             Conversation(
-                messages=[{"role": "system", "content": dedent(value["content"]).strip()}],
-                tags=["^" + key],
-                plugins=value.get("plugins"),
-                model=value.get("model"),
+                {
+                    "messages": [{"role": "system", "content": dedent(value["content"]).strip()}],
+                    "tags": ["^" + key],
+                    "plugins": value.get("plugins"),
+                    "model": value.get("model"),
+                },
             ),
             path=CHAT_LOG,
         )
 
 
 def conversation_log():
     log_path = find_log()
@@ -166,20 +185,24 @@
         version = line.get("version")
         if version is None:
             fh.close()
             lines = list(convert_log_pre_0_4(log_path))
             backup_file = log_path.with_suffix(".log.bak.0_3")
             sys.stderr.write(f"Upgrading log file. Making backup in: {backup_file}\n")
             shutil.copyfile(log_path, backup_file)
-            with log_path.open("w", encoding="utf-8") as fh:
-                fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
-                for line in lines:
-                    fh.write(line + "\n")
-            return [Conversation(**json.loads(line)) for line in lines]
-        return [Conversation(**json.loads(line)) for line in fh]
+            rewrite_log(log_path, lines)
+            return [Conversation(json.loads(line)) for line in lines]
+        return [Conversation(json.loads(line)) for line in fh]
+
+
+def rewrite_log(path, lines):
+    with path.open("w", encoding="utf-8") as fh:
+        fh.write(json.dumps({"version": LOG_FILE_VERSION}) + "\n")
+        for line in lines:
+            fh.write(line + "\n")
 
 
 def find_log():
     path = CHAT_LOG
     for directory in Path(path).resolve().parents:
         if (directory / path).exists():
             return directory / path
@@ -195,15 +218,15 @@
             continue
         if tag and tag not in conversation.tags:
             continue
         yield idx, conversation
 
 
 def convert_log_pre_0_4(filename):
-    with open(filename, "r", encoding="utf-8") as fh:
+    with Path(filename).open(encoding="utf-8") as fh:
         for line in fh:
             data = json.loads(line)
 
             messages = data["messages"]
             usage = data["usage"]
 
             if usage and "request_tokens" in usage:
@@ -211,16 +234,16 @@
                 del usage["request_tokens"]
 
             tags = data.get("tags", [])
             completion = data.get("completion") or data.get("response")
 
             timestamp = (
                 data.get("timestamp")
-                or (completion and datetime.datetime.fromtimestamp(completion.get("created")).isoformat())
-                or datetime.datetime.now().isoformat()
+                or (completion and datetime.fromtimestamp(completion.get("created"), tz=timezone.utc).isoformat())
+                or datetime.now(tz=timezone.utc).isoformat()
             )
 
             assert isinstance(messages, list), data
             assert isinstance(tags, list), data
             assert isinstance(completion, dict) or completion is None, (
                 completion,
                 data,
```

### Comparing `chatcli_gpt-0.5.0/chatcli_gpt/plugins.py` & `chatcli_gpt-0.5.1/chatcli_gpt/plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 import os
 import sys
 import contextlib
 import ast
 import traceback
 import json
 import subprocess
+from pathlib import Path
 import duckduckgo_search
 import wolframalpha
+import requests
+import openai
 
 
 BLOCK_PATTERNS = {
     "bash": r"EVALUATE:\n+```(?:bash)?\n(.*?)```",
     "pyeval": r"EVALUATE:\n+```(?:python)?\n(.*?)```",
     "search": r"SEARCH\((.*)\)",
     "wolfram": r"WOLFRAM\((.*)\)",
     "save": r"SAVE\((.*?)\)\n```\w*\n(.*?)```",
+    "image": r"IMAGE\((.*?)\)\n```\w*\n(.*?)```",
 }
 
 
 def evaluate_plugins(response_text, plugins):
     formatted_output = []
     for active_plugin in plugins:
         blocks = extract_blocks(response_text, active_plugin)
@@ -40,26 +44,31 @@
                     if search_term[0] in "\"'":
                         search_term = ast.literal_eval(search_term)
                     output = exec_wolfram(search_term)
                 case "save":
                     filename, contents = block
                     if filename[0] in "\"'":
                         filename = ast.literal_eval(filename)
-                    with open(filename, "w", encoding="utf-8") as fh:
+                    with Path(filename).open("w", encoding="utf-8") as fh:
                         fh.write(contents)
                     output = {"result": f"Saved to: {filename}"}
+                case "image":
+                    filename, prompt = block
+                    if filename[0] in "\"'":
+                        filename = ast.literal_eval(filename)
+                    with Path(filename).open("wb") as fh:
+                        fh.write(generate_image(prompt))
+                    output = {"result": f"Saved to: {filename}"}
 
             formatted_output.append(format_block(output))
     return "\n".join(formatted_output)
 
 
 def extract_blocks(response_text, plugin):
-    block_pattern = BLOCK_PATTERNS[plugin]
-    matches = re.findall(block_pattern, response_text, re.DOTALL)
-    return matches
+    return re.findall(BLOCK_PATTERNS[plugin], response_text, re.DOTALL)
 
 
 def exec_bash(code):
     result = subprocess.run(["/bin/bash", "-c", code], capture_output=True, text=True, check=False)
 
     return {
         "result": result.stdout.strip(),
@@ -82,15 +91,15 @@
                     compile(ast.Expression(last_expr.value), "<ast>", "eval"),
                     global_scope,
                 )
                 if result is not None:
                     print(result)
             else:
                 exec(code, global_scope)
-        except Exception:  # pylint: disable=broad-except
+        except Exception:  # noqa: ble001
             print(traceback.format_exc())
 
     return {
         "result": stdout.getvalue().strip(),
         "error": stderr.getvalue().strip(),
     }
 
@@ -104,14 +113,21 @@
     if not api_key:
         return {"error": "WOLFRAM_ALPHA_API_KEY is not configured. (Set as an environment variable.)"}
     client = wolframalpha.Client(api_key)
     result = client.query(query)
     return {"result": next(result.results).text}
 
 
+def generate_image(prompt):
+    image_api_response = openai.Image.create(prompt=prompt, n=1, size="256x256")
+    image_url = image_api_response["data"][0]["url"]
+    http_response = requests.get(image_url)
+    return http_response.content
+
+
 # TODO: Truncate the output to meet token requirement and save $$.
 def format_block(output):
     output_blocks = []
     if output.get("result"):
         output_blocks.append(f"RESULT:\n```\n{output['result']}\n```")
     if output.get("error"):
         output_blocks.append(f"ERROR:\n```\n{output['error']}\n```")
```

### Comparing `chatcli_gpt-0.5.0/pyproject.toml` & `chatcli_gpt-0.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 [tool.poetry]
 name = "chatcli-gpt"
-version = "0.5.0"
+version = "0.5.1"
 description = "A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations."
 readme = "README.md"
 license = "MIT"
 authors = ["Adam Kelly <adam@cthulahoops.org>"]
 repository = "https://github.com/cthulahoops/chatcli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.2"
 prompt-toolkit = "^3.0.38"
 markdown = "^3.4.1"
 click = "^8.1.3"
 click-default-group = "^1.2.2"
-pytest = "^7.2.2"
-pytest-mock = "^3.10.0"
 tiktoken = "^0.3.2"
 python-dateutil = "^2.8.2"
 duckduckgo-search = "^2.8.5"
-pillow = "^9.4.0"
 wolframalpha = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-pylint = "^2.17.1"
+pytest = "^7.2.2"
+pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.261"
 
 [tool.poetry.scripts]
-chatcli = "chatcli_gpt.chatcli:main"
+chatcli = "chatcli_gpt.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+select = ["A", "B", "C","E", "F", "G", "I", "N", "Q", "T", "W", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "UP", "YTT"]
+ignore = ["INP001", "I001", "PLR2004", "T201", "EM101", "PGH001"]
+line-length = 120
+
+[tool.black]
+line-length = 120
```

### Comparing `chatcli_gpt-0.5.0/PKG-INFO` & `chatcli_gpt-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcli-gpt
-Version: 0.5.0
+Version: 0.5.1
 Summary: A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations.
 Home-page: https://github.com/cthulahoops/chatcli
 License: MIT
 Author: Adam Kelly
 Author-email: adam@cthulahoops.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,18 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: duckduckgo-search (>=2.8.5,<3.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.2,<0.4.0)
 Requires-Dist: wolframalpha (>=5.0.0,<6.0.0)
 Project-URL: Repository, https://github.com/cthulahoops/chatcli
 Description-Content-Type: text/markdown
 
 # ChatCLI
@@ -87,15 +84,15 @@
 This will start a conversation with the chat bot, which will prompt you for a question. You can also include a text file as context for your question by using the `-f` or `--file` option:
 ```
 chatcli --file myfile.txt
 ```
 
 You can also specify the personality that the chat bot should use with the `-p` or `--personality` option:
 ```
-chatcli --personality concise
+chatcli --personality pyeval
 ```
 
 ### Continue a conversation
 
 To continue a previous conversation, use the `chat` command with the `--continue` option:
 ```
 chatcli --continue
```

