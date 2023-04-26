# Comparing `tmp/nonebot_plugin_autoreply-0.2.6.tar.gz` & `tmp/nonebot_plugin_autoreply-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_autoreply-0.2.6.tar", last modified: Sun Apr 23 14:22:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_autoreply-0.2.7.tar", last modified: Tue Apr 25 16:35:11 2023, max compression
```

## Comparing `nonebot_plugin_autoreply-0.2.6.tar` & `nonebot_plugin_autoreply-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/LICENSE
--rw-r--r--   0        0        0    11043 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/README.md
--rw-r--r--   0        0        0      303 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/__init__.py
--rw-r--r--   0        0        0     5154 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/__main__.py
--rw-r--r--   0        0        0     2449 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/config.py
--rw-r--r--   0        0        0     1005 2023-04-23 14:21:50.600650 nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/util.py
--rw-r--r--   0        0        0      610 2023-04-23 14:22:00.536596 nonebot_plugin_autoreply-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    11584 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/LICENSE
+-rw-r--r--   0        0        0    12495 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/README.md
+-rw-r--r--   0        0        0      303 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__init__.py
+-rw-r--r--   0        0        0     6387 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__main__.py
+-rw-r--r--   0        0        0     3104 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/config.py
+-rw-r--r--   0        0        0       49 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/cool_down.py
+-rw-r--r--   0        0        0     1749 2023-04-25 16:35:00.347938 nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/util.py
+-rw-r--r--   0        0        0      610 2023-04-25 16:35:11.400227 nonebot_plugin_autoreply-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_autoreply-0.2.6/LICENSE` & `nonebot_plugin_autoreply-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_autoreply-0.2.6/README.md` & `nonebot_plugin_autoreply-0.2.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,19 +27,22 @@
 </a>
 </div>
 
 ## 🛒 回复市场
 
 ![market](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/autoreply/QQ截图20230423192951.png)
 
-[点击进入](https://autoreply.lgc2333.top)
+### [点击进入](https://autoreply.lgc2333.top)
 
 我们的回复配置市场上线啦~  
 在这里，你可以分享你的回复配置，也可以找到其他人分享的回复配置，欢迎各位使用！
 
+_如果大家需要，我可以做一个直接使用指令下载安装市场中回复配置的功能 qwq_  
+_想要的话就提个 issue 吧，没人想要的话就不做了（_
+
 ## 📖 介绍
 
 一个简单的关键词自动回复插件，支持 模糊匹配、完全匹配 与 正则匹配，配置文件高度自定义  
 因为商店里没有我想要的那种关键词回复，所以我就自己写了一个  
 这个插件是从 [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/main/src/plugins/shigure_bot/plugins/keyword_reply) 那边拆出来的，我重写了一下做成了单品插件
 
 插件并没有经过深度测试，如果在使用中遇到任何问题请一定一定要过来发 issue 向我汇报，我会尽快解决  
@@ -110,26 +113,43 @@
 在里面新建一个 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
+    // 该组配置是否阻塞其他回复配置
+    // 可以不填，默认为 `true`
+    "block": true,
+
+    // 该组配置的优先级，越大越高
+    // 可以不填，默认为 1
+    "priority": 1,
+
     // 消息的匹配规则，可以放置多个
     "matches": [
       {
-        // 用于匹配消息的文本
-        "match": "测试",
-
-        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)
-        // 在正则匹配下，请使用 `\\` 在 json 里的正则表达式里表示 `\`，因为 json 解析时本身就会将 `\` 作为转义字符
+        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)、`poke`(双击头像戳一戳)
+        //
+        // 使用 `poke` 匹配时，除了 `possibility` 和 `to_me` 条件，其他的匹配条件都会被忽略
+        // 注意：`poke` 会匹配所有戳一戳事件，如果你只想要匹配 Bot 被戳的事件，请将 `to_me` 设为 `true`
+        //
         // 可以不填，默认为 `fuzzy`
         "type": "fuzzy",
 
+        // 该匹配触发的概率，范围在 0 ~ 1 之间
+        // 可以不填，默认为 1.0
+        "possibility": 1.0,
+
+        // 用于匹配消息的文本
+        // 在正则匹配下，请使用 `\\` 在 json 里的正则表达式里表示 `\`，因为 json 解析时本身就会将 `\` 作为转义字符
+        "match": "测试",
+
         // 是否需要 at 机器人才能触发（叫机器人昵称也可以）
+        // 当匹配模式为 `poke` 时，只有 被戳 的对象是 Bot，事件才会匹配成功
         // 可以不填，默认为 `false`
         "to_me": false,
 
         // 是否忽略大小写
         // 可以不填，默认为 `true`
         "ignore_case": true,
 
@@ -257,19 +277,21 @@
 
 插件提供了一些变量，他们可以被用在 `normal` 和 `array` 类型的消息，以及 `multi` 类型中嵌套的这两个类型的消息中；`plain` 类型的消息则无法使用变量  
 变量使用 `str.format()` 方法替换，所以如果想要转义 `{` 或 `}`，使用 `{{` 或 `}}` 即可
 
 下面是插件提供的变量列表
 
 - `{self_id}` - 机器人 QQ
-- `｛message_id｝` - 消息 ID
+- `{message_id}` - 消息 ID _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 - `{user_id}` - 发送者 QQ
-- `｛nickname｝` - 发送者昵称
-- `｛card｝` - 发送者群名片
-- `｛group_id｝` - 消息来源群号（私聊等为 `None`）
+- `{group_id}` - 消息来源群号 _（私聊等为 `None`）_
+- `{target_id}` - 被戳者 QQ _（仅当 `match` 的 `type` 为 `poke` 时有值，其他情况为 `None`）_
+- `{nickname}` - 发送者昵称
+- `{card}` - 发送者群名片
+- `{display_name}` - 发送者显示名称 _（优先群名片，当群名片为空时为昵称）_
 
 下面放出几个示例，帮助大家更好的理解如何使用变量
 
 ```jsonc
 [
   {
     "matches": [
@@ -317,15 +339,15 @@
         ]
       },
 
       // 无法在 plain 类型消息中使用，{user_id}、{nickname} 会原样显示
       "@[plain] [CQ:at,qq={user_id}] 啊咧？怎么 At 不了 {nickname}？",
 
       // 可以在消息中使用 {{ 和 }} 来转义大括号
-      // 前面的 ｛｛user_id｝｝ 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
+      // 前面的 {{user_id}} 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
       "[normal] [CQ:at,qq={{user_id}}] 啊咧？怎么 At 不了 {nickname}？"
     ]
   }
 ]
 ```
 
 ### 常规配置
@@ -364,14 +386,26 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.7
+
+- 新增了配置的 `block` 和 `priority` 属性
+- 新增 `type` 为 `poke` (双击头像，戳一戳) 的 `match`
+- 新增了 `match` 的 `possibility` 属性
+- 新增了 `{display_name}` 变量
+
+### 0.2.6
+
+- 回复中可以使用变量了
+- 新增配置市场
+
 ### 0.2.5
 
 - 可以加载多个回复 Json
 
 ### 0.2.4
 
 - 让字符串可以作为默认属性的 `match` 使用
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-AutoReply _â¨ èªå¨åå¤ â¨_ [license] [pypi] [python]
                           [pypi_download] [wakatime]
 ## ð åå¤å¸åº ![market](https://raw.githubusercontent.com/lgc-NB2Dev/
-readme/main/autoreply/QQæªå¾20230423192951.png) [ç¹å»è¿å¥](https://
+readme/main/autoreply/QQæªå¾20230423192951.png) ### [ç¹å»è¿å¥](https://
 autoreply.lgc2333.top) æä»¬çåå¤éç½®å¸åºä¸çº¿å¦~
 å¨è¿éï¼ä½ å¯ä»¥åäº«ä½ çåå¤éç½®ï¼ä¹å¯ä»¥æ¾å°å¶ä»äººåäº«çåå¤éç½®ï¼æ¬¢è¿åä½ä½¿ç¨ï¼
-## ð ä»ç» ä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
+_å¦æå¤§å®¶éè¦ï¼æå¯ä»¥åä¸ä¸ªç´æ¥ä½¿ç¨æä»¤ä¸è½½å®è£å¸åºä¸­åå¤éç½®çåè½
+qwq_ _æ³è¦çè¯å°±æä¸ª issue å§ï¼æ²¡äººæ³è¦çè¯å°±ä¸åäºï¼_ ##
+ð ä»ç» ä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
 æ¨¡ç³å¹éãå®å¨å¹é ä¸ æ­£åå¹éï¼éç½®æä»¶é«åº¦èªå®ä¹
 å ä¸ºååºéæ²¡æææ³è¦çé£ç§å³é®è¯åå¤ï¼æä»¥æå°±èªå·±åäºä¸ä¸ª
 è¿ä¸ªæä»¶æ¯ä» [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/
 main/src/plugins/shigure_bot/plugins/keyword_reply)
 é£è¾¹æåºæ¥çï¼æéåäºä¸ä¸åæäºååæä»¶
 æä»¶å¹¶æ²¡æç»è¿æ·±åº¦æµè¯ï¼å¦æå¨ä½¿ç¨ä¸­éå°ä»»ä½é®é¢è¯·ä¸å®ä¸å®è¦è¿æ¥å
 issue åææ±æ¥ï¼æä¼å°½å¿«è§£å³ å¦ææåè½è¯·æ±ä¹å¯ä»¥ç´æ¥å
@@ -23,21 +25,31 @@
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
 æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
 åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
-```jsonc [ { // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
-/ ç¨äºå¹éæ¶æ¯çææ¬ "match": "æµè¯", // å¹éæ¨¡å¼ï¼å¯é
-`full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é) /
-/ å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
-`\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\` ä½ä¸ºè½¬ä¹å­ç¬¦ /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
-æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ /
+```jsonc [ { // è¯¥ç»éç½®æ¯å¦é»å¡å¶ä»åå¤éç½® /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "block": true, /
+/ è¯¥ç»éç½®çä¼åçº§ï¼è¶å¤§è¶é« // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1
+"priority": 1, // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
+/ å¹éæ¨¡å¼ï¼å¯é `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`
+(æ­£åå¹é)ã`poke`(åå»å¤´åæ³ä¸æ³) // // ä½¿ç¨ `poke`
+å¹éæ¶ï¼é¤äº `possibility` å `to_me`
+æ¡ä»¶ï¼å¶ä»çå¹éæ¡ä»¶é½ä¼è¢«å¿½ç¥ // æ³¨æï¼`poke`
+ä¼å¹éæææ³ä¸æ³äºä»¶ï¼å¦æä½ åªæ³è¦å¹é Bot
+è¢«æ³çäºä»¶ï¼è¯·å° `to_me` è®¾ä¸º `true` // // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º
+`fuzzy` "type": "fuzzy", // è¯¥å¹éè§¦åçæ¦çï¼èå´å¨ 0 ~ 1 ä¹é´ /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1.0 "possibility": 1.0, /
+/ ç¨äºå¹éæ¶æ¯çææ¬ // å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json
+éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º `\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\`
+ä½ä¸ºè½¬ä¹å­ç¬¦ "match": "æµè¯", // æ¯å¦éè¦ at
+æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ // å½å¹éæ¨¡å¼ä¸º
+`poke` æ¶ï¼åªæ è¢«æ³ çå¯¹è±¡æ¯ Botï¼äºä»¶æä¼å¹éæå /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `false` "to_me": false, // æ¯å¦å¿½ç¥å¤§å°å /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "ignore_case": true, /
 / æ¯å¦å»ææ¶æ¯ååçç©ºæ ¼åå¹é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
 "strip": true, // å½å¸¦ cq ç çæ¶æ¯å¹éå¤±è´¥æ¶ï¼æ¯å¦ä½¿ç¨å»æ cq
 ç çæ¶æ¯åå¹éä¸é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
 "allow_plaintext": true }, /
 / å¦æè§åä¸ºä¸ä¸ªå­ç¬¦ä¸²ï¼åä¼è½¬æ¢ä¸ºä¸ä¸ªå±æ§å¨é¨é»è®¤ç
@@ -77,45 +89,52 @@
 "black", // è¦è¿æ»¤çQQå· "values": [ 1145141919, 9191415411 /
 / æ´å¤QQå·... ] } } // ... ] ```
 æä»¶æä¾äºä¸äºåéï¼ä»ä»¬å¯ä»¥è¢«ç¨å¨ `normal` å `array`
 ç±»åçæ¶æ¯ï¼ä»¥å `multi`
 ç±»åä¸­åµå¥çè¿ä¸¤ä¸ªç±»åçæ¶æ¯ä¸­ï¼`plain`
 ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ `str.format()`
 æ¹æ³æ¿æ¢ï¼æä»¥å¦ææ³è¦è½¬ä¹ `{` æ `}`ï¼ä½¿ç¨ `{{` æ `}}`
-å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ -
-`ï½message_idï½` - æ¶æ¯ ID - `{user_id}` - åéè QQ - `ï½nicknameï½`
-- åéèæµç§° - `ï½cardï½` - åéèç¾¤åç - `ï½group_idï½` -
-æ¶æ¯æ¥æºç¾¤å·ï¼ç§èç­ä¸º `None`ï¼
+å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ - `
+{message_id}` - æ¶æ¯ ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º
+`None`ï¼_ - `{user_id}` - åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å·
+_ï¼ç§èç­ä¸º `None`ï¼_ - `{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match`
+ç `type` ä¸º `poke` æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` -
+åéèæµç§° - `{card}` - åéèç¾¤åç - `{display_name}` -
+åéèæ¾ç¤ºåç§° _ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_
 ä¸é¢æ¾åºå ä¸ªç¤ºä¾ï¼å¸®å©å¤§å®¶æ´å¥½ççè§£å¦ä½ä½¿ç¨åé
 ```jsonc [ { "matches": [ { "match": "^(@|at|è¾ç¹)æ$", "type": "regex" } ],
 "replies": [ // å¨ normal ç±»åæ¶æ¯ä¸­ä½¿ç¨ "[normal] Atäº [CQ:at,qq=
 {user_id}]", // å¨ array ç±»åæ¶æ¯ä¸­ä½¿ç¨ [ { "type": "text", "data":
 { "text": "[array] Atäº " } }, { "type": "at", "data": { "qq": "{user_id}" } }
 ], // å¨ multi ç±»åæ¶æ¯ä¸­ä½¿ç¨ { "type": "multi", "message": [ /
 / åµå¥ç array ç±»åæ¶æ¯ [ { "type": "at", "data": { "qq": "{user_id}" }
 } ], // åµå¥ç normal ç±»åæ¶æ¯ "[multi] æåå At äºä¸ä¸ä½ å¦~
 æ¶å°äºåï¼" ] }, // æ æ³å¨ plain ç±»åæ¶æ¯ä¸­ä½¿ç¨ï¼{user_id}ã
 {nickname} ä¼åæ ·æ¾ç¤º "@[plain] [CQ:at,qq={user_id}] åå§ï¼æä¹ At
 ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {{ å }} æ¥è½¬ä¹å¤§æ¬å·
-// åé¢ç ï½ï½user_idï½ï½ ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
+// åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
 {nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={{user_id}}] åå§ï¼æä¹ At
 ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
 ä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
 éç½®é¡¹è¯·åèä¸é¢çææ¬ ```ini # matcher æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤
 False AUTOREPLY_BLOCK=False # matcher ä¼åçº§ AUTOREPLY_PRIORITY=99 ``` ##
 ð¬ æä»¤ ### `éè½½èªå¨åå¤`
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤
-Json ### 0.2.4 - è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®©
-`@` å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.7 - æ°å¢äºéç½®ç `block`
+å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke` (åå»å¤´åï¼æ³ä¸æ³) ç
+`match` - æ°å¢äº `match` ç `possibility` å±æ§ - æ°å¢äº `
+{display_name}` åé ### 0.2.6 - åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº -
+æ°å¢éç½®å¸åº ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
+è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
+å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
 `.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

### Comparing `nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/__main__.py` & `nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 import asyncio
 import random
 import re
 from itertools import starmap
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, TypeVar, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
-from nonebot import on_command, on_message
+from nonebot import on_command, on_message, on_notice
 from nonebot.adapters.onebot.v11 import (
+    Bot,
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
+    PokeNotifyEvent,
 )
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 from typing_extensions import TypeVarTuple, Unpack
 
 from nonebot_plugin_autoreply.util import (
@@ -52,17 +65,20 @@
     # 判断黑名单 值不在列表中ok
     ok = val not in will_check.values
     if will_check.type == "white":  # 白名单则反过来
         ok = not ok
     return ok
 
 
-def check_match(match: MatchType, event: MessageEvent) -> bool:
-    if isinstance(match, str):
-        match = MatchModel(match=match)
+def check_message(match: MatchModel, event: MessageEvent) -> bool:
+    if match.type == "poke":
+        return False
+
+    if not match.match:
+        raise ValueError("存在 type 不为 poke，且 match 为空的不合法匹配规则")
 
     if match.to_me and (not event.is_tome()):
         return False
 
     msg_str = str(event.message)
     msg_plaintext = event.message.extract_plain_text()
     match_template = match.match
@@ -96,31 +112,61 @@
     if (not msg_str) or (match.allow_plaintext and (not msg_plaintext)):
         return False
     return (match_template in msg_str) or (
         (match_template in msg_plaintext) if match.allow_plaintext else False
     )
 
 
-async def message_checker(event: MessageEvent, state: T_State) -> bool:
-    group = event.group_id if isinstance(event, GroupMessageEvent) else None
+def check_poke(match: MatchModel, event: PokeNotifyEvent) -> bool:
+    if match.type != "poke":
+        return False
+    return event.is_tome() if match.to_me else True
+
+
+def check_match(match: MatchType, event: Union[MessageEvent, PokeNotifyEvent]) -> bool:
+    if isinstance(match, str):
+        match = MatchModel(match=match)
+
+    if match.possibility < 1 and random.random() > match.possibility:
+        return False
 
+    return (
+        check_message(match, event)
+        if isinstance(event, MessageEvent)
+        else check_poke(match, event)
+    )
+
+
+async def message_checker(
+    event: Union[MessageEvent, PokeNotifyEvent],
+    state: T_State,
+) -> bool:
+    group = (
+        event.group_id
+        if isinstance(event, (GroupMessageEvent, PokeNotifyEvent))
+        else None
+    )
+
+    state_reply = []
     for reply in replies:
         filter_checks = [(reply.groups, group), (reply.users, event.user_id)]
         match_checks = [(x, event) for x in reply.matches]
 
         if not (
             check_list(check_filter, filter_checks)
             and check_list(check_match, match_checks, True)
         ):
             continue
 
-        state["reply"] = random.choice(reply.replies)
-        return True
+        state_reply.append(random.choice(reply.replies))
+        if reply.block:
+            break
 
-    return False
+    state["reply"] = state_reply
+    return bool(state_reply)
 
 
 def get_reply_msgs(
     reply: ReplyType,
     var_dict: Dict[str, Any],
     refuse_multi: bool = False,
 ) -> Tuple[List[Message], Optional[Tuple[int, int]]]:
@@ -153,28 +199,43 @@
             get_reply_msgs(x, var_dict, True)[0][0] for x in cast(List[ReplyModel], msg)
         ], reply.delay
 
     # default normal
     return [Message(replace_str_var(cast(str, msg), var_dict))], None
 
 
-autoreply_matcher = on_message(
+message_matcher = on_message(
+    rule=message_checker,
+    block=config.autoreply_block,
+    priority=config.autoreply_priority,
+)
+
+poke_matcher = on_notice(
     rule=message_checker,
     block=config.autoreply_block,
     priority=config.autoreply_priority,
 )
 
 
-@autoreply_matcher.handle()
-async def _(event: MessageEvent, matcher: Matcher, state: T_State):
-    reply: ReplyType = state["reply"]
-
-    msg, delay = get_reply_msgs(reply, get_var_dict(event))
-    for m in msg:
-        await matcher.send(m)
+@message_matcher.handle()
+@poke_matcher.handle()
+async def _(
+    bot: Bot,
+    event: Union[MessageEvent, PokeNotifyEvent],
+    matcher: Matcher,
+    state: T_State,
+):
+    reply: List[ReplyType] = state["reply"]
+
+    var_dict = await get_var_dict(bot, event)
+    reply_msgs = [get_reply_msgs(x, var_dict) for x in reply]
+
+    for msgs, delay in reply_msgs:
+        for x in msgs:
+            await matcher.send(x)
 
         if delay:
             await asyncio.sleep(random.randint(*delay) / 1000)
 
 
 reload_matcher = on_command("重载自动回复", permission=SUPERUSER)
```

### Comparing `nonebot_plugin_autoreply-0.2.6/nonebot_plugin_autoreply/config.py` & `nonebot_plugin_autoreply-0.2.7/nonebot_plugin_autoreply/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from typing import Any, Dict, Generic, List, Literal, Tuple, TypeVar, Union
+from typing import Any, Dict, Generic, List, Literal, Optional, Tuple, TypeVar, Union
 
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
@@ -15,16 +15,18 @@
 
 MatchType = Union[str, "MatchModel"]
 ReplyType = Union[str, List["MessageSegmentModel"], "ReplyModel"]
 MessageType = Union[str, List["MessageSegmentModel"], List[ReplyType]]
 
 
 class MatchModel(BaseModel):
-    match: str
-    type: Literal["full", "fuzzy", "regex"] = "fuzzy"  # noqa: A003
+    type: Literal["full", "fuzzy", "regex", "poke"] = "fuzzy"  # noqa: A003
+    possibility: float = 1.0
+
+    match: Optional[str] = None
     to_me: bool = False
     ignore_case: bool = True
     strip: bool = True
     allow_plaintext: bool = True
 
 
 class MessageSegmentModel(BaseModel):
@@ -39,21 +41,38 @@
 
 
 class FilterModel(BaseModel, Generic[T]):
     type: Literal["black", "white"] = "black"  # noqa: A003
     values: List[T]
 
 
+# TODO cool down
+# class CoolDownModel(BaseModel):
+#     type: Literal["user", "group"] = "group"  # noqa: A003
+#     """cd类型，user为每个人的cd，group为每个群的cd"""
+#     time: float
+#     """cd时长，单位秒"""
+#     tip: Optional[str] = None
+#     """正在cd中的提示，None或空字符串为不提示"""
+
+
 class ReplyEntryModel(BaseModel):
+    block: bool = True
+    priority: int = 1
+    # cool_down: Optional[CoolDownModel] = None
     matches: List[MatchType]
     replies: List[ReplyType]
     groups: FilterModel[int] = FilterModel(values=[])
     users: FilterModel[int] = FilterModel(values=[])
 
 
+# TODO class ResolvedReplyEntryModel
+# 在配置项载入的之后就规范化配置项模型，减少运行时开销
+
+
 class ConfigModel(BaseModel):
     autoreply_block: bool = False
     autoreply_priority: int = 99
 
 
 replies: List[ReplyEntryModel] = []
 config = ConfigModel.parse_obj(get_driver().config)
@@ -82,14 +101,15 @@
             )
             fail += 1
 
         else:
             logger.opt(colors=True).info(f"加载回复配置 <y>{file_name}</y> <l><g>成功</g></l>")
             success += 1
 
+    replies.sort(key=lambda x: x.priority)
     logger.opt(colors=True).info(
         "加载回复配置完毕，"
         f"<l><g>成功</g></l> <y>{success}</y> 个，"
         f"<l><r>失败</r></l> <y>{fail}</y> 个",
     )
     return success, fail
```

### Comparing `nonebot_plugin_autoreply-0.2.6/pyproject.toml` & `nonebot_plugin_autoreply-0.2.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-autoreply"
-version = "0.2.6"
+version = "0.2.7"
 description = "A powerful auto reply plugin for NoneBot2"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc1",
     "pydantic>=1.10.4",
```

### Comparing `nonebot_plugin_autoreply-0.2.6/PKG-INFO` & `nonebot_plugin_autoreply-0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-autoreply
-Version: 0.2.6
+Version: 0.2.7
 Summary: A powerful auto reply plugin for NoneBot2
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0rc1
@@ -42,19 +42,22 @@
 </a>
 </div>
 
 ## 🛒 回复市场
 
 ![market](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/autoreply/QQ截图20230423192951.png)
 
-[点击进入](https://autoreply.lgc2333.top)
+### [点击进入](https://autoreply.lgc2333.top)
 
 我们的回复配置市场上线啦~  
 在这里，你可以分享你的回复配置，也可以找到其他人分享的回复配置，欢迎各位使用！
 
+_如果大家需要，我可以做一个直接使用指令下载安装市场中回复配置的功能 qwq_  
+_想要的话就提个 issue 吧，没人想要的话就不做了（_
+
 ## 📖 介绍
 
 一个简单的关键词自动回复插件，支持 模糊匹配、完全匹配 与 正则匹配，配置文件高度自定义  
 因为商店里没有我想要的那种关键词回复，所以我就自己写了一个  
 这个插件是从 [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/main/src/plugins/shigure_bot/plugins/keyword_reply) 那边拆出来的，我重写了一下做成了单品插件
 
 插件并没有经过深度测试，如果在使用中遇到任何问题请一定一定要过来发 issue 向我汇报，我会尽快解决  
@@ -125,26 +128,43 @@
 在里面新建一个 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
+    // 该组配置是否阻塞其他回复配置
+    // 可以不填，默认为 `true`
+    "block": true,
+
+    // 该组配置的优先级，越大越高
+    // 可以不填，默认为 1
+    "priority": 1,
+
     // 消息的匹配规则，可以放置多个
     "matches": [
       {
-        // 用于匹配消息的文本
-        "match": "测试",
-
-        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)
-        // 在正则匹配下，请使用 `\\` 在 json 里的正则表达式里表示 `\`，因为 json 解析时本身就会将 `\` 作为转义字符
+        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)、`poke`(双击头像戳一戳)
+        //
+        // 使用 `poke` 匹配时，除了 `possibility` 和 `to_me` 条件，其他的匹配条件都会被忽略
+        // 注意：`poke` 会匹配所有戳一戳事件，如果你只想要匹配 Bot 被戳的事件，请将 `to_me` 设为 `true`
+        //
         // 可以不填，默认为 `fuzzy`
         "type": "fuzzy",
 
+        // 该匹配触发的概率，范围在 0 ~ 1 之间
+        // 可以不填，默认为 1.0
+        "possibility": 1.0,
+
+        // 用于匹配消息的文本
+        // 在正则匹配下，请使用 `\\` 在 json 里的正则表达式里表示 `\`，因为 json 解析时本身就会将 `\` 作为转义字符
+        "match": "测试",
+
         // 是否需要 at 机器人才能触发（叫机器人昵称也可以）
+        // 当匹配模式为 `poke` 时，只有 被戳 的对象是 Bot，事件才会匹配成功
         // 可以不填，默认为 `false`
         "to_me": false,
 
         // 是否忽略大小写
         // 可以不填，默认为 `true`
         "ignore_case": true,
 
@@ -272,19 +292,21 @@
 
 插件提供了一些变量，他们可以被用在 `normal` 和 `array` 类型的消息，以及 `multi` 类型中嵌套的这两个类型的消息中；`plain` 类型的消息则无法使用变量  
 变量使用 `str.format()` 方法替换，所以如果想要转义 `{` 或 `}`，使用 `{{` 或 `}}` 即可
 
 下面是插件提供的变量列表
 
 - `{self_id}` - 机器人 QQ
-- `｛message_id｝` - 消息 ID
+- `{message_id}` - 消息 ID _（当 `match` 的 `type` 为 `poke` 时为 `None`）_
 - `{user_id}` - 发送者 QQ
-- `｛nickname｝` - 发送者昵称
-- `｛card｝` - 发送者群名片
-- `｛group_id｝` - 消息来源群号（私聊等为 `None`）
+- `{group_id}` - 消息来源群号 _（私聊等为 `None`）_
+- `{target_id}` - 被戳者 QQ _（仅当 `match` 的 `type` 为 `poke` 时有值，其他情况为 `None`）_
+- `{nickname}` - 发送者昵称
+- `{card}` - 发送者群名片
+- `{display_name}` - 发送者显示名称 _（优先群名片，当群名片为空时为昵称）_
 
 下面放出几个示例，帮助大家更好的理解如何使用变量
 
 ```jsonc
 [
   {
     "matches": [
@@ -332,15 +354,15 @@
         ]
       },
 
       // 无法在 plain 类型消息中使用，{user_id}、{nickname} 会原样显示
       "@[plain] [CQ:at,qq={user_id}] 啊咧？怎么 At 不了 {nickname}？",
 
       // 可以在消息中使用 {{ 和 }} 来转义大括号
-      // 前面的 ｛｛user_id｝｝ 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
+      // 前面的 {{user_id}} 会转义成 {user_id} 发送，而后面的 {nickname} 会被替换
       "[normal] [CQ:at,qq={{user_id}}] 啊咧？怎么 At 不了 {nickname}？"
     ]
   }
 ]
 ```
 
 ### 常规配置
@@ -379,14 +401,26 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.7
+
+- 新增了配置的 `block` 和 `priority` 属性
+- 新增 `type` 为 `poke` (双击头像，戳一戳) 的 `match`
+- 新增了 `match` 的 `possibility` 属性
+- 新增了 `{display_name}` 变量
+
+### 0.2.6
+
+- 回复中可以使用变量了
+- 新增配置市场
+
 ### 0.2.5
 
 - 可以加载多个回复 Json
 
 ### 0.2.4
 
 - 让字符串可以作为默认属性的 `match` 使用
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.6 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.7 Summary: A
 powerful auto reply plugin for NoneBot2 Home-page: https://github.com/lgc-
 NB2Dev/nonebot-plugin-autoreply Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-autoreply Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0rc1 Requires-Dist: pydantic>=1.10.4 Requires-Dist: nonebot-
 adapter-onebot>=2.1.0 Requires-Dist: typing-extensions>=4.4.0 Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-AutoReply _â¨ èªå¨åå¤ â¨_ [license] [pypi] [python]
                           [pypi_download] [wakatime]
 ## ð åå¤å¸åº ![market](https://raw.githubusercontent.com/lgc-NB2Dev/
-readme/main/autoreply/QQæªå¾20230423192951.png) [ç¹å»è¿å¥](https://
+readme/main/autoreply/QQæªå¾20230423192951.png) ### [ç¹å»è¿å¥](https://
 autoreply.lgc2333.top) æä»¬çåå¤éç½®å¸åºä¸çº¿å¦~
 å¨è¿éï¼ä½ å¯ä»¥åäº«ä½ çåå¤éç½®ï¼ä¹å¯ä»¥æ¾å°å¶ä»äººåäº«çåå¤éç½®ï¼æ¬¢è¿åä½ä½¿ç¨ï¼
-## ð ä»ç» ä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
+_å¦æå¤§å®¶éè¦ï¼æå¯ä»¥åä¸ä¸ªç´æ¥ä½¿ç¨æä»¤ä¸è½½å®è£å¸åºä¸­åå¤éç½®çåè½
+qwq_ _æ³è¦çè¯å°±æä¸ª issue å§ï¼æ²¡äººæ³è¦çè¯å°±ä¸åäºï¼_ ##
+ð ä»ç» ä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
 æ¨¡ç³å¹éãå®å¨å¹é ä¸ æ­£åå¹éï¼éç½®æä»¶é«åº¦èªå®ä¹
 å ä¸ºååºéæ²¡æææ³è¦çé£ç§å³é®è¯åå¤ï¼æä»¥æå°±èªå·±åäºä¸ä¸ª
 è¿ä¸ªæä»¶æ¯ä» [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/
 main/src/plugins/shigure_bot/plugins/keyword_reply)
 é£è¾¹æåºæ¥çï¼æéåäºä¸ä¸åæäºååæä»¶
 æä»¶å¹¶æ²¡æç»è¿æ·±åº¦æµè¯ï¼å¦æå¨ä½¿ç¨ä¸­éå°ä»»ä½é®é¢è¯·ä¸å®ä¸å®è¦è¿æ¥å
 issue åææ±æ¥ï¼æä¼å°½å¿«è§£å³ å¦ææåè½è¯·æ±ä¹å¯ä»¥ç´æ¥å
@@ -31,21 +33,31 @@
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
 æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
 åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
-```jsonc [ { // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
-/ ç¨äºå¹éæ¶æ¯çææ¬ "match": "æµè¯", // å¹éæ¨¡å¼ï¼å¯é
-`full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é) /
-/ å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
-`\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\` ä½ä¸ºè½¬ä¹å­ç¬¦ /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
-æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ /
+```jsonc [ { // è¯¥ç»éç½®æ¯å¦é»å¡å¶ä»åå¤éç½® /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "block": true, /
+/ è¯¥ç»éç½®çä¼åçº§ï¼è¶å¤§è¶é« // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1
+"priority": 1, // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
+/ å¹éæ¨¡å¼ï¼å¯é `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`
+(æ­£åå¹é)ã`poke`(åå»å¤´åæ³ä¸æ³) // // ä½¿ç¨ `poke`
+å¹éæ¶ï¼é¤äº `possibility` å `to_me`
+æ¡ä»¶ï¼å¶ä»çå¹éæ¡ä»¶é½ä¼è¢«å¿½ç¥ // æ³¨æï¼`poke`
+ä¼å¹éæææ³ä¸æ³äºä»¶ï¼å¦æä½ åªæ³è¦å¹é Bot
+è¢«æ³çäºä»¶ï¼è¯·å° `to_me` è®¾ä¸º `true` // // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º
+`fuzzy` "type": "fuzzy", // è¯¥å¹éè§¦åçæ¦çï¼èå´å¨ 0 ~ 1 ä¹é´ /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º 1.0 "possibility": 1.0, /
+/ ç¨äºå¹éæ¶æ¯çææ¬ // å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json
+éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º `\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\`
+ä½ä¸ºè½¬ä¹å­ç¬¦ "match": "æµè¯", // æ¯å¦éè¦ at
+æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ // å½å¹éæ¨¡å¼ä¸º
+`poke` æ¶ï¼åªæ è¢«æ³ çå¯¹è±¡æ¯ Botï¼äºä»¶æä¼å¹éæå /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `false` "to_me": false, // æ¯å¦å¿½ç¥å¤§å°å /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "ignore_case": true, /
 / æ¯å¦å»ææ¶æ¯ååçç©ºæ ¼åå¹é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
 "strip": true, // å½å¸¦ cq ç çæ¶æ¯å¹éå¤±è´¥æ¶ï¼æ¯å¦ä½¿ç¨å»æ cq
 ç çæ¶æ¯åå¹éä¸é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
 "allow_plaintext": true }, /
 / å¦æè§åä¸ºä¸ä¸ªå­ç¬¦ä¸²ï¼åä¼è½¬æ¢ä¸ºä¸ä¸ªå±æ§å¨é¨é»è®¤ç
@@ -85,45 +97,52 @@
 "black", // è¦è¿æ»¤çQQå· "values": [ 1145141919, 9191415411 /
 / æ´å¤QQå·... ] } } // ... ] ```
 æä»¶æä¾äºä¸äºåéï¼ä»ä»¬å¯ä»¥è¢«ç¨å¨ `normal` å `array`
 ç±»åçæ¶æ¯ï¼ä»¥å `multi`
 ç±»åä¸­åµå¥çè¿ä¸¤ä¸ªç±»åçæ¶æ¯ä¸­ï¼`plain`
 ç±»åçæ¶æ¯åæ æ³ä½¿ç¨åé åéä½¿ç¨ `str.format()`
 æ¹æ³æ¿æ¢ï¼æä»¥å¦ææ³è¦è½¬ä¹ `{` æ `}`ï¼ä½¿ç¨ `{{` æ `}}`
-å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ -
-`ï½message_idï½` - æ¶æ¯ ID - `{user_id}` - åéè QQ - `ï½nicknameï½`
-- åéèæµç§° - `ï½cardï½` - åéèç¾¤åç - `ï½group_idï½` -
-æ¶æ¯æ¥æºç¾¤å·ï¼ç§èç­ä¸º `None`ï¼
+å³å¯ ä¸é¢æ¯æä»¶æä¾çåéåè¡¨ - `{self_id}` - æºå¨äºº QQ - `
+{message_id}` - æ¶æ¯ ID _ï¼å½ `match` ç `type` ä¸º `poke` æ¶ä¸º
+`None`ï¼_ - `{user_id}` - åéè QQ - `{group_id}` - æ¶æ¯æ¥æºç¾¤å·
+_ï¼ç§èç­ä¸º `None`ï¼_ - `{target_id}` - è¢«æ³è QQ _ï¼ä»å½ `match`
+ç `type` ä¸º `poke` æ¶æå¼ï¼å¶ä»æåµä¸º `None`ï¼_ - `{nickname}` -
+åéèæµç§° - `{card}` - åéèç¾¤åç - `{display_name}` -
+åéèæ¾ç¤ºåç§° _ï¼ä¼åç¾¤åçï¼å½ç¾¤åçä¸ºç©ºæ¶ä¸ºæµç§°ï¼_
 ä¸é¢æ¾åºå ä¸ªç¤ºä¾ï¼å¸®å©å¤§å®¶æ´å¥½ççè§£å¦ä½ä½¿ç¨åé
 ```jsonc [ { "matches": [ { "match": "^(@|at|è¾ç¹)æ$", "type": "regex" } ],
 "replies": [ // å¨ normal ç±»åæ¶æ¯ä¸­ä½¿ç¨ "[normal] Atäº [CQ:at,qq=
 {user_id}]", // å¨ array ç±»åæ¶æ¯ä¸­ä½¿ç¨ [ { "type": "text", "data":
 { "text": "[array] Atäº " } }, { "type": "at", "data": { "qq": "{user_id}" } }
 ], // å¨ multi ç±»åæ¶æ¯ä¸­ä½¿ç¨ { "type": "multi", "message": [ /
 / åµå¥ç array ç±»åæ¶æ¯ [ { "type": "at", "data": { "qq": "{user_id}" }
 } ], // åµå¥ç normal ç±»åæ¶æ¯ "[multi] æåå At äºä¸ä¸ä½ å¦~
 æ¶å°äºåï¼" ] }, // æ æ³å¨ plain ç±»åæ¶æ¯ä¸­ä½¿ç¨ï¼{user_id}ã
 {nickname} ä¼åæ ·æ¾ç¤º "@[plain] [CQ:at,qq={user_id}] åå§ï¼æä¹ At
 ä¸äº {nickname}ï¼", // å¯ä»¥å¨æ¶æ¯ä¸­ä½¿ç¨ {{ å }} æ¥è½¬ä¹å¤§æ¬å·
-// åé¢ç ï½ï½user_idï½ï½ ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
+// åé¢ç {{user_id}} ä¼è½¬ä¹æ {user_id} åéï¼èåé¢ç
 {nickname} ä¼è¢«æ¿æ¢ "[normal] [CQ:at,qq={{user_id}}] åå§ï¼æä¹ At
 ä¸äº {nickname}ï¼" ] } ] ``` ### å¸¸è§éç½®
 ä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
 éç½®é¡¹è¯·åèä¸é¢çææ¬ ```ini # matcher æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤
 False AUTOREPLY_BLOCK=False # matcher ä¼åçº§ AUTOREPLY_PRIORITY=99 ``` ##
 ð¬ æä»¤ ### `éè½½èªå¨åå¤`
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤
-Json ### 0.2.4 - è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®©
-`@` å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.7 - æ°å¢äºéç½®ç `block`
+å `priority` å±æ§ - æ°å¢ `type` ä¸º `poke` (åå»å¤´åï¼æ³ä¸æ³) ç
+`match` - æ°å¢äº `match` ç `possibility` å±æ§ - æ°å¢äº `
+{display_name}` åé ### 0.2.6 - åå¤ä¸­å¯ä»¥ä½¿ç¨åéäº -
+æ°å¢éç½®å¸åº ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤ Json ### 0.2.4 -
+è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
+å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
 `.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

