# Comparing `tmp/nonebot_plugin_bawiki-0.7.4.tar.gz` & `tmp/nonebot_plugin_bawiki-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.7.5.tar", last modified: Tue Apr 25 14:30:55 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.4.tar` & `nonebot_plugin_bawiki-0.7.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/LICENSE
--rw-r--r--   0        0        0     7591 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/README.md
--rw-r--r--   0        0        0    15523 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    22508 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0      899 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5568 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     7741 2023-04-02 05:13:10.631492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    17914 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     6778 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-04-02 05:13:10.635492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-04-02 05:13:10.639492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-04-02 05:13:10.639492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     2722 2023-04-02 05:13:10.639492 nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1402 2023-04-02 05:13:10.639492 nonebot_plugin_bawiki-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     9395 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/LICENSE
+-rw-r--r--   0        0        0     7660 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/README.md
+-rw-r--r--   0        0        0    15528 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0    22575 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__main__.py
+-rw-r--r--   0        0        0     1881 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0     5812 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_bawiki.py
+-rw-r--r--   0        0        0     8291 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_gamekee.py
+-rw-r--r--   0        0        0    18827 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_schaledb.py
+-rw-r--r--   0        0        0     7390 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0    21514 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-04-25 14:30:37.375213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gradient.png
+-rw-r--r--   0        0        0      872 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/resource.py
+-rw-r--r--   0        0        0     3555 2023-04-25 14:30:37.379213 nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1381 2023-04-25 14:30:55.087487 nonebot_plugin_bawiki-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.5/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.4/LICENSE` & `nonebot_plugin_bawiki-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/README.md` & `nonebot_plugin_bawiki-0.7.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/nonebot-plugin-bawiki.png" width="200" height="200" alt="BAWiki"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/bawiki/nonebot-plugin-bawiki.png" width="200" height="200" alt="BAWiki"></a>
 </div>
 
 <div align="center">
 
 # NoneBot-Plugin-BAWiki
 
 _✨ 基于 NoneBot2 的碧蓝档案 Wiki 插件 ✨_
@@ -44,116 +44,105 @@
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```bash
-nb plugin install nonebot-plugin-example
+nb plugin install nonebot-plugin-bawiki
 ```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
 ```bash
-pip install nonebot-plugin-example
+pip install nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>pdm</summary>
 
 ```bash
-pdm add nonebot-plugin-example
+pdm add nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>poetry</summary>
 
 ```bash
-poetry add nonebot-plugin-example
+poetry add nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>conda</summary>
 
 ```bash
-conda install nonebot-plugin-example
+conda install nonebot-plugin-bawiki
 ```
 
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
 ```toml
 [tool.nonebot]
 plugins = [
     # ...
-    "nonebot_plugin_example"
+    "nonebot_plugin_bawiki"
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值 |                         说明                          |
-| :--------------------: | :--: | :----: | :---------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None` | 访问`SchaleDB`、`bawiki-data`的 json 数据时使用的代理 |
-|    `BA_GAMEKEE_URL`    |  否  |  ...   |                 GameKee 数据源的地址                  |
-|    `BA_SCHALE_URL`     |  否  |  ...   |               SchaleDB Json 数据的地址                |
-| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                SchaleDB 网页截图的地址                |
-|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                  bawiki-data 的地址                   |
+|         配置项         | 必填 | 默认值 |                          说明                           |
+| :--------------------: | :--: | :----: | :-----------------------------------------------------: |
+|       `BA_PROXY`       |  否  | `None` | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
+|  `BA_GACHA_COOL_DOWN`  |  否  |  `0`   |               每群每人的抽卡冷却，单位秒                |
+|    `BA_GAMEKEE_URL`    |  否  |  ...   |                  GameKee 数据源的地址                   |
+|    `BA_SCHALE_URL`     |  否  |  ...   |                SchaleDB Json 数据的地址                 |
+| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                 SchaleDB 网页截图的地址                 |
+|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                   bawiki-data 的地址                    |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
-见[这里](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py#L17)
+**现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
 
-待更新
-
-<!--
-### 效果图
-
-<details>
-<summary>长图，点击展开</summary>
-
-![example](https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/example.png)
-![example2](https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/example2.png)
-
-</details>
--->
+如果你不想用 PicMenu 的话，那么请看 [\_\_init\_\_.py](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py)
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
 ### [RainNight0](https://github.com/RainNight0)
 
 - 日程表 html 模板提供（已弃用）
 
-### `bawiki-data`数据源贡献列表
+### `bawiki-data` 数据源贡献列表
 
 - 见 [bawiki-data](http://github.com/lgc2333/bawiki-data)
 
 ## 💰 赞助
 
 感谢各位大佬的投喂……！！本 fw 实在感激不尽……
 
@@ -163,19 +152,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-### 0.7.3
+### 0.7.5
 
-- 修复 bug
+- 插件可以自动帮你配置 PicMenu 的字体了
+- 给抽卡新增了冷却
 
-### 0.7.2
+### 0.7.2 ~ 0.7.4
 
 - 修复 bug
 
 ### 0.7.1
 
 - 更改配置项名称
```

#### html2text {}

```diff
@@ -6,45 +6,50 @@
 [ç¹å»è·³è½¬ bawiki-data](https://github.com/lgc2333/bawiki-data)
 ä¿®æ¹åæäº¤ Pull Request å³å¯ï¼ ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç
 Wiki æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
 [SchaleDB](https://lonqie.github.io/SchaleDB/) æä»¶çµææ¥æºï¼
 [ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145) ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-example
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-bawiki
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip ```bash pip install nonebot-plugin-example ```   pdm ```bash pdm add
-nonebot-plugin-example ```   poetry ```bash poetry add nonebot-plugin-example
-```   conda ```bash conda install nonebot-plugin-example ```  æå¼ nonebot2
+pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
+nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
+conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_example" ] ```  ## âï¸ éç½® å¨ nonebot2
+"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :----: | :--------------
--------------------------------------: | | `BA_PROXY` | å¦ | `None` |
-è®¿é®`SchaleDB`ã`bawiki-data`ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+---------------------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
+`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
 `BA_GAMEKEE_URL` | å¦ | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` |
 å¦ | ... | SchaleDB Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ |
 ... | SchaleDB ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... |
 bawiki-data çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) è§[è¿é]
-(https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/
-nonebot_plugin_bawiki/__init__.py#L17) å¾æ´æ°  ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+ä¼èªå¨å¸®ä½ æ PicMenu
+çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
+å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
+github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
+__init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
+lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
+é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
-æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-
-data`æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/
-bawiki-data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
+æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
+æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
+data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.3 - ä¿®å¤ bug ### 0.7.2 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ###
-0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
+æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
-from .__main__ import *  # noqa: E402, F403
+from . import __main__ as __main__  # noqa: E402
 
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=(
         "感谢各位sensei使用本插件！\n"
         "插件有缓存机制，每3小时自动清空一次，如果插件遇到问题可以先手动清空缓存试一下捏\n"
         "装载PicMenu插件即可查看插件详细菜单哦\n"
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/__main__.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Dict, List, Optional
 
 from nonebot import on_command, on_shell_command
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
+    GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
 )
 from nonebot.exception import FinishedException, ParserExit
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
@@ -58,15 +59,15 @@
     draw_fav_li,
     find_current_event,
     schale_calender,
     schale_get_common,
     schale_get_stu_dict,
     schale_get_stu_info,
 )
-from .gacha import gacha
+from .gacha import gacha, get_gacha_cool_down, set_gacha_cool_down
 from .util import async_req, clear_req_cache, recover_alia, splice_msg
 
 
 @dataclass()
 class GachaPool:
     name: str
     pool: List[int]
@@ -110,115 +111,115 @@
 
             await asyncio.gather(
                 *[
                     matcher.send(x)
                     for x in (
                         await asyncio.gather(*[schale_calender(x) for x in servers])
                     )
-                ]
+                ],
             )
             await matcher.finish()
         else:
             await matcher.finish(await game_kee_calender())
     except (FinishedException, ActionFailed):  # type: ignore
         raise
     except:
         logger.exception("绘制日程表图片出错")
-        return await matcher.finish("绘制日程表图片出错，请检查后台输出")
+        await matcher.finish("绘制日程表图片出错，请检查后台输出")
 
 
 async def send_wiki_page(sid, matcher: Matcher):
     url = game_kee_page_url(sid)
     await matcher.send(f"请稍等，正在截取Wiki页面……\n{url}")
 
     try:
         img = await game_kee_get_page(url)
     except:
         logger.exception(f"截取wiki页面出错 {url}")
-        return await matcher.finish("截取页面出错，请检查后台输出")
+        await matcher.finish("截取页面出错，请检查后台输出")
 
     await matcher.finish(MessageSegment.image(img))
 
 
 stu_schale = on_command("ba学生图鉴")
 
 
 @stu_schale.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
-        return await matcher.finish("请提供学生名称")
+        await matcher.finish("请提供学生名称")
 
     try:
         ret = await schale_get_stu_dict()
     except:
         logger.exception("获取学生列表出错")
-        return await matcher.finish("获取学生列表表出错，请检查后台输出")
+        await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if not ret:
-        return await matcher.finish("没有获取到学生列表数据")
+        await matcher.finish("没有获取到学生列表数据")
 
     if not (data := ret.get(await recover_stu_alia(arg))):
-        return await matcher.finish("未找到该学生")
+        await matcher.finish("未找到该学生")
 
     stu_name = data["PathName"]
     await matcher.send(f"请稍等，正在截取SchaleDB页面～\n{config.ba_schale_url}?chara={stu_name}")
 
     try:
         img = MessageSegment.image(await schale_get_stu_info(stu_name))
     except:
         logger.exception(f"截取schale db页面出错 chara={stu_name}")
-        return await matcher.finish("截取页面出错，请检查后台输出")
+        await matcher.finish("截取页面出错，请检查后台输出")
 
     await matcher.finish(img)
 
 
 stu_rank = on_command("ba学生评价", aliases={"ba角评"})
 
 
 @stu_rank.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
-        return await matcher.finish("请提供学生名称")
+        await matcher.finish("请提供学生名称")
 
     if arg == "总览" or arg == "全部" or arg.lower() == "all":
         arg = "all"
     else:
         arg = await recover_stu_alia(arg)
 
     try:
         im = await db_wiki_stu(arg)
     except:
         logger.exception("获取角评出错")
-        return await matcher.finish("获取角评出错，请检查后台输出")
+        await matcher.finish("获取角评出错，请检查后台输出")
 
     await matcher.finish(im)
 
 
 stu_wiki = on_command("ba学生wiki", aliases={"ba学生Wiki", "ba学生WIKI"})
 
 
 @stu_wiki.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
-        return await matcher.finish("请提供学生名称")
+        await matcher.finish("请提供学生名称")
 
     try:
         ret = await game_kee_get_stu_cid_li()
     except:
         logger.exception("获取学生列表出错")
-        return await matcher.finish("获取学生列表出错，请检查后台输出")
+        await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
-        return await matcher.finish("没有获取到学生列表数据")
+        await matcher.finish("没有获取到学生列表数据")
 
     if not (sid := ret.get(await recover_stu_alia(arg, True))):
-        return await matcher.finish("未找到该学生")
+        await matcher.finish("未找到该学生")
 
     await send_wiki_page(sid, matcher)
 
 
 fav = on_command("ba好感度", aliases={"ba羁绊", "bal2d", "baL2D", "balive2d", "baLive2D"})
 
 
@@ -228,74 +229,80 @@
         if r := (await db_get_extra_l2d_list()).get(stu_name):
             return f"{config.ba_bawiki_db_url}{r}"
 
         return await game_kee_grab_l2d((await game_kee_get_stu_cid_li()).get(stu_name))
 
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
-        return await matcher.finish("请提供学生名称或所需的羁绊等级")
+        await matcher.finish("请提供学生名称或所需的羁绊等级")
 
     # 好感度等级
     if arg.isdigit():
         arg = int(arg)
         if arg > 9:
-            return await matcher.finish("学生解锁L2D最高只需要羁绊等级9")
+            await matcher.finish("学生解锁L2D最高只需要羁绊等级9")
         if arg < 1:
-            return await matcher.finish("学生解锁L2D最低只需要羁绊等级1")
+            await matcher.finish("学生解锁L2D最低只需要羁绊等级1")
 
         try:
             p = await draw_fav_li(arg)
         except:
             logger.exception("绘制图片出错")
-            return await matcher.finish("绘制图片出错，请检查后台输出")
+            await matcher.finish("绘制图片出错，请检查后台输出")
 
-        return await matcher.finish(p)
+        await matcher.finish(p)
 
     # 学生名称
     arg = await recover_stu_alia(arg)
 
     try:
         ret = await schale_get_stu_dict()
     except:
         logger.exception("获取学生列表出错")
-        return await matcher.finish("获取学生列表表出错，请检查后台输出")
+        await matcher.finish("获取学生列表表出错，请检查后台输出")
 
     if stu := ret.get(arg):
         if not (lvl := stu["MemoryLobby"]):
-            return await matcher.finish("该学生没有L2D")
+            await matcher.finish("该学生没有L2D")
 
         im = MessageSegment.text(f'{stu["Name"]} 在羁绊等级 {lvl[0]} 时即可解锁L2D\nL2D预览：')
         if p := await get_l2d(await schale_to_gamekee(arg)):
             im += [MessageSegment.image(await async_req(x, raw=True)) for x in p]
         else:
             im += (
                 "没找到该学生的L2D看板\n"
                 "可能原因：\n"
                 "- GameKee页面爬取不到角色L2D图片\n"
                 "- GameKee和插件没有收录该学生的L2D\n"
             )
-        return await matcher.finish(im)
+        await matcher.finish(im)
 
-    return await matcher.finish("未找到学生")
+    await matcher.finish("未找到学生")
 
 
 raid_wiki_parser = ArgumentParser("ba总力战")
 raid_wiki_parser.add_argument(
-    "name", nargs="?", default=None, help="总力战Boss名称，不指定默认取当前服务器总力战Boss"
+    "name",
+    nargs="?",
+    default=None,
+    help="总力战Boss名称，不指定默认取当前服务器总力战Boss",
 )
 raid_wiki_parser.add_argument(
     "-s",
     "--server",
     nargs="*",
     help="服务器名称，`j`或`日`代表日服，`g`或`国`代表国际服，可指定多个，默认全选",
     default=["j", "g"],
 )
 raid_wiki_parser.add_argument("-t", "--terrain", help="指定总力战环境，不指定默认全选，不带Boss名称该参数无效")
 raid_wiki_parser.add_argument(
-    "-w", "--wiki", action="store_true", help="发送该总力战Boss的技能机制而不是配队推荐"
+    "-w",
+    "--wiki",
+    action="store_true",
+    help="发送该总力战Boss的技能机制而不是配队推荐",
 )
 
 raid_wiki = on_shell_command("ba总力战", parser=raid_wiki_parser)
 
 
 @raid_wiki.handle()
 async def _(matcher: Matcher, foo: ParserExit = ShellCommandArgs()):
@@ -323,139 +330,139 @@
     if not args.name:
         try:
             common = await schale_get_common()
             for s in server:
                 raid = common["regions"][s]["current_raid"]
                 if (r := find_current_event(raid)) and (raid := r[0]["raid"]) < 1000:
                     tasks.append(
-                        db_wiki_raid(raid, [s], args.wiki, r[0].get("terrain"))
+                        db_wiki_raid(raid, [s], args.wiki, r[0].get("terrain")),
                     )
         except:
             logger.exception("获取当前总力战失败")
-            return await matcher.finish("获取当前总力战失败")
+            await matcher.finish("获取当前总力战失败")
 
         if not tasks:
-            return await matcher.finish("目前服务器没有正在进行的总力战，请手动指定")
+            await matcher.finish("目前服务器没有正在进行的总力战，请手动指定")
     else:
         tasks.append(
             db_wiki_raid(
                 recover_alia(args.name, await db_get_raid_alias()),
                 server,
                 args.wiki,
                 (
                     recover_alia(args.terrain, await db_get_terrain_alias())
                     if args.terrain
                     else None
                 ),
-            )
+            ),
         )
 
     try:
         ret = await asyncio.gather(*tasks)
     except:
         logger.exception("获取总力战wiki失败")
-        return await matcher.finish("获取图片失败，请检查后台输出")
+        await matcher.finish("获取图片失败，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
 
 
 event_wiki = on_command("ba活动")
 
 
 @event_wiki.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().lower().strip()
 
     server = []
-    if arg.startswith("日") or arg.startswith("j") or (not arg):
+    if arg.startswith(("日", "j")) or not arg:
         server.append(0)
-    if arg.startswith("国") or arg.startswith("g") or (not arg):
+    if arg.startswith(("国", "g")) or not arg:
         server.append(1)
 
     events = []
     if server:
         try:
             common = await schale_get_common()
             for s in server:
                 ev = common["regions"][s]["current_events"]
                 if e := find_current_event(ev):
                     events.append((e[0]["event"]) % 10000)
         except:
             logger.exception("获取当前活动失败")
-            return await matcher.finish("获取当前活动失败")
+            await matcher.finish("获取当前活动失败")
 
         if not events:
             await matcher.finish("当前服务器没有正在进行的活动")
 
     else:
         events.append(recover_alia(arg, await db_get_event_alias()))
 
     try:
         ret = await asyncio.gather(*[db_wiki_event(x) for x in events])
     except:
         logger.exception("获取活动wiki出错")
-        return await matcher.finish("获取图片出错，请检查后台输出")
+        await matcher.finish("获取图片出错，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
 
 
 time_atk_wiki = on_command("ba综合战术考试", aliases={"ba合同火力演习", "ba战术考试", "ba火力演习"})
 
 
 @time_atk_wiki.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().lower().strip()
 
     server = []
-    if arg.startswith("日") or arg.startswith("j") or (not arg):
+    if arg.startswith(("日", "j")) or not arg:
         server.append(0)
-    if arg.startswith("国") or arg.startswith("g") or (not arg):
+    if arg.startswith(("国", "g")) or not arg:
         server.append(1)
 
     events = []
     if server:
         try:
             common = await schale_get_common()
             for s in server:
                 raid = common["regions"][s]["current_raid"]
                 if (r := find_current_event(raid)) and (raid := r[0]["raid"]) >= 1000:
                     events.append(raid)
         except:
             logger.exception("获取当前综合战术考试失败")
-            return await matcher.finish("获取当前综合战术考试失败")
+            await matcher.finish("获取当前综合战术考试失败")
 
         if not events:
             await matcher.finish("当前服务器没有正在进行的综合战术考试")
 
     else:
         if (not str(arg).isdigit()) or ((arg := int(arg)) < 1):
             await matcher.finish("综合战术考试ID需为整数，从1开始，代表第1个综合战术考试")
         events.append(arg)
 
     try:
         ret = await asyncio.gather(*[db_wiki_time_atk(x) for x in events])
     except:
         logger.exception("获取综合战术考试wiki出错")
-        return await matcher.finish("获取图片出错，请检查后台输出")
+        await matcher.finish("获取图片出错，请检查后台输出")
 
     await matcher.finish(splice_msg(ret))
 
 
 craft_wiki = on_command("ba制造", aliases={"ba合成", "ba制作"})
 
 
 @craft_wiki.handle()
 async def _(matcher: Matcher):
     try:
         im = await db_wiki_craft()
     except:
         logger.exception("获取合成wiki图片错误")
-        return await matcher.finish("获取图片失败，请检查后台输出")
+        await matcher.finish("获取图片失败，请检查后台输出")
 
-    await matcher.finish(im)
+    await matcher.finish(Message(im))
 
 
 global_future = on_command("ba国际服千里眼", aliases={"ba千里眼", "ba国际服前瞻", "ba前瞻"})
 
 
 @global_future.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()):
@@ -484,73 +491,75 @@
             except ValueError:
                 pass
         if not parsed_date:
             await matcher.finish("日期格式不正确！")
         date = parsed_date
         if date.year == 1900:
             now = datetime.datetime.now().replace(
-                hour=0, minute=0, second=0, microsecond=0
+                hour=0,
+                minute=0,
+                second=0,
+                microsecond=0,
             )
             date = date.replace(year=now.year)
             if date < now:
                 date = date.replace(year=now.year + 1)
 
-    if isinstance(num, str):
-        if (not num.isdigit()) or (num := int(num)) < 1:
-            await matcher.finish("前瞻项目数量格式不正确！")
+    if isinstance(num, str) and ((not num.isdigit()) or (num := int(num)) < 1):
+        await matcher.finish("前瞻项目数量格式不正确！")
 
-    await matcher.finish(await db_global_future(date, num))
+    await matcher.finish(await db_global_future(date or None, num))
 
 
 furniture_wiki = on_command("ba互动家具")
 
 
 @furniture_wiki.handle()
 async def _(matcher: Matcher):
     try:
         im = await db_wiki_furniture()
     except:
         logger.exception("获取互动家具wiki图片错误")
-        return await matcher.finish("获取图片失败，请检查后台输出")
+        await matcher.finish("获取图片失败，请检查后台输出")
 
-    await matcher.finish(im)
+    await matcher.finish(Message(im))
 
 
 voice = on_command("ba语音")
 
 
 @voice.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
-        return await matcher.finish("请提供学生名称")
+        await matcher.finish("请提供学生名称")
 
     arg = arg.split()
     arg_len = len(arg)
     name = " ".join(arg[:-1]) if arg_len > 1 else arg[0]
     v_type = arg[-1].strip().lower() if arg_len > 1 else None
 
     try:
         ret = await game_kee_get_stu_cid_li()
     except:
         logger.exception("获取学生列表出错")
-        return await matcher.finish("获取学生列表出错，请检查后台输出")
+        await matcher.finish("获取学生列表出错，请检查后台输出")
 
     if not ret:
-        return await matcher.finish("没有获取到学生列表数据")
+        await matcher.finish("没有获取到学生列表数据")
 
     try:
         org_stu_name = await recover_stu_alia(name, True)
         stu_name = await schale_to_gamekee(org_stu_name)
     except:
         logger.exception("还原学生别名失败")
-        return await matcher.finish("还原学生别名失败，请检查后台输出")
+        await matcher.finish("还原学生别名失败，请检查后台输出")
 
     if not (sid := ret.get(stu_name)):
-        return await matcher.finish("未找到该学生")
+        await matcher.finish("未找到该学生")
 
     voices = await game_kee_get_voice(sid)
     if v_type:
         voices = [x for x in voices if v_type in x.title.lower()]
     if not voices:
         await matcher.finish("没找到符合要求的语音捏")
 
@@ -564,20 +573,19 @@
         im.append(v.cn)
     await matcher.send("\n".join(im))
     await matcher.send(MessageSegment.record(v_data))
 
 
 def get_1st_pool(data: dict) -> Optional[GachaPool]:
     if not data:
-        return
+        return None
 
     pool_data = data["current_pools"]
     pool = pool_data[0]
-    pool_obj = GachaPool(name=pool["name"], pool=pool["pool"], index=0)
-    return pool_obj
+    return GachaPool(name=pool["name"], pool=pool["pool"], index=0)
 
 
 change_pool = on_command("ba切换卡池")
 
 
 @change_pool.handle()
 async def _(matcher: Matcher, event: MessageEvent, cmd_arg: Message = CommandArg()):
@@ -590,15 +598,15 @@
         else:
             pool = []
             try:
                 stu_li = await schale_get_stu_dict()
                 stu_alias = await db_get_stu_alias()
             except:
                 logger.exception("获取学生列表或别名失败")
-                return await matcher.finish("获取学生列表或别名失败，请检查后台输出")
+                await matcher.finish("获取学生列表或别名失败，请检查后台输出")
 
             for i in arg.split():
                 if not (stu := stu_li.get(recover_alia(i, stu_alias))):
                     await matcher.finish(f"未找到学生 {i}")
                 if stu["StarGrade"] == 1:
                     await matcher.finish("不能UP一星角色")
                 pool.append(stu)
@@ -609,15 +617,15 @@
             )
 
     else:
         try:
             gacha_data = await db_get_gacha_data()
         except:
             logger.exception("获取抽卡基本数据失败")
-            return await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
+            await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
 
         pool_data = gacha_data["current_pools"]
         if not pool_data:
             await matcher.finish("当前没有可切换的卡池")
 
         pool_obj = gacha_pool_index.get(qq) or get_1st_pool(gacha_data)
         if not pool_obj:
@@ -638,63 +646,70 @@
 
 
 gacha_once = on_command("ba抽卡")
 
 
 @gacha_once.handle()
 async def _(matcher: Matcher, event: MessageEvent, cmd_arg: Message = CommandArg()):
+    user_id = event.user_id
+    group_id = event.group_id if isinstance(event, GroupMessageEvent) else None
+
+    if cool_down := get_gacha_cool_down(user_id, group_id):
+        await matcher.finish(f"你先别急，先等 {cool_down} 秒再来抽吧qwq")
+
+    set_gacha_cool_down(user_id, group_id)
+
     arg = cmd_arg.extract_plain_text().strip().lower()
 
     gacha_times = 10
-    if arg:
-        if (not arg.isdigit()) or (not (1 <= (gacha_times := int(arg)) <= 90)):
-            await matcher.finish("请输入有效的抽卡次数，在1~90之间")
+    if arg and ((not arg.isdigit()) or (not (1 <= (gacha_times := int(arg)) <= 90))):
+        await matcher.finish("请输入有效的抽卡次数，在1~90之间")
 
     try:
         gacha_data = await db_get_gacha_data()
     except:
         logger.exception("获取抽卡基本数据失败")
-        return await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
+        await matcher.finish("获取抽卡基本数据失败，请检查后台输出")
 
     pool_obj = gacha_pool_index.get(qq := event.get_user_id()) or get_1st_pool(
-        gacha_data
+        gacha_data,
     )
     if not pool_obj:
         await matcher.finish("目前没有UP池，请使用[ba切换卡池]指令来切换到常驻池或组建一个自定义UP池")
 
     try:
         img = []
         for _ in range(math.ceil(gacha_times / 10)):
             img.append(
                 await gacha(
                     qq,
                     10 if gacha_times >= 10 else gacha_times,
                     gacha_data,
                     pool_obj.pool,
-                )
+                ),
             )
             gacha_times -= 10
     except:
         logger.exception("抽卡错误")
-        return await matcher.finish("抽卡出错了，请检查后台输出")
+        await matcher.finish("抽卡出错了，请检查后台输出")
 
     await matcher.finish(MessageSegment.at(qq) + f"当前抽取卡池：{pool_obj.name}" + img)
 
 
 random_emoji = on_command("ba表情")
 
 
 @random_emoji.handle()
 async def _(matcher: Matcher):
     try:
         emojis = await db_get_emoji()
         emo = await db_get(random.choice(emojis), True)
     except:
         logger.exception("获取表情失败")
-        return await matcher.finish("获取表情失败，请检查后台输出")
+        await matcher.finish("获取表情失败，请检查后台输出")
     await matcher.finish(MessageSegment.image(emo))
 
 
 random_manga = on_command("ba漫画")
 
 
 @random_manga.handle()
@@ -706,14 +721,14 @@
         return p
 
     try:
         manga: MangaDict = random.choice(await db_get_manga())
         pics = await asyncio.gather(*[get_pic(x) for x in manga["pics"]])
     except:
         logger.exception("获取漫画失败")
-        return await matcher.finish("获取漫画失败，请检查后台输出")
+        await matcher.finish("获取漫画失败，请检查后台输出")
 
     await matcher.finish(
         Message()
         + f'{manga["title"]}\n-=-=-=-=-=-=-=-\n{manga["detail"]}'
-        + [MessageSegment.image(x) for x in pics]
+        + [MessageSegment.image(x) for x in pics],
     )
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_bawiki.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import datetime
 from io import BytesIO
-from typing import Any, Dict, List, TypedDict
+from typing import Any, Dict, List, Literal, Optional, TypedDict, cast, overload
 
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
 from .config import config
 from .util import async_req, recover_alia
 
@@ -13,16 +13,26 @@
 class MangaDict(TypedDict):
     cid: int
     title: str
     detail: str
     pics: List[str]
 
 
-async def db_get(suffix, raw=False):
-    return await async_req(f"{config.ba_bawiki_db_url}{suffix}", raw=raw)
+@overload
+async def db_get(suffix: str, raw: Literal[False] = False) -> Any:
+    ...
+
+
+@overload
+async def db_get(suffix: str, raw: Literal[True] = True) -> bytes:
+    ...
+
+
+async def db_get(suffix: str, raw=False):
+    return await async_req(f"{config.ba_bawiki_db_url}{suffix}", raw=raw)  # type: ignore
 
 
 async def db_get_wiki_data() -> Dict[str, Any]:
     return await db_get("data/wiki.json")
 
 
 async def db_get_stu_alias() -> Dict[str, List[str]]:
@@ -91,30 +101,27 @@
 
     if not (boss := wiki.get(str(raid_id))):
         return "没有找到该总力战Boss"
 
     terrain_raid = None
     if terrain:
         if t := boss["terrains"].get(
-            recover_alia(terrain, await db_get_terrain_alias())
+            recover_alia(terrain, await db_get_terrain_alias()),
         ):
             terrain_raid = t
         else:
             return "还没有进行过该环境的总力战"
 
     img = []
     if is_wiki:
         if not (wiki_url := boss.get("wiki")):
             return "该总力战Boss暂无机制介绍"
         img.append(wiki_url)
     else:
-        if terrain_raid:
-            img_ = [terrain_raid]
-        else:
-            img_ = list(boss["terrains"].values())
+        img_ = [terrain_raid] if terrain_raid else list(boss["terrains"].values())
         for i in img_:
             for s in servers:
                 img.append(i[s])
 
     return [
         MessageSegment.image(x)
         for x in await asyncio.gather(*[db_get(x, True) for x in img])
@@ -136,15 +143,15 @@
     if raid_id >= 1000:
         raid_id = int(raid_id / 1000)
     wiki = (await db_get_wiki_data())["time_atk"]
     if raid_id > len(wiki):
         return f"没有找到该综合战术考试（目前共有{len(wiki)}个综合战术考试）"
     raid_id -= 1
 
-    return MessageSegment.image(await db_get(wiki[raid_id], True))
+    return MessageSegment.image(await db_get(wiki[raid_id], True))  # type: ignore
 
 
 async def db_wiki_craft():
     wiki = (await db_get_wiki_data())["craft"]
     return [
         MessageSegment.image(x)
         for x in await asyncio.gather(*[db_get(y, True) for y in wiki])
@@ -155,17 +162,21 @@
     wiki = (await db_get_wiki_data())["furniture"]
     return [
         MessageSegment.image(x)
         for x in await asyncio.gather(*[db_get(y, True) for y in wiki])
     ]
 
 
-async def db_global_future(date: datetime.datetime = None, num=1, all_img=False):
+async def db_global_future(
+    date: Optional[datetime.datetime] = None,
+    num=1,
+    all_img=False,
+):
     data = (await db_get_wiki_data())["global_future"]
-    img = await db_get(data["img"], True)
+    img = cast(bytes, await db_get(data["img"], True))
 
     if all_img:
         return MessageSegment.image(img)
 
     compare_date = date or datetime.datetime.now()
     index = -1
     for i, v in enumerate(parts := data["parts"]):
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_gamekee.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,107 @@
 import asyncio
+import contextlib
 import re
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, cast
 
 from bs4 import BeautifulSoup, ResultSet, Tag
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_htmlrender import get_new_page
-from PIL import Image
+from PIL.Image import Resampling
 from pil_utils import BuildImage, text2image
+from playwright.async_api import Page
 
 from .config import config
 from .resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
 from .util import async_req, parse_time_delta
 
 
 async def game_kee_request(url, **kwargs) -> Union[List, Dict[str, Any]]:
-    ret = await async_req(
-        url, headers={"game-id": "0", "game-alias": "ba"}, proxy=None, **kwargs
+    ret = cast(
+        dict,
+        await async_req(
+            url,
+            headers={"game-id": "0", "game-alias": "ba"},
+            proxy=None,
+            **kwargs,
+        ),
     )
     if ret["code"] != 0:
         raise ConnectionError(ret["msg"])
     return ret["data"]
 
 
 async def game_kee_get_calender():
-    ret: List = await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/index")
+    ret = cast(list, await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/index"))
 
     for i in ret:
         if i["module"]["id"] == 12:
             li: list = i["list"]
 
             now = time.time()
             li = [x for x in li if (now < x["end_at"])]
 
             li.sort(key=lambda x: x["begin_at"] if now < x["begin_at"] else x["end_at"])
             li.sort(key=lambda x: now < x["begin_at"])
             li.sort(key=lambda x: x["importance"], reverse=True)
             return li
 
+    return []
+
 
 async def game_kee_get_stu_li():
-    ret = await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/entry")
+    ret = cast(dict, await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/entry"))
 
     for i in ret["entry_list"]:
         if i["id"] == 23941:
             for ii in i["child"]:
                 if ii["id"] == 49443:
                     return {x["name"]: x for x in ii["child"]}
 
+    return {}
+
 
 async def game_kee_get_stu_cid_li():
     return {x: y["content_id"] for x, y in (await game_kee_get_stu_li()).items()}
 
 
 def game_kee_page_url(sid):
     return f"{config.ba_gamekee_url}{sid}.html"
 
 
 async def game_kee_get_page(url):
-    async with get_new_page() as page:  # type:Page
+    async with cast(Page, get_new_page()) as page:
         await page.goto(url, timeout=60 * 1000)
 
         # 删掉header
         await page.add_script_tag(
             content='document.getElementsByClassName("wiki-header")'
-            ".forEach((v)=>{v.remove()})"
+            ".forEach((v)=>{v.remove()})",
         )
 
         # 展开折叠的语音
         folds = await page.query_selector_all('xpath=//div[@class="fold-table-btn"]')
         for i in folds:
-            try:
+            with contextlib.suppress(Exception):
                 await i.click()
-            except:
-                pass
 
         # 隐藏 header 和 footer
         js_str = "(obj) => { obj.style.display = 'none' }"
         await page.eval_on_selector(".wiki-header", js_str)
         await page.eval_on_selector(".wiki-footer", js_str)
 
-        return await (
-            await page.query_selector('xpath=//div[@class="wiki-detail-body"]')
-        ).screenshot()
+        element = await page.query_selector('xpath=//div[@class="wiki-detail-body"]')
+        if not element:
+            raise ValueError
+        return await element.screenshot()
 
 
 async def game_kee_calender():
     ret = await game_kee_get_calender()
     if not ret:
         return "没有获取到GameKee日程表数据"
 
@@ -118,18 +129,24 @@
         started = begin <= now
         time_remain = (end if started else begin) - now
         dd, hh, mm, ss = parse_time_delta(time_remain)
 
         # logger.debug(f'{it["title"]} | {started} | {time_remain}')
 
         title_p = text2image(
-            f'[b]{it["title"]}[/b]', "#ffffff00", max_width=1290, fontsize=65
+            f'[b]{it["title"]}[/b]',
+            "#ffffff00",
+            max_width=1290,
+            fontsize=65,
         )
         time_p = text2image(
-            f"{begin} ~ {end}", "#ffffff00", max_width=1290, fontsize=40
+            f"{begin} ~ {end}",
+            "#ffffff00",
+            max_width=1290,
+            fontsize=40,
         )
         desc_p = (
             text2image(
                 desc.replace("<br>", ""),
                 "#ffffff00",
                 max_width=1290,
                 fontsize=40,
@@ -151,15 +168,16 @@
             + (title_p.height + 25)
             + (time_p.height + 25)
             + (_p.height + 25 if _p else 0)
             + (desc_p.height + 25 if desc_p else 0)
             + remain_p.height
         )
         img = BuildImage.new("RGBA", (1400, h), (255, 255, 255, 70)).draw_rectangle(
-            (0, 0, 10, h), "#fc6475" if it["importance"] else "#4acf75"
+            (0, 0, 10, h),
+            "#fc6475" if it["importance"] else "#4acf75",
         )
 
         if not started:
             img.draw_rectangle((1250, 0, 1400, 60), "gray")
             img.draw_text((1250, 0, 1400, 60), "未开始", max_fontsize=50, fill="white")
 
         ii = 50
@@ -175,15 +193,15 @@
             ii += desc_p.height + 25
         img.paste(remain_p, (60, ii), True)
         # img = img.circle_corner(15)
 
         return img
 
     pics: List[BuildImage] = await asyncio.gather(  # type: ignore
-        *[draw(x) for x in ret]
+        *[draw(x) for x in ret],
     )
 
     bg_w = 1500
     bg_h = 200 + sum([x.height + 50 for x in pics])
     bg = (
         BuildImage.new("RGBA", (bg_w, bg_h))
         .paste(RES_CALENDER_BANNER.copy().resize((1500, 150)))
@@ -192,66 +210,75 @@
             "GameKee丨活动日程",
             max_fontsize=100,
             weight="bold",
             fill="#ffffff",
             halign="left",
         )
         .paste(
-            RES_GRADIENT_BG.copy().resize((1500, bg_h - 150), resample=Image.NEAREST),
+            RES_GRADIENT_BG.copy().resize(
+                (1500, bg_h - 150),
+                resample=Resampling.NEAREST,
+            ),
             (0, 150),
         )
     )
 
     index = 200
     for p in pics:
         bg.paste(p.circle_corner(10), (50, index), True)
         index += p.height + 50
 
     return bg.save_jpg()
 
 
 async def game_kee_grab_l2d(cid):
-    r: dict = await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}")
-    r: str = r["content"]
+    ret = cast(
+        dict,
+        await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}"),
+    )
+    content: str = ret["content"]
 
-    i = r.find('<div class="input-wrapper">官方介绍</div>')
-    i = r.find('class="slide-item" data-index="2"', i)
-    ii = r.find('data-index="3"', i)
+    x = content.find('<div class="input-wrapper">官方介绍</div>')
+    x = content.find('class="slide-item" data-index="2"', x)
+    y = content.find('data-index="3"', x)
 
-    r: str = r[i:ii]
+    content: str = content[x:y]
 
-    img = re.findall('data-real="([^"]*)"', r)
+    img = re.findall('data-real="([^"]*)"', content)
 
     return [f"https:{x}" for x in img]
 
 
 @dataclass()
 class GameKeeVoice:
     title: str
     jp: str
     cn: str
     url: str
 
 
 async def game_kee_get_voice(cid) -> List[GameKeeVoice]:
     wiki_html = (
-        await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}")
+        cast(
+            dict,
+            await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}"),
+        )
     )["content"]
     bs = BeautifulSoup(wiki_html, "lxml")
     audios = bs.select(".mould-table>tbody>tr>td>div>div>audio")
 
     parsed: List[GameKeeVoice] = []
     for au in audios:
-        url: str = au["src"]
+        url: str = cast(str, au["src"])
         if not url.startswith("http"):
             url = f"https:{url}"
 
-        tr1: Tag = au.parent.parent.parent.parent
+        tr1: Tag = au.parent.parent.parent.parent  # type: ignore
         tds: ResultSet[Tag] = tr1.find_all("td")
         title = tds[0].text.strip()
         jp = "\n".join(tds[2].stripped_strings)
 
         tr2 = tr1.next_sibling
-        cn = "\n".join(tr2.stripped_strings)
+        cn = "\n".join(tr2.stripped_strings)  # type: ignore
         parsed.append(GameKeeVoice(title, jp, cn, url))
 
     return parsed
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/data_schaledb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 import asyncio
 import math
 import time
 from datetime import datetime
 from io import BytesIO
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Literal, cast, overload
 
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_htmlrender import get_new_page
 from PIL import Image, ImageFilter
+from PIL.Image import Resampling
 from pil_utils import BuildImage, text2image
-from playwright.async_api import ViewportSize
+from playwright.async_api import Page, ViewportSize
 
 from .config import config
 from .resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
 from .util import async_req, img_invert_rgba, parse_time_delta
 
 PAGE_KWARGS = {
     "is_mobile": True,
     "viewport": ViewportSize(width=767, height=800),
 }
 
 
+@overload
+async def schale_get(suffix: str, raw: Literal[False] = False, **kwargs) -> Any:
+    ...
+
+
+@overload
+async def schale_get(suffix: str, raw: Literal[True] = True, **kwargs) -> bytes:
+    ...
+
+
 async def schale_get(suffix, raw=False, **kwargs):
-    return await async_req(f"{config.ba_schale_url}{suffix}", raw=raw, **kwargs)
+    return await async_req(f"{config.ba_schale_url}{suffix}", raw=raw, **kwargs)  # type: ignore
 
 
 async def schale_get_stu_data(loc: str = "cn") -> List[Dict[str, Any]]:
     return await schale_get(f"data/{loc}/students.min.json")
 
 
 async def schale_get_common() -> Dict[str, Any]:
     return await schale_get("data/common.min.json")
 
 
 async def schale_get_localization(loc: str = "cn") -> Dict[str, Any]:
-    return await schale_get(f"data/{loc}/localization.min.json")
+    return cast(dict, await schale_get(f"data/{loc}/localization.min.json"))
 
 
 async def schale_get_raids(loc: str = "cn") -> Dict[str, Any]:
-    return await schale_get(f"data/{loc}/raids.min.json")
+    return cast(dict, await schale_get(f"data/{loc}/raids.min.json"))
 
 
 async def schale_get_stu_dict(key="Name"):
     return {x[key]: x for x in await schale_get_stu_data()}
 
 
 async def schale_get_stu_info(stu):
-    async with get_new_page(**PAGE_KWARGS) as page:  # type:Page
+    async with cast(Page, get_new_page(**PAGE_KWARGS)) as page:
         await page.goto(
             f"{config.ba_schale_mirror_url}?chara={stu}",
             timeout=60 * 1000,
             wait_until="networkidle",
         )
 
         # 进度条拉最大
@@ -68,27 +79,28 @@
                 await asyncio.gather(
                     schale_get_stu_data(),
                     schale_get_common(),
                     schale_get_localization(),
                     schale_get_raids(),
                 )
             ),
-        )
+        ),
     )
 
 
 def find_current_event(ev, now=None):
     if not now:
         now = datetime.now()
     for _e in ev:
         _start = datetime.fromtimestamp(_e["start"])
         _end = datetime.fromtimestamp(_e["end"])
         if _start <= now < _end:
             _remain = _end - now
             return _e, _start, _end, _remain
+    return None
 
 
 async def schale_get_calender(server, students, common, localization, raids):
     students = {x["Id"]: x for x in students}
 
     region = common["regions"][server]
     now = datetime.now()
@@ -100,38 +112,45 @@
         return (
             f"{_start} ~ {_end} | "
             f"剩余 [b][color=#fc6475]{dd}天 {hh:0>2d}:{mm:0>2d}:{ss:0>2d}[color=#fc6475][/b]"
         )
 
     async def draw_gacha():
         pic = pic_bg.copy().draw_text(
-            (25, 25, 1375, 150), "特选招募", weight="bold", max_fontsize=80
+            (25, 25, 1375, 150),
+            "特选招募",
+            weight="bold",
+            max_fontsize=80,
         )
         c_gacha = region["current_gacha"]
         if r := find_current_event(c_gacha):
             g = r[0]
             t = format_time(*(r[1:]))
             pic = pic.paste(
                 ti := text2image(
-                    t, (255, 255, 255, 0), fontsize=45, max_width=1350, align="center"
+                    t,
+                    (255, 255, 255, 0),
+                    fontsize=45,
+                    max_width=1350,
+                    align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
                 True,
             )
             stu = [students[x] for x in g["characters"]]
 
             async def process_avatar(s):
                 return (
                     BuildImage.open(
                         BytesIO(
                             await schale_get(
                                 f'images/student/collection/{s["CollectionTexture"]}.webp',
                                 raw=True,
-                            )
-                        )
+                            ),
+                        ),
                     )
                     .resize((300, 340))
                     .paste(
                         BuildImage.new("RGBA", (300, 65), (255, 255, 255, 120)),
                         (0, 275),
                         True,
                     )
@@ -145,41 +164,50 @@
             x_index = int((1400 - (300 + 25) * ava_len + 25) / 2)
 
             for p in avatars:
                 pic = pic.paste(p, (x_index, 250), True)
                 x_index += p.width + 25
 
             return pic
+        return None
 
     async def draw_event():
         pic = pic_bg.copy().draw_text(
-            (25, 25, 1375, 150), "当前活动", weight="bold", max_fontsize=80
+            (25, 25, 1375, 150),
+            "当前活动",
+            weight="bold",
+            max_fontsize=80,
         )
         c_event = region["current_events"]
         if r := find_current_event(c_event):
             g = r[0]
             t = format_time(*(r[1:]))
             pic = pic.paste(
                 ti := text2image(
-                    t, (255, 255, 255, 0), fontsize=45, max_width=1350, align="center"
+                    t,
+                    (255, 255, 255, 0),
+                    fontsize=45,
+                    max_width=1350,
+                    align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
                 True,
             )
             ev = g["event"]
             ev_name = ""
             if ev >= 10000:
                 ev_name = " (复刻)"
                 ev %= 10000
             ev_name = localization["EventName"][str(ev)] + ev_name
 
             ev_bg, ev_img = await asyncio.gather(
                 schale_get(f"images/campaign/Campaign_Event_{ev}_Normal.png", True),
                 schale_get(
-                    f"images/eventlogo/Event_{ev}_{'Tw' if server else 'Jp'}.png", True
+                    f"images/eventlogo/Event_{ev}_{'Tw' if server else 'Jp'}.png",
+                    True,
                 ),
             )
 
             ev_bg = (
                 BuildImage.open(BytesIO(ev_bg))
                 .convert("RGBA")
                 .resize_height(340)
@@ -207,23 +235,28 @@
                 .draw_text(
                     (0, ev_bg.height - 65, ev_bg.width, ev_bg.height),
                     ev_name,
                     max_fontsize=50,
                 )
             )
             return pic.paste(ev_bg, (int((pic.width - ev_bg.width) / 2), 250), True)
+        return None
 
     async def draw_raid():
         pic = pic_bg.copy()
         if r := find_current_event(region["current_raid"]):
             ri = r[0]
             t = format_time(*(r[1:]))
             pic = pic.paste(
                 ti := text2image(
-                    t, (255, 255, 255, 0), fontsize=45, max_width=1350, align="center"
+                    t,
+                    (255, 255, 255, 0),
+                    fontsize=45,
+                    max_width=1350,
+                    align="center",
                 ),
                 (int((1400 - ti.width) / 2), 150),
                 True,
             )
 
             tp = "TimeAttack" if (time_atk := (ri["raid"] >= 1000)) else "Raid"
             raid = {x["Id"]: x for x in raids[tp]}
@@ -268,15 +301,15 @@
             c_bg, c_fg, icon_def, icon_atk, icon_tr = await asyncio.gather(
                 *[
                     schale_get(bg_url, True),
                     schale_get(fg_url, True),
                     schale_get("images/ui/Type_Defense_s.png", True),
                     schale_get("images/ui/Type_Attack_s.png", True),
                     schale_get(f"images/ui/Terrain_{terrain}.png", True),
-                ]
+                ],
             )
 
             icon_def = (
                 BuildImage.new("RGBA", (64, 64), def_color)
                 .paste(
                     BuildImage.open(BytesIO(icon_def))
                     .convert("RGBA")
@@ -341,30 +374,34 @@
                         if time_atk
                         else (c_ri["Name"])
                     ),
                     max_fontsize=50,
                 )
             )
             return pic.paste(c_bg, (int((pic.width - c_bg.width) / 2), 250), True)
+        return None
 
     async def draw_birth():
         pic = pic_bg.copy().draw_text(
-            (25, 25, 1375, 150), "学生生日", weight="bold", max_fontsize=80
+            (25, 25, 1375, 150),
+            "学生生日",
+            weight="bold",
+            max_fontsize=80,
         )
         now_t = time.mktime(now.date().timetuple())
         now_w = now.weekday()
         this_week_t = now_t - now_w * 86400
         next_week_t = now_t + (7 - now_w) * 86400
         next_next_week_t = next_week_t + 7 * 86400
 
         birth_this_week = []
         birth_next_week = []
         for s in [x for x in students.values() if x["IsReleased"][server]]:
             birth = time.mktime(
-                time.strptime(f'{now.year}/{s["BirthDay"]}', "%Y/%m/%d")
+                time.strptime(f'{now.year}/{s["BirthDay"]}', "%Y/%m/%d"),
             )
             if this_week_t <= birth < next_week_t:
                 birth_this_week.append(s)
             elif next_week_t <= birth <= next_next_week_t:
                 birth_next_week.append(s)
 
         sort_key = lambda x: x["BirthDay"].split("/")  # noqa: E731
@@ -381,18 +418,19 @@
 
         if p_h:
             stu_pics = [
                 BuildImage.open(BytesIO(x)).convert("RGBA").resize_height(180).circle()
                 for x in await asyncio.gather(
                     *[
                         schale_get(
-                            f'images/student/icon/{x["CollectionTexture"]}.png', True
+                            f'images/student/icon/{x["CollectionTexture"]}.png',
+                            True,
                         )
                         for x in birth_this_week + birth_next_week
-                    ]
+                    ],
                 )
             ]
             y_index = int((415 - p_h) / 2) + 125
             if birth_this_week:
                 x_index = (
                     int((1400 - (len(birth_this_week) * (180 + 10) - 10)) / 2) + 75
                 )
@@ -423,22 +461,26 @@
                     pic.paste(stu_pics.pop(0), (x_index, y_index), True).draw_text(
                         (x_index, y_index + 180, x_index + 180, y_index + 220),
                         s["BirthDay"],
                     )
                     x_index += 180 + 10
 
             return pic
+        return None
 
     img = await asyncio.gather(  # type: ignore
-        draw_gacha(), draw_event(), draw_raid(), draw_birth()
+        draw_gacha(),
+        draw_event(),
+        draw_raid(),
+        draw_birth(),
     )
     img: List[BuildImage] = [x for x in img if x]
     if not img:
         img.append(
-            pic_bg.copy().draw_text((0, 0, 1400, 640), "没有获取到任何数据", max_fontsize=60)
+            pic_bg.copy().draw_text((0, 0, 1400, 640), "没有获取到任何数据", max_fontsize=60),
         )
 
     bg_w = 1500
     bg_h = 200 + sum([x.height + 50 for x in img])
     bg = (
         BuildImage.new("RGBA", (bg_w, bg_h))
         .paste(RES_CALENDER_BANNER.copy().resize((1500, 150)))
@@ -447,15 +489,18 @@
             f"SchaleDB丨活动日程丨{localization['ServerName'][str(server)]}",
             max_fontsize=100,
             weight="bold",
             fill="#ffffff",
             halign="left",
         )
         .paste(
-            RES_GRADIENT_BG.copy().resize((1500, bg_h - 150), resample=Image.NEAREST),
+            RES_GRADIENT_BG.copy().resize(
+                (1500, bg_h - 150),
+                resample=Resampling.NEAREST,
+            ),
             (0, 150),
         )
     )
 
     h_index = 200
     for im in img:
         bg.paste(im.circle_corner(10), (50, h_index), True)
@@ -487,26 +532,28 @@
         line = 1
         length = li_len
     else:
         line = math.ceil(li_len / line_max_icon)
         length = line_max_icon
 
     img = RES_GRADIENT_BG.copy().resize(
-        (icon_w * length, icon_h * line + 5), resample=Image.NEAREST
+        (icon_w * length, icon_h * line + 5),
+        resample=Resampling.NEAREST,
     )
 
     async def draw_stu(name_, dev_name_, line_, index_):
         left = index_ * icon_w
         top = line_ * icon_h + 5
 
         ret = await schale_get(
-            f"images/student/lobby/Lobbyillust_Icon_{dev_name_}_01.png", True
+            f"images/student/lobby/Lobbyillust_Icon_{dev_name_}_01.png",
+            True,
         )
         icon_img = Image.open(BytesIO(ret)).convert("RGBA")
-        img.paste(icon_img, (left, top), icon_img)
+        img.paste(icon_img, (left, top), True)
         img.draw_text(
             (left, top + pic_h, left + icon_w, top + icon_h),
             name_,
             max_fontsize=25,
             min_fontsize=1,
         )
 
@@ -518,9 +565,9 @@
             i = 0
             line += 1
         task_li.append(draw_stu(stu["Name"], stu["DevName"], line, i))
         i += 1
     await asyncio.gather(*task_li)
 
     return MessageSegment.text(f"羁绊等级 {lvl} 时解锁L2D的学生有以下这些：") + MessageSegment.image(
-        img.save("png")
+        img.save("png"),
     )
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/gacha.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
 import json
 import random
+import time
 from dataclasses import dataclass
 from io import BytesIO
-from typing import Dict, Iterable, List, Optional, Tuple, TypedDict
+from typing import Dict, Iterable, List, Optional, TypedDict, Union, cast
 
 import aiofiles
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
+from .config import config
 from .data_schaledb import schale_get, schale_get_stu_dict
 from .resource import (
     DATA_PATH,
     RES_GACHA_BG,
     RES_GACHA_CARD_BG,
     RES_GACHA_CARD_MASK,
     RES_GACHA_NEW,
@@ -24,29 +26,49 @@
 from .util import split_list
 
 GACHA_DATA_PATH = DATA_PATH / "gacha.json"
 if not GACHA_DATA_PATH.exists():
     GACHA_DATA_PATH.write_text("{}")
 
 
+DEFAULT_GACHA_DATA: "GachaData" = {"collected": [], "total_count": 0}
+COOL_DOWN_DICT: Dict[str, float] = {}
+
+
 class GachaData(TypedDict):
     collected: List[int]
     total_count: int
 
 
-DEFAULT_GACHA_DATA: GachaData = {"collected": [], "total_count": 0}
-
-
 @dataclass()
 class GachaStudent:
-    id: int
+    id: int  # noqa: A003
     new: bool = False
     pickup: bool = False
 
 
+def get_gacha_cool_down(
+    user: Union[str, int],
+    group: Optional[Union[str, int]] = None,
+) -> int:
+    key = f"{group}.{user}" if group else f"{user}"
+    now = time.time()
+
+    if last := COOL_DOWN_DICT.get(key):
+        remain = config.ba_gacha_cool_down - round(now - last)
+        return remain if remain >= 0 else 0
+
+    return 0
+
+
+def set_gacha_cool_down(user: Union[str, int], group: Optional[Union[str, int]] = None):
+    key = f"{group}.{user}" if group else f"{user}"
+    COOL_DOWN_DICT[key] = time.time()
+
+
 async def set_gacha_data(qq: str, data: GachaData):
     async with aiofiles.open(str(GACHA_DATA_PATH), "r+", encoding="u8") as f:
         j = json.loads(await f.read())
         j[qq] = data
 
         await f.seek(0)
         await f.truncate()
@@ -62,15 +84,15 @@
     if not (user_data := data.get(qq)):
         user_data = DEFAULT_GACHA_DATA.copy()
         await set_gacha_data(qq, user_data)
 
     return user_data
 
 
-async def gen_stu_img(students: Iterable[GachaStudent]) -> Tuple[BuildImage]:
+async def gen_stu_img(students: Iterable[GachaStudent]) -> List[BuildImage]:
     stu_li = await schale_get_stu_dict("Id")
 
     async def gen_single(stu: GachaStudent) -> BuildImage:
         bg = RES_GACHA_CARD_BG.copy()
 
         stu_star = 0
         try:
@@ -109,24 +131,20 @@
         if stu.pickup:
             font_x_offset -= 4
             font_y_offset -= 4
             bg = bg.paste(RES_GACHA_PICKUP, (font_x_offset, font_y_offset), True)
 
         return bg
 
-    return await asyncio.gather(*[gen_single(x) for x in students])  # noqa
+    return await asyncio.gather(*[gen_single(x) for x in students])
 
 
-async def gen_gacha_img(
-    students: Iterable[GachaStudent], count: int
-) -> Optional[BytesIO]:
+async def gen_gacha_img(students: Iterable[GachaStudent], count: int) -> BytesIO:
     line_limit = 5
     stu_cards = split_list(await gen_stu_img(students), line_limit)
-    if not stu_cards:
-        return
     card_w, card_h = stu_cards[0][0].size
 
     bg = RES_GACHA_BG.copy()
 
     x_gap = 10
     y_gap = 80
     y_offset = int((bg.height - (len(stu_cards) * (y_gap + card_h) - y_gap)) / 2)
@@ -150,60 +168,65 @@
         weight="bold",
         fill=(255, 255, 255),
     )
 
     return bg.save("PNG")
 
 
-async def gacha(qq: str, times: int, gacha_data: dict, up_pool: List[int] = None):
+async def gacha(
+    qq: str,
+    times: int,
+    gacha_data_json: dict,
+    up_pool: Optional[List[int]] = None,
+):
     # 屎山代码 别骂了别骂了
     # 如果有大佬指点指点怎么优化或者愿意发个PR就真的太感激了
 
     if not up_pool:
         up_pool = []
 
     stu_li = await schale_get_stu_dict("Id")
     up_3_li, up_2_li = [
         [x for x in up_pool if x in stu_li and stu_li[x]["StarGrade"] == y]
         for y in [3, 2]
     ]
 
-    base_char: dict = gacha_data["base"]
+    base_char: dict = gacha_data_json["base"]
     for up in up_pool:
-        for li in base_char.values():  # type: List[int]
+        for li in cast(List[List[int]], base_char.values()):
             if up in li:
                 li.remove(up)
 
     star_3_base, star_2_base, star_1_base = [base_char[x] for x in ["3", "2", "1"]]
     star_3_chance, star_2_chance, star_1_chance = [
         x["chance"] for x in [star_3_base, star_2_base, star_1_base]
     ]
 
     up_3_chance = 0
     up_2_chance = 0
     if up_3_li:
-        up_3_chance = gacha_data["up"]["3"]["chance"]
+        up_3_chance = gacha_data_json["up"]["3"]["chance"]
         star_3_chance -= up_3_chance
     if up_2_li:
-        up_2_chance = gacha_data["up"]["2"]["chance"]
+        up_2_chance = gacha_data_json["up"]["2"]["chance"]
         star_2_chance -= up_2_chance
 
     gacha_data = await get_gacha_data(qq)
     gacha_result: List[GachaStudent] = []
 
     picked_3star_up = False
     last_count = gacha_data["total_count"]
     for i in range(1, times + 1):
         pool_and_weight = [
             (up_3_li, up_3_chance),
             (up_2_li, up_2_chance),
             (star_3_base["char"], star_3_chance),
             (star_2_base["char"], star_2_chance),
         ]
-        if not i % 10 == 0:
+        if i % 10 != 0:
             pool_and_weight.append((star_1_base["char"], star_1_chance))
 
         pool_and_weight = [x for x in pool_and_weight if x[0]]
         pool = [x[0] for x in pool_and_weight]
         weight = [x[1] for x in pool_and_weight]
 
         random.seed()
```

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.4/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.7.5/nonebot_plugin_bawiki/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,105 @@
 import datetime
 import json
 from copy import deepcopy
-from typing import Dict, Iterator, List, TypeVar, Union
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from aiohttp import ClientSession
 from nonebot.adapters.onebot.v11 import Message
 from PIL import Image, ImageOps
 
 from .config import config
 
 _T = TypeVar("_T")
 
 req_cache = {}
 
 
-def format_timestamp(t):
+@overload
+async def async_req(
+    url,
+    *,
+    is_json: Literal[True] = True,
+    raw: Literal[False] = False,
+    ignore_cache=False,
+    proxy=config.ba_proxy,
+    method="GET",
+    session: Optional[ClientSession] = None,
+    **kwargs,
+) -> Union[Dict[str, Any], list]:
+    ...
+
+
+@overload
+async def async_req(
+    url,
+    *,
+    is_json: Literal[False] = False,
+    raw: Literal[True] = True,
+    ignore_cache=False,
+    proxy=config.ba_proxy,
+    method="GET",
+    session: Optional[ClientSession] = None,
+    **kwargs,
+) -> bytes:
+    ...
+
+
+@overload
+async def async_req(
+    url,
+    *,
+    is_json: Literal[False] = False,
+    raw: Literal[False] = False,
+    ignore_cache=False,
+    proxy=config.ba_proxy,
+    method="GET",
+    session: Optional[ClientSession] = None,
+    **kwargs,
+) -> str:
+    ...
+
+
+async def async_req(
+    url,
+    is_json=True,
+    raw=False,
+    ignore_cache=False,
+    proxy=config.ba_proxy,
+    method="GET",
+    session: Optional[ClientSession] = None,
+    **kwargs,
+):
+    if (not ignore_cache) and (c := req_cache.get(url)):
+        return c
+
+    async with (session or ClientSession()) as c:
+        async with c.request(method, url, **kwargs, proxy=proxy) as r:
+            ret = (await r.read()) if raw else (await r.text())
+            if is_json and (not raw):
+                ret = json.loads(ret)
+            req_cache[url] = ret
+            return ret
+
+
+def clear_req_cache():
+    req_cache.clear()
+
+
+def format_timestamp(t: int):
     return datetime.datetime.fromtimestamp(t).strftime("%Y-%m-%d %H:%M:%S")
 
 
 def recover_alia(origin: str, alia_dict: Dict[str, List[str]]):
     origin = replace_brackets(origin).strip()
     origin_ = origin.lower()
 
@@ -26,15 +107,15 @@
     for k, li in alia_dict.items():
         if origin_ in li or origin_ == k:
             return k
 
     # 没找到，模糊匹配
     origin_ = origin.replace(" ", "")
     for k, li in alia_dict.items():
-        li = [x.replace(" ", "") for x in ([k] + li)]
+        li = [x.replace(" ", "") for x in ([k, *li])]
         for v in li:
             if origin_ in v:
                 return k
 
     return origin
 
 
@@ -47,58 +128,31 @@
 
 def img_invert_rgba(im: Image.Image):
     # https://stackoverflow.com/questions/2498875/how-to-invert-colors-of-image-with-pil-python-imaging
     r, g, b, a = im.split()
     rgb_image = Image.merge("RGB", (r, g, b))
     inverted_image = ImageOps.invert(rgb_image)
     r2, g2, b2 = inverted_image.split()
-    final_transparent_image = Image.merge("RGBA", (r2, g2, b2, a))
-    return final_transparent_image
-
-
-async def async_req(
-    url,
-    is_json=True,
-    raw=False,
-    ignore_cache=False,
-    proxy=config.ba_proxy,
-    method="GET",
-    session: ClientSession = None,
-    **kwargs,
-) -> Union[str, bytes, dict, list]:
-    if (not ignore_cache) and (c := req_cache.get(url)):
-        return c
-
-    async with (session or ClientSession()) as c:
-        async with c.request(method, url, **kwargs, proxy=proxy) as r:
-            ret = (await r.read()) if raw else (await r.text())
-            if is_json and (not raw):
-                ret = json.loads(ret)
-            req_cache[url] = ret
-            return ret
-
-
-def clear_req_cache():
-    req_cache.clear()
+    return Image.merge("RGBA", (r2, g2, b2, a))
 
 
 def replace_brackets(original: str):
     return original.replace("（", "(").replace("）", "(")
 
 
-def splice_msg(msgs):
+def splice_msg(msgs: list) -> Message:
     im = Message()
     for i, v in enumerate(msgs):
-        if isinstance(v, str) and (not i == 0):
+        if isinstance(v, str) and (i != 0):
             v = f"\n{v}"
         im += v
     return im
 
 
-def split_list(li: Iterator[_T], length: int) -> List[List[_T]]:
+def split_list(li: Iterable[_T], length: int) -> List[List[_T]]:
     latest = []
     tmp = []
     for n, i in enumerate(li):
         tmp.append(i)
         if (n + 1) % length == 0:
             latest.append(deepcopy(tmp))
             tmp.clear()
```

### Comparing `nonebot_plugin_bawiki-0.7.4/PKG-INFO` & `nonebot_plugin_bawiki-0.7.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.4
+Version: 0.7.5
 Summary: A nonebot2 plugin for Blue Archive.
+Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
+Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
-Keywords: blue archive,nonebot,nonebot2,bot,qq
-Author: student_2333
-Author-email: lgc2333@126.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Board Games
-Classifier: Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
+Classifier: Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
-Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.1)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.1,<0.3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.5)
-Requires-Dist: pil-utils (>=0.1.4,<0.2.0)
-Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Project-URL: Repository, https://github.com/lgc2333/nonebot-plugin-bawiki/
+Project-URL: Homepage, https://github.com/lgc2333/nonebot-plugin-bawiki/
+Requires-Python: <4.0,>=3.8
+Requires-Dist: aiohttp>=3.8.3
+Requires-Dist: nonebot2>=2.0.0b5
+Requires-Dist: nonebot-adapter-onebot>=2.1.1
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1
+Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
+Requires-Dist: beautifulsoup4>=4.11.1
+Requires-Dist: lxml>=4.9.1
+Requires-Dist: pil-utils>=0.1.4
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/nonebot-plugin-bawiki.png" width="200" height="200" alt="BAWiki"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/bawiki/nonebot-plugin-bawiki.png" width="200" height="200" alt="BAWiki"></a>
 </div>
 
 <div align="center">
 
 # NoneBot-Plugin-BAWiki
 
 _✨ 基于 NoneBot2 的碧蓝档案 Wiki 插件 ✨_
@@ -85,116 +76,105 @@
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```bash
-nb plugin install nonebot-plugin-example
+nb plugin install nonebot-plugin-bawiki
 ```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
 ```bash
-pip install nonebot-plugin-example
+pip install nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>pdm</summary>
 
 ```bash
-pdm add nonebot-plugin-example
+pdm add nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>poetry</summary>
 
 ```bash
-poetry add nonebot-plugin-example
+poetry add nonebot-plugin-bawiki
 ```
 
 </details>
 <details>
 <summary>conda</summary>
 
 ```bash
-conda install nonebot-plugin-example
+conda install nonebot-plugin-bawiki
 ```
 
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
 ```toml
 [tool.nonebot]
 plugins = [
     # ...
-    "nonebot_plugin_example"
+    "nonebot_plugin_bawiki"
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值 |                         说明                          |
-| :--------------------: | :--: | :----: | :---------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None` | 访问`SchaleDB`、`bawiki-data`的 json 数据时使用的代理 |
-|    `BA_GAMEKEE_URL`    |  否  |  ...   |                 GameKee 数据源的地址                  |
-|    `BA_SCHALE_URL`     |  否  |  ...   |               SchaleDB Json 数据的地址                |
-| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                SchaleDB 网页截图的地址                |
-|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                  bawiki-data 的地址                   |
+|         配置项         | 必填 | 默认值 |                          说明                           |
+| :--------------------: | :--: | :----: | :-----------------------------------------------------: |
+|       `BA_PROXY`       |  否  | `None` | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
+|  `BA_GACHA_COOL_DOWN`  |  否  |  `0`   |               每群每人的抽卡冷却，单位秒                |
+|    `BA_GAMEKEE_URL`    |  否  |  ...   |                  GameKee 数据源的地址                   |
+|    `BA_SCHALE_URL`     |  否  |  ...   |                SchaleDB Json 数据的地址                 |
+| `BA_SCHALE_MIRROR_URL` |  否  |  ...   |                 SchaleDB 网页截图的地址                 |
+|   `BA_BAWIKI_DB_URL`   |  否  |  ...   |                   bawiki-data 的地址                    |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
-见[这里](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py#L17)
-
-待更新
-
-<!--
-### 效果图
-
-<details>
-<summary>长图，点击展开</summary>
-
-![example](https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/example.png)
-![example2](https://raw.githubusercontent.com/lgc2333/nonebot-plugin-bawiki/master/readme/example2.png)
+**现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
 
-</details>
--->
+如果你不想用 PicMenu 的话，那么请看 [\_\_init\_\_.py](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py)
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
 ### [RainNight0](https://github.com/RainNight0)
 
 - 日程表 html 模板提供（已弃用）
 
-### `bawiki-data`数据源贡献列表
+### `bawiki-data` 数据源贡献列表
 
 - 见 [bawiki-data](http://github.com/lgc2333/bawiki-data)
 
 ## 💰 赞助
 
 感谢各位大佬的投喂……！！本 fw 实在感激不尽……
 
@@ -204,19 +184,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-### 0.7.3
+### 0.7.5
 
-- 修复 bug
+- 插件可以自动帮你配置 PicMenu 的字体了
+- 给抽卡新增了冷却
 
-### 0.7.2
+### 0.7.2 ~ 0.7.4
 
 - 修复 bug
 
 ### 0.7.1
 
 - 更改配置项名称
 
@@ -312,8 +293,7 @@
 
 ### 0.1.1
 
 - 日程表改为以图片形式发送
 - 日程表不会显示未开始的活动了
 - 小 bug 修复
 - ~~移除了 herobrine~~
-
```

#### html2text {}

```diff
@@ -1,75 +1,74 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.4 Summary: A
-nonebot2 plugin for Blue Archive. Home-page: https://github.com/lgc2333/
-nonebot-plugin-bawiki/ License: MIT Keywords: blue
-archive,nonebot,nonebot2,bot,qq Author: student_2333 Author-email:
-lgc2333@126.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: Chinese (Simplified) Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Communications Classifier: Topic ::
-Communications :: Chat Classifier: Topic :: Communications :: Chat :: ICQ
-Classifier: Topic :: Games/Entertainment Classifier: Topic :: Games/
-Entertainment :: Board Games Classifier: Topic :: Games/Entertainment :: Side-
-Scrolling/Arcade Games Classifier: Topic :: Games/Entertainment :: Turn Based
-Strategy Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/
-HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier:
-Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki Requires-Dist: Pillow
-(>=9.2.0,<10.0.0) Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist:
-beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: lxml (>=4.9.1,<5.0.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.1.1) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
-(>=0.2.0.1,<0.3.0.0) Requires-Dist: nonebot2 (>=2.0.0-beta.5) Requires-Dist:
-pil-utils (>=0.1.4,<0.2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Project-URL:
-Repository, https://github.com/lgc2333/nonebot-plugin-bawiki/ Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.5 Summary: A
+nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
+qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
+student_2333
+126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
+Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
+Classifier: Topic :: Games/Entertainment :: Turn Based Strategy Classifier:
+Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games Classifier: Topic
+:: Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Internet :: WWW/
+HTTP :: Dynamic Content :: Wiki Project-URL: Homepage, https://github.com/
+lgc2333/nonebot-plugin-bawiki/ Requires-Python: <4.0,>=3.8 Requires-Dist:
+aiohttp>=3.8.3 Requires-Dist: nonebot2>=2.0.0b5 Requires-Dist: nonebot-adapter-
+onebot>=2.1.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1 Requires-Dist:
+nonebot-plugin-apscheduler>=0.2.0 Requires-Dist: beautifulsoup4>=4.11.1
+Requires-Dist: lxml>=4.9.1 Requires-Dist: pil-utils>=0.1.4 Description-Content-
+Type: text/markdown
                                    [BAWiki]
 # NoneBot-Plugin-BAWiki _â¨ åºäº NoneBot2 çç¢§èæ¡£æ¡ Wiki æä»¶ â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð¬ åè¨
 è¯éåä½å¸®å¿æ´æ°æä»¶æ°æ®æºä»åºï¼è½å¸®è¿ä¸ªå°å°æä»¶è´¡ç®å¾®èä¹åï¼éäººææ¿ä¸å°½ï¼ï¼
 [ç¹å»è·³è½¬ bawiki-data](https://github.com/lgc2333/bawiki-data)
 ä¿®æ¹åæäº¤ Pull Request å³å¯ï¼ ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç
 Wiki æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
 [SchaleDB](https://lonqie.github.io/SchaleDB/) æä»¶çµææ¥æºï¼
 [ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145) ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-example
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-bawiki
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip ```bash pip install nonebot-plugin-example ```   pdm ```bash pdm add
-nonebot-plugin-example ```   poetry ```bash poetry add nonebot-plugin-example
-```   conda ```bash conda install nonebot-plugin-example ```  æå¼ nonebot2
+pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
+nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
+conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_example" ] ```  ## âï¸ éç½® å¨ nonebot2
+"nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :----: | :--------------
--------------------------------------: | | `BA_PROXY` | å¦ | `None` |
-è®¿é®`SchaleDB`ã`bawiki-data`ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+---------------------------------------: | | `BA_PROXY` | å¦ | `None` | è®¿é®
+`SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
+`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
 `BA_GAMEKEE_URL` | å¦ | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` |
 å¦ | ... | SchaleDB Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ |
 ... | SchaleDB ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... |
 bawiki-data çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) è§[è¿é]
-(https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/
-nonebot_plugin_bawiki/__init__.py#L17) å¾æ´æ°  ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+ä¼èªå¨å¸®ä½ æ PicMenu
+çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
+å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
+github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
+__init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
+lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
+é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
-æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-
-data`æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/
-bawiki-data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
+æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
+æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
+data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.3 - ä¿®å¤ bug ### 0.7.2 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ###
-0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
+æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

