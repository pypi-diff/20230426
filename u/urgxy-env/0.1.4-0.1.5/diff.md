# Comparing `tmp/urgxy_env-0.1.4.tar.gz` & `tmp/urgxy_env-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.4.tar", last modified: Wed Apr 26 10:08:35 2023, max compression
+gzip compressed data, was "urgxy_env-0.1.5.tar", last modified: Wed Apr 26 10:59:30 2023, max compression
```

## Comparing `urgxy_env-0.1.4.tar` & `urgxy_env-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:35.001289 urgxy_env-0.1.4/
--rw-rw-rw-   0        0        0      172 2023-04-26 10:08:35.000287 urgxy_env-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 10:08:35.001289 urgxy_env-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-04-26 10:08:20.000000 urgxy_env-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:34.970289 urgxy_env-0.1.4/urgxy_env/
--rw-rw-rw-   0        0        0      127 2023-04-26 10:08:20.000000 urgxy_env-0.1.4/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:34.998288 urgxy_env-0.1.4/urgxy_env/envs/
--rw-rw-rw-   0        0        0       45 2023-04-25 15:35:12.000000 urgxy_env-0.1.4/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0     8602 2023-04-26 10:07:26.000000 urgxy_env-0.1.4/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:34.996291 urgxy_env-0.1.4/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      172 2023-04-26 10:08:34.000000 urgxy_env-0.1.4/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-26 10:08:34.000000 urgxy_env-0.1.4/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:08:34.000000 urgxy_env-0.1.4/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-26 10:08:34.000000 urgxy_env-0.1.4/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 10:08:34.000000 urgxy_env-0.1.4/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/
+-rw-rw-rw-   0        0        0      172 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.513991 urgxy_env-0.1.5/urgxy_env/
+-rw-rw-rw-   0        0        0      127 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.548740 urgxy_env-0.1.5/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       45 2023-04-25 15:35:12.000000 urgxy_env-0.1.5/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     8671 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.540740 urgxy_env-0.1.5/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      172 2023-04-26 10:59:29.000000 urgxy_env-0.1.5/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 10:59:29.000000 urgxy_env-0.1.5/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.4/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.1.5/urgxy_env/envs/env_urgxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,23 @@
         #p.setJointMotorControlArray(self.pandaUid, list(range(12)), p.POSITION_CONTROL, list(jointPoses))
         # p.setJointMotorControl2(self.pandaUid, 15 , p.POSITION_CONTROL, jointPoses[6])
         # p.setJointMotorControl2(self.pandaUid, 16,  p.POSITION_CONTROL, jointPoses[7])
         # p.setJointMotorControl2(self.pandaUid, 17,  p.POSITION_CONTROL, jointPoses[8])
         # p.setJointMotorControl2(self.pandaUid, 18,  p.POSITION_CONTROL, jointPoses[9])
         # p.setJointMotorControl2(self.pandaUid, 19,  p.POSITION_CONTROL, jointPoses[10])
         # p.setJointMotorControl2(self.pandaUid, 20,  p.POSITION_CONTROL, jointPoses[11])
-        p.setJointMotorControlArray(self.pandaUid, [15, 20], p.POSITION_CONTROL, [jointPoses[6], jointPoses[11]])
+        p.setJointMotorControlArray(self.pandaUid, [15,16,17,18,19,20], p.POSITION_CONTROL, [jointPoses[6],jointPoses[7],jointPoses[8],jointPoses[9],jointPoses[10],jointPoses[11]])
         p.stepSimulation()
         state_robot = p.getLinkState(self.pandaUid, 20)[0]  #得到位置
 
         done = False
         goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
         current = np.array( [state_robot[0],state_robot[1],state_robot[2]] )
         reward = -np.linalg.norm( current-goal )
+
         # reward = 0
         # if action[0]>0 and state_robot[0]-(-0.8746627265025098) < 0:
         #     reward += 1
         #     done = False
         #
         # if action[0]<0 and state_robot[0]-(-0.8746627265025098) > 0:
         #     reward += 1
```

