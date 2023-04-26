# Comparing `tmp/terka-1.6.4.9.tar.gz` & `tmp/terka-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.9.tar", last modified: Mon Apr 24 19:07:55 2023, max compression
+gzip compressed data, was "terka-1.7.0.tar", last modified: Wed Apr 26 19:54:36 2023, max compression
```

## Comparing `terka-1.6.4.9.tar` & `terka-1.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:55.551545 terka-1.6.4.9/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-24 19:07:55.551545 terka-1.6.4.9/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      905 2023-04-24 19:07:53.000000 terka-1.6.4.9/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.9/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.9/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.9/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.9/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.9/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.9/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.9/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.9/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.9/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.9/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.9/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.9/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.9/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.9/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.9/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2120 2023-04-24 19:07:46.000000 terka-1.6.4.9/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.9/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.9/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.9/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.9/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.551545 terka-1.6.4.9/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.9/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.9/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.9/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.9/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.9/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-24 18:36:30.000000 terka-1.6.4.9/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-23 14:24:46.000000 terka-1.6.4.9/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 19:07:55.547546 terka-1.6.4.9/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-24 19:07:55.000000 terka-1.6.4.9/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-26 19:54:36.686519 terka-1.7.0/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-26 19:54:36.686519 terka-1.7.0/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-04-26 19:51:31.000000 terka-1.7.0/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.682520 terka-1.7.0/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.0/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.0/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41931 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1556 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.0/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.0/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1538 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-26 19:47:22.000000 terka-1.7.0/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    26315 2023-04-26 19:48:32.000000 terka-1.7.0/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-26 19:47:22.000000 terka-1.7.0/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/top_level.txt
```

### Comparing `terka-1.6.4.9/setup.py` & `terka-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4.9",
+    version="1.7.0",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.4.9/terka/adapters/orm.py` & `terka-1.7.0/terka/adapters/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 from terka.domain.project import Project, ProjectStatus
 from terka.domain.event_history import TaskEvent, ProjectEvent, EventType
 from terka.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
 from terka.domain.tag import BaseTag, TaskTag, ProjectTag
 from terka.domain.collaborators import TaskCollaborator, ProjectCollaborator
 from terka.domain.sprint import Sprint, SprintStatus, SprintTask
 from terka.domain.time_tracker import TimeTrackerEntry
-from terka.domain.epic import Epic, EpicTask
-from terka.domain.story import Story, StoryTask
+from terka.domain.epic import Epic, EpicTask, EpicStatus
+from terka.domain.story import Story, StoryTask, StoryStatus
 
 from terka.domain.external_connectors.asana import AsanaTask, AsanaProject
 
 Base = declarative_base()
 metadata = MetaData()
 
 tasks = Table("tasks", metadata,
               Column("id", Integer, primary_key=True, autoincrement=True),
               Column("name", String(255)),
               Column("creation_date", DateTime, nullable=True),
+              Column("modification_date", DateTime, nullable=True),
               Column("description", String(1000), nullable=True),
               Column("project", ForeignKey("projects.id"), nullable=True),
               Column("assignee", ForeignKey("users.id"), nullable=True),
               Column("created_by", ForeignKey("users.id"), nullable=True),
               Column("due_date", Date, nullable=True),
               Column("status", Enum(TaskStatus)),
               Column("priority", Enum(TaskPriority)))
@@ -188,28 +189,30 @@
 epics = Table("epics", metadata,
               Column("id", Integer, primary_key=True, autoincrement=True),
               Column("name", String(255)),
               Column("creation_date", DateTime, nullable=True),
               Column("description", String(1000), nullable=True),
               Column("project", ForeignKey("projects.id"), nullable=True),
               Column("assignee", ForeignKey("users.id"), nullable=True),
+              Column("status", Enum(EpicStatus)),
               Column("created_by", ForeignKey("users.id"), nullable=True))
 
 epic_tasks = Table("epic_tasks", metadata,
                    Column("id", Integer, primary_key=True, autoincrement=True),
                    Column("task", ForeignKey("tasks.id"), nullable=False),
                    Column("epic", ForeignKey("epics.id"), nullable=False))
 
 stories = Table("stories", metadata,
                 Column("id", Integer, primary_key=True, autoincrement=True),
                 Column("name", String(255)),
                 Column("creation_date", DateTime, nullable=True),
                 Column("description", String(1000), nullable=True),
                 Column("project", ForeignKey("projects.id"), nullable=True),
                 Column("assignee", ForeignKey("users.id"), nullable=True),
+                Column("status", Enum(StoryStatus)),
                 Column("created_by", ForeignKey("users.id"), nullable=True))
 
 story_tasks = Table(
     "story_tasks", metadata,
     Column("id", Integer, primary_key=True, autoincrement=True),
     Column("task", ForeignKey("tasks.id"), nullable=False),
     Column("story", ForeignKey("stories.id"), nullable=False))
@@ -221,21 +224,23 @@
 #     ta
 
 asana_tasks = Table(
     "external_connectors.asana.tasks", metadata,
     # Column("id", Integer, primary_key=True, autoincrement=True),
     Column("project", ForeignKey("projects.id")),
     Column("id", ForeignKey("tasks.id"), nullable=False, primary_key=True),
-    Column("asana_task_id", String(20)))
+    Column("asana_task_id", String(20)),
+    Column("sync_date", DateTime, nullable=True))
 
 asana_projects = Table(
     "external_connectors.asana.projects", metadata,
     # Column("id", Integer, primary_key=True, autoincrement=True),
     Column("id", ForeignKey("projects.id"), nullable=False, primary_key=True),
-    Column("asana_project_id", String(20)))
+    Column("asana_project_id", String(20)),
+    Column("sync_date", DateTime, nullable=True))
 
 def start_mappers():
     asana_task_mapper = mapper(AsanaTask, asana_tasks)
     asana_project_mapper = mapper(AsanaProject, asana_projects)
     task_commentary_mapper = mapper(TaskCommentary, task_commentaries)
     project_commentary_mapper = mapper(ProjectCommentary, project_commentaries)
     epic_commentary_mapper = mapper(EpicCommentary, epic_commentaries)
@@ -299,30 +304,30 @@
     epic_mapper = mapper(Epic,
                          epics,
                          properties={
                              "commentaries":
                              relationship(epic_commentary_mapper,
                                           collection_class=list,
                                           cascade="all, delete-orphan"),
-                             "epic_tasks":
+                             "tasks":
                              relationship(epic_tasks_mapper,
                                           collection_class=list)
                          })
     story_tasks_mapper = mapper(
         StoryTask,
         story_tasks,
         properties={"tasks": relationship(task_mapper, collection_class=list)})
     story_mapper = mapper(Story,
                           stories,
                           properties={
                              "commentaries":
                              relationship(story_commentary_mapper,
                                           collection_class=list,
                                           cascade="all, delete-orphan"),
-                              "story_tasks":
+                              "tasks":
                               relationship(story_tasks_mapper,
                                            collection_class=list)
                           })
     project_mapper = mapper(Project,
                             projects,
                             properties={
                                 "collaborators":
@@ -357,11 +362,11 @@
     sprint_mapper = mapper(Sprint,
                            sprints,
                            properties={
                                "commentaries":
                                relationship(sprint_commentary_mapper,
                                             collection_class=list,
                                         cascade="all, delete-orphan"),
-                               "sprint_tasks":
+                               "tasks":
                                relationship(sprint_tasks_mapper,
                                             collection_class=list)
                            })
```

### Comparing `terka-1.6.4.9/terka/adapters/repository.py` & `terka-1.7.0/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/collaborators.py` & `terka-1.7.0/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/commands.py` & `terka-1.7.0/terka/domain/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,21 @@
             if entity_type == "tasks":
                 if "status" not in kwargs and "all" not in kwargs:
                     kwargs["status"] = "BACKLOG,TODO,IN_PROGRESS,REVIEW"
                 else:
                     if "all" in kwargs:
                         del kwargs["all"]
                     show_completed = True
+            if entity_type in ("stories", "epics"):
+                if "all" in kwargs:
+                    kwargs["status"] = "ACTIVE,COMPLETED"
+                    del kwargs["all"]
+                    print_options.show_completed = True
+                else:
+                    kwargs["status"] = "ACTIVE"
             if entity_type == "sprints":
                 if "all" in kwargs:
                     kwargs["status"] = "PLANNED,ACTIVE,COMPLETED"
                     del kwargs["all"]
                 else:
                     kwargs["status"] = "PLANNED,ACTIVE"
             if entity_type == "projects":
@@ -530,14 +537,15 @@
             if entity_type == "tasks":
                 existing_task = self.repo.list(Task, {"id": kwargs["id"]})
                 if not existing_task:
                     raise ValueError(
                         f"Task with id {kwargs['id']} is not found!")
                 obj = TaskCommentary(**kwargs)
                 self.repo.add(obj)
+                self.repo.update(Task, kwargs["id"], {"modification_date": datetime.now()})
                 session.commit()
             elif entity_type == "projects":
                 existing_project = self.repo.list(Project,
                                                   {"id": kwargs["id"]})
                 if not existing_project:
                     raise ValueError(
                         f"Project with id {kwargs['id']} is not found!")
@@ -690,20 +698,21 @@
                     }):
                         exit("task already added to sprint")
                     self.repo.add(obj)
                     sprint_task_id = obj.id
                 else:
                     sprint_task_id = None
                 # Update task status and due date
-                task_params = {"id": added_task.id}
-                if added_task.status.name == "BACKLOG":
-                    task_params.update({"status": "TODO"})
-                if not added_task.due_date or added_task.due_date > sprint.end_date:
-                    task_params.update({"due_date": sprint.end_date})
-                self.execute("update", "tasks", task_params)
+                if sprint_task_id:
+                    task_params = {"id": added_task.id}
+                    if added_task.status.name == "BACKLOG":
+                        task_params.update({"status": "TODO"})
+                    if not added_task.due_date or added_task.due_date > sprint.end_date:
+                        task_params.update({"due_date": sprint.end_date})
+                    self.execute("update", "tasks", task_params)
                 if story_points := kwargs.get("story_points"):
                     if not sprint_task_id:
                         sprint_task = self.execute("get", "sprint_tasks",
                                                    {"task": task_id})
                         if not sprint_task:
                             exit(
                                 f"Task id {task_id} is not part of any sprint")
@@ -773,14 +782,16 @@
                                     if entity_type == "projects":
                                         event = ProjectEvent
                                     elif entity_type == "tasks":
                                         event = TaskEvent
                                     self.repo.add(
                                         event(task, key, old_value, value,
                                               now))
+                            if hasattr(entity, "modification_date"):
+                                self.repo.update(entity, task, {"modification_date": now})
                         else:
                             print(
                                 "No changes were proposed to the existing entity"
                             )
                     session.commit()
                 return entity, None
             else:
@@ -835,15 +846,15 @@
                 self.execute("update", entity_type, new_kwargs)
                 return entities, None, None
         elif command == "start":
             sprint_id = kwargs.get("id")
             kwargs.update({"status": "ACTIVE"})
             self.execute("update", "sprints", kwargs)
             [sprint] = self.execute("get", "sprints", {"id": sprint_id})
-            for sprint_task in sprint.sprint_tasks:
+            for sprint_task in sprint.tasks:
                 task = sprint_task.tasks
                 task_params = {"id": task.id}
                 if task.status.name == "BACKLOG":
                     task_params.update({"status": "TODO"})
                 if not task.due_date or task.due_date > sprint.end_date:
                     task_params.update({"due_date": sprint.end_date})
                 self.execute("update", "tasks", task_params)
@@ -880,26 +891,32 @@
                 else:
                     entities = self.repo.list(entity, {"name": task})
                 self.printer.print_entity(task, entity_type, entities,
                                           self.repo, print_options, kwargs)
                 logger.info("<show> %s: %s", entity_type, task_id)
             return entities, None, None
         elif command == "done":
-            if entity_type not in ("tasks", "sprints"):
+            if entity_type not in ("tasks", "sprints", "stories", "epics"):
                 raise ValueError("can complete only tasks and sprints")
             elif entity_type == "tasks":
                 kwargs.update({"status": "DONE"})
                 self.execute("update", entity_type, kwargs)
                 self.console.print(
                     "[green]Yay! You've just completed a task![/green]")
-            elif entity_type == "sprints":
+            elif entity_type in ("sprints", "epics", "stories"):
                 kwargs.update({"status": "COMPLETED"})
-                [sprint] = self.execute("get", "sprints",
+                [entity] = self.execute("get", entity_type,
                                         {"id": kwargs.get("id")})
-                sprint.complete(sprint.sprint_tasks)
+
+                if entity_type == "sprints":
+                    entity.complete(entity.tasks)
+                else:
+                    entity.complete(entity.tasks)
+                    for entity_task in entity.tasks:
+                        self.execute("update", "tasks", {"id": entity_task.task, "status": "DONE"})
                 self.execute("update", entity_type, kwargs)
         elif command == "track":
             if entity_type != "tasks":
                 raise ValueError("can track only tasks")
             if "hours" in kwargs and "minutes" in kwargs:
                 exit("specify only -H (hours) or -M (minutes) value")
             if "hours" in kwargs or "minutes" in kwargs:
```

### Comparing `terka-1.6.4.9/terka/domain/commentary.py` & `terka-1.7.0/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/epic.py` & `terka-1.7.0/terka/domain/story.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,56 @@
 from dataclasses import dataclass
 from datetime import datetime
+from enum import Enum
 
-from terka.domain.task import Task
+from .task import Task
 
 
-class Epic:
+class StoryStatus(Enum):
+    ACTIVE = 1
+    COMPLETED = 2
+
+
+class Story:
 
     def __init__(self,
                  name: str,
                  description: str = None,
                  creation_date: datetime = datetime.now(),
                  project: int = None,
                  assignee: int = None,
+                 status: str = "ACTIVE",
                  created_by: int = None,
                  **kwargs) -> None:
         if not name:
             raise ValueError("task name cannot be empty!")
         if not isinstance(creation_date, datetime):
             raise ValueError(
                 "creation_date should be of type datetime.datetime!")
         self.name = name
         self.creation_date = creation_date
         self.description = description
         self.project = project
         self.assignee = assignee
         self.created_by = created_by
+        self.status = status
         self.tasks: Set[Task, ...] = set()
+        self.is_completed = False
+
+    def complete(self, tasks) -> None:
+        incompleted_tasks = list()
+        for task in tasks:
+            if task.tasks.status.name != "DONE":
+                incompleted_tasks.append(task)
+        if incompleted_tasks:
+            logging.warning("[story %d]: %d tasks haven't been completed",
+                            self.id, len(incompleted_tasks))
+        self.is_completed = True
 
 
 @dataclass
-class EpicTask:
-    epic: int
+class StoryTask:
+    story: int
     task: int
+
+
+
```

### Comparing `terka-1.6.4.9/terka/domain/event_history.py` & `terka-1.7.0/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/project.py` & `terka-1.7.0/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/sprint.py` & `terka-1.7.0/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/story.py` & `terka-1.7.0/terka/domain/time_tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,17 @@
-from dataclasses import dataclass
 from datetime import datetime
 
-from .task import Task
 
-
-class Story:
+class TimeTrackerEntry:
 
     def __init__(self,
-                 name: str,
-                 description: str = None,
+                 task: int,
+                 time_spent_minutes: float,
                  creation_date: datetime = datetime.now(),
-                 project: int = None,
-                 assignee: int = None,
-                 created_by: int = None,
-                 **kwargs) -> None:
-        if not name:
-            raise ValueError("task name cannot be empty!")
+                 **kwargs
+                 ):
         if not isinstance(creation_date, datetime):
             raise ValueError(
                 "creation_date should be of type datetime.datetime!")
-        self.name = name
+        self.task = task
+        self.time_spent_minutes = time_spent_minutes
         self.creation_date = creation_date
-        self.description = description
-        self.project = project
-        self.assignee = assignee
-        self.created_by = created_by
-        self.tasks: Set[Task, ...] = set()
-
-
-@dataclass
-class StoryTask:
-    story: int
-    task: int
-
-
-
```

### Comparing `terka-1.6.4.9/terka/domain/tag.py` & `terka-1.7.0/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/domain/task.py` & `terka-1.7.0/terka/domain/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,25 +18,26 @@
     HIGH = 3
     URGENT = 4
 
 
 class Task:
 
     _next_task_id = 1
-    def __init__(self, name: str,
+
+    def __init__(self,
+                 name: str,
                  description: str = None,
                  creation_date: datetime = datetime.now(),
                  project: int = None,
                  assignee: int = None,
                  created_by: int = None,
                  due_date: datetime = None,
                  status: str = "BACKLOG",
                  priority: str = "NORMAL",
-                 **kwargs
-                 ):
+                 **kwargs):
         if not name:
             raise ValueError("task name cannot be empty!")
         if not isinstance(creation_date, datetime):
             raise ValueError(
                 "creation_date should be of type datetime.datetime!")
         self._task_id = Task._next_task_id
         Task._next_task_id += 1
@@ -44,29 +45,27 @@
         self.name = name
         self.creation_date = creation_date
         self.description = description
         self.project = project
         self.assignee = assignee
         self.created_by = created_by
         if due_date and due_date.date() < datetime.today().date():
-            raise ValueError(f"Due date {due_date.date()} cannot be less than today")
+            raise ValueError(
+                f"Due date {due_date.date()} cannot be less than today")
         else:
             self.due_date = due_date
         self.status = self._validate_status(status)
         if priority and priority not in [p.name for p in TaskPriority]:
             raise ValueError(f"{priority} is invalid priority")
         else:
             self.priority = priority
 
-    @property
-    def last_modified(self):
-        # TODO: return 
-        pass
-
     def _validate_status(self, status):
-        if status and status not in [s.name for s in TaskStatus if s.name != "DELETED"]:
+        if status and status not in [
+                s.name for s in TaskStatus if s.name != "DELETED"
+        ]:
             raise ValueError(f"{status} is invalid status")
         else:
             return status
 
     def __repr__(self):
         return f"<Task {self.id}>: {self.name}, {self.status.name}, {self.creation_date}"
```

### Comparing `terka-1.6.4.9/terka/entrypoints/cli.py` & `terka-1.7.0/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/service_layer/printer.py` & `terka-1.7.0/terka/service_layer/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,24 +73,19 @@
                      print_options: PrintOptions = PrintOptions(),
                      kwargs: Optional[Dict[str, Any]] = None):
         if entity_type == "sprints":
             if entities:
                 self.print_sprint(entities, repo, print_options, kwargs)
             else:
                 exit(f"No sprint with id '{task}' found!")
-        if entity_type == "epics":
+        if entity_type in ("epics", "stories"):
             if entities:
-                self.print_epic(entities, repo, print_options)
+                self.print_composite(entities, repo, print_options, entity_type)
             else:
-                exit(f"No epic with id '{task}' found!")
-        if entity_type == "stories":
-            if entities:
-                self.print_story(entities, repo, print_options)
-            else:
-                exit(f"No story with id '{task}' found!")
+                exit(f"No {entity_type} with id '{task}' found!")
         if entity_type == "projects":
             if entities:
                 self.print_project(entities, print_options, kwargs)
             else:
                 exit(f"No project '{task}' found!")
         if entity_type == "tasks":
             if entities:
@@ -119,22 +114,19 @@
             self.print_tag(entities=entities)
         elif type == "users":
             self.print_user(entities=entities)
         elif type == "sprints":
             self.print_sprint(entities=entities,
                               repo=repo,
                               print_options=print_options)
-        elif type == "epics":
-            self.print_epic(entities=entities,
+        elif type in ("epics", "stories"):
+            self.print_composite(entities=entities,
                             repo=repo,
-                            print_options=print_options)
-        elif type == "stories":
-            self.print_story(entities=entities,
-                             repo=repo,
-                             print_options=print_options)
+                            print_options=print_options,
+                            composite_type=type)
         else:
             self.print_default_entity(self, entities)
 
     def print_user(self, entities):
         table = Table(box=self.box)
         for column in ("id", "name"):
             table.add_column(column)
@@ -164,63 +156,45 @@
             table.add_column(column)
         for entity in entities:
             table.add_row(f"[red]{entity.id}[/red]",
                           entity.date.strftime("%Y-%m-%d %H:%M"), entity.text)
         if table.row_count:
             self.console.print(table)
 
-    def print_epic(self, entities, repo, print_options):
-        table = Table(box=self.box, title="EPICS", expand=True)
+    def print_composite(self, entities, repo, print_options, composite_type):
+        table = Table(box=self.box, title=composite_type.upper(), expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
         for i, entity in enumerate(entities):
             tasks = []
-            for epic_task in entity.epic_tasks:
-                task = epic_task.tasks
-                tasks.append(task)
+            completed_tasks = []
+            for entity_task in entity.tasks:
+                task = entity_task.tasks
+                if task.status.name not in ("DONE", "DELETED"):
+                    tasks.append(task)
+                else:
+                    completed_tasks.append(task)
             try:
                 project_obj = services.lookup_project_name(
                     entity.project, repo)
                 project = project_obj.name
             except:
                 project = None
-            table.add_row(f"E{entity.id}", str(entity.name),
-                          entity.description, project, str(len(tasks)))
+            if i == 0 or tasks or print_options.show_completed:
+                table.add_row(f"E{entity.id}", str(entity.name),
+                              entity.description, project, str(len(tasks)))
         if table.row_count:
             self.console.print(table)
-        if print_options.show_tasks:
+        if print_options.show_tasks and tasks:
             self.print_task(entities=tasks,
                             repo=repo,
                             print_options=print_options,
                             show_window=False)
-        if i == 0 and print_options.show_commentaries and (
-                commentaries := entity.commentaries):
-            self.print_commentaries(commentaries)
-
-    def print_story(self, entities, repo, print_options):
-        table = Table(box=self.box, title="STORIES", expand=True)
-        for column in ("id", "name", "description", "project", "tasks"):
-            table.add_column(column, style="bold")
-        for i, entity in enumerate(entities):
-            tasks = []
-            for story_task in entity.story_tasks:
-                task = story_task.tasks
-                tasks.append(task)
-            try:
-                project_obj = services.lookup_project_name(
-                    entity.project, repo)
-                project = project_obj.name
-            except:
-                project = None
-            table.add_row(f"S{entity.id}", str(entity.name),
-                          entity.description, project, str(len(tasks)))
-        if table.row_count:
-            self.console.print(table)
-        if print_options.show_tasks and tasks:
-            self.print_task(entities=tasks,
+        if print_options.show_tasks and completed_tasks:
+            self.print_task(entities=completed_tasks,
                             repo=repo,
                             print_options=print_options,
                             show_window=False)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
@@ -231,15 +205,15 @@
                        "time_spent"):
             table.add_column(column)
         for i, entity in enumerate(entities):
             story_points = []
             tasks = []
             collaborators = []
             collaborators_dict = defaultdict(int)
-            for sprint_task in entity.sprint_tasks:
+            for sprint_task in entity.tasks:
                 story_points.append(sprint_task.story_points)
                 task = sprint_task.tasks
                 tasks.append(task)
                 if task_collaborators := task.collaborators:
                     for collaborator in task.collaborators:
                         collaborators_dict[collaborator.users.
                                            name] += sprint_task.story_points
@@ -354,18 +328,18 @@
         if non_active_projects.row_count:
             self.console.print("[green]Inactive projects[/green]")
             self.console.print(non_active_projects)
         non_task_view_options = deepcopy(print_options)
         non_task_view_options.show_tasks = False
         if print_options.show_epics and (epics := entity.epics):
             self.console.print("")
-            self.print_epic(epics, self.repo, non_task_view_options)
+            self.print_composite(epics, self.repo, non_task_view_options, "epics")
         if print_options.show_stories and (stories := entity.stories):
             self.console.print("")
-            self.print_story(stories, self.repo, non_task_view_options)
+            self.print_composite(stories, self.repo, non_task_view_options, "stories")
         if print_options.show_tasks and (tasks := entity.tasks):
             task_print_options = deepcopy(print_options)
             task_print_options.show_commentaries = False
             self.console.print("")
             self.print_task(entities=tasks,
                             repo=self.repo,
                             print_options=task_print_options,
```

### Comparing `terka-1.6.4.9/terka/service_layer/services.py` & `terka-1.7.0/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/service_layer/ui.py` & `terka-1.7.0/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/service_layer/vertical_layout.css` & `terka-1.7.0/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/service_layer/views.py` & `terka-1.7.0/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka/utils.py` & `terka-1.7.0/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.9/terka.egg-info/SOURCES.txt` & `terka-1.7.0/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

