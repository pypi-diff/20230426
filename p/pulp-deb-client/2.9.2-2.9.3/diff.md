# Comparing `tmp/pulp_deb-client-2.9.2.tar.gz` & `tmp/pulp_deb-client-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp_deb-client-2.9.2.tar", last modified: Tue May 25 14:44:51 2021, max compression
+gzip compressed data, was "dist/pulp_deb-client-2.9.3.tar", last modified: Tue Nov 16 09:49:35 2021, max compression
```

## Comparing `pulp_deb-client-2.9.2.tar` & `pulp_deb-client-2.9.3.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16669 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7920 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulp_deb_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/
--rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22619 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_generic_contents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23577 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_installer_file_indices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26700 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_installer_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    24011 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_package_indices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21864 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_package_release_components_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    25992 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    22025 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_architectures_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21794 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_components_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23508 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_files_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23299 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_releases_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    39656 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/distributions_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28983 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/publications_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28462 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/publications_verbatim_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    39954 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/remotes_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    50516 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/repositories_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    31278 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/repositories_deb_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26274 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13952 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5072 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6454 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     9144 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7026 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     8841 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    26987 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    30368 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6108 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_base_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    31719 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_base_package_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6331 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_generic_content.py
--rw-r--r--   0 runner    (1001) docker     (121)    10941 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_generic_content_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7924 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_installer_file_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     9771 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_installer_file_index_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7702 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     9501 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_index_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_release_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     6706 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_release_component_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_architecture.py
--rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_architecture_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4601 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     6336 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_component_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     9065 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_file_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6802 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4473 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_verbatim_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     6232 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_verbatim_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5560 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5606 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_base_package_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_generic_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5767 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_installer_file_index_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_package_index_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5882 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_package_release_component_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_architecture_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_component_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5606 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_file_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5514 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_verbatim_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    27189 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     4893 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6396 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7166 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12311 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:51.000000 pulp_deb-client-2.9.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_generic_contents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_installer_file_indices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_installer_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_package_indices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_package_release_components_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_release_architectures_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_release_components_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_release_files_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_content_releases_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_apt_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_base_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_base_package_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_generic_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_generic_content_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_installer_file_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_installer_file_index_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_package_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_package_index_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_package_release_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_package_release_component_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_architecture.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_architecture_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_component_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_file_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_release_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_verbatim_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_deb_verbatim_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_distributions_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_apt_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_apt_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_apt_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_apt_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_base_package_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_generic_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_installer_file_index_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_package_index_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_package_release_component_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_release_architecture_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_release_component_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_release_file_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_release_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_paginateddeb_verbatim_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_patcheddeb_apt_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_patcheddeb_apt_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_patcheddeb_apt_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_publications_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_publications_verbatim_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_remotes_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_repositories_apt_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-05-25 14:44:50.000000 pulp_deb-client-2.9.2/test/test_repositories_deb_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-05-25 14:44:49.000000 pulp_deb-client-2.9.2/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7920 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulp_deb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulpcore/client/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/
+-rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5606 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_base_package_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_release_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9771 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_installer_file_index_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7274 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26987 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5790 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_architecture_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4601 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4481 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_package_index_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8841 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6706 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_release_component_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6281 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_component_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5790 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_verbatim_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7026 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5560 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30368 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4712 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5882 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_package_release_component_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5514 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7702 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9501 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_index_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2859 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3698 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9065 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10941 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_generic_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6802 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9144 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_architecture_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4893 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7166 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7924 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_installer_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8408 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6331 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_generic_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_generic_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6108 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_base_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6232 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_verbatim_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5072 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6454 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27189 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6396 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4473 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_verbatim_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6336 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_component_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5606 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_file_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5767 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_installer_file_index_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31719 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_base_package_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26274 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13952 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12311 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/
+-rw-r--r--   0 runner    (1001) docker     (121)    23508 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28462 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/publications_verbatim_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22025 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_architectures_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28983 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/publications_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23577 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_installer_file_indices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21864 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_package_release_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39954 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/remotes_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39656 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/distributions_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23299 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21794 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50516 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/repositories_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25992 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24011 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_package_indices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22619 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_generic_contents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26700 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_installer_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31278 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/repositories_deb_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:49:35.000000 pulp_deb-client-2.9.3/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_generic_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_apt_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_apt_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1911 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_package_release_component_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2318 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_installer_file_indices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_verbatim_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_release_file_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_patcheddeb_apt_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_verbatim_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2347 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_verbatim_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_package_index_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_remotes_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_package_index_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_patcheddeb_apt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_package_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_release_component_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_patcheddeb_apt_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1682 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_package_release_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repositories_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_release_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_release_architecture_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3697 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_base_package_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_generic_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_generic_contents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_release_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_architecture_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_distributions_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2123 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_installer_file_index_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2888 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_base_package_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_installer_file_index_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_package_release_component_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_installer_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_generic_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_package_indices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_publications_apt_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_release_architectures_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_apt_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_package_release_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_base_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_release_component_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_apt_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_repositories_deb_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_publications_verbatim_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-11-16 09:49:33.000000 pulp_deb-client-2.9.3/test/test_deb_apt_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_installer_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_content_releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/test/test_paginateddeb_release_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16669 2021-11-16 09:49:34.000000 pulp_deb-client-2.9.3/README.md
```

### Comparing `pulp_deb-client-2.9.2/README.md` & `pulp_deb-client-2.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_deb-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 2.9.2
+- Package version: 2.9.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_deb-client-2.9.2/pulp_deb_client.egg-info/SOURCES.txt` & `pulp_deb-client-2.9.3/pulp_deb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/__init__.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.9.2"
+__version__ = "2.9.3"
 
 # import apis into sdk package
 from pulpcore.client.pulp_deb.api.content_generic_contents_api import ContentGenericContentsApi
 from pulpcore.client.pulp_deb.api.content_installer_file_indices_api import ContentInstallerFileIndicesApi
 from pulpcore.client.pulp_deb.api.content_installer_packages_api import ContentInstallerPackagesApi
 from pulpcore.client.pulp_deb.api.content_package_indices_api import ContentPackageIndicesApi
 from pulpcore.client.pulp_deb.api.content_package_release_components_api import ContentPackageReleaseComponentsApi
```

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/__init__.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_generic_contents_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_generic_contents_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_installer_file_indices_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_installer_file_indices_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_installer_packages_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_installer_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_package_indices_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_package_indices_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_package_release_components_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_package_release_components_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_packages_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_architectures_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_architectures_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_components_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_components_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_release_files_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_release_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/content_releases_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/content_releases_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/distributions_apt_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/distributions_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/publications_apt_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/publications_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/publications_verbatim_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/publications_verbatim_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/remotes_apt_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/remotes_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/repositories_apt_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/repositories_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api/repositories_deb_versions_api.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api/repositories_deb_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/api_client.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.9.2/python'
+        self.user_agent = 'OpenAPI-Generator/2.9.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/configuration.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 2.9.2".\
+               "SDK Package Version: 2.9.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/exceptions.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/__init__.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/async_operation_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/content_summary.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/content_summary_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_distribution.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_distribution_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_publication.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_publication_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_remote.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_remote_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_repository.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_apt_repository_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_apt_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_base_package.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_base_package.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_base_package_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_base_package_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_generic_content.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_generic_content.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_generic_content_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_generic_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_installer_file_index.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_installer_file_index.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_installer_file_index_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_installer_file_index_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_index.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_index.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_index_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_index_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_release_component.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_release_component.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_package_release_component_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_package_release_component_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_architecture.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_architecture.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_architecture_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_architecture_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_component.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_component.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_component_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_component_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_file.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_file.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_file_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_file_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_release_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_release_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_verbatim_publication.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_verbatim_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/deb_verbatim_publication_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/deb_verbatim_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginated_repository_version_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_distribution_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_publication_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_remote_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_apt_repository_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_apt_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_base_package_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_base_package_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_generic_content_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_generic_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_installer_file_index_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_installer_file_index_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_package_index_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_package_index_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_package_release_component_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_package_release_component_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_architecture_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_architecture_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_component_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_component_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_file_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_file_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_release_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_release_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/paginateddeb_verbatim_publication_response_list.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/paginateddeb_verbatim_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_distribution.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_remote.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/patcheddeb_apt_repository.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/patcheddeb_apt_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/policy_enum.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_add_remove_content.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_sync_url.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_version.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/models/repository_version_response.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/pulpcore/client/pulp_deb/rest.py` & `pulp_deb-client-2.9.3/pulpcore/client/pulp_deb/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/setup.py` & `pulp_deb-client-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_deb-client"
-VERSION = "2.9.2"
+VERSION = "2.9.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_deb-client-2.9.2/test/test_async_operation_response.py` & `pulp_deb-client-2.9.3/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_generic_contents_api.py` & `pulp_deb-client-2.9.3/test/test_content_generic_contents_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_installer_file_indices_api.py` & `pulp_deb-client-2.9.3/test/test_content_installer_file_indices_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_installer_packages_api.py` & `pulp_deb-client-2.9.3/test/test_content_installer_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_package_indices_api.py` & `pulp_deb-client-2.9.3/test/test_content_package_indices_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_package_release_components_api.py` & `pulp_deb-client-2.9.3/test/test_content_package_release_components_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_packages_api.py` & `pulp_deb-client-2.9.3/test/test_content_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_release_architectures_api.py` & `pulp_deb-client-2.9.3/test/test_content_release_architectures_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_release_components_api.py` & `pulp_deb-client-2.9.3/test/test_content_release_components_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_release_files_api.py` & `pulp_deb-client-2.9.3/test/test_content_release_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_releases_api.py` & `pulp_deb-client-2.9.3/test/test_content_releases_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_summary.py` & `pulp_deb-client-2.9.3/test/test_content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_content_summary_response.py` & `pulp_deb-client-2.9.3/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_distribution.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_distribution_response.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_publication.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_publication_response.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_remote.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_remote_response.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_repository.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_apt_repository_response.py` & `pulp_deb-client-2.9.3/test/test_deb_apt_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_base_package.py` & `pulp_deb-client-2.9.3/test/test_deb_base_package.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_base_package_response.py` & `pulp_deb-client-2.9.3/test/test_deb_base_package_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_generic_content.py` & `pulp_deb-client-2.9.3/test/test_deb_generic_content.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_generic_content_response.py` & `pulp_deb-client-2.9.3/test/test_deb_generic_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_installer_file_index.py` & `pulp_deb-client-2.9.3/test/test_deb_installer_file_index.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_installer_file_index_response.py` & `pulp_deb-client-2.9.3/test/test_deb_installer_file_index_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_package_index.py` & `pulp_deb-client-2.9.3/test/test_deb_package_index.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_package_index_response.py` & `pulp_deb-client-2.9.3/test/test_deb_package_index_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_package_release_component.py` & `pulp_deb-client-2.9.3/test/test_deb_package_release_component.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_package_release_component_response.py` & `pulp_deb-client-2.9.3/test/test_deb_package_release_component_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release.py` & `pulp_deb-client-2.9.3/test/test_deb_release.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_architecture.py` & `pulp_deb-client-2.9.3/test/test_deb_release_architecture.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_architecture_response.py` & `pulp_deb-client-2.9.3/test/test_deb_release_architecture_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_component.py` & `pulp_deb-client-2.9.3/test/test_deb_release_component.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_component_response.py` & `pulp_deb-client-2.9.3/test/test_deb_release_component_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_file.py` & `pulp_deb-client-2.9.3/test/test_deb_release_file.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_file_response.py` & `pulp_deb-client-2.9.3/test/test_deb_release_file_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_release_response.py` & `pulp_deb-client-2.9.3/test/test_deb_release_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_verbatim_publication.py` & `pulp_deb-client-2.9.3/test/test_deb_verbatim_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_deb_verbatim_publication_response.py` & `pulp_deb-client-2.9.3/test/test_deb_verbatim_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_distributions_apt_api.py` & `pulp_deb-client-2.9.3/test/test_distributions_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginated_repository_version_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_apt_distribution_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_apt_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_apt_publication_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_apt_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_apt_remote_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_apt_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_apt_repository_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_apt_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_base_package_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_base_package_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_generic_content_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_generic_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_installer_file_index_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_installer_file_index_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_package_index_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_package_index_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_package_release_component_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_package_release_component_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_release_architecture_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_release_architecture_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_release_component_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_release_component_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_release_file_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_release_file_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_release_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_release_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_paginateddeb_verbatim_publication_response_list.py` & `pulp_deb-client-2.9.3/test/test_paginateddeb_verbatim_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_patcheddeb_apt_distribution.py` & `pulp_deb-client-2.9.3/test/test_patcheddeb_apt_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_patcheddeb_apt_remote.py` & `pulp_deb-client-2.9.3/test/test_patcheddeb_apt_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_patcheddeb_apt_repository.py` & `pulp_deb-client-2.9.3/test/test_patcheddeb_apt_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_policy_enum.py` & `pulp_deb-client-2.9.3/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_publications_apt_api.py` & `pulp_deb-client-2.9.3/test/test_publications_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_publications_verbatim_api.py` & `pulp_deb-client-2.9.3/test/test_publications_verbatim_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_remotes_apt_api.py` & `pulp_deb-client-2.9.3/test/test_remotes_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repositories_apt_api.py` & `pulp_deb-client-2.9.3/test/test_repositories_apt_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repositories_deb_versions_api.py` & `pulp_deb-client-2.9.3/test/test_repositories_deb_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repository_add_remove_content.py` & `pulp_deb-client-2.9.3/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repository_sync_url.py` & `pulp_deb-client-2.9.3/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repository_version.py` & `pulp_deb-client-2.9.3/test/test_repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_deb-client-2.9.2/test/test_repository_version_response.py` & `pulp_deb-client-2.9.3/test/test_repository_version_response.py`

 * *Files identical despite different names*

