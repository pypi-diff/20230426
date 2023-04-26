# Comparing `tmp/resoto-plugin-github-3.3.3.tar.gz` & `tmp/resoto-plugin-github-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-github-3.3.3.tar", last modified: Fri Apr 21 14:35:41 2023, max compression
+gzip compressed data, was "resoto-plugin-github-3.3.4.tar", last modified: Wed Apr 26 16:52:03 2023, max compression
```

## Comparing `resoto-plugin-github-3.3.3.tar` & `resoto-plugin-github-3.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:41.356224 resoto-plugin-github-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 14:35:41.356224 resoto-plugin-github-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:41.352224 resoto-plugin-github-3.3.3/resoto_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/resoto_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/resoto_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/resoto_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:41.352224 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 14:35:41.000000 resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:35:41.356224 resoto-plugin-github-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:41.356224 resoto-plugin-github-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 14:33:59.000000 resoto-plugin-github-3.3.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:03.281636 resoto-plugin-github-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 16:52:03.281636 resoto-plugin-github-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:03.273636 resoto-plugin-github-3.3.4/resoto_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/resoto_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/resoto_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/resoto_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:03.277636 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 16:52:03.000000 resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:52:03.281636 resoto-plugin-github-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:03.281636 resoto-plugin-github-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 16:49:36.000000 resoto-plugin-github-3.3.4/test/test_config.py
```

### Comparing `resoto-plugin-github-3.3.3/PKG-INFO` & `resoto-plugin-github-3.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto Github Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.3.3/resoto_plugin_github/resources.py` & `resoto-plugin-github-3.3.4/resoto_plugin_github/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from github.Organization import Organization
 from github.NamedUser import NamedUser
 from github.Clones import Clones
 from github.View import View
 from github.Referrer import Referrer
 from github.Path import Path
 from github.GithubException import GithubException
+from github.PullRequest import PullRequest
 
 
 @define(eq=False, slots=False)
 class GithubAccount(BaseAccount):
     kind: ClassVar[str] = "github_account"
 
     def delete(self, graph: Graph) -> bool:
@@ -96,16 +97,16 @@
             id=str(org.login),
             name=org.name,
             avatar_url=org.avatar_url,
             billing_email=org.billing_email,
             blog=org.blog,
             collaborators=org.collaborators,
             company=org.company,
-            created_at=org.created_at,
-            ctime=org.created_at,
+            created_at=make_valid_timestamp(org.created_at),
+            ctime=make_valid_timestamp(org.created_at),
             default_repository_permission=org.default_repository_permission,
             description=org.description,
             disk_usage=org.disk_usage,
             email=org.email,
             events_url=org.events_url,
             followers=org.followers,
             following=org.following,
@@ -124,16 +125,16 @@
             private_gists=org.private_gists,
             public_gists=org.public_gists,
             public_members_url=org.public_members_url,
             public_repos=org.public_repos,
             repos_url=org.repos_url,
             total_private_repos=org.total_private_repos,
             org_type=org.type,
-            updated_at=org.updated_at,
-            mtime=org.updated_at,
+            updated_at=make_valid_timestamp(org.updated_at),
+            mtime=make_valid_timestamp(org.updated_at),
             url=org.url,
         )
 
 
 @define(eq=False, slots=False)
 class GithubUser(GithubResource, BaseUser):
     kind: ClassVar[str] = "github_user"
@@ -187,16 +188,16 @@
             id=str(user.login),
             avatar_url=user.avatar_url,
             bio=user.bio,
             blog=user.blog,
             collaborators=user.collaborators,
             company=user.company,
             contributions=user.contributions,
-            created_at=user.created_at,
-            ctime=user.created_at,
+            created_at=make_valid_timestamp(user.created_at),
+            ctime=make_valid_timestamp(user.created_at),
             disk_usage=user.disk_usage,
             email=user.email,
             events_url=user.events_url,
             followers=user.followers,
             followers_url=user.followers_url,
             following=user.following,
             following_url=user.following_url,
@@ -217,21 +218,21 @@
             public_repos=user.public_repos,
             received_events_url=user.received_events_url,
             repos_url=user.repos_url,
             role=user.role,
             site_admin=user.site_admin,
             starred_url=user.starred_url,
             subscriptions_url=user.subscriptions_url,
-            suspended_at=user.suspended_at,
+            suspended_at=make_valid_timestamp(user.suspended_at),
             team_count=user.team_count,
             total_private_repos=user.total_private_repos,
             twitter_username=user.twitter_username,
             user_type=user.type,
-            updated_at=user.updated_at,
-            mtime=user.updated_at,
+            updated_at=make_valid_timestamp(user.updated_at),
+            mtime=make_valid_timestamp(user.updated_at),
             url=user.url,
         )
 
 
 @define(eq=False, slots=False)
 class GithubRepoClones:
     kind: ClassVar[str] = "github_repo_clones"
@@ -324,14 +325,105 @@
 
     @staticmethod
     def new(path: Path):
         return GithubRepoTopPath(title=path.title, path=path.path, count=path.count, uniques=path.uniques)
 
 
 @define(eq=False, slots=False)
+class GithubPullRequest(GithubResource, BaseResource):
+    kind: ClassVar[str] = "github_pull_request"
+
+    additions: Optional[int] = None
+    # assignee: Optional[str] = None
+    # assignees: Optional[List[str]] = None
+    # base: Optional[str] = None
+    body: Optional[str] = None
+    changed_files: Optional[int] = None
+    closed_at: Optional[datetime] = None
+    comments: Optional[int] = None
+    comments_url: Optional[str] = None
+    commits: Optional[int] = None
+    commits_url: Optional[str] = None
+    created_at: Optional[datetime] = None
+    deletions: Optional[int] = None
+    diff_url: Optional[str] = None
+    draft: Optional[bool] = None
+    # head: Optional[str] = None
+    html_url: Optional[str] = None
+    pr_id: Optional[int] = None
+    issue_url: Optional[str] = None
+    # labels: Optional[List[str]] = None
+    merge_commit_sha: Optional[str] = None
+    mergeable: Optional[bool] = None
+    mergeable_state: Optional[str] = None
+    merged: Optional[bool] = None
+    merged_at: Optional[datetime] = None
+    # merged_by: Optional[str] = None
+    # milestone: Optional[str] = None
+    number: Optional[int] = None
+    patch_url: Optional[str] = None
+    rebaseable: Optional[bool] = None
+    review_comments: Optional[int] = None
+    review_comments_url: Optional[str] = None
+    state: Optional[str] = None
+    title: Optional[str] = None
+    updated_at: Optional[datetime] = None
+    url: Optional[str] = None
+    # user: Optional[str] = None
+    maintainer_can_modify: Optional[bool] = None
+
+    @staticmethod
+    def new(pr: PullRequest):
+        return GithubPullRequest(
+            name=str(pr.title),
+            additions=pr.additions,
+            # assignee=pr.assignee,
+            # assignees=pr.assignees,
+            # base=pr.base,
+            body=pr.body,
+            changed_files=pr.changed_files,
+            closed_at=make_valid_timestamp(pr.closed_at),
+            comments=pr.comments,
+            comments_url=pr.comments_url,
+            commits=pr.commits,
+            commits_url=pr.commits_url,
+            created_at=make_valid_timestamp(pr.created_at),
+            ctime=make_valid_timestamp(pr.created_at),
+            deletions=pr.deletions,
+            diff_url=pr.diff_url,
+            draft=pr.draft,
+            # head=pr.head,
+            html_url=pr.html_url,
+            pr_id=pr.id,
+            issue_url=pr.issue_url,
+            # labels=pr.labels,
+            merge_commit_sha=pr.merge_commit_sha,
+            mergeable=pr.mergeable,
+            mergeable_state=pr.mergeable_state,
+            merged=pr.merged,
+            merged_at=make_valid_timestamp(pr.merged_at),
+            # merged_by=pr.merged_by,
+            # milestone=pr.milestone,
+            number=pr.number,
+            id=str(pr.number),
+            patch_url=pr.patch_url,
+            rebaseable=pr.rebaseable,
+            review_comments=pr.review_comments,
+            review_comments_url=pr.review_comments_url,
+            state=pr.state,
+            title=pr.title,
+            updated_at=make_valid_timestamp(pr.updated_at),
+            mtime=make_valid_timestamp(pr.updated_at),
+            url=pr.url,
+            # user=pr.user,
+            maintainer_can_modify=pr.maintainer_can_modify,
+        )
+
+
+@define(eq=False, slots=False)
 class GithubRepo(GithubResource, BaseResource):
     kind: ClassVar[str] = "github_repo"
 
     allow_merge_commit: Optional[bool] = None
     allow_rebase_merge: Optional[bool] = None
     allow_squash_merge: Optional[bool] = None
     archived: Optional[bool] = None
@@ -429,16 +521,16 @@
             clone_url=repo.clone_url,
             collaborators_url=repo.collaborators_url,
             comments_url=repo.comments_url,
             commits_url=repo.commits_url,
             compare_url=repo.compare_url,
             contents_url=repo.contents_url,
             contributors_url=repo.contributors_url,
-            created_at=repo.created_at,
-            ctime=repo.created_at,
+            created_at=make_valid_timestamp(repo.created_at),
+            ctime=make_valid_timestamp(repo.created_at),
             default_branch=repo.default_branch,
             delete_branch_on_merge=repo.delete_branch_on_merge,
             deployments_url=repo.deployments_url,
             description=repo.description,
             downloads_url=repo.downloads_url,
             events_url=repo.events_url,
             fork=repo.fork,
@@ -472,30 +564,30 @@
             mirror_url=repo.mirror_url,
             network_count=repo.network_count,
             notifications_url=repo.notifications_url,
             open_issues=repo.open_issues,
             open_issues_count=repo.open_issues_count,
             private=repo.private,
             pulls_url=repo.pulls_url,
-            pushed_at=repo.pushed_at,
+            pushed_at=make_valid_timestamp(repo.pushed_at),
             releases_url=repo.releases_url,
             size=repo.size,
             ssh_url=repo.ssh_url,
             stargazers_count=repo.stargazers_count,
             stargazers_url=repo.stargazers_url,
             statuses_url=repo.statuses_url,
             subscribers_count=repo.subscribers_count,
             subscribers_url=repo.subscribers_url,
             subscription_url=repo.subscription_url,
             svn_url=repo.svn_url,
             tags_url=repo.tags_url,
             teams_url=repo.teams_url,
             trees_url=repo.trees_url,
-            updated_at=repo.updated_at,
-            mtime=repo.updated_at,
+            updated_at=make_valid_timestamp(repo.updated_at),
+            mtime=make_valid_timestamp(repo.updated_at),
             url=repo.url,
             watchers=repo.watchers,
             watchers_count=repo.watchers_count,
             clones_traffic=GithubRepoClonesTraffic.new(get_clones_traffic(repo)),
             views_traffic=GithubRepoViewsTraffic.new(get_views_traffic(repo)),
             top_referrers=[GithubRepoTopReferrer.new(referrer) for referrer in get_top_referrers(repo)],
             top_paths=[GithubRepoTopPath.new(path) for path in get_top_paths(repo)],
```

### Comparing `resoto-plugin-github-3.3.3/resoto_plugin_github.egg-info/PKG-INFO` & `resoto-plugin-github-3.3.4/resoto_plugin_github.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto Github Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.3.3/setup.py` & `resoto-plugin-github-3.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-github",
-    version="3.3.3",
+    version="3.3.4",
     description="Resoto Github Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["github = resoto_plugin_github:GithubCollectorPlugin"]},
     include_package_data=True,
```

