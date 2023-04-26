# Comparing `tmp/lifescale-utils-0.0.5.tar.gz` & `tmp/lifescale-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifescale-utils-0.0.5.tar", last modified: Tue Jan 31 21:06:02 2023, max compression
+gzip compressed data, was "lifescale-utils-0.0.6.tar", last modified: Wed Apr 26 20:35:30 2023, max compression
```

## Comparing `lifescale-utils-0.0.5.tar` & `lifescale-utils-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.803218 lifescale-utils-0.0.5/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2020-07-16 17:28:33.000000 lifescale-utils-0.0.5/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-01-31 21:04:18.000000 lifescale-utils-0.0.5/MANIFEST.in
--rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-01-31 21:06:02.803218 lifescale-utils-0.0.5/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2331 2022-12-30 08:58:48.000000 lifescale-utils-0.0.5/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.799218 lifescale-utils-0.0.5/lifescale/
--rw-rw-r--   0 heller    (1000) heller    (1000)      961 2023-01-31 20:55:39.000000 lifescale-utils-0.0.5/lifescale/__init__.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.799218 lifescale-utils-0.0.5/lifescale/command_line/
--rw-rw-r--   0 heller    (1000) heller    (1000)      723 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/command_line/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4451 2023-01-21 16:58:52.000000 lifescale-utils-0.0.5/lifescale/command_line/command_line.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.799218 lifescale-utils-0.0.5/lifescale/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    18865 2023-01-31 20:29:48.000000 lifescale-utils-0.0.5/lifescale/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12101 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/gui/MainWindow_old.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      718 2023-01-21 16:42:41.000000 lifescale-utils-0.0.5/lifescale/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    43364 2023-01-31 20:29:48.000000 lifescale-utils-0.0.5/lifescale/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    24260 2023-01-31 20:52:01.000000 lifescale-utils-0.0.5/lifescale/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5898 2023-01-31 12:40:21.000000 lifescale-utils-0.0.5/lifescale/gui/masses_model.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4958 2023-01-22 16:31:40.000000 lifescale-utils-0.0.5/lifescale/gui/panel_metadata_model.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6335 2023-01-31 14:49:20.000000 lifescale-utils-0.0.5/lifescale/gui/sample_summary_model.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.799218 lifescale-utils-0.0.5/lifescale/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    28845 2023-01-31 18:04:59.000000 lifescale-utils-0.0.5/lifescale/models/ls_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1692 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/models/ls_run.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.803218 lifescale-utils-0.0.5/lifescale/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1170 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/scripts/ls2csv.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      264 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/lifescale/scripts/run_gui.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-01-31 21:06:02.803218 lifescale-utils-0.0.5/lifescale_utils.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)      839 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      120 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       38 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       10 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-01-31 21:06:02.000000 lifescale-utils-0.0.5/lifescale_utils.egg-info/zip-safe
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-12-30 08:49:47.000000 lifescale-utils-0.0.5/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)      836 2023-01-31 21:06:02.803218 lifescale-utils-0.0.5/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2020-07-16 17:28:33.000000 lifescale-utils-0.0.6/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/MANIFEST.in
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2331 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1002 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/__init__.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/command_line/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      723 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/command_line/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4451 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/command_line/command_line.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18823 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      718 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    43282 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    24410 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5898 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/masses_model.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4958 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/panel_metadata_model.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    30974 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/resources.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6323 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/sample_summary_model.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    28693 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/models/ls_data.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1170 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/ls2csv.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      264 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/run_gui.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/lifescale_utils.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)      807 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)      120 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       38 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       10 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/zip-safe
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      836 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/setup.cfg
```

### Comparing `lifescale-utils-0.0.5/LICENSE` & `lifescale-utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/PKG-INFO` & `lifescale-utils-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifescale-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lifescale utility software.
 Home-page: https://gitlab.com/hellerdev/lifescale_utils
 Author: Andreas Hellerschmied
 Author-email: heller182@gmx.at
 License: GNU GPLv3
 Keywords: Lifescale
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `lifescale-utils-0.0.5/README.md` & `lifescale-utils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/__init__.py` & `lifescale-utils-0.0.6/lifescale/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (heller182@gmx.at)
 """
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 __author__ = 'Andreas Hellerschmied'
-__git_repo__ = 'tba'
+__git_repo__ = 'https://gitlab.com/hellerdev/lifescale_utils'
 __email__ = 'heller182@gmx.at'
 __copyright__ = '(c) 2023 Andreas Hellerschmied'
 __pypi_repo__ = 'https://pypi.org/project/lifescale-utils/'
```

### Comparing `lifescale-utils-0.0.5/lifescale/command_line/__init__.py` & `lifescale-utils-0.0.6/lifescale/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/command_line/command_line.py` & `lifescale-utils-0.0.6/lifescale/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/gui/MainWindow.py` & `lifescale-utils-0.0.6/lifescale/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,18 +131,18 @@
         self.label_iqr = QtWidgets.QLabel(self.groupBoxLSDataSampleStatistics)
         self.label_iqr.setText("")
         self.label_iqr.setObjectName("label_iqr")
         self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.label_iqr)
         self.label_13 = QtWidgets.QLabel(self.groupBoxLSDataSampleStatistics)
         self.label_13.setObjectName("label_13")
         self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_13)
-        self.label_median_iqr = QtWidgets.QLabel(self.groupBoxLSDataSampleStatistics)
-        self.label_median_iqr.setText("")
-        self.label_median_iqr.setObjectName("label_median_iqr")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.label_median_iqr)
+        self.label_rcv = QtWidgets.QLabel(self.groupBoxLSDataSampleStatistics)
+        self.label_rcv.setText("")
+        self.label_rcv.setObjectName("label_rcv")
+        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.label_rcv)
         self.horizontalLayout.addLayout(self.formLayout)
         self.horizontalLayout_2.addWidget(self.groupBoxLSDataSampleStatistics)
         self.groupBox_histOptions = QtWidgets.QGroupBox(self.tab_LSData_hist)
         self.groupBox_histOptions.setObjectName("groupBox_histOptions")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.groupBox_histOptions)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.formLayout_2 = QtWidgets.QFormLayout()
@@ -254,15 +254,15 @@
         self.groupBoxLSDataSampleStatistics.setTitle(_translate("MainWindow", "Sample statistics (current selection)"))
         self.label.setText(_translate("MainWindow", "Selected masses"))
         self.label_3.setText(_translate("MainWindow", "Selection limits"))
         self.label_5.setText(_translate("MainWindow", "Mean"))
         self.label_7.setText(_translate("MainWindow", "Median"))
         self.label_9.setText(_translate("MainWindow", "Std"))
         self.label_11.setText(_translate("MainWindow", "IQR"))
-        self.label_13.setText(_translate("MainWindow", "Median/IQR"))
+        self.label_13.setText(_translate("MainWindow", "rCV"))
         self.groupBox_histOptions.setTitle(_translate("MainWindow", "Histogram options"))
         self.label_2.setText(_translate("MainWindow", "Bin determination method"))
         self.label_numberOfBins.setText(_translate("MainWindow", "Number of bins"))
         self.checkBox_plotMedian.setText(_translate("MainWindow", "Plot median"))
         self.checkBox_plotMean.setText(_translate("MainWindow", "Plot mean"))
         self.tabWidget_LSData.setTabText(self.tabWidget_LSData.indexOf(self.tab_LSData_hist), _translate("MainWindow", "Sample histogram and statistics"))
         self.tabWidget_LSData.setTabText(self.tabWidget_LSData.indexOf(self.tab_Masses), _translate("MainWindow", "Masses per Sample"))
```

### Comparing `lifescale-utils-0.0.5/lifescale/gui/__init__.py` & `lifescale-utils-0.0.6/lifescale/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/gui/dialog_about.py` & `lifescale-utils-0.0.6/lifescale/gui/dialog_about.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,30 +66,28 @@
         self.label_author.setObjectName("label_author")
         self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.label_author)
         self.verticalLayout_3.addLayout(self.formLayout)
         spacerItem = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         self.verticalLayout_3.addItem(spacerItem)
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.label = QtWidgets.QLabel(Dialog_about)
-        self.label.setText("")
-        self.label.setPixmap(QtGui.QPixmap("lifescale/gui/../../../GravTools/gravtools/gui/BEV-Logo 230px breit.png"))
-        self.label.setScaledContents(False)
-        self.label.setObjectName("label")
-        self.horizontalLayout.addWidget(self.label)
         self.label_4 = QtWidgets.QLabel(Dialog_about)
         self.label_4.setWordWrap(True)
         self.label_4.setOpenExternalLinks(True)
         self.label_4.setObjectName("label_4")
         self.horizontalLayout.addWidget(self.label_4)
-        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout.addItem(spacerItem1)
+        self.label = QtWidgets.QLabel(Dialog_about)
+        self.label.setText("")
+        self.label.setPixmap(QtGui.QPixmap(":/logos/logos/Uni_Logo_2016_SW_230px-wide.jpg"))
+        self.label.setScaledContents(False)
+        self.label.setObjectName("label")
+        self.horizontalLayout.addWidget(self.label)
         self.verticalLayout_3.addLayout(self.horizontalLayout)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
-        self.verticalLayout_3.addItem(spacerItem2)
+        spacerItem1 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
+        self.verticalLayout_3.addItem(spacerItem1)
         self.groupBox = QtWidgets.QGroupBox(Dialog_about)
         self.groupBox.setObjectName("groupBox")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.groupBox)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.verticalLayout = QtWidgets.QVBoxLayout()
         self.verticalLayout.setObjectName("verticalLayout")
         self.label_3 = QtWidgets.QLabel(self.groupBox)
@@ -127,15 +125,15 @@
         self.label_copyright.setText(_translate("Dialog_about", "copyright"))
         self.label_9.setText(_translate("Dialog_about", "Git repository:"))
         self.label_git_repo.setText(_translate("Dialog_about", "git_repo"))
         self.label_5.setText(_translate("Dialog_about", "pypi.org repository:"))
         self.label_pypi_repo.setText(_translate("Dialog_about", "pypi_repo"))
         self.label_10.setText(_translate("Dialog_about", "Author:"))
         self.label_author.setText(_translate("Dialog_about", "author"))
-        self.label_4.setText(_translate("Dialog_about", "GravTools was developed as an open source software at the <a href=\"https://www.bev.gv.at/\">Austrian Federal Office of Metrology and Surveying (BEV)</a>."))
+        self.label_4.setText(_translate("Dialog_about", "<html><head/><body><p>LifeScale utils was funded by the <a href=\"https://cmess.univie.ac.at/\"><span style=\" text-decoration: underline; color:#0000ff;\">Centre for Microbiology and Environmental Systems Science (CMESS) of the University of Vienna</span></a>.</p></body></html>"))
         self.groupBox.setTitle(_translate("Dialog_about", "License"))
         self.label_3.setText(_translate("Dialog_about", "<html><head/><body><p>LifeScale utils is licensed under the <a href=\"https://www.gnu.org/licenses/gpl-3.0.de.html\"><span style=\" text-decoration: underline; color:#0000ff;\">GNU General Public License 3</span></a>.</p></body></html>"))
         self.plainTextEdit.setPlainText(_translate("Dialog_about", " GNU GENERAL PUBLIC LICENSE\n"
 "                       Version 3, 29 June 2007\n"
 "\n"
 " Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>\n"
 " Everyone is permitted to copy and distribute verbatim copies\n"
```

### Comparing `lifescale-utils-0.0.5/lifescale/gui/gui_main.py` & `lifescale-utils-0.0.6/lifescale/gui/gui_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from lifescale.gui.MainWindow import Ui_MainWindow
 from lifescale.gui.dialog_about import Ui_Dialog_about
 from lifescale.models.ls_data import LSData
 from lifescale.gui.panel_metadata_model import PanelMetadataModel
 from lifescale.gui.sample_summary_model import SampleSummaryModel
 from lifescale.gui.masses_model import MassesModel
+from lifescale.gui import resources
 from lifescale import __version__, __author__, __git_repo__, __email__, __copyright__, __pypi_repo__
 
 # https://numpy.org/doc/stable/reference/generated/numpy.histogram_bin_edges.html#numpy.histogram_bin_edges
 NUMPY_HISTOGRAM_BIN_EDGES_OPTIONS = {
     'auto': 'Maximum of the ‘sturges’ and ‘fd’ estimators. Provides good all around performance.',
     'fd': 'Freedman Diaconis Estimator: Robust (resilient to outliers) estimator that takes into account data variability and data size.',
     'doane': 'An improved version of Sturges’ estimator that works better with non-normal datasets.',
@@ -60,14 +61,16 @@
         self.action_About.triggered.connect(self.on_menu_help_about)
         self.action_csvFiles.triggered.connect(self.on_action_csvFiles)
         self.listWidget_Samples.itemSelectionChanged.connect(self.on_selection_changed_sample_list)
         self.checkBox_MassesShowTable.stateChanged.connect(self.on_checkBox_MassesShowTable_stateChanged)
         self.comboBox_histMethod.currentIndexChanged.connect(self.on_histogram_bin_method_currentIndexChanged)
         self.checkBox_plotMedian.stateChanged.connect(self.on_checkBox_plotMedian_stateChanged)
         self.checkBox_plotMean.stateChanged.connect(self.on_checkBox_plotMean_stateChanged)
+        self.comboBox_histMethod.currentIndexChanged.connect(self.on_selection_changed_sample_list)
+        self.spinBox_histBins.valueChanged.connect(self.on_selection_changed_sample_list)
 
         # Set up GUI items and widgets:
         self.status = self.statusBar()
         self.set_up_sample_histogram()
         self.set_up_sample_list()
         self.set_up_hist_method_comboBox()
 
@@ -210,15 +213,14 @@
                 ls_data = LSData.from_xlsm_file(xlsm_filename)
                 ls_data.calc_sample_statistics()
             except Exception as e:
                 QMessageBox.critical(self, 'Error!', str(e))
                 self.statusBar().showMessage(f"No LS data loaded.")
             else:
                 self.ls_data = ls_data
-                # TODO: Set up gui models and update gui!
                 self.status.showMessage(f'Loaded: {ls_data}')
                 self.setWindowTitle(self.ls_data.run_name)
                 self.set_up_panel_metadata_view_model()
                 self.set_up_sample_summary_view_model()
                 self.set_up_masses_view_model()
                 self.update_sample_list()
         else:
@@ -235,16 +237,16 @@
             raise IndexError(f'No sample dataset found for sample ID = {sample_id}')
 
         self.label_median.setText(
             f'{sample_data["Mass_median"].item():.3f} ({sample_data["Mass_median_keep"].item():.3f})')
         self.label_mean.setText(f'{sample_data["MeanMass"].item():.3f} ({sample_data["Mass_mean_keep"].item():.3f})')
         self.label_std.setText(f'{sample_data["Mass_std"].item():.3f} ({sample_data["Mass_std_keep"].item():.3f})')
         self.label_iqr.setText(f'{sample_data["Mass_iqr"].item():.3f} ({sample_data["Mass_iqr_keep"].item():.3f})')
-        self.label_median_iqr.setText(
-            f'{sample_data["Mass_stdmedian"].item():.3f} ({sample_data["Mass_stdmedian_keep"].item():.3f})')
+        self.label_rcv.setText(
+            f'{sample_data["Mass_rCV"].item():.3f} ({sample_data["Mass_rCV_keep"].item():.3f})')
         if sample_data["keep_min_mass"].isna().item() and sample_data["keep_max_mass"].isna().item():
             self.label_selectionLimits.clear()
             self.label_SelectedMasse.setText('No selection')
         else:
             self.label_selectionLimits.setText(
                 f'[{sample_data["keep_min_mass"].item():.3f}, {sample_data["keep_max_mass"].item():.3f}]')
             num_selected = sample_data['DetectedParticles_keep'].item()
@@ -462,14 +464,15 @@
         return os.getcwd()
 
     @pyqtSlot()
     def on_menu_help_about(self):
         """Launch the about dialog."""
         return_value = self.dlg_about.exec()
 
+
 class DialogAbout(QDialog, Ui_Dialog_about):
     """About dialog."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # Run the .setupUi() method to show the GUI
```

### Comparing `lifescale-utils-0.0.5/lifescale/gui/masses_model.py` & `lifescale-utils-0.0.6/lifescale/gui/masses_model.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/gui/panel_metadata_model.py` & `lifescale-utils-0.0.6/lifescale/gui/panel_metadata_model.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/gui/sample_summary_model.py` & `lifescale-utils-0.0.6/lifescale/gui/sample_summary_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         'DetectedParticles_keep': 0,
         'Mass_mean_keep': 3,
         'Mass_median_keep': 3,
         'Mass_std_keep': 3,
         'Mass_q25_keep': 3,
         'Mass_q75_keep': 3,
         'Mass_iqr_keep': 3,
-        'Mass_stdmedian_keep': 3,
-        'Mass_stdmedian': 3,
+        'Mass_rCV_keep': 3,
+        'Mass_rCV': 3,
     }
 
     def __init__(self, df):
         QAbstractTableModel.__init__(self)
         self._data = None
         self.load_data(df)
```

### Comparing `lifescale-utils-0.0.5/lifescale/models/__init__.py` & `lifescale-utils-0.0.6/lifescale/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/models/ls_data.py` & `lifescale-utils-0.0.6/lifescale/models/ls_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,14 @@
         # Write PanelData:
         filename = os.path.join(output_filepath, f'Metadata_{filename_ending}')
         if verbose:
             print(f'Write PanelData to: {filename}')
         self.df_panel_data.to_csv(filename, index=False)
 
         # Write Masses:
-
         filename = os.path.join(output_filepath, f'Masses_{filename_ending}')
         if verbose:
             print(f'Write Masses to: {filename}')
         if sort_by_time:
             if verbose:
                 print(f' - Sort Masses by Time.')
             self.df_masses.sort_values(by=['Time']).to_csv(filename, index=False)
@@ -469,17 +468,14 @@
 
         # Write IntervalAnalysis:
         filename = os.path.join(output_filepath, f'SamplesSummary_{filename_ending}')
         if verbose:
             print(f'Write IntervalAnalysis to: {filename}')
         self.df_interval_analysis.to_csv(filename, index=False)
 
-        # TODO: Output format (number of digits)
-        # TODO: Select columns for output (settable as parameter + default settings for each csv file)
-
     def calc_sample_statistics(self, verbose=True, selection_only=False):
         """Calculate statistical values for each sample and add it to the self.df_interval_analysis."""
         if verbose & selection_only:
             print('Calculate sample statistics (selection only).')
         elif verbose:
             print('Calculate sample statistics.')
 
@@ -494,17 +490,17 @@
                 self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q25'] = \
                     self.df_masses.loc[tmp_filter, 'Mass'].quantile(0.25)
                 self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q75'] = \
                     self.df_masses.loc[tmp_filter, 'Mass'].quantile(0.75)
                 self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr'] = \
                     self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q75'] - \
                     self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q25']
-                self.df_interval_analysis.loc[tmp_filter_1, 'Mass_stdmedian'] = \
-                    self.df_interval_analysis.loc[tmp_filter_1, 'Mass_median'] / \
-                    self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr']
+                self.df_interval_analysis.loc[tmp_filter_1, 'Mass_rCV'] = \
+                    74.1 * self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr'] / \
+                    self.df_interval_analysis.loc[tmp_filter_1, 'Mass_median']
 
             # For selected items only (flag `keep` = True):
             tmp_filter = (self.df_masses['Id'] == row.Id) & (self.df_masses['IntervalNumber'] == row.IntervalNumber) & (self.df_masses['keep'])
             tmp_filter_1 = (self.df_interval_analysis['Id'] == row.Id) & \
                            (self.df_interval_analysis['IntervalNumber'] == row.IntervalNumber)
             self.df_interval_analysis.loc[tmp_filter_1, 'Mass_median_keep'] = self.df_masses.loc[tmp_filter, 'Mass'].median()
             self.df_interval_analysis.loc[tmp_filter_1, 'Mass_mean_keep'] = self.df_masses.loc[tmp_filter, 'Mass'].mean()
@@ -512,17 +508,17 @@
             self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q25_keep'] = \
                 self.df_masses.loc[tmp_filter, 'Mass'].quantile(0.25)
             self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q75_keep'] = \
                 self.df_masses.loc[tmp_filter, 'Mass'].quantile(0.75)
             self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr_keep'] = \
                 self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q75_keep'] - \
                 self.df_interval_analysis.loc[tmp_filter_1, 'Mass_q25_keep']
-            self.df_interval_analysis.loc[tmp_filter_1, 'Mass_stdmedian_keep'] = \
-                self.df_interval_analysis.loc[tmp_filter_1, 'Mass_median_keep'] / \
-                self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr_keep']
+            self.df_interval_analysis.loc[tmp_filter_1, 'Mass_rCV_keep'] = \
+                74.1 * self.df_interval_analysis.loc[tmp_filter_1, 'Mass_iqr_keep'] / \
+                self.df_interval_analysis.loc[tmp_filter_1, 'Mass_median_keep']
             self.df_interval_analysis.loc[tmp_filter_1, 'DetectedParticles_keep'] = len(self.df_masses.loc[tmp_filter, 'Mass'])
 
     @property
     def get_number_of_observations(self):
         """Return the number of observations (items in the data series)."""
         if self.df_masses is not None:
             return len(self.df_masses)
```

### Comparing `lifescale-utils-0.0.5/lifescale/scripts/__init__.py` & `lifescale-utils-0.0.6/lifescale/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale/scripts/ls2csv.py` & `lifescale-utils-0.0.6/lifescale/scripts/ls2csv.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.5/lifescale_utils.egg-info/PKG-INFO` & `lifescale-utils-0.0.6/lifescale_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifescale-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lifescale utility software.
 Home-page: https://gitlab.com/hellerdev/lifescale_utils
 Author: Andreas Hellerschmied
 Author-email: heller182@gmx.at
 License: GNU GPLv3
 Keywords: Lifescale
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `lifescale-utils-0.0.5/lifescale_utils.egg-info/SOURCES.txt` & `lifescale-utils-0.0.6/lifescale_utils.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 README.md
 pyproject.toml
 setup.cfg
 lifescale/__init__.py
 lifescale/command_line/__init__.py
 lifescale/command_line/command_line.py
 lifescale/gui/MainWindow.py
-lifescale/gui/MainWindow_old.py
 lifescale/gui/__init__.py
 lifescale/gui/dialog_about.py
 lifescale/gui/gui_main.py
 lifescale/gui/masses_model.py
 lifescale/gui/panel_metadata_model.py
+lifescale/gui/resources.py
 lifescale/gui/sample_summary_model.py
 lifescale/models/__init__.py
 lifescale/models/ls_data.py
-lifescale/models/ls_run.py
 lifescale/scripts/__init__.py
 lifescale/scripts/ls2csv.py
 lifescale/scripts/run_gui.py
 lifescale_utils.egg-info/PKG-INFO
 lifescale_utils.egg-info/SOURCES.txt
 lifescale_utils.egg-info/dependency_links.txt
 lifescale_utils.egg-info/entry_points.txt
```

### Comparing `lifescale-utils-0.0.5/setup.cfg` & `lifescale-utils-0.0.6/setup.cfg`

 * *Files identical despite different names*

