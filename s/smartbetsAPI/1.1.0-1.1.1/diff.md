# Comparing `tmp/smartbetsAPI-1.1.0.tar.gz` & `tmp/smartbetsAPI-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.1.0.tar", last modified: Wed Mar 15 13:17:19 2023, max compression
+gzip compressed data, was "smartbetsAPI-1.1.1.tar", last modified: Wed Apr 26 13:33:06 2023, max compression
```

## Comparing `smartbetsAPI-1.1.0.tar` & `smartbetsAPI-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:17:19.578701 smartbetsAPI-1.1.0/
--rw-r--r--   0 root         (0) root         (0)    14753 2023-03-15 13:17:19.578701 smartbetsAPI-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9443 2023-03-15 13:14:02.000000 smartbetsAPI-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 13:17:19.578701 smartbetsAPI-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:17:19.575367 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14753 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-15 13:17:19.000000 smartbetsAPI-1.1.0/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:17:19.578701 smartbetsAPI-1.1.0/smartbets_API/
--rw-r--r--   0 root         (0) root         (0)       51 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/bet_analyzer.py
--rw-r--r--   0 root         (0) root         (0)    11218 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/bet_common.py
--rw-r--r--   0 root         (0) root         (0)     4205 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/configuration_handler.py
--rw-r--r--   0 root         (0) root         (0)     6613 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/figure_harvester.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/googler.py
--rw-r--r--   0 root         (0) root         (0)     5341 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/html_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     6472 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/interface.py
--rw-r--r--   0 root         (0) root         (0)     8775 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/predictor.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-03-15 13:02:47.000000 smartbetsAPI-1.1.0/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9441 2023-04-26 13:12:46.000000 smartbetsAPI-1.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-04-26 13:31:03.000000 smartbetsAPI-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.179994 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/smartbets_API/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-26 12:51:40.000000 smartbetsAPI-1.1.1/smartbets_API/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-04-26 12:26:14.000000 smartbetsAPI-1.1.1/smartbets_API/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-04-26 12:39:32.000000 smartbetsAPI-1.1.1/smartbets_API/bet_at_api_level.py
+-rw-r--r--   0 root         (0) root         (0)    11304 2023-03-31 20:51:37.000000 smartbetsAPI-1.1.1/smartbets_API/bet_common.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2023-03-31 20:48:34.000000 smartbetsAPI-1.1.1/smartbets_API/configuration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6613 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/figure_harvester.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/googler.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-03-31 20:20:15.000000 smartbetsAPI-1.1.1/smartbets_API/html_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     6611 2023-03-31 20:17:33.000000 smartbetsAPI-1.1.1/smartbets_API/interface.py
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-03-26 16:28:20.000000 smartbetsAPI-1.1.1/smartbets_API/proxyh.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-03-12 10:54:19.000000 smartbetsAPI-1.1.1/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.1.0/PKG-INFO` & `smartbetsAPI-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,491 +1,18 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
-Description: <h1 align="center">smartbetsAPI</h1>
-        
-         <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="https://github.com/Simatwa/smartbetsAPI/raw/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI/1.1.0/"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a><br>
-        
-         
-        
-         > "Punter's choice" 
-        
-        
-        
-         Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
-        
-        
-        
-         ## Features
-        
-         - REST-API
-        
-         - Script intergration (package)
-        
-         - Non-AI 
-        
-        
-        
-         ## Installation and usage
-        
-        
-        
-         ### Installation
-        
-        
-        
-        1. Linux 
-        
-        
-        
-        *Python 3.7+* is required for this script to be fruitful to you. 
-        
-        - Installing through pip is always the most preferred way:
-        
-        
-        
-         ```sh
-        
-         $ pip  install smartbetsAPI
-        
-         
-        
-         ```
-        
-        
-        
-         - For those who like enjoying the **latest** releases from [Github](https://github.com) like [me](https://github.com/Simatwa), rather than  waiting for the next release:
-        
-        
-        
-         ```sh
-        
-         $ pip install git+https://github.com/Simatwa/smartbetsAPI.git
-        
-        
-        
-         ```
-        
-        
-        
-        - The hard-core guys with _trust issues_ are very much sorted this way:
-        
-        
-        
-         ```sh
-        
-        
-        
-         $ git clone https://github.com/Simatwa/smartbetsAPI.git
-        
-        
-        
-         $ cd smartbetsAPI
-        
-        
-        
-         $ bash install.sh 
-        
-        
-        
-           #or
-        
-        
-        
-        $ sudo bash install.sh
-        
-        
-        
-        ```
-        
-        
-        
-        ### Usage
-        
-        
-        
-        1. Terminal
-        
-        
-        
-         Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](https://github.com/pallets/Flask) server with the following default configurations.
-        
-        
-        
-        <table align="center"> 
-        
-        <thead>
-        
-        <tr><th>Command        </th><th>Default  </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>Port           </td><td>8000     </td></tr>
-        
-        <tr><td>Username       </td><td>API</td></tr>
-        
-        <tr><td>Filename       </td><td>None     </td></tr>
-        
-        <tr><td>level (Logging)</td><td>20       </td></tr>
-        
-        <tr><td>host           </td><td>False    </td></tr>
-        
-        <tr><td>debug          </td><td>False    </td></tr>
-        
-        <tr><td>no-net         </td><td>False    </td></tr>
-        
-        <tr><td>log            </td><td>False    </td></tr>
-        
-        <tr><td>colorize       </td><td>False    </td></tr>
-        
-        <tr><td>gui (Termux)   </td><td>False    </td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        - For instance :
-        
-        
-        
-         ```sh
-        
-         $ smartbetsAPI mypass9876
-        
-        
-        
-        ``` 
-        
-        
-        
-        Here is an example of a [simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/bet_at_api_level.py) that makes prediction using the `api`.
-        
-        
-        
-        ![api running](https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif)
-        
-        
-        
-        
-        
-        > **Note** 
-        
-          - Content-Type of the response (predictions) is `application/json`
-        
-          - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
-        
-        
-        
-        
-        
-        * For more information you can run `smartbetsAPI -h` 
-        
-        
-        
-        
-        
-        2. Importing Package
-        
-        
-        
-        Module `predictor`  provides two ways of interacting with it at the programming level, based on the `data-type` in which the teams have been packed and parsed to it:
-        
-        
-        
-        * Using `predictorL` object which accepts *teams* (**List** data-type).
-        
-        > For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_list.py):
-        
-        
-        
-        ```py
-        
-        #!/usr/bin/env python3
-        
-        from smartbets_API.predictor import predictor
-        
-        
-        
-        teams = [
-        
-            "Napoli",  # Home team (index [0])
-        
-            "AC Milan",  # Away team (index [1])
-        
-        ]
-        
-        # Instantiating predictor
-        
-        predict = predictor()
-        
-        
-        
-        # Using predictorL object to handle teams (List data-type)
-        
-        predictions = predict.predictorL(teams)
-        
-        
-        
-        # Display info
-        
-        print(predictions)
-        
-        
-        
-        #Output
-        
-        #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'}
-        
-        
-        
-        ```
-        
-        
-        
-        * Using `predictorD` object which takes *teams* (**Dictionary** data-type):
-        
-        > For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py):
-        
-        
-        
-        ```py
-        
-        #!/usr/bin/env python3
-        
-        from smartbets_API.predictor import predictor
-        
-        
-        
-        teams = {
-        
-            1: "Manchester City",  # 1 for home-team
-        
-            2: "Liverpool",  # 2 for away-team
-        
-        }
-        
-        
-        
-        # Instantiating predictor
-        
-        predict = predictor()
-        
-        
-        
-        # Using predictorD object to handle teams (Dictionary data-type)
-        
-        predictions = predict.predictorD(teams)
-        
-        
-        
-        # Display info
-        
-        print(predictions)
-        
-        
-        
-        #Output
-        
-        #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'}
-        
-        
-        
-        ```
-        
-        
-        
-        - The output initials are explained in the table below.
-        
-        
-        
-        <table>
-        
-        <thead>
-        
-        <tr><th>Parameter  </th><th>Function                                                 </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>g          </td><td>Goal-average of the two teams                              </td></tr>
-        
-        <tr><td>gg         </td><td>Probability of both teams to score                         </td></tr>
-        
-        <tr><td>ov15       </td><td>Probability of having more than 2 goals                    </td></tr>
-        
-        <tr><td>ov25       </td><td>Probability of having more than 3 goals                    </td></tr>
-        
-        <tr><td>ov35       </td><td>Probability of having more than 4 goals                    </td></tr>
-        
-        <tr><td>choice     </td><td>Probability of the specified &#x27;result&#x27; to occur            </td></tr>
-        
-        <tr><td>result     </td><td>The most suitable outcome from [1,1x,x,2x,2]                  </td></tr>
-        
-        <tr><td>pick       </td><td>The most suitable outcome from [1,1x,x,2x,2,gg,ov15,ov25,ov35]</td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        > **Note** 
-        
-          - Probabilities are in percentange (%)
-        
-        
-        
-        #### Further info 
-        
-        
-        
-        The `predictor` _class_ accepts multiple parameters that includes :
-        
-        
-        
-        <table>
-        
-        <thead>
-        
-        <tr><th>Parameter       </th><th>Function                                              </th><th>Default  </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>include_position</td><td>Include team&#x27;s league ranking in making predictions     </td><td>False    </td></tr>
-        
-        <tr><td>log             </td><td>Log at api default log&#x27;s path                           </td><td>False    </td></tr>
-        
-        <tr><td>level           </td><td>Logging level                                           </td><td>0        </td></tr>
-        
-        <tr><td>filename        </td><td>Log to the filename specified                           </td><td>None     </td></tr>
-        
-        <tr><td>color           </td><td>Colorize the logs                                       </td><td>False    </td></tr>
-        
-        <tr><td>gui             </td><td>Run with some Graphical interface notifications (Termux)</td><td>False    </td></tr>
-        
-        <tr><td>api             </td><td>Run with api-server&#x27;s configurations                    </td><td>False    </td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        The two predictor's object (`predictorD`, `predictorL`) accepts two parameters i.e.
-        
-        * **teams** - Required
-        
-        * **net** - Source of team's data - Default `True` (Online)
-        
-        
-        
-        ## Source of data
-        
-        
-        
-        Team performances are sourced from [Soccerway](https://int.soccerway.com) after retrieving the *uri* from [Google](https://www.google.com).
-        
-        
-        
-        > **Warning** Copyright related issues are liable to the user of this script!
-        
-        
-        
-        ## Disclaimer
-        
-        
-        
-        This project aims to help *punters* and *bookmarkers* to make informed and well researched soccer-predictions. Nevertheless, it is important to specify that 100% accuracy does not exist and smartbetsAPI can't guarantee the accuracy of the predictions. It is therefore your responsibility to trust the information generated by smartbetsAPI after evaluating its reliability. As the [creator](https://github.com/Simatwa), I **CANNOT** be held responsible for any loss of capital that may occur during the use of this program.
-        
-        
-        
-        ## Contributing and Support
-        
-        
-        
-        ### Contributing
-        
-        
-        
-        Contributions are always welcome! <br>
-        
-        Please take a look at the [Contribution guidelines](CONTRIBUTING.md). <br>
-        
-        Feel free to open an [Issue](https://github.com/Simatwa/smartbetsAPI/issues) or to [Fork](https://github.com/Simatwa/smartbetsAPI/fork) this repo.
-        
-        
-        
-        ### ToDo
-        
-        
-        
-        - [ ] Upgrade to Machine learning
-        
-        - [ ] Improve algorithim's accuracy
-        
-        - [ ] General code improvements
-        
-        - [ ] Fix bugs
-        
-        
-        
-        ### Support 
-        
-        
-        
-        Consider donating to this project if you find it useful:
-        
-        <p align="center">
-        
-        <a href="https://www.paypal.com/donate/?hosted_button_id=KLNYKSGUXY8R2"><img src="https://img.shields.io/static/v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal"/></a>
-        
-        </p>
-        
-        
-        
-        ## Credits
-        
-        
-        
-        - [x] [Soccerway](https://int.soccerway.com)
-        
-        - [x] [Google](https://www.google.com)
-        
-        - [x] [Python.org](https://python.org)
-        
-        
-        
-        ## Special Thanks
-        
-        
-        
-        * [x] [victhepythonista](https://github.com/victhepythonista)
-        
-        * [x] YOU.
-        
-        
-        
-         [View updated version of this info.](https://simatwa.github.io/smartbetsAPI)
-        
 Keywords: Football,Predictions,Betting API,Soccer predictions,Football Predictions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -496,7 +23,500 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">smartbetsAPI</h1>
+
+<p align="center">
+
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+
+ 
+
+ > "Punter's choice" 
+
+
+
+ Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
+
+
+
+ ## Features
+
+ - REST-API
+
+ - Script intergration (package)
+
+ - Non-AI 
+
+
+
+ ## Installation and usage
+
+
+
+ ### Installation
+
+
+
+1. Linux 
+
+
+
+*Python 3.7+* is required for this script to be fruitful to you. 
+
+- Installing through pip is always the most preferred way:
+
+
+
+ ```sh
+
+ pip  install smartbetsAPI
+
+ 
+
+ ```
+
+
+
+ - For those who like enjoying the **latest** releases from [Github](https://github.com) like [me](https://github.com/Simatwa), rather than  waiting for the next release:
+
+
+
+ ```sh
+
+ pip install git+https://github.com/Simatwa/smartbetsAPI.git
+
+
+
+ ```
+
+
+
+- The hard-core guys with _trust issues_ are very much sorted this way:
+
+
+
+ ```sh
+
+
+
+ git clone https://github.com/Simatwa/smartbetsAPI.git
+
+
+
+ cd smartbetsAPI
+
+
+
+ bash install.sh 
+
+
+
+   #or
+
+
+
+sudo bash install.sh
+
+
+
+```
+
+
+
+### Usage
+
+
+
+1. Terminal
+
+
+
+ Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
+
+
+
+<table align="center"> 
+
+<thead>
+
+<tr><th>Command        </th><th>Default  </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>Port           </td><td>8000     </td></tr>
+
+<tr><td>Username       </td><td>API</td></tr>
+
+<tr><td>Filename       </td><td>None     </td></tr>
+
+<tr><td>level (Logging)</td><td>20       </td></tr>
+
+<tr><td>host           </td><td>False    </td></tr>
+
+<tr><td>debug          </td><td>False    </td></tr>
+
+<tr><td>no-net         </td><td>False    </td></tr>
+
+<tr><td>log            </td><td>False    </td></tr>
+
+<tr><td>colorize       </td><td>False    </td></tr>
+
+<tr><td>gui (Termux)   </td><td>False    </td></tr>
+
+</tbody>
+
+</table>
+
+
+
+- For instance :
+
+
+
+ ```sh
+
+ $ smartbetsAPI mypass9876
+
+
+
+``` 
+
+
+
+Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
+
+
+
+![api running](assets/api_running.gif)
+
+
+
+
+
+> **Note** 
+
+  - Content-Type of the response (predictions) is `application/json`
+
+  - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
+
+
+
+> Example predicting using REST API
+
+
+
+```py
+
+from smartbets_API import predictor
+
+predict = predictor('http://localhost:8080','password')
+
+bets=predict.get_predictions('Arsenal','Manchester')
+
+print(bets)
+
+#Output
+
+#(True, {'choice': 55.56, 'g': 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15', 'result': '1'})
+
+```
+
+
+
+
+
+* For more information you can run `smartbetsAPI -h` 
+
+
+
+
+
+2. Importing Package
+
+
+
+Module `predictor`  provides two ways of interacting with it at the programming level, based on the `data-type` in which the teams have been packed and parsed to it:
+
+
+
+* Using `predictorL` object which accepts *teams* (**List** data-type).
+
+> For [example](examples/predict_using_list.py):
+
+
+
+```py
+
+#!/usr/bin/env python3
+
+from smartbets_API.predictor import predictor
+
+
+
+teams = [
+
+    "Napoli",  # Home team (index [0])
+
+    "AC Milan",  # Away team (index [1])
+
+]
+
+# Instantiating predictor
+
+predict = predictor()
+
+
+
+# Using predictorL object to handle teams (List data-type)
+
+predictions = predict.predictorL(teams)
+
+
+
+# Display info
+
+print(predictions)
+
+
+
+#Output
+
+#{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'}
+
+
+
+```
+
+
+
+* Using `predictorD` object which takes *teams* (**Dictionary** data-type):
+
+> For [example](examples/predict_using_dict.py):
+
+
+
+```py
+
+#!/usr/bin/env python3
+
+from smartbets_API.predictor import predictor
+
+
+
+teams = {
+
+    1: "Manchester City",  # 1 for home-team
+
+    2: "Liverpool",  # 2 for away-team
+
+}
+
+
+
+# Instantiating predictor
+
+predict = predictor()
+
+
+
+# Using predictorD object to handle teams (Dictionary data-type)
+
+predictions = predict.predictorD(teams)
+
+
+
+# Display info
+
+print(predictions)
+
+
+
+#Output
+
+#{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'}
+
+
+
+```
+
+
+
+- The output initials are explained in the table below.
+
+
+
+<table>
+
+<thead>
+
+<tr><th>Parameter  </th><th>Function                                                 </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>g          </td><td>Goal-average of the two teams                              </td></tr>
+
+<tr><td>gg         </td><td>Probability of both teams to score                         </td></tr>
+
+<tr><td>ov15       </td><td>Probability of having more than 2 goals                    </td></tr>
+
+<tr><td>ov25       </td><td>Probability of having more than 3 goals                    </td></tr>
+
+<tr><td>ov35       </td><td>Probability of having more than 4 goals                    </td></tr>
+
+<tr><td>choice     </td><td>Probability of the specified &#x27;result&#x27; to occur            </td></tr>
+
+<tr><td>result     </td><td>The most suitable outcome from [1,1x,x,2x,2]                  </td></tr>
+
+<tr><td>pick       </td><td>The most suitable outcome from [1,1x,x,2x,2,gg,ov15,ov25,ov35]</td></tr>
+
+</tbody>
+
+</table>
+
+
+
+> **Note** 
+
+  - Probabilities are in percentange (%)
+
+
+
+#### Further info 
+
+
+
+The `predictor` _class_ accepts multiple parameters that includes :
+
+
+
+<table>
+
+<thead>
+
+<tr><th>Parameter       </th><th>Function                                              </th><th>Default  </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>include_position</td><td>Include team&#x27;s league ranking in making predictions     </td><td>False    </td></tr>
+
+<tr><td>log             </td><td>Log at api default log&#x27;s path                           </td><td>False    </td></tr>
+
+<tr><td>level           </td><td>Logging level                                           </td><td>0        </td></tr>
+
+<tr><td>filename        </td><td>Log to the filename specified                           </td><td>None     </td></tr>
+
+<tr><td>color           </td><td>Colorize the logs                                       </td><td>False    </td></tr>
+
+<tr><td>gui             </td><td>Run with some Graphical interface notifications (Termux)</td><td>False    </td></tr>
+
+<tr><td>api             </td><td>Run with api-server&#x27;s configurations                    </td><td>False    </td></tr>
+
+</tbody>
+
+</table>
+
+
+
+The two predictor's object (`predictorD`, `predictorL`) accepts two parameters i.e.
+
+* **teams** - Required
+
+* **net** - Source of team's data - Default `True` (Online)
+
+
+
+## Source of data
+
+
+
+Team performances are sourced from [Soccerway](https://int.soccerway.com) after retrieving the *uri* from [Google](https://www.google.com).
+
+
+
+> **Warning** Copyright related issues are liable to the user of this script!
+
+
+
+## Disclaimer
+
+
+
+This project aims to help *punters* and *bookmarkers* to make informed and well researched soccer-predictions. Nevertheless, it is important to specify that 100% accuracy does not exist and smartbetsAPI can't guarantee the accuracy of the predictions. It is therefore your responsibility to trust the information generated by smartbetsAPI after evaluating its reliability. As the [creator](https://github.com/Simatwa), I **CANNOT** be held responsible for any loss of capital that may occur during the use of this program.
+
+
+
+## Contributing and Support
+
+
+
+### Contributing
+
+
+
+Contributions are always welcome! <br>
+
+Please take a look at the [Contribution guidelines](CONTRIBUTING.md). <br>
+
+Feel free to open an [Issue](https://github.com/Simatwa/smartbetsAPI/issues) or to [Fork](https://github.com/Simatwa/smartbetsAPI/fork) this repo.
+
+
+
+### ToDo
+
+
+
+- [ ] Upgrade to Machine learning
+
+- [ ] Improve algorithim's accuracy
+
+- [ ] General code improvements
+
+- [ ] Fix bugs
+
+
+
+### Support 
+
+
+
+Consider donating to this project if you find it useful:
+
+<p align="center">
+
+<a href="https://www.paypal.com/donate/?hosted_button_id=KLNYKSGUXY8R2"><img src="https://img.shields.io/static/v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal"/></a>
+
+</p>
+
+
+
+## Credits
+
+
+
+- [x] [Soccerway](https://int.soccerway.com)
+
+- [x] [Google](https://www.google.com)
+
+- [x] [Python.org](https://python.org)
+
+
+
+## Special Thanks
+
+
+
+* [x] [victhepythonista](https://github.com/victhepythonista)
+
+* [x] YOU.
```

#### html2text {}

```diff
@@ -1,67 +1,83 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.0 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.1 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
-Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Description:
+Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
+Football,Predictions,Betting API,Soccer predictions,Football Predictions
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Console Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Customer Service Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Natural Language :: English Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic :: Games/
+Entertainment Description-Content-Type: text/markdown License-File: LICENSE
                           ****** smartbetsAPI ******
-[Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
-[Downloads]
+ [Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
+                                  [Downloads]
+
 > "Punter's choice" Worldwide soccer-matches predictor with a dedicated
 standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
 a package for intergrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script intergration (package) - Non-AI ##
 Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
 this script to be fruitful to you. - Installing through pip is always the most
-preferred way: ```sh $ pip install smartbetsAPI ``` - For those who like
-enjoying the **latest** releases from [Github](https://github.com) like [me]
-(https://github.com/Simatwa), rather than waiting for the next release: ```sh $
-pip install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
-guys with _trust issues_ are very much sorted this way: ```sh $ git clone
-https://github.com/Simatwa/smartbetsAPI.git $ cd smartbetsAPI $ bash install.sh
-#or $ sudo bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI `
-will fire up the [Flask](https://github.com/pallets/Flask) server with the
-following default configurations.
+preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
+the **latest** releases from [Github](https://github.com) like [me](https://
+github.com/Simatwa), rather than waiting for the next release: ```sh pip
+install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
+guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
+/github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
+up the [Flask](/pallets/Flask) server with the following default
+configurations.
                             Command         Default
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
 - For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-bet_at_api_level.py) that makes prediction using the `api`. ![api running]
-(https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif) >
-**Note** - Content-Type of the response (predictions) is `application/json` -
-Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found. *
-For more information you can run `smartbetsAPI -h` 2. Importing Package Module
-`predictor` provides two ways of interacting with it at the programming level,
-based on the `data-type` in which the teams have been packed and parsed to it:
-* Using `predictorL` object which accepts *teams* (**List** data-type). > For
-[example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-predict_using_list.py): ```py #!/usr/bin/env python3 from
-smartbets_API.predictor import predictor teams = [ "Napoli", # Home team (index
-[0]) "AC Milan", # Away team (index [1]) ] # Instantiating predictor predict =
-predictor() # Using predictorL object to handle teams (List data-type)
-predictions = predict.predictorL(teams) # Display info print(predictions)
-#Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0,
-'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using `predictorD` object
-which takes *teams* (**Dictionary** data-type): > For [example](https://
-github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py): ```py
+[simple program](examples/bet_at_api_level.py) that makes prediction using the
+`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
+response (predictions) is `application/json` - Reinstall with `sudo` privileges
+if `smartbetsAPI` command can't be found. > Example predicting using REST API
+```py from smartbets_API import predictor predict = predictor('http://
+localhost:8080','password') bets=predict.get_predictions
+('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
+14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
+'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
+Importing Package Module `predictor` provides two ways of interacting with it
+at the programming level, based on the `data-type` in which the teams have been
+packed and parsed to it: * Using `predictorL` object which accepts *teams*
+(**List** data-type). > For [example](examples/predict_using_list.py): ```py
 #!/usr/bin/env python3 from smartbets_API.predictor import predictor teams =
-{ 1: "Manchester City", # 1 for home-team 2: "Liverpool", # 2 for away-team } #
-Instantiating predictor predict = predictor() # Using predictorD object to
-handle teams (Dictionary data-type) predictions = predict.predictorD(teams) #
-Display info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0,
-'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` -
-The output initials are explained in the table below.
+[ "Napoli", # Home team (index [0]) "AC Milan", # Away team (index [1]) ] #
+Instantiating predictor predict = predictor() # Using predictorL object to
+handle teams (List data-type) predictions = predict.predictorL(teams) # Display
+info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25':
+40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using
+`predictorD` object which takes *teams* (**Dictionary** data-type): > For
+[example](examples/predict_using_dict.py): ```py #!/usr/bin/env python3 from
+smartbets_API.predictor import predictor teams = { 1: "Manchester City", # 1
+for home-team 2: "Liverpool", # 2 for away-team } # Instantiating predictor
+predict = predictor() # Using predictorD object to handle teams (Dictionary
+data-type) predictions = predict.predictorD(teams) # Display info print
+(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0,
+'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` - The output
+initials are explained in the table below.
 Parameter Function
 g         Goal-average of the two teams
 gg        Probability of both teams to score
 ov15      Probability of having more than 2 goals
 ov25      Probability of having more than 3 goals
 ov35      Probability of having more than 4 goals
 choice    Probability of the specified &#x27;result&#x27; to occur
@@ -99,23 +115,8 @@
 [ ] Upgrade to Machine learning - [ ] Improve algorithim's accuracy - [ ]
 General code improvements - [ ] Fix bugs ### Support Consider donating to this
 project if you find it useful:
                         [https://img.shields.io/static/
          v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal]
 ## Credits - [x] [Soccerway](https://int.soccerway.com) - [x] [Google](https://
 www.google.com) - [x] [Python.org](https://python.org) ## Special Thanks * [x]
-[victhepythonista](https://github.com/victhepythonista) * [x] YOU. [View
-updated version of this info.](https://simatwa.github.io/smartbetsAPI)
-Keywords: Football,Predictions,Betting API,Soccer predictions,Football
-Predictions Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Environment :: Console Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Customer Service Classifier:
-Intended Audience :: Other Audience Classifier: License :: OSI Approved :: GNU
-General Public License v3 (GPLv3) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Natural Language
-:: English Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Games/Entertainment Description-Content-Type:
-text/markdown
+[victhepythonista](https://github.com/victhepythonista) * [x] YOU.
```

### Comparing `smartbetsAPI-1.1.0/README.md` & `smartbetsAPI-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <h1 align="center">smartbetsAPI</h1>
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="https://github.com/Simatwa/smartbetsAPI/raw/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI/1.1.0/"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a><br>
+<p align="center">
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
  
  > "Punter's choice" 
 
  Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
 
  ## Features
  - REST-API
@@ -16,46 +17,46 @@
 
 1. Linux 
 
 *Python 3.7+* is required for this script to be fruitful to you. 
 - Installing through pip is always the most preferred way:
 
  ```sh
- $ pip  install smartbetsAPI
+ pip  install smartbetsAPI
  
  ```
 
  - For those who like enjoying the **latest** releases from [Github](https://github.com) like [me](https://github.com/Simatwa), rather than  waiting for the next release:
 
  ```sh
- $ pip install git+https://github.com/Simatwa/smartbetsAPI.git
+ pip install git+https://github.com/Simatwa/smartbetsAPI.git
 
  ```
 
 - The hard-core guys with _trust issues_ are very much sorted this way:
 
  ```sh
 
- $ git clone https://github.com/Simatwa/smartbetsAPI.git
+ git clone https://github.com/Simatwa/smartbetsAPI.git
 
- $ cd smartbetsAPI
+ cd smartbetsAPI
 
- $ bash install.sh 
+ bash install.sh 
 
    #or
 
-$ sudo bash install.sh
+sudo bash install.sh
 
 ```
 
 ### Usage
 
 1. Terminal
 
- Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](https://github.com/pallets/Flask) server with the following default configurations.
+ Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
 
 <table align="center"> 
 <thead>
 <tr><th>Command        </th><th>Default  </th></tr>
 </thead>
 <tbody>
 <tr><td>Port           </td><td>8000     </td></tr>
@@ -74,33 +75,44 @@
 - For instance :
 
  ```sh
  $ smartbetsAPI mypass9876
 
 ``` 
 
-Here is an example of a [simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/bet_at_api_level.py) that makes prediction using the `api`.
+Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
 
-![api running](https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif)
+![api running](assets/api_running.gif)
 
 
 > **Note** 
   - Content-Type of the response (predictions) is `application/json`
   - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
 
+> Example predicting using REST API
+
+```py
+from smartbets_API import predictor
+predict = predictor('http://localhost:8080','password')
+bets=predict.get_predictions('Arsenal','Manchester')
+print(bets)
+#Output
+#(True, {'choice': 55.56, 'g': 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15', 'result': '1'})
+```
+
 
 * For more information you can run `smartbetsAPI -h` 
 
 
 2. Importing Package
 
 Module `predictor`  provides two ways of interacting with it at the programming level, based on the `data-type` in which the teams have been packed and parsed to it:
 
 * Using `predictorL` object which accepts *teams* (**List** data-type).
-> For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_list.py):
+> For [example](examples/predict_using_list.py):
 
 ```py
 #!/usr/bin/env python3
 from smartbets_API.predictor import predictor
 
 teams = [
     "Napoli",  # Home team (index [0])
@@ -117,15 +129,15 @@
 
 #Output
 #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'}
 
 ```
 
 * Using `predictorD` object which takes *teams* (**Dictionary** data-type):
-> For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py):
+> For [example](examples/predict_using_dict.py):
 
 ```py
 #!/usr/bin/env python3
 from smartbets_API.predictor import predictor
 
 teams = {
     1: "Manchester City",  # 1 for home-team
@@ -228,9 +240,7 @@
 - [x] [Google](https://www.google.com)
 - [x] [Python.org](https://python.org)
 
 ## Special Thanks
 
 * [x] [victhepythonista](https://github.com/victhepythonista)
 * [x] YOU.
-
- [View updated version of this info.](https://simatwa.github.io/smartbetsAPI)
```

#### html2text {}

```diff
@@ -1,63 +1,66 @@
                           ****** smartbetsAPI ******
-[Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
-[Downloads]
+ [Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
+                                  [Downloads]
+
 > "Punter's choice" Worldwide soccer-matches predictor with a dedicated
 standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
 a package for intergrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script intergration (package) - Non-AI ##
 Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
 this script to be fruitful to you. - Installing through pip is always the most
-preferred way: ```sh $ pip install smartbetsAPI ``` - For those who like
-enjoying the **latest** releases from [Github](https://github.com) like [me]
-(https://github.com/Simatwa), rather than waiting for the next release: ```sh $
-pip install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
-guys with _trust issues_ are very much sorted this way: ```sh $ git clone
-https://github.com/Simatwa/smartbetsAPI.git $ cd smartbetsAPI $ bash install.sh
-#or $ sudo bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI `
-will fire up the [Flask](https://github.com/pallets/Flask) server with the
-following default configurations.
+preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
+the **latest** releases from [Github](https://github.com) like [me](https://
+github.com/Simatwa), rather than waiting for the next release: ```sh pip
+install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
+guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
+/github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
+up the [Flask](/pallets/Flask) server with the following default
+configurations.
                             Command         Default
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
 - For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-bet_at_api_level.py) that makes prediction using the `api`. ![api running]
-(https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif) >
-**Note** - Content-Type of the response (predictions) is `application/json` -
-Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found. *
-For more information you can run `smartbetsAPI -h` 2. Importing Package Module
-`predictor` provides two ways of interacting with it at the programming level,
-based on the `data-type` in which the teams have been packed and parsed to it:
-* Using `predictorL` object which accepts *teams* (**List** data-type). > For
-[example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-predict_using_list.py): ```py #!/usr/bin/env python3 from
-smartbets_API.predictor import predictor teams = [ "Napoli", # Home team (index
-[0]) "AC Milan", # Away team (index [1]) ] # Instantiating predictor predict =
-predictor() # Using predictorL object to handle teams (List data-type)
-predictions = predict.predictorL(teams) # Display info print(predictions)
-#Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0,
-'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using `predictorD` object
-which takes *teams* (**Dictionary** data-type): > For [example](https://
-github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py): ```py
+[simple program](examples/bet_at_api_level.py) that makes prediction using the
+`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
+response (predictions) is `application/json` - Reinstall with `sudo` privileges
+if `smartbetsAPI` command can't be found. > Example predicting using REST API
+```py from smartbets_API import predictor predict = predictor('http://
+localhost:8080','password') bets=predict.get_predictions
+('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
+14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
+'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
+Importing Package Module `predictor` provides two ways of interacting with it
+at the programming level, based on the `data-type` in which the teams have been
+packed and parsed to it: * Using `predictorL` object which accepts *teams*
+(**List** data-type). > For [example](examples/predict_using_list.py): ```py
 #!/usr/bin/env python3 from smartbets_API.predictor import predictor teams =
-{ 1: "Manchester City", # 1 for home-team 2: "Liverpool", # 2 for away-team } #
-Instantiating predictor predict = predictor() # Using predictorD object to
-handle teams (Dictionary data-type) predictions = predict.predictorD(teams) #
-Display info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0,
-'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` -
-The output initials are explained in the table below.
+[ "Napoli", # Home team (index [0]) "AC Milan", # Away team (index [1]) ] #
+Instantiating predictor predict = predictor() # Using predictorL object to
+handle teams (List data-type) predictions = predict.predictorL(teams) # Display
+info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25':
+40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using
+`predictorD` object which takes *teams* (**Dictionary** data-type): > For
+[example](examples/predict_using_dict.py): ```py #!/usr/bin/env python3 from
+smartbets_API.predictor import predictor teams = { 1: "Manchester City", # 1
+for home-team 2: "Liverpool", # 2 for away-team } # Instantiating predictor
+predict = predictor() # Using predictorD object to handle teams (Dictionary
+data-type) predictions = predict.predictorD(teams) # Display info print
+(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0,
+'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` - The output
+initials are explained in the table below.
 Parameter Function
 g         Goal-average of the two teams
 gg        Probability of both teams to score
 ov15      Probability of having more than 2 goals
 ov25      Probability of having more than 3 goals
 ov35      Probability of having more than 4 goals
 choice    Probability of the specified &#x27;result&#x27; to occur
@@ -95,9 +98,8 @@
 [ ] Upgrade to Machine learning - [ ] Improve algorithim's accuracy - [ ]
 General code improvements - [ ] Fix bugs ### Support Consider donating to this
 project if you find it useful:
                         [https://img.shields.io/static/
          v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal]
 ## Credits - [x] [Soccerway](https://int.soccerway.com) - [x] [Google](https://
 www.google.com) - [x] [Python.org](https://python.org) ## Special Thanks * [x]
-[victhepythonista](https://github.com/victhepythonista) * [x] YOU. [View
-updated version of this info.](https://simatwa.github.io/smartbetsAPI)
+[victhepythonista](https://github.com/victhepythonista) * [x] YOU.
```

### Comparing `smartbetsAPI-1.1.0/setup.py` & `smartbetsAPI-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,31 @@
         return file.readlines()
 
 
 setup(
     name="smartbetsAPI",
     packages=["smartbets_API"],
     version=__version__,
-    install_requires=get_file("requirements.txt"),
     url="https://github.com/Simatwa/smartbetsAPI",
     license="GPL-3.0",
     author=__author__,
     author_email="smartwacaleb@gmail.com",
     maintainer="Smartwa Caleb",
     maintainer_email="smartwacaleb@gmail.com",
     description="Simple football prediction API",
     long_description="\n".join(get_file("README.md")),
     long_description_content_type="text/markdown",
+    install_requires=[
+        "Flask>=2.2.2",
+        "appdirs==1.4.4",
+        "requests>=2.28.1",
+        "colorama>=0.4.6",
+        "bs4==0.0.1",
+        "Faker>=15.3.4",
+    ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `smartbetsAPI-1.1.0/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.1.1/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,491 +1,18 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
-Description: <h1 align="center">smartbetsAPI</h1>
-        
-         <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="https://github.com/Simatwa/smartbetsAPI/raw/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI/1.1.0/"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a><br>
-        
-         
-        
-         > "Punter's choice" 
-        
-        
-        
-         Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
-        
-        
-        
-         ## Features
-        
-         - REST-API
-        
-         - Script intergration (package)
-        
-         - Non-AI 
-        
-        
-        
-         ## Installation and usage
-        
-        
-        
-         ### Installation
-        
-        
-        
-        1. Linux 
-        
-        
-        
-        *Python 3.7+* is required for this script to be fruitful to you. 
-        
-        - Installing through pip is always the most preferred way:
-        
-        
-        
-         ```sh
-        
-         $ pip  install smartbetsAPI
-        
-         
-        
-         ```
-        
-        
-        
-         - For those who like enjoying the **latest** releases from [Github](https://github.com) like [me](https://github.com/Simatwa), rather than  waiting for the next release:
-        
-        
-        
-         ```sh
-        
-         $ pip install git+https://github.com/Simatwa/smartbetsAPI.git
-        
-        
-        
-         ```
-        
-        
-        
-        - The hard-core guys with _trust issues_ are very much sorted this way:
-        
-        
-        
-         ```sh
-        
-        
-        
-         $ git clone https://github.com/Simatwa/smartbetsAPI.git
-        
-        
-        
-         $ cd smartbetsAPI
-        
-        
-        
-         $ bash install.sh 
-        
-        
-        
-           #or
-        
-        
-        
-        $ sudo bash install.sh
-        
-        
-        
-        ```
-        
-        
-        
-        ### Usage
-        
-        
-        
-        1. Terminal
-        
-        
-        
-         Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](https://github.com/pallets/Flask) server with the following default configurations.
-        
-        
-        
-        <table align="center"> 
-        
-        <thead>
-        
-        <tr><th>Command        </th><th>Default  </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>Port           </td><td>8000     </td></tr>
-        
-        <tr><td>Username       </td><td>API</td></tr>
-        
-        <tr><td>Filename       </td><td>None     </td></tr>
-        
-        <tr><td>level (Logging)</td><td>20       </td></tr>
-        
-        <tr><td>host           </td><td>False    </td></tr>
-        
-        <tr><td>debug          </td><td>False    </td></tr>
-        
-        <tr><td>no-net         </td><td>False    </td></tr>
-        
-        <tr><td>log            </td><td>False    </td></tr>
-        
-        <tr><td>colorize       </td><td>False    </td></tr>
-        
-        <tr><td>gui (Termux)   </td><td>False    </td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        - For instance :
-        
-        
-        
-         ```sh
-        
-         $ smartbetsAPI mypass9876
-        
-        
-        
-        ``` 
-        
-        
-        
-        Here is an example of a [simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/bet_at_api_level.py) that makes prediction using the `api`.
-        
-        
-        
-        ![api running](https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif)
-        
-        
-        
-        
-        
-        > **Note** 
-        
-          - Content-Type of the response (predictions) is `application/json`
-        
-          - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
-        
-        
-        
-        
-        
-        * For more information you can run `smartbetsAPI -h` 
-        
-        
-        
-        
-        
-        2. Importing Package
-        
-        
-        
-        Module `predictor`  provides two ways of interacting with it at the programming level, based on the `data-type` in which the teams have been packed and parsed to it:
-        
-        
-        
-        * Using `predictorL` object which accepts *teams* (**List** data-type).
-        
-        > For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_list.py):
-        
-        
-        
-        ```py
-        
-        #!/usr/bin/env python3
-        
-        from smartbets_API.predictor import predictor
-        
-        
-        
-        teams = [
-        
-            "Napoli",  # Home team (index [0])
-        
-            "AC Milan",  # Away team (index [1])
-        
-        ]
-        
-        # Instantiating predictor
-        
-        predict = predictor()
-        
-        
-        
-        # Using predictorL object to handle teams (List data-type)
-        
-        predictions = predict.predictorL(teams)
-        
-        
-        
-        # Display info
-        
-        print(predictions)
-        
-        
-        
-        #Output
-        
-        #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'}
-        
-        
-        
-        ```
-        
-        
-        
-        * Using `predictorD` object which takes *teams* (**Dictionary** data-type):
-        
-        > For [example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py):
-        
-        
-        
-        ```py
-        
-        #!/usr/bin/env python3
-        
-        from smartbets_API.predictor import predictor
-        
-        
-        
-        teams = {
-        
-            1: "Manchester City",  # 1 for home-team
-        
-            2: "Liverpool",  # 2 for away-team
-        
-        }
-        
-        
-        
-        # Instantiating predictor
-        
-        predict = predictor()
-        
-        
-        
-        # Using predictorD object to handle teams (Dictionary data-type)
-        
-        predictions = predict.predictorD(teams)
-        
-        
-        
-        # Display info
-        
-        print(predictions)
-        
-        
-        
-        #Output
-        
-        #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'}
-        
-        
-        
-        ```
-        
-        
-        
-        - The output initials are explained in the table below.
-        
-        
-        
-        <table>
-        
-        <thead>
-        
-        <tr><th>Parameter  </th><th>Function                                                 </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>g          </td><td>Goal-average of the two teams                              </td></tr>
-        
-        <tr><td>gg         </td><td>Probability of both teams to score                         </td></tr>
-        
-        <tr><td>ov15       </td><td>Probability of having more than 2 goals                    </td></tr>
-        
-        <tr><td>ov25       </td><td>Probability of having more than 3 goals                    </td></tr>
-        
-        <tr><td>ov35       </td><td>Probability of having more than 4 goals                    </td></tr>
-        
-        <tr><td>choice     </td><td>Probability of the specified &#x27;result&#x27; to occur            </td></tr>
-        
-        <tr><td>result     </td><td>The most suitable outcome from [1,1x,x,2x,2]                  </td></tr>
-        
-        <tr><td>pick       </td><td>The most suitable outcome from [1,1x,x,2x,2,gg,ov15,ov25,ov35]</td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        > **Note** 
-        
-          - Probabilities are in percentange (%)
-        
-        
-        
-        #### Further info 
-        
-        
-        
-        The `predictor` _class_ accepts multiple parameters that includes :
-        
-        
-        
-        <table>
-        
-        <thead>
-        
-        <tr><th>Parameter       </th><th>Function                                              </th><th>Default  </th></tr>
-        
-        </thead>
-        
-        <tbody>
-        
-        <tr><td>include_position</td><td>Include team&#x27;s league ranking in making predictions     </td><td>False    </td></tr>
-        
-        <tr><td>log             </td><td>Log at api default log&#x27;s path                           </td><td>False    </td></tr>
-        
-        <tr><td>level           </td><td>Logging level                                           </td><td>0        </td></tr>
-        
-        <tr><td>filename        </td><td>Log to the filename specified                           </td><td>None     </td></tr>
-        
-        <tr><td>color           </td><td>Colorize the logs                                       </td><td>False    </td></tr>
-        
-        <tr><td>gui             </td><td>Run with some Graphical interface notifications (Termux)</td><td>False    </td></tr>
-        
-        <tr><td>api             </td><td>Run with api-server&#x27;s configurations                    </td><td>False    </td></tr>
-        
-        </tbody>
-        
-        </table>
-        
-        
-        
-        The two predictor's object (`predictorD`, `predictorL`) accepts two parameters i.e.
-        
-        * **teams** - Required
-        
-        * **net** - Source of team's data - Default `True` (Online)
-        
-        
-        
-        ## Source of data
-        
-        
-        
-        Team performances are sourced from [Soccerway](https://int.soccerway.com) after retrieving the *uri* from [Google](https://www.google.com).
-        
-        
-        
-        > **Warning** Copyright related issues are liable to the user of this script!
-        
-        
-        
-        ## Disclaimer
-        
-        
-        
-        This project aims to help *punters* and *bookmarkers* to make informed and well researched soccer-predictions. Nevertheless, it is important to specify that 100% accuracy does not exist and smartbetsAPI can't guarantee the accuracy of the predictions. It is therefore your responsibility to trust the information generated by smartbetsAPI after evaluating its reliability. As the [creator](https://github.com/Simatwa), I **CANNOT** be held responsible for any loss of capital that may occur during the use of this program.
-        
-        
-        
-        ## Contributing and Support
-        
-        
-        
-        ### Contributing
-        
-        
-        
-        Contributions are always welcome! <br>
-        
-        Please take a look at the [Contribution guidelines](CONTRIBUTING.md). <br>
-        
-        Feel free to open an [Issue](https://github.com/Simatwa/smartbetsAPI/issues) or to [Fork](https://github.com/Simatwa/smartbetsAPI/fork) this repo.
-        
-        
-        
-        ### ToDo
-        
-        
-        
-        - [ ] Upgrade to Machine learning
-        
-        - [ ] Improve algorithim's accuracy
-        
-        - [ ] General code improvements
-        
-        - [ ] Fix bugs
-        
-        
-        
-        ### Support 
-        
-        
-        
-        Consider donating to this project if you find it useful:
-        
-        <p align="center">
-        
-        <a href="https://www.paypal.com/donate/?hosted_button_id=KLNYKSGUXY8R2"><img src="https://img.shields.io/static/v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal"/></a>
-        
-        </p>
-        
-        
-        
-        ## Credits
-        
-        
-        
-        - [x] [Soccerway](https://int.soccerway.com)
-        
-        - [x] [Google](https://www.google.com)
-        
-        - [x] [Python.org](https://python.org)
-        
-        
-        
-        ## Special Thanks
-        
-        
-        
-        * [x] [victhepythonista](https://github.com/victhepythonista)
-        
-        * [x] YOU.
-        
-        
-        
-         [View updated version of this info.](https://simatwa.github.io/smartbetsAPI)
-        
 Keywords: Football,Predictions,Betting API,Soccer predictions,Football Predictions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -496,7 +23,500 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">smartbetsAPI</h1>
+
+<p align="center">
+
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+
+ 
+
+ > "Punter's choice" 
+
+
+
+ Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
+
+
+
+ ## Features
+
+ - REST-API
+
+ - Script intergration (package)
+
+ - Non-AI 
+
+
+
+ ## Installation and usage
+
+
+
+ ### Installation
+
+
+
+1. Linux 
+
+
+
+*Python 3.7+* is required for this script to be fruitful to you. 
+
+- Installing through pip is always the most preferred way:
+
+
+
+ ```sh
+
+ pip  install smartbetsAPI
+
+ 
+
+ ```
+
+
+
+ - For those who like enjoying the **latest** releases from [Github](https://github.com) like [me](https://github.com/Simatwa), rather than  waiting for the next release:
+
+
+
+ ```sh
+
+ pip install git+https://github.com/Simatwa/smartbetsAPI.git
+
+
+
+ ```
+
+
+
+- The hard-core guys with _trust issues_ are very much sorted this way:
+
+
+
+ ```sh
+
+
+
+ git clone https://github.com/Simatwa/smartbetsAPI.git
+
+
+
+ cd smartbetsAPI
+
+
+
+ bash install.sh 
+
+
+
+   #or
+
+
+
+sudo bash install.sh
+
+
+
+```
+
+
+
+### Usage
+
+
+
+1. Terminal
+
+
+
+ Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
+
+
+
+<table align="center"> 
+
+<thead>
+
+<tr><th>Command        </th><th>Default  </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>Port           </td><td>8000     </td></tr>
+
+<tr><td>Username       </td><td>API</td></tr>
+
+<tr><td>Filename       </td><td>None     </td></tr>
+
+<tr><td>level (Logging)</td><td>20       </td></tr>
+
+<tr><td>host           </td><td>False    </td></tr>
+
+<tr><td>debug          </td><td>False    </td></tr>
+
+<tr><td>no-net         </td><td>False    </td></tr>
+
+<tr><td>log            </td><td>False    </td></tr>
+
+<tr><td>colorize       </td><td>False    </td></tr>
+
+<tr><td>gui (Termux)   </td><td>False    </td></tr>
+
+</tbody>
+
+</table>
+
+
+
+- For instance :
+
+
+
+ ```sh
+
+ $ smartbetsAPI mypass9876
+
+
+
+``` 
+
+
+
+Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
+
+
+
+![api running](assets/api_running.gif)
+
+
+
+
+
+> **Note** 
+
+  - Content-Type of the response (predictions) is `application/json`
+
+  - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
+
+
+
+> Example predicting using REST API
+
+
+
+```py
+
+from smartbets_API import predictor
+
+predict = predictor('http://localhost:8080','password')
+
+bets=predict.get_predictions('Arsenal','Manchester')
+
+print(bets)
+
+#Output
+
+#(True, {'choice': 55.56, 'g': 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15', 'result': '1'})
+
+```
+
+
+
+
+
+* For more information you can run `smartbetsAPI -h` 
+
+
+
+
+
+2. Importing Package
+
+
+
+Module `predictor`  provides two ways of interacting with it at the programming level, based on the `data-type` in which the teams have been packed and parsed to it:
+
+
+
+* Using `predictorL` object which accepts *teams* (**List** data-type).
+
+> For [example](examples/predict_using_list.py):
+
+
+
+```py
+
+#!/usr/bin/env python3
+
+from smartbets_API.predictor import predictor
+
+
+
+teams = [
+
+    "Napoli",  # Home team (index [0])
+
+    "AC Milan",  # Away team (index [1])
+
+]
+
+# Instantiating predictor
+
+predict = predictor()
+
+
+
+# Using predictorL object to handle teams (List data-type)
+
+predictions = predict.predictorL(teams)
+
+
+
+# Display info
+
+print(predictions)
+
+
+
+#Output
+
+#{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'}
+
+
+
+```
+
+
+
+* Using `predictorD` object which takes *teams* (**Dictionary** data-type):
+
+> For [example](examples/predict_using_dict.py):
+
+
+
+```py
+
+#!/usr/bin/env python3
+
+from smartbets_API.predictor import predictor
+
+
+
+teams = {
+
+    1: "Manchester City",  # 1 for home-team
+
+    2: "Liverpool",  # 2 for away-team
+
+}
+
+
+
+# Instantiating predictor
+
+predict = predictor()
+
+
+
+# Using predictorD object to handle teams (Dictionary data-type)
+
+predictions = predict.predictorD(teams)
+
+
+
+# Display info
+
+print(predictions)
+
+
+
+#Output
+
+#{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'}
+
+
+
+```
+
+
+
+- The output initials are explained in the table below.
+
+
+
+<table>
+
+<thead>
+
+<tr><th>Parameter  </th><th>Function                                                 </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>g          </td><td>Goal-average of the two teams                              </td></tr>
+
+<tr><td>gg         </td><td>Probability of both teams to score                         </td></tr>
+
+<tr><td>ov15       </td><td>Probability of having more than 2 goals                    </td></tr>
+
+<tr><td>ov25       </td><td>Probability of having more than 3 goals                    </td></tr>
+
+<tr><td>ov35       </td><td>Probability of having more than 4 goals                    </td></tr>
+
+<tr><td>choice     </td><td>Probability of the specified &#x27;result&#x27; to occur            </td></tr>
+
+<tr><td>result     </td><td>The most suitable outcome from [1,1x,x,2x,2]                  </td></tr>
+
+<tr><td>pick       </td><td>The most suitable outcome from [1,1x,x,2x,2,gg,ov15,ov25,ov35]</td></tr>
+
+</tbody>
+
+</table>
+
+
+
+> **Note** 
+
+  - Probabilities are in percentange (%)
+
+
+
+#### Further info 
+
+
+
+The `predictor` _class_ accepts multiple parameters that includes :
+
+
+
+<table>
+
+<thead>
+
+<tr><th>Parameter       </th><th>Function                                              </th><th>Default  </th></tr>
+
+</thead>
+
+<tbody>
+
+<tr><td>include_position</td><td>Include team&#x27;s league ranking in making predictions     </td><td>False    </td></tr>
+
+<tr><td>log             </td><td>Log at api default log&#x27;s path                           </td><td>False    </td></tr>
+
+<tr><td>level           </td><td>Logging level                                           </td><td>0        </td></tr>
+
+<tr><td>filename        </td><td>Log to the filename specified                           </td><td>None     </td></tr>
+
+<tr><td>color           </td><td>Colorize the logs                                       </td><td>False    </td></tr>
+
+<tr><td>gui             </td><td>Run with some Graphical interface notifications (Termux)</td><td>False    </td></tr>
+
+<tr><td>api             </td><td>Run with api-server&#x27;s configurations                    </td><td>False    </td></tr>
+
+</tbody>
+
+</table>
+
+
+
+The two predictor's object (`predictorD`, `predictorL`) accepts two parameters i.e.
+
+* **teams** - Required
+
+* **net** - Source of team's data - Default `True` (Online)
+
+
+
+## Source of data
+
+
+
+Team performances are sourced from [Soccerway](https://int.soccerway.com) after retrieving the *uri* from [Google](https://www.google.com).
+
+
+
+> **Warning** Copyright related issues are liable to the user of this script!
+
+
+
+## Disclaimer
+
+
+
+This project aims to help *punters* and *bookmarkers* to make informed and well researched soccer-predictions. Nevertheless, it is important to specify that 100% accuracy does not exist and smartbetsAPI can't guarantee the accuracy of the predictions. It is therefore your responsibility to trust the information generated by smartbetsAPI after evaluating its reliability. As the [creator](https://github.com/Simatwa), I **CANNOT** be held responsible for any loss of capital that may occur during the use of this program.
+
+
+
+## Contributing and Support
+
+
+
+### Contributing
+
+
+
+Contributions are always welcome! <br>
+
+Please take a look at the [Contribution guidelines](CONTRIBUTING.md). <br>
+
+Feel free to open an [Issue](https://github.com/Simatwa/smartbetsAPI/issues) or to [Fork](https://github.com/Simatwa/smartbetsAPI/fork) this repo.
+
+
+
+### ToDo
+
+
+
+- [ ] Upgrade to Machine learning
+
+- [ ] Improve algorithim's accuracy
+
+- [ ] General code improvements
+
+- [ ] Fix bugs
+
+
+
+### Support 
+
+
+
+Consider donating to this project if you find it useful:
+
+<p align="center">
+
+<a href="https://www.paypal.com/donate/?hosted_button_id=KLNYKSGUXY8R2"><img src="https://img.shields.io/static/v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal"/></a>
+
+</p>
+
+
+
+## Credits
+
+
+
+- [x] [Soccerway](https://int.soccerway.com)
+
+- [x] [Google](https://www.google.com)
+
+- [x] [Python.org](https://python.org)
+
+
+
+## Special Thanks
+
+
+
+* [x] [victhepythonista](https://github.com/victhepythonista)
+
+* [x] YOU.
```

#### html2text {}

```diff
@@ -1,67 +1,83 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.0 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.1 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
-Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Description:
+Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
+Football,Predictions,Betting API,Soccer predictions,Football Predictions
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Console Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Customer Service Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Natural Language :: English Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic :: Games/
+Entertainment Description-Content-Type: text/markdown License-File: LICENSE
                           ****** smartbetsAPI ******
-[Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
-[Downloads]
+ [Github] [License] [PyPi] [Black] [Accuracy] [Passing] [coverage] [Progress]
+                                  [Downloads]
+
 > "Punter's choice" Worldwide soccer-matches predictor with a dedicated
 standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
 a package for intergrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script intergration (package) - Non-AI ##
 Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
 this script to be fruitful to you. - Installing through pip is always the most
-preferred way: ```sh $ pip install smartbetsAPI ``` - For those who like
-enjoying the **latest** releases from [Github](https://github.com) like [me]
-(https://github.com/Simatwa), rather than waiting for the next release: ```sh $
-pip install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
-guys with _trust issues_ are very much sorted this way: ```sh $ git clone
-https://github.com/Simatwa/smartbetsAPI.git $ cd smartbetsAPI $ bash install.sh
-#or $ sudo bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI `
-will fire up the [Flask](https://github.com/pallets/Flask) server with the
-following default configurations.
+preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
+the **latest** releases from [Github](https://github.com) like [me](https://
+github.com/Simatwa), rather than waiting for the next release: ```sh pip
+install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
+guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
+/github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
+up the [Flask](/pallets/Flask) server with the following default
+configurations.
                             Command         Default
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
 - For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-bet_at_api_level.py) that makes prediction using the `api`. ![api running]
-(https://github.com/Simatwa/smartbetsAPI/raw/main/assets/api_running.gif) >
-**Note** - Content-Type of the response (predictions) is `application/json` -
-Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found. *
-For more information you can run `smartbetsAPI -h` 2. Importing Package Module
-`predictor` provides two ways of interacting with it at the programming level,
-based on the `data-type` in which the teams have been packed and parsed to it:
-* Using `predictorL` object which accepts *teams* (**List** data-type). > For
-[example](https://github.com/Simatwa/smartbetsAPI/raw/main/examples/
-predict_using_list.py): ```py #!/usr/bin/env python3 from
-smartbets_API.predictor import predictor teams = [ "Napoli", # Home team (index
-[0]) "AC Milan", # Away team (index [1]) ] # Instantiating predictor predict =
-predictor() # Using predictorL object to handle teams (List data-type)
-predictions = predict.predictorL(teams) # Display info print(predictions)
-#Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25': 40.0, 'ov35': 30.0,
-'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using `predictorD` object
-which takes *teams* (**Dictionary** data-type): > For [example](https://
-github.com/Simatwa/smartbetsAPI/raw/main/examples/predict_using_dict.py): ```py
+[simple program](examples/bet_at_api_level.py) that makes prediction using the
+`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
+response (predictions) is `application/json` - Reinstall with `sudo` privileges
+if `smartbetsAPI` command can't be found. > Example predicting using REST API
+```py from smartbets_API import predictor predict = predictor('http://
+localhost:8080','password') bets=predict.get_predictions
+('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
+14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
+'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
+Importing Package Module `predictor` provides two ways of interacting with it
+at the programming level, based on the `data-type` in which the teams have been
+packed and parsed to it: * Using `predictorL` object which accepts *teams*
+(**List** data-type). > For [example](examples/predict_using_list.py): ```py
 #!/usr/bin/env python3 from smartbets_API.predictor import predictor teams =
-{ 1: "Manchester City", # 1 for home-team 2: "Liverpool", # 2 for away-team } #
-Instantiating predictor predict = predictor() # Using predictorD object to
-handle teams (Dictionary data-type) predictions = predict.predictorD(teams) #
-Display info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0,
-'ov25': 45.0, 'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` -
-The output initials are explained in the table below.
+[ "Napoli", # Home team (index [0]) "AC Milan", # Away team (index [1]) ] #
+Instantiating predictor predict = predictor() # Using predictorL object to
+handle teams (List data-type) predictions = predict.predictorL(teams) # Display
+info print(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 70.0, 'ov25':
+40.0, 'ov35': 30.0, 'choice': 60.0, 'result': '2', 'pick': 'ov15'} ``` * Using
+`predictorD` object which takes *teams* (**Dictionary** data-type): > For
+[example](examples/predict_using_dict.py): ```py #!/usr/bin/env python3 from
+smartbets_API.predictor import predictor teams = { 1: "Manchester City", # 1
+for home-team 2: "Liverpool", # 2 for away-team } # Instantiating predictor
+predict = predictor() # Using predictorD object to handle teams (Dictionary
+data-type) predictions = predict.predictorD(teams) # Display info print
+(predictions) #Output #{'g': 8.0, 'gg': 65.0, 'ov15': 60.0, 'ov25': 45.0,
+'ov35': 30.0, 'choice': 56.16, 'result': '1', 'pick': 'gg'} ``` - The output
+initials are explained in the table below.
 Parameter Function
 g         Goal-average of the two teams
 gg        Probability of both teams to score
 ov15      Probability of having more than 2 goals
 ov25      Probability of having more than 3 goals
 ov35      Probability of having more than 4 goals
 choice    Probability of the specified &#x27;result&#x27; to occur
@@ -99,23 +115,8 @@
 [ ] Upgrade to Machine learning - [ ] Improve algorithim's accuracy - [ ]
 General code improvements - [ ] Fix bugs ### Support Consider donating to this
 project if you find it useful:
                         [https://img.shields.io/static/
          v1?logo=paypal&message=Donate&color=blueviolet&label=Paypal]
 ## Credits - [x] [Soccerway](https://int.soccerway.com) - [x] [Google](https://
 www.google.com) - [x] [Python.org](https://python.org) ## Special Thanks * [x]
-[victhepythonista](https://github.com/victhepythonista) * [x] YOU. [View
-updated version of this info.](https://simatwa.github.io/smartbetsAPI)
-Keywords: Football,Predictions,Betting API,Soccer predictions,Football
-Predictions Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Environment :: Console Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Customer Service Classifier:
-Intended Audience :: Other Audience Classifier: License :: OSI Approved :: GNU
-General Public License v3 (GPLv3) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Natural Language
-:: English Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Games/Entertainment Description-Content-Type:
-text/markdown
+[victhepythonista](https://github.com/victhepythonista) * [x] YOU.
```

### Comparing `smartbetsAPI-1.1.0/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.1.1/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+LICENSE
 README.md
 setup.py
 smartbetsAPI.egg-info/PKG-INFO
 smartbetsAPI.egg-info/SOURCES.txt
 smartbetsAPI.egg-info/dependency_links.txt
 smartbetsAPI.egg-info/entry_points.txt
 smartbetsAPI.egg-info/requires.txt
 smartbetsAPI.egg-info/top_level.txt
 smartbets_API/__init__.py
+smartbets_API/__main__.py
 smartbets_API/bet_analyzer.py
+smartbets_API/bet_at_api_level.py
 smartbets_API/bet_common.py
 smartbets_API/configuration_handler.py
 smartbets_API/figure_harvester.py
 smartbets_API/googler.py
 smartbets_API/html_fetcher.py
 smartbets_API/interface.py
 smartbets_API/predictor.py
+smartbets_API/proxyh.py
 smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.1.0/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.1.1/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.0/smartbets_API/bet_common.py` & `smartbetsAPI-1.1.1/smartbets_API/bet_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from bs4 import BeautifulSoup as bts
 from .configuration_handler import dbnm, root
 from random import randint
 import logging as log
 import colorama as col
 import threading as thr
 import colorama as col
+from appdirs import AppDirs
 
 version = 1.1
 config = {}
 env = {"api": False}
 now, ht = datetime.datetime.today(), "text/"
 timeNow = now.strftime("%H:%M:%S")
 timeStamp = now.strftime("%d_%b_%Y-%H_%M_%S.")
 tablee = now.strftime("%b_%d_%Y")
 tbe = "Bet_" + tablee
 predictionTb = "Prediction_" + tablee
 developer = "Smartwa"
 root_image = os.getcwd() + "static/image/"
 logo = root_image + "logo.jpg"
 predbets_img = root_image + "predbets.png"
+dirs = AppDirs("Smartwa", "smartbets_API").user_data_dir
+config_filepath=os.path.join(dirs,'configurations.json')
 
 
 # Runs system cmds at API level
 def get_output(command):
     success = False
     try:
         output = subprocess.check_output(command, stderr=subprocess.STDOUT).decode()
@@ -288,28 +291,26 @@
     except:
         pass
 
 
 # Updates configurations parsed
 class booter:
     def __init__(self):
-        self.target = ["log", "color", "filename", "gui", "level"]
+        self.target = ["log", "color", "filename", "gui", "level", "proxy"]
 
     def get_info(self):
-        info = queryDb(f'SELECT {",".join(self.target)} FROM Booter WHERE ID=1')[0]
-        for x in range(len(self.target)):
-            if str(info[x]).lower() in ("false", "0", "none"):
-                config[self.target[x]] = False
-            else:
-                config[self.target[x]] = info[x]
-
+        from json import load
+        try:
+            with open(config_filepath) as fh:
+                config.update(load(fh))
+        except Exception as e:
+            exit('Failed to load configurations - '+config_filepath+' '+str(e))
 
 booter().get_info()
 
-
 # Logging configurations
 def log_level():
     tg = int(config["level"])
     return tg if tg > 0 else 60
 
 
 if config.get("log"):
```

### Comparing `smartbetsAPI-1.1.0/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.1.1/smartbets_API/configuration_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import sqlite3
 import subprocess
 from sys import exit, prefix
 import colorama as col
+from appdirs import AppDirs
+from json import dumps
+dirs = AppDirs("Smartwa", "smartbets_API").user_data_dir
 
 
 def get_output(command):
     success = False
     try:
         output = subprocess.check_output(command, stderr=subprocess.STDOUT).decode()
         success = True
@@ -15,18 +18,15 @@
     except Exception as e:
         # check_call can raise other exceptions, such as FileNotFoundError
         output = str(e)
     return (success, output)
 
 
 def createDir():
-    from appdirs import AppDirs
-
-    dirs = AppDirs("Smartwa", "smartbets_API")
-    root = dirs.user_data_dir + "/"
+    root = dirs + "/"
     try:
         if not os.path.isdir(root):
             os.makedirs(root)
     except PermissionError:
         exit(col.Fore.RED + "[*] Run with Sudo PERMISSION!" + col.Fore.RESET)
     except Exception as e:
         pass
@@ -123,29 +123,24 @@
             conn.close()
         except Exception as e:
             pass
 
 
 class set_config:
     def __init__(self, args):
-        self.args = args
-        self.target = ["log", "color", "filename", "gui", "level"]
-        self.db = database()
+        self.target = ["log", "color", "filename", "gui", "level", "proxy"]
+        self.values = [args.log, args.color, args.filename, args.gui, args.level, args.proxy]
+        self.config_filepath=os.path.join(dirs,'configurations.json')
 
     # Creates db initially
     def createTable(self):
         self.db.queryDb("DROP TABLE Booter")
         run = f"""CREATE TABLE IF NOT EXISTS Booter(ID INTEGER PRIMARY 
-		KEY AUTOINCREMENT, log TEXT, Color TEXT, Filename TEXT, Gui TEXT, Level INTEGER)"""
+		KEY AUTOINCREMENT, log TEXT, Color TEXT, Filename TEXT, Gui TEXT, Level INTEGER, Proxy TEXT)"""
         self.db.queryDb(run)
 
     def main(self):
-        self.createTable()
-        log = self.args.log if self.args.log else False
-        color = self.args.color if self.args.color else False
-        filename = self.args.filename if self.args.filename else False
-        gui = self.args.gui if self.args.gui else False
-        level = self.args.level
-        self.db.queryDb(
-            f"""INSERT INTO Booter(log,color,filename,gui,level)
-		VALUES('{log}','{color}','{filename}','{gui}','{level}')"""
-        )
+        try:
+            with open(self.config_filepath,'w') as fh:
+                fh.write(dumps(dict(zip(self.target,self.values))))
+        except Exception as e:
+            exit(print(f'[*] Failed to save configurations - {self.config_filepath} - {e}'))
```

### Comparing `smartbetsAPI-1.1.0/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.1.1/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.0/smartbets_API/googler.py` & `smartbetsAPI-1.1.1/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.0/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.1.1/smartbets_API/html_fetcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from .bet_common import *
 import requests as req
 import random as rand
 from faker import Faker
+from .proxyh import hunter45
 
 
 class web:
     def __init__(self):
         self.used, self.exc, self.user_agent, self.ref = [], [], [], []
+        self.hunter = hunter45(req)
+        pr = self.hunter.get_proxy() 
+        if pr[0]:
+            self.proxies = pr[1]
+        else:
+            logging.error(pr[1])
+            self.proxies = [] 
 
     def sampl(self):
         etc = [
             "int",
             "ke",
             "us",
             "ca",
@@ -94,53 +102,74 @@
             "Connection": "Keep-Alive",
             "User-Agent": userA,
             "Sec-Fetch-Site": setchF,
             "Sec-Fetch-Mode": "navigate",
             "Sec-Fetch-Dest": "document",
         }
         return content
+    
+    def get_proxy(self,code:int=429) -> dict:
+        """Hunts down proxies"""
+        proxy = None
+        if not config.get('proxy'):
+            return proxy
+        if code == 429 or code == 403:
+            pr = self.hunter.sample(self.proxies)
+            if pr[0]:
+                proxy = pr[1]
+                logging.info('Loading new proxy - '+proxy['https'])
+                logging.debug(f'Proxy assigned - {proxy}')
+            else:
+                logging.error(pr[1])
+        return proxy
 
     # Getting html from web
-    def sender(self, link, info="Requesting", g=0, head=0):
+    def sender(self, link, info="Requesting", g=0, head=0,proxy=None):
         ht = "http"
         if ht in link:
             url = link
         else:
             url = "https://" + link
         try:
             logging.info(f"{info} - {url}")
-            resp = req.get(url=url, headers=self.header())
+            params= {'url':url, 'headers':self.header(),'timeout':15}
+            if proxy:
+                params['proxies']=proxy
+            resp = req.get(**params)
+        except TimeoutError:
+            return (self.sender,info,g,head,self.get_proxy())
         except Exception as e:
             if len(self.exc) > 1:
                 return "0"
             logging.error(str(e))
             self.exc.append("1")
-            return self.sender(url, "Retrying")
+            return self.sender(url, "Retrying",proxy=self.get_proxy())
         else:
             self.ref.insert(0, url)
             self.status(resp.status_code, resp.reason)
             try:
                 content = resp.text
             except:
                 pass
             finally:
                 code = resp.status_code
                 g += 1
                 if not code == 200:
+                    proxy = self.get_proxy(code)
                     self.user_agent.clear()
                     gui.toast(f"Http-code {code}", b="red", c="lime")
                     logging.debug(f"{g}s of SLEEP")
                     time.sleep(g)
-                    return self.sender(self.repair(url), "Retrying", g, 1)
+                    return self.sender(self.repair(url), "Retrying", g, 1,proxy)
                 if "access denied" in soupHtml(content).lower():
                     logging.warning("ACCESS DENIED".center(37))
                     self.user_agent.clear()
                     logging.warning(f"{g}s of SLEEP")
                     time.sleep(g)
-                    return self.sender(self.repair(url), "Retrying", g, 1)
+                    return self.sender(self.repair(url), "Retrying", g, 1,proxy)
                 nm = filter(link, "html")
                 queryDb(f"DELETE FROM html where F_name='{nm}' ")
                 insertDb("Html", "F_name", "File", nm, content)
                 return self.launcher(link)
 
     # Query link's contents from db
     def launcher(self, link):
```

### Comparing `smartbetsAPI-1.1.0/smartbets_API/interface.py` & `smartbetsAPI-1.1.1/smartbets_API/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,22 @@
         help="Logging level",
         choices=[0, 10, 20, 30, 40, 50],
         type=int,
         default=20,
         metavar="0-50",
     )
     parser.add_argument(
+        "--enable-proxy",
+        dest='proxy',
+        action='store_true',
+        help="Access internet via rotating proxies",
+    )
+    parser.add_argument(
         "--no-net",
         action="store_true",
-        dest="no_net",
         help="Force the API to use cached data rather than from internet.",
     )
     parser.add_argument("--host", help="Host the API on net [LAN]", action="store_true")
     parser.add_argument(
         "--debug", help="Debug the API at web level - developers", action="store_true"
     )
     parser.add_argument(
@@ -195,15 +200,15 @@
         return error("Wrong credentials!"), 400
 
 
 def start_server():
     try:
         if args.host:
             app.run(host="0.0.0.0", port=args.port, debug=args.debug, threaded=True)
-        else:
+        else: 
             app.run(port=args.port, debug=args.debug)
     except (KeyboardInterrupt, EOFError):
         from sys import exit
 
         print(col.Fore.RED + "[*] Goodbye !" + col.Fore.RESET)
         exit(logging.critical("KeyboardInterrupt"))
     except Exception as e:
```

### Comparing `smartbetsAPI-1.1.0/smartbets_API/predictor.py` & `smartbetsAPI-1.1.1/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.0/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.1.1/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

