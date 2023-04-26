# Comparing `tmp/copymanga_dl-3.1.tar.gz` & `tmp/copymanga_dl-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copymanga_dl-3.1.tar", max compression
+gzip compressed data, was "copymanga_dl-3.2.tar", max compression
```

## Comparing `copymanga_dl-3.1.tar` & `copymanga_dl-3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1328 2023-04-14 02:44:01.000000 copymanga_dl-3.1/Image_stitching.py
--rw-r--r--   0        0        0    35149 2023-04-14 02:44:01.000000 copymanga_dl-3.1/LICENSE
--rw-r--r--   0        0        0    12983 2023-04-14 02:44:01.000000 copymanga_dl-3.1/README.md
--rw-r--r--   0        0        0    30446 2023-04-14 02:44:01.000000 copymanga_dl-3.1/main.py
--rw-r--r--   0        0        0      958 2023-04-14 02:44:01.000000 copymanga_dl-3.1/pyproject.toml
--rw-r--r--   0        0        0    13971 1970-01-01 00:00:00.000000 copymanga_dl-3.1/PKG-INFO
+-rw-r--r--   0        0        0     1328 2023-04-25 13:34:17.000000 copymanga_dl-3.2/Image_stitching.py
+-rw-r--r--   0        0        0    35149 2023-04-25 13:34:17.000000 copymanga_dl-3.2/LICENSE
+-rw-r--r--   0        0        0    12983 2023-04-25 13:34:17.000000 copymanga_dl-3.2/README.md
+-rw-r--r--   0        0        0    32808 2023-04-25 13:34:17.000000 copymanga_dl-3.2/main.py
+-rw-r--r--   0        0        0      958 2023-04-25 13:34:17.000000 copymanga_dl-3.2/pyproject.toml
+-rw-r--r--   0        0        0    13971 1970-01-01 00:00:00.000000 copymanga_dl-3.2/PKG-INFO
```

### Comparing `copymanga_dl-3.1/Image_stitching.py` & `copymanga_dl-3.2/Image_stitching.py`

 * *Files identical despite different names*

### Comparing `copymanga_dl-3.1/LICENSE` & `copymanga_dl-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `copymanga_dl-3.1/README.md` & `copymanga_dl-3.2/README.md`

 * *Files identical despite different names*

### Comparing `copymanga_dl-3.1/main.py` & `copymanga_dl-3.2/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,33 +31,38 @@
 SETTINGS = {
     "download_path": None,
     "authorization": None,
     "use_oversea_cdn": None,
     "use_webp": None,
     "proxies": None,
     "api_url": None,
+    "HC": None,
     "api_time": 0.0,
     "API_COUNTER": 0
 }
 
 # 全局化设置,备份,防止命令行参数导致设置错位
 OG_SETTINGS = {
     "download_path": None,
     "authorization": None,
     "use_oversea_cdn": None,
     "use_webp": None,
     "proxies": None,
     "api_url": None,
+    "HC": None,
     "api_time": 0.0,
     "API_COUNTER": 0
 }
 
 UPDATE_LIST = []
 
+# API限制相关
 API_COUNTER = 0
+IMG_API_COUNTER = 0
+IMG_CURRENT_TIME = 0
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         '--MangaPath',
@@ -119,19 +124,23 @@
     print(f"[bold green][:white_check_mark: ]漫画已经下载完成！[/]")
 
 
 # 正常模式
 
 def welcome():
     choice_manga_path_word = None
-    want_to = int(Prompt.ask("您是想搜索还是查看您的收藏？[italic yellow](0:导出收藏,1:搜索,2:收藏,3:添加半自动更新)[/]",
-                             choices=["0", "1", "2", "3"], default="1"))
+    want_to = int(Prompt.ask(
+        "您是想搜索还是查看您的收藏？[italic yellow](0:导出收藏,1:搜索,2:收藏,3:添加半自动更新,9:修改设置)[/]",
+        choices=["0", "1", "2", "3", "9"], default="1"))
     if want_to == 0:
         collect_expect()
         return
+    if want_to == 9:
+        change_settings()
+        return
     if want_to == 3:
         updates()
         return
     if want_to == 1:
         choice_manga_path_word = search()
     if want_to == 2:
         choice_manga_path_word = search_on_collect()
@@ -162,58 +171,34 @@
     search_content = Prompt.ask("您需要搜索添加什么漫画呢")
     url = "https://api.%s/api/v3/search/comic?format=json&platform=3&q=%s&limit=10&offset={}" % (
         SETTINGS["api_url"], search_content)
     offset = 0
     current_page_count = 1
     while True:
         # 发送GET请求
-        response = requests.get(url.format(offset), headers=API_HEADER, proxies=PROXIES)
-        # 记录API访问量
-        api_restriction()
-        # 解析JSON数据
-        data = response.json()
-
-        console.rule(f"[bold blue]当前为第{current_page_count}页")
-        # 输出每个comic的名称和对应的序号
-        for i, comic in enumerate(data["results"]["list"]):
-            print("[{}] {}".format(i + 1, comic["name"]))
-
-        # 让用户输入数字来选择comic
-        selection = Prompt.ask("请选择一个漫画[italic yellow]（输入Q退出,U为上一页,D为下一页）[/]")
+        selection = search_list(url, offset, current_page_count)
+        data = selection[1]
+        selection = selection[0]
         if selection.upper() == "Q":
             break
         try:
             # 将用户输入的字符串转换为整数
             index = int(selection) - 1
             # 获取用户选择的comic的名称并输出
             print("你选择了：{}".format(data["results"]["list"][index]["name"]))
             # 让用户选择分组
             manga_group_path_word = manga_group(data["results"]["list"][index]["path_word"])
             # 返回两个pathWord与漫画名称
             return data["results"]["list"][index]["path_word"], manga_group_path_word, data["results"]["list"][index][
                 "name"]
 
         except (ValueError, IndexError):
-            # 判断是否是输入的U/D
-            # 根据用户输入更新offset
-            if selection.upper() == "U":
-                offset -= data["results"]["limit"]
-                if offset < 0:
-                    offset = 0
-                else:
-                    current_page_count -= 1
-            elif selection.upper() == "D":
-                offset += data["results"]["limit"]
-                if offset > data["results"]["total"]:
-                    offset = data["results"]["total"] - data["results"]["limit"]
-                else:
-                    current_page_count += 1
-            else:
-                # 处理输入错误的情况
-                print("[italic red]无效的选择！[/]")
+            offset = page_turning(selection, offset, data, current_page_count)
+            current_page_count = offset[1]
+            offset = offset[0]
 
 
 def load_updates():
     global UPDATE_LIST
     # 获取用户目录的路径
     home_dir = os.path.expanduser("~")
     updates_path = os.path.join(home_dir, ".copymanga-downloader/update.json")
@@ -291,16 +276,16 @@
         if manga_chapter_json != 0:
             chapter_allocation(manga_chapter_json)
 
 
 def update_get_chapter(manga_path_word, manga_group_path_word, now_chapter):
     # 因为将偏移设置到最后下载的章节，所以可以直接下载全本
     response = requests.get(
-        f"https://api.{SETTINGS['api_url']}/api/v3/comic/{manga_path_word}/group/{manga_group_path_word}/chapters?limit=500"
-        f"&offset={now_chapter}&platform=3",
+        f"https://api.{SETTINGS['api_url']}/api/v3/comic/{manga_path_word}/group/{manga_group_path_word}/chapters"
+        f"?limit=500&offset={now_chapter}&platform=3",
         headers=API_HEADER, proxies=PROXIES)
     # 记录API访问量
     api_restriction()
     response.raise_for_status()
     manga_chapter_json = response.json()
     # Todo 创建传输的json,并且之后会将此json保存为temp.json修复这个问题https://github.com/misaka10843/copymanga-downloader/issues/35
     return_json = {
@@ -316,63 +301,77 @@
         print("[bold red]我们暂时不支持下载到500话以上，还请您去Github中创建Issue！[/]")
         sys.exit()
     return return_json
 
 
 # 搜索相关
 
+def search_list(url, offset, current_page_count):
+    response = requests.get(url.format(offset), headers=API_HEADER, proxies=PROXIES)
+    # 记录API访问量
+    api_restriction()
+    # 解析JSON数据
+    data = response.json()
+
+    console.rule(f"[bold blue]当前为第{current_page_count}页")
+    # 输出每个comic的名称和对应的序号
+    for i, comic in enumerate(data["results"]["list"]):
+        print("[{}] {}".format(i + 1, comic["name"]))
+
+    # 让用户输入数字来选择comic
+    selection = Prompt.ask("请选择一个漫画[italic yellow]（输入Q退出,U为上一页,D为下一页）[/]")
+    return selection, data
+
+
+def page_turning(selection, offset, data, current_page_count):
+    # 判断是否是输入的U/D
+    # 根据用户输入更新offset
+    if selection.upper() == "U":
+        offset -= data["results"]["limit"]
+        if offset < 0:
+            offset = 0
+        else:
+            current_page_count -= 1
+    elif selection.upper() == "D":
+        offset += data["results"]["limit"]
+        if offset > data["results"]["total"]:
+            offset = data["results"]["total"] - data["results"]["limit"]
+        else:
+            current_page_count += 1
+    else:
+        # 处理输入错误的情况
+        print("[italic red]无效的选择！[/]")
+    return offset, current_page_count
+
+
 def search():
     search_content = Prompt.ask("您需要搜索什么漫画呢")
     url = "https://api.%s/api/v3/search/comic?format=json&platform=3&q=%s&limit=10&offset={}" % (
         SETTINGS["api_url"], search_content)
     offset = 0
     current_page_count = 1
     while True:
         # 发送GET请求
-        response = requests.get(url.format(offset), headers=API_HEADER, proxies=PROXIES)
-        # 记录API访问量
-        api_restriction()
-        # 解析JSON数据
-        data = response.json()
-
-        console.rule(f"[bold blue]当前为第{current_page_count}页")
-        # 输出每个comic的名称和对应的序号
-        for i, comic in enumerate(data["results"]["list"]):
-            print("[{}] {}".format(i + 1, comic["name"]))
-
-        # 让用户输入数字来选择comic
-        selection = Prompt.ask("请选择一个漫画[italic yellow]（输入Q退出,U为上一页,D为下一页）[/]")
+        selection = search_list(url, offset, current_page_count)
+        data = selection[1]
+        selection = selection[0]
         if selection.upper() == "Q":
             break
         try:
             # 将用户输入的字符串转换为整数
             index = int(selection) - 1
             # 获取用户选择的comic的名称并输出
             print("你选择了：{}".format(data["results"]["list"][index]["name"]))
             # 返回pathWord
             return data["results"]["list"][index]["path_word"]
 
         except (ValueError, IndexError):
-            # 判断是否是输入的U/D
-            # 根据用户输入更新offset
-            if selection.upper() == "U":
-                offset -= data["results"]["limit"]
-                if offset < 0:
-                    offset = 0
-                else:
-                    current_page_count -= 1
-            elif selection.upper() == "D":
-                offset += data["results"]["limit"]
-                if offset > data["results"]["total"]:
-                    offset = data["results"]["total"] - data["results"]["limit"]
-                else:
-                    current_page_count += 1
-            else:
-                # 处理输入错误的情况
-                print("[italic red]无效的选择！[/]")
+            offset = page_turning(selection, offset, data, current_page_count)
+            current_page_count = offset[1]
+            offset = offset[0]
 
 
 # 收藏相关
 
 def search_on_collect():
     url = "https://%s/api/v3/member/collect/comics?limit=12&offset={}&free_type=1&ordering=-datetime_modifier" % (
         SETTINGS["api_url"])
@@ -405,31 +404,17 @@
             index = int(selection) - 1
             # 获取用户选择的comic的名称并输出
             print("你选择了：{}".format(data["results"]["list"][index]['comic']["name"]))
             # 返回pathWord
             return data["results"]["list"][index]['comic']["path_word"]
 
         except (ValueError, IndexError):
-            # 判断是否是输入的U/D
-            # 根据用户输入更新offset
-            if selection.upper() == "U":
-                offset -= data["results"]["limit"]
-                if offset < 0:
-                    offset = 0
-                else:
-                    current_page_count -= 1
-            elif selection.upper() == "D":
-                offset += data["results"]["limit"]
-                if offset > data["results"]["total"]:
-                    offset = data["results"]["total"] - data["results"]["limit"]
-                else:
-                    current_page_count += 1
-            else:
-                # 处理输入错误的情况
-                print("[italic red]无效的选择！[/]")
+            offset = page_turning(selection, offset, data, current_page_count)
+            current_page_count = offset[1]
+            offset = offset[0]
 
 
 def collect_expect():
     url = f"https://api.{SETTINGS['api_url']}/api/v3/member/collect/comics"
     params = {
         "limit": 12,
         "offset": 0
@@ -572,14 +557,15 @@
                 if not os.path.exists(f"{download_path}/{manga_name}/{chapter_name}/"):
                     os.mkdir(f"{download_path}/{manga_name}/{chapter_name}/")
                 # 组成下载路径
                 filename = f"{download_path}/{manga_name}/{chapter_name}/{str(img_words[i] + 1).zfill(3)}.jpg"
                 t = threading.Thread(target=download, args=(url, filename))
                 # 开始线程
                 threads.append(t)
+                img_api_restriction()
                 # 限制线程数量(十分不建议修改，不然很可能会被禁止访问)
                 if len(threads) == 4 or i == num_images - 1:
                     for t in threads:
                         # 添加一点延迟，错峰请求
                         time.sleep(0.5)
                         t.start()
                     for t in threads:
@@ -593,123 +579,209 @@
 
         print(f"[bold green][:white_check_mark:][{manga_name}]{chapter_name}下载完成！[/]")
 
 
 # API限制相关
 
 def api_restriction():
-    global API_COUNTER
+    global API_COUNTER, IMG_API_COUNTER
     API_COUNTER += 1
     # 防止退出后立马再次运行
     current_time = OG_SETTINGS['api_time']
     time_diff = time.time() - current_time
     # 判断是否超过60秒
     if time_diff < 60 and API_COUNTER <= 1:
         API_COUNTER = API_COUNTER + OG_SETTINGS['API_COUNTER']
     if API_COUNTER >= 15:
         API_COUNTER = 0
         print("[bold yellow]您已经触发到了API请求阈值，我们将等60秒后再进行[/]")
         time.sleep(60)
     OG_SETTINGS['API_COUNTER'] = API_COUNTER
     OG_SETTINGS['api_time'] = time.time()
     # 将时间戳与API请求数量写入配置文件
-    home_dir = os.path.expanduser("~")
-    if not os.path.exists(os.path.join(home_dir, '.copymanga-downloader/')):
-        os.mkdir(os.path.join(home_dir, '.copymanga-downloader/'))
-    settings_path = os.path.join(home_dir, ".copymanga-downloader/settings.json")
-    # 写入settings.json文件
-    with open(settings_path, "w") as f:
-        json.dump(OG_SETTINGS, f)
+    save_settings(OG_SETTINGS)
+
+
+def img_api_restriction():
+    global IMG_API_COUNTER, IMG_CURRENT_TIME
+    IMG_API_COUNTER += 1
+    # 防止退出后立马再次运行
+
+    time_diff = time.time() - IMG_CURRENT_TIME
+    # 判断是否超过60秒
+    if time_diff < 60 and IMG_API_COUNTER >= 100:
+        print("[bold yellow]您已经触发到了图片服务器API请求阈值，我们将等60秒后再进行[/]")
+        time.sleep(60)
+        IMG_CURRENT_TIME = 0
+        IMG_API_COUNTER = 0
 
 
 # 下载相关
 
 @retrying.retry(stop_max_attempt_number=3)
 def download(url, filename):
     # 判断是否已经下载
     if os.path.exists(filename):
         print(f"[blue]您已经下载了{filename}，跳过下载[/]")
         return
     try:
+        if SETTINGS['HC'] == "1":
+            url = url.replace("c800x.jpg", "c1500x.jpg")
         response = requests.get(url, headers=API_HEADER, proxies=PROXIES)
         with open(filename, "wb") as f:
             f.write(response.content)
-    except:
+    except Exception as e:
         print(
-            f"[bold red]无法下载{filename}，似乎是CopyManga暂时屏蔽了您的IP，请稍后手动下载对应章节(章节话数为每话下载输出的索引ID)[/]")
+            f"[bold red]无法下载{filename}，似乎是CopyManga暂时屏蔽了您的IP，请稍后手动下载对应章节(章节话数为每话下载输出的索引ID),ErrMsg:{e}[/]")
 
 
 # 设置相关
 
 def get_org_url():
     print("[italic yellow]正在获取CopyManga网站Url...[/]")
     url = "https://cdn.jsdelivr.net/gh/misaka10843/copymanga-downloader@master/url.json"
     try:
-        response = requests.get(url,proxies=PROXIES)
+        response = requests.get(url, proxies=PROXIES)
         response.raise_for_status()
         return response.json()
-    except:
+    except Exception as e:
         print("[bold yellow]无法链接至jsdelivr，准备直接访问Github[/]")
         # 更换URL
         url = "https://raw.githubusercontent.com/misaka10843/copymanga-downloader/master/url.json"
         try:
-            response = requests.get(url,proxies=PROXIES)
+            response = requests.get(url, proxies=PROXIES)
             response.raise_for_status()
             return response.json()
-        except:
-            print("[bold red]无法链接至GitHub，请检查网络连接[/]", )
+        except Exception as e:
+            print(f"[bold red]无法链接至GitHub，请检查网络连接,ErrMsg:{e}[/]", )
             sys.exit()
 
 
 def set_settings():
     global PROXIES
     # 获取用户输入
     download_path = Prompt.ask("请输入保存路径")
     authorization = Prompt.ask("请输入账号Token")
     use_oversea_cdn_input = Confirm.ask("是否使用海外CDN？", default=False)
     use_webp_input = Confirm.ask("是否使用Webp？[italic yellow](可以节省服务器资源,下载速度也会加快)[/]",
                                  default=True)
     proxy = Prompt.ask("请输入代理地址[italic yellow](没有的话可以直接回车跳过)[/]")
+    hc_input = Confirm.ask("是否下载高分辨率图片[italic yellow](不选择可以节省服务器资源,下载速度也会加快)[/]",
+                           default=False)
     if proxy:
         PROXIES = {
             "http": proxy,
             "https": proxy
         }
     api_urls = get_org_url()
     for i, url in enumerate(api_urls):
         print(f"{i + 1}->{url}")
     choice = IntPrompt.ask("请输入要使用的API前面的数字")
 
     # input转bool
     use_oversea_cdn = "0"
     use_webp = "0"
+    hc = "0"
     if use_oversea_cdn_input:
         use_oversea_cdn = "1"
     if use_webp_input:
         use_webp = "1"
+    if hc_input:
+        hc = "1"
 
     # 构造settings字典
     settings = {
         "download_path": download_path,
         "authorization": authorization,
         "use_oversea_cdn": use_oversea_cdn,
         "use_webp": use_webp,
         "proxies": proxy,
         "api_url": api_urls[choice - 1],
+        "HC": hc,
         "api_time": 0.0,
         "API_COUNTER": 0
     }
     home_dir = os.path.expanduser("~")
+    settings_path = os.path.join(home_dir, ".copymanga-downloader/settings.json")
+    save_settings(settings)
+    print(f"[yellow]已将配置文件存放到{settings_path}中[/]")
+
+
+def change_settings():
+    global PROXIES
+    # 获取用户输入
+    download_path = Prompt.ask("请输入保存路径", default=SETTINGS['download_path'])
+    authorization = Prompt.ask("请输入账号Token", default=SETTINGS['authorization'])
+    use_oversea_cdn = True
+    use_webp = True
+    if SETTINGS['use_oversea_cdn'] == "0":
+        use_oversea_cdn = False
+    if SETTINGS['use_webp'] == "0":
+        use_webp = False
+    use_oversea_cdn_input = Confirm.ask("是否使用海外CDN？", default=use_oversea_cdn)
+    use_webp_input = Confirm.ask("是否使用Webp？[italic yellow](可以节省服务器资源,下载速度也会加快)[/]",
+                                 default=use_webp)
+    proxy = Prompt.ask("请输入代理地址[italic yellow](如果需要清除请输入0)[/]", default=SETTINGS['proxies'])
+    if SETTINGS['HC'] is None:
+        hc_input = Confirm.ask("是否下载高分辨率图片[italic yellow](不选择可以节省服务器资源,下载速度也会加快)[/]",
+                               default=False)
+    else:
+        hc_c = True
+        if SETTINGS['HC'] == "0":
+            hc_c = False
+        hc_input = Confirm.ask("请输入代理地址[italic yellow](如果需要清除请输入0)[/]", default=hc_c)
+    if proxy != SETTINGS['proxies'] and proxy != "0":
+        PROXIES = {
+            "http": proxy,
+            "https": proxy
+        }
+    if proxy == "0":
+        proxy = ""
+    api_urls = get_org_url()
+    for i, url in enumerate(api_urls):
+        print(f"{i + 1}->{url}")
+    choice = IntPrompt.ask("请输入要使用的API前面的数字")
+    print(f"[yellow]我们正在更改您的设置中，请稍后[/]")
+    # input转bool
+    use_oversea_cdn = "0"
+    use_webp = "0"
+    hc = "0"
+    if use_oversea_cdn_input:
+        use_oversea_cdn = "1"
+    if use_webp_input:
+        use_webp = "1"
+    if hc_input:
+        hc = "1"
+
+    # 构造settings字典
+    settings = {
+        "download_path": download_path,
+        "authorization": authorization,
+        "use_oversea_cdn": use_oversea_cdn,
+        "use_webp": use_webp,
+        "proxies": proxy,
+        "api_url": api_urls[choice - 1],
+        "HC": hc,
+        "api_time": 0.0,
+        "API_COUNTER": 0
+    }
+    home_dir = os.path.expanduser("~")
+    settings_path = os.path.join(home_dir, ".copymanga-downloader/settings.json")
+    save_settings(settings)
+    print(f"[yellow]已将重新修改配置文件并存放到{settings_path}中[/]")
+
+
+def save_settings(settings):
+    home_dir = os.path.expanduser("~")
     if not os.path.exists(os.path.join(home_dir, '.copymanga-downloader/')):
         os.mkdir(os.path.join(home_dir, '.copymanga-downloader/'))
     settings_path = os.path.join(home_dir, ".copymanga-downloader/settings.json")
     # 写入settings.json文件
     with open(settings_path, "w") as f:
         json.dump(settings, f)
-    print(f"[yellow]已将配置文件存放到{settings_path}中[/]")
 
 
 def load_settings():
     global SETTINGS, PROXIES, OG_SETTINGS, API_HEADER
     # 获取用户目录的路径
     home_dir = os.path.expanduser("~")
     settings_path = os.path.join(home_dir, ".copymanga-downloader/settings.json")
@@ -722,14 +794,20 @@
 
     # 判断必要的字段是否存在
     necessary_fields = ["download_path", "authorization", "use_oversea_cdn", "use_webp", "proxies", "api_url"]
     for field in necessary_fields:
         if field not in settings:
             return False, "settings.json中缺少必要字段{}".format(field)
     SETTINGS = settings
+    if "HC" not in settings:
+        SETTINGS['HC'] = None
+        print("[bold yellow]我们更新了设置，请您按照需求重新设置一下，还请谅解[/]")
+        change_settings()
+        print("[bold yellow]感谢您的支持，重新启动本程序后新的设置将会生效[/]")
+        exit(0)
     OG_SETTINGS = settings
     # 设置请求头
     API_HEADER['use_oversea_cdn'] = settings['use_oversea_cdn']
     API_HEADER['use_webp'] = settings['use_webp']
     # 设置代理
     if settings["proxies"]:
         PROXIES = {
```

### Comparing `copymanga_dl-3.1/pyproject.toml` & `copymanga_dl-3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copymanga-dl"
-version = "3.1"
+version = "3.2"
 description = "Copymanga Downloader"
 license = "GPL-3.0-or-later"
 authors = ["misaka10843 <misaka10843@outlook.jp>"]
 readme = "README.md"
 homepage = "https://misaka.sakurakoi.top/"
 repository = "https://github.com/misaka10843/copymanga-downloader"
 documentation = ""
```

### Comparing `copymanga_dl-3.1/PKG-INFO` & `copymanga_dl-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copymanga-dl
-Version: 3.1
+Version: 3.2
 Summary: Copymanga Downloader
 Home-page: https://misaka.sakurakoi.top/
 License: GPL-3.0-or-later
 Keywords: copymanga,downloader
 Author: misaka10843
 Author-email: misaka10843@outlook.jp
 Requires-Python: >=3.10,<4
```

