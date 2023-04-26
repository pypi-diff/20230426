# Comparing `tmp/aa_structures-2.2.0.tar.gz` & `tmp/aa_structures-2.3.0.tar.gz`

## Comparing `aa_structures-2.2.0.tar` & `aa_structures-2.3.0.tar`

### file list

```diff
@@ -1,171 +1,176 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/__init__.py
--rw-r--r--   0        0        0    35982 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/admin.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/app_settings.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/apps.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/auth_hooks.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/checks.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/constants.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/forms.py
--rw-r--r--   0        0        0    18930 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/managers.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/providers.py
--rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/swagger.json
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tasks.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/urls.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/__init__.py
--rw-r--r--   0        0        0    71555 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/notification_embeds.py
--rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/notification_timers.py
--rw-r--r--   0        0        0    19834 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/serializers.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/starbases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/helpers/__init__.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/helpers/general.py
--rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    60908 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47014 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    55395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47024 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47177 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58666 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0    59315 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/__init__.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    42377 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/notifications.py
--rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/owners.py
--rw-r--r--   0        0        0    37246 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/structures.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/css/global.css
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/css/main.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/base.html
--rw-r--r--   0        0        0    21200 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/main.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/jump_gates_list.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/poco_list.html
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/structure_list.html
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/structure_summary.html
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/__init__.py
--rw-r--r--   0        0        0    20318 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_admin.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_checks.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    20151 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_integration.py
--rw-r--r--   0        0        0    26102 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_managers_3.py
--rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_tasks.py
--rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/__init__.py
--rw-r--r--   0        0        0    10982 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_embeds.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_embeds_2.py
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    38429 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31553 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    26807 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    54158 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    37407 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    37744 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   979813 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0    26820 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/core.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/managers.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_structures-2.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structures-2.2.0/LICENSE
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 aa_structures-2.2.0/README.md
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 aa_structures-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 aa_structures-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/__init__.py
+-rw-r--r--   0        0        0    36110 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/admin.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/app_settings.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/apps.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/auth_hooks.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/checks.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/constants.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/forms.py
+-rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/managers.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/swagger.json
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tasks.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/urls.py
+-rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/__init__.py
+-rw-r--r--   0        0        0    71519 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/notification_embeds.py
+-rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    19834 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/serializers.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/helpers/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/helpers/general.py
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/django.pot
+-rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    61204 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47274 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55691 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47267 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47437 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58962 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    59315 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/__init__.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    42691 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/notifications.py
+-rw-r--r--   0        0        0    53967 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/owners.py
+-rw-r--r--   0        0        0    37256 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/structures.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/__init__.py
+-rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_checks.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    20151 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    26102 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notification_embeds.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    38429 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31553 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26807 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54158 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37407 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37744 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26820 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_structures-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structures-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 aa_structures-2.3.0/README.md
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 aa_structures-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 aa_structures-2.3.0/PKG-INFO
```

### Comparing `aa_structures-2.2.0/structures/admin.py` & `aa_structures-2.3.0/structures/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         return False
 
 
 if settings.DEBUG:
 
     @admin.register(FuelAlert)
     class StructureFuelAlertAdmin(BaseFuelAlertAdmin):
-        list_display = BaseFuelAlertAdmin.list_display + ("hours",)
-        ordering = BaseFuelAlertAdmin.ordering + ("-hours",)
+        list_display = tuple(BaseFuelAlertAdmin.list_display) + ("hours",)
+        ordering = tuple(BaseFuelAlertAdmin.ordering) + ("-hours",)
 
     @admin.register(JumpFuelAlert)
     class JumpFuelAlertAdmin(BaseFuelAlertAdmin):
         pass
 
 
 class BaseFuelAlertConfigAdmin(admin.ModelAdmin):
@@ -124,46 +124,46 @@
 @admin.register(FuelAlertConfig)
 class StructureFuelAlertConfigAdmin(BaseFuelAlertConfigAdmin):
     list_display = (
         "_id",
         "start",
         "end",
         "repeat",
-    ) + BaseFuelAlertConfigAdmin.list_display
+    ) + tuple(BaseFuelAlertConfigAdmin.list_display)
     fieldsets = (
         (
-            "Timeing",
+            "Timing",
             {
                 "description": _(
                     "Timing configuration for sending fuel notifications. "
                     "Note that the first notification will be sent at the exact "
                     "start hour, and the last notification will be sent one repeat "
                     "before the end hour."
                 ),
                 "fields": ("start", "end", "repeat"),
             },
         ),
-    ) + BaseFuelAlertConfigAdmin.fieldsets
+    ) + tuple(BaseFuelAlertConfigAdmin.fieldsets)
 
 
 @admin.register(JumpFuelAlertConfig)
 class JumpFuelAlertConfigAdmin(BaseFuelAlertConfigAdmin):
     list_display = (
         "_id",
         "_threshold",
-    ) + BaseFuelAlertConfigAdmin.list_display
+    ) + tuple(BaseFuelAlertConfigAdmin.list_display)
     fieldsets = (
         (
             "Fuel levels",
             {
                 "description": ("tbd."),
                 "fields": ("threshold",),
             },
         ),
-    ) + BaseFuelAlertConfigAdmin.fieldsets
+    ) + tuple(BaseFuelAlertConfigAdmin.fieldsets)
 
     @admin.display(ordering="threshold")
     def _threshold(self, obj) -> str:
         return f"{obj.threshold:,}"
 
 
 class RenderableNotificationFilter(admin.SimpleListFilter):
@@ -469,51 +469,51 @@
     def deactivate_owners(self, request, queryset):
         queryset.update(is_active=False)
         self.message_user(request, f"Deactivated {queryset.count()} owners")
 
     @admin.display(description=_("Update all from EVE server for selected owners"))
     def update_all(self, request, queryset):
         for obj in queryset:
-            tasks.update_all_for_owner.delay(obj.pk, user_pk=request.user.pk)
+            tasks.update_all_for_owner.delay(obj.pk, user_pk=request.user.pk)  # type: ignore
             text = _(
                 "Started updating structures and notifications for %s. "
                 "You will receive a notification once it is completed." % obj
             )
             self.message_user(request, text)
 
     @admin.display(
         description=_("Update structures from EVE server for selected owners")
     )
     def update_structures(self, request, queryset):
         for obj in queryset:
-            tasks.update_structures_for_owner.delay(obj.pk, user_pk=request.user.pk)
+            tasks.update_structures_for_owner.delay(obj.pk, user_pk=request.user.pk)  # type: ignore
             text = (
                 f"Started updating structures for {obj}. "
                 "You will receive a notification once it is completed."
             )
             self.message_user(request, text)
 
     @admin.display(
         description=_("Fetch notifications from EVE server for selected owners")
     )
     def fetch_notifications(self, request, queryset):
         for obj in queryset:
-            tasks.process_notifications_for_owner.delay(obj.pk, user_pk=request.user.pk)
+            tasks.process_notifications_for_owner.delay(obj.pk, user_pk=request.user.pk)  # type: ignore
             text = (
                 f"Started fetching notifications for {obj}. "
                 "You will receive a notification once it is completed."
             )
             self.message_user(request, text)
 
     def has_add_permission(self, request):
         return False
 
     def get_readonly_fields(self, request, obj=None):
         if obj:  # editing an existing object
-            return self.readonly_fields + (
+            return tuple(self.readonly_fields) + (
                 "assets_last_update_at",
                 "corporation",
                 "forwarding_last_update_at",
                 "notifications_last_update_at",
                 "structures_last_update_at",
                 "_avg_turnaround_time",
                 "_are_all_syncs_ok",
@@ -1044,15 +1044,15 @@
         return obj.queue_size()
 
     @admin.display(description=_("Send test notification to selected webhook"))
     def test_notification(self, request, queryset):
         for obj in queryset:
             tasks.send_test_notifications_to_webhook.delay(
                 obj.pk, user_pk=request.user.pk
-            )
+            )  # type: ignore
             self.message_user(
                 request,
                 'Initiated sending test notification to webhook "{}". '
                 "You will receive a report on completion.".format(obj),
             )
 
     @admin.display(description=_("Activate selected webhook"))
@@ -1082,13 +1082,13 @@
             f"deleting a total of {killmails_deleted} messages.",
         )
 
     @admin.display(description=_("Send queued messages from selected webhooks"))
     def send_messages(self, request, queryset):
         items_count = 0
         for webhook in queryset:
-            tasks.send_messages_for_webhook.delay(webhook.pk)
+            tasks.send_messages_for_webhook.delay(webhook.pk)  # type: ignore
             items_count += 1
 
         self.message_user(
             request, f"Started sending queued messages for {items_count} webhooks."
         )
```

### Comparing `aa_structures-2.2.0/structures/app_settings.py` & `aa_structures-2.3.0/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/auth_hooks.py` & `aa_structures-2.3.0/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/checks.py` & `aa_structures-2.3.0/structures/checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/constants.py` & `aa_structures-2.3.0/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/managers.py` & `aa_structures-2.3.0/structures/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime as dt
 import itertools
-from typing import Optional, Set, Tuple
+from typing import Optional, Set, Tuple, TypeVar
 
 from django.contrib.auth.models import User
 from django.db import models, transaction
 from django.db.models import Case, Count, Exists, OuterRef, Q, Value, When
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
@@ -17,14 +17,16 @@
 from .app_settings import STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION
 from .constants import EveCategoryId, EveTypeId
 from .providers import esi
 from .webhooks.managers import WebhookBaseManager
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
+ModelType = TypeVar("ModelType", bound=models.Model)
+
 
 class EveSovereigntyMapManager(models.Manager):
     def update_from_esi(self):
         sov_map = esi.client.Sovereignty.get_sovereignty_map().results()
         logger.info("Retrieved sovereignty map from ESI")
         last_updated = now()
         obj_list = list()
@@ -49,32 +51,30 @@
         if obj_list:
             logger.info("Storing sovereignty map ...")
             with transaction.atomic():
                 self.all().delete()
                 self.bulk_create(obj_list, batch_size=1000)
 
     def corporation_has_sov(
-        self, eve_solar_system: models.Model, corporation: EveCorporationInfo
+        self, eve_solar_system, corporation: EveCorporationInfo
     ) -> bool:
         """returns true if given corporation has sov in this solar system
         else False
         """
         if not eve_solar_system.is_null_sec:
             return False
         else:
             alliance_id = (
                 int(corporation.alliance.alliance_id) if corporation.alliance else None
             )
             return bool(alliance_id) and (
                 self.solar_system_sov_alliance_id(eve_solar_system) == alliance_id
             )
 
-    def solar_system_sov_alliance_id(
-        self, eve_solar_system: models.Model
-    ) -> Optional[int]:
+    def solar_system_sov_alliance_id(self, eve_solar_system) -> Optional[int]:
         """returns ID of sov owning alliance for this system or None"""
         if not eve_solar_system.is_null_sec:
             return None
         try:
             sov_map = self.get(solar_system_id=eve_solar_system.id)
             return sov_map.alliance_id if sov_map.alliance_id else None
         except self.model.DoesNotExist:
@@ -129,26 +129,24 @@
 class GeneratedNotificationQuerySet(NotificationBaseQuerySet):
     pass
 
 
 class GeneratedNotificationManagerBase(NotificationBaseManagerBase):
     def get_or_create_from_structure(
         self, structure: models.Model, notif_type: models.TextChoices
-    ) -> Tuple[models.Model, bool]:
+    ) -> Tuple[ModelType, bool]:
         """Get or create an object from given structure."""
         from .models import NotificationType
 
         if notif_type not in {NotificationType.TOWER_REINFORCED_EXTRA}:
             raise ValueError(f"Unsupported notification type: {notif_type}")
 
         return self._get_or_create_tower_reinforced(structure)
 
-    def _get_or_create_tower_reinforced(
-        self, structure: models.Model
-    ) -> Tuple[models.Model, bool]:
+    def _get_or_create_tower_reinforced(self, structure) -> Tuple[ModelType, bool]:
         from .models import NotificationType
 
         if not structure.is_starbase:
             raise ValueError(f"Structure is not a starbase: {structure}")
         if not structure.is_reinforced:
             raise ValueError(f"Starbase is not reinforced: {structure}")
         if not structure.state_timer_end:
@@ -229,29 +227,31 @@
             "eve_planet",
             "eve_moon",
             "eve_type__eve_group",
             "eve_type__eve_group__eve_category",
         )
 
     # TODO: Add specific tests
-    def visible_for_user(self, user: User, tags: list = None) -> models.QuerySet:
+    def visible_for_user(
+        self, user: User, tags: Optional[list] = None
+    ) -> models.QuerySet:
         if user.has_perm("structures.view_all_structures"):
             structures_query = self.select_related_defaults()
             if tags:
                 structures_query = structures_query.filter(
                     tags__name__in=tags
                 ).distinct()
 
         else:
             if user.has_perm("structures.view_corporation_structures") or user.has_perm(
                 "structures.view_alliance_structures"
             ):
                 corporation_ids = {
                     character_ownership.character.corporation_id
-                    for character_ownership in user.character_ownerships.all()
+                    for character_ownership in user.character_ownerships.all()  # type: ignore
                 }
                 corporations = list(
                     EveCorporationInfo.objects.select_related("alliance").filter(
                         corporation_id__in=corporation_ids
                     )
                 )
             else:
@@ -458,15 +458,15 @@
             try:
                 obj = self.get(name=params["name"])
                 return obj, False
             except self.model.DoesNotExist:
                 return self.update_or_create_for_space_type(solar_system)
         return None, None
 
-    def update_or_create_for_space_type(self, solar_system: object) -> tuple:
+    def update_or_create_for_space_type(self, solar_system) -> tuple:
         from .models import EveSpaceType
 
         space_type = EveSpaceType.from_solar_system(solar_system)
         params = self.model.SPACE_TYPE_MAP.get(space_type)
         if params:
             return self.update_or_create(
                 name=params["name"],
```

### Comparing `aa_structures-2.2.0/structures/swagger.json` & `aa_structures-2.3.0/structures/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tasks.py` & `aa_structures-2.3.0/structures/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/urls.py` & `aa_structures-2.3.0/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/views.py` & `aa_structures-2.3.0/structures/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 from collections import defaultdict
 from enum import IntEnum
+from typing import Dict
 from urllib.parse import urlencode
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.db.models import Count, Q
 from django.http import HttpResponse, HttpResponseServerError, JsonResponse
 from django.shortcuts import get_object_or_404, redirect, render
@@ -350,15 +351,15 @@
     )
     fuels = structure.starbase_detail.fuels.select_related("eve_type").order_by(
         "eve_type__name"
     )
     assets = defaultdict(int)
     for item in structure.items.select_related("eve_type"):
         assets[item.eve_type_id] += item.quantity
-    eve_types = EveType.objects.in_bulk(id_list=assets.keys())
+    eve_types: Dict[int, EveType] = EveType.objects.in_bulk(id_list=assets.keys())
     modules = sorted(
         [
             {"eve_type": eve_types.get(eve_type_id), "quantity": quantity}
             for eve_type_id, quantity in assets.items()
         ],
         key=lambda obj: obj["eve_type"].name,
     )
@@ -428,15 +429,15 @@
         default_webhooks = Webhook.objects.filter(is_default=True)
         if default_webhooks:
             for webhook in default_webhooks:
                 owner.webhooks.add(webhook)
             owner.save()
 
     if owner.characters.count() == 1:
-        tasks.update_all_for_owner.delay(owner_pk=owner.pk, user_pk=request.user.pk)
+        tasks.update_all_for_owner.delay(owner_pk=owner.pk, user_pk=request.user.pk)  # type: ignore
         messages_plus.info(
             request,
             format_html(
                 _(
                     "%(corporation)s has been added with %(character)s "
                     "as sync character. "
                     "We have started fetching structures and notifications "
```

### Comparing `aa_structures-2.2.0/structures/core/notification_embeds.py` & `aa_structures-2.3.0/structures/core/notification_embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime as dt
 from collections import namedtuple
+from typing import Optional
 
 import dhooks_lite
 
 from django.conf import settings
 from django.db import models
 from django.template import Context, Template
 from django.utils.html import strip_tags
@@ -15,26 +16,27 @@
 from app_utils.datetime import (
     DATETIME_FORMAT,
     ldap_time_2_datetime,
     ldap_timedelta_2_timedelta,
 )
 from app_utils.urls import reverse_absolute, static_file_absolute_url
 
-from .. import __title__
-from ..app_settings import STRUCTURES_NOTIFICATION_SHOW_MOON_ORE
-from ..constants import EveTypeId
-from ..models.notifications import (
+from structures import __title__
+from structures.app_settings import STRUCTURES_NOTIFICATION_SHOW_MOON_ORE
+from structures.constants import EveTypeId
+from structures.models.notifications import (
     EveEntity,
     GeneratedNotification,
     Notification,
     NotificationBase,
     NotificationType,
     Webhook,
 )
-from ..models.structures import Structure
+from structures.models.structures import Structure
+
 from . import sovereignty, starbases
 
 
 class BillType(models.IntegerChoices):
     UNKNOWN = 0, gettext_lazy("Unknown Bill")
     INFRASTRUCTURE_HUB = 7, gettext_lazy("Infrastructure Hub Bill")
 
@@ -42,15 +44,15 @@
     def to_enum(cls, bill_id: int):
         try:
             return cls(bill_id)
         except ValueError:
             return cls.UNKNOWN
 
 
-def timeuntil(to_date: dt.datetime, from_date: dt.datetime = None) -> str:
+def timeuntil(to_date: dt.datetime, from_date: Optional[dt.datetime] = None) -> str:
     """Render timeuntil template tag for given datetime to string."""
     if not from_date:
         from_date = now()
     template = Template("{{ to_date|timeuntil:from_date }}")
     context = Context({"to_date": to_date, "from_date": from_date})
     return template.render(context)
 
@@ -73,15 +75,15 @@
     ICON_DEFAULT_SIZE = 64
 
     def __init__(self, notification: Notification) -> None:
         if not isinstance(notification, NotificationBase):
             raise TypeError("notification must be of type Notification")
         self._notification = notification
         self._parsed_text = notification.parsed_text()
-        self._title = None
+        self._title = ""
         self._description = ""
         self._color = None
         self._thumbnail = None
         self._ping_type = None
 
     def __str__(self) -> str:
         return str(self.notification)
@@ -90,31 +92,27 @@
         return "%s(notification=%r)" % (self.__class__.__name__, self.notification)
 
     @property
     def notification(self) -> Notification:
         return self._notification
 
     @property
-    def ping_type(self) -> Webhook.PingType:
+    def ping_type(self) -> Optional[Webhook.PingType]:
         return self._ping_type
 
     def generate_embed(self) -> dhooks_lite.Embed:
         """Returns generated Discord embed for this object.
 
         Will use custom color for embeds if self.notification has the \
             property "color_override" defined
 
         Will use custom ping type if self.notification has the \
             property "ping_type_override" defined
 
         """
-        if self._title is None:
-            raise ValueError(f"title not defined for {type(self)}")
-        if self._description is None:
-            raise ValueError(f"description not defined for {type(self)}")
         corporation = self.notification.owner.corporation
         if self.notification.is_alliance_level and corporation.alliance:
             author_name = corporation.alliance.alliance_name
             author_url = corporation.alliance.logo_url(size=self.ICON_DEFAULT_SIZE)
         else:
             author_name = corporation.corporation_name
             author_url = corporation.logo_url(size=self.ICON_DEFAULT_SIZE)
@@ -154,15 +152,15 @@
             footer=footer,
             timestamp=self.notification.timestamp,
             title=self._title,
             thumbnail=self._thumbnail,
         )
 
     @staticmethod
-    def create(notification: Notification) -> "NotificationBaseEmbed":
+    def create(notification: "NotificationBase") -> "NotificationBaseEmbed":
         """Creates a new instance of the respective subclass for given Notification."""
         if not isinstance(notification, NotificationBase):
             raise TypeError("notification must be of type NotificationBase")
         notif_type = notification.notif_type
 
         # character
         if notif_type == NotificationType.CORP_APP_NEW_MSG:
@@ -317,34 +315,35 @@
         return text
 
     @staticmethod
     def _gen_alliance_link(alliance_name: str) -> str:
         return Webhook.create_link(alliance_name, dotlan.alliance_url(alliance_name))
 
     @staticmethod
-    def _gen_eveentity_external_url(eve_entity: EveEntity) -> str:
+    def _gen_eve_entity_external_url(eve_entity: EveEntity) -> str:
         if eve_entity.category == EveEntity.CATEGORY_ALLIANCE:
             return dotlan.alliance_url(eve_entity.name)
         elif eve_entity.category == EveEntity.CATEGORY_CORPORATION:
             return dotlan.corporation_url(eve_entity.name)
         elif eve_entity.category == EveEntity.CATEGORY_CHARACTER:
             return evewho.character_url(eve_entity.id)
+        return ""
 
     @classmethod
-    def _gen_eveentity_link(cls, eve_entity: EveEntity) -> str:
+    def _gen_eve_entity_link(cls, eve_entity: EveEntity) -> str:
         return Webhook.create_link(
-            eve_entity.name, cls._gen_eveentity_external_url(eve_entity)
+            eve_entity.name, cls._gen_eve_entity_external_url(eve_entity)
         )
 
     @classmethod
-    def _gen_eveentity_link_from_id(cls, id: int) -> str:
+    def _gen_eve_entity_link_from_id(cls, id: int) -> str:
         if not id:
             return ""
         entity, _ = EveEntity.objects.get_or_create_esi(id=id)
-        return cls._gen_eveentity_link(entity)
+        return cls._gen_eve_entity_link(entity)
 
     @staticmethod
     def _gen_corporation_link(corporation_name: str) -> str:
         return Webhook.create_link(
             corporation_name, dotlan.corporation_url(corporation_name)
         )
 
@@ -728,15 +727,15 @@
         self._title = gettext("Moon mining extraction started")
         self._description = gettext(
             "A moon mining extraction has been started "
             "for %(structure_name)s at %(moon)s in %(solar_system)s "
             "belonging to %(owner_link)s. "
             "Extraction was started by %(character)s.\n"
             "The chunk will be ready on location at %(ready_time)s, "
-            "and will autofracture on %(auto_time)s.\n"
+            "and will fracture automatically on %(auto_time)s.\n"
             "%(ore_text)s"
         ) % {
             "structure_name": Webhook.text_bold(self._structure_name),
             "moon": self._moon.name,
             "solar_system": self._solar_system_link,
             "owner_link": self._owner_link,
             "character": started_by,
@@ -777,15 +776,15 @@
 
 
 class NotificationMoonminningAutomaticFracture(NotificationMoonminingEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         self._title = gettext("Automatic Fracture")
         self._description = gettext(
-            "The moondrill fitted to %(structure_name)s at %(moon)s"
+            "The moon drill fitted to %(structure_name)s at %(moon)s"
             " in %(solar_system)s belonging to %(owner_link)s "
             "has automatically been fired "
             "and the moon products are ready to be harvested.\n"
             "%(ore_text)s"
         ) % {
             "structure_name": Webhook.text_bold(self._structure_name),
             "moon": self._moon.name,
@@ -824,17 +823,17 @@
 
 class NotificationMoonminningLaserFired(NotificationMoonminingEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         fired_by, _ = EveEntity.objects.get_or_create_esi(
             id=self._parsed_text["firedBy"]
         )
-        self._title = gettext("Moondrill fired")
+        self._title = gettext("Moon drill fired")
         self._description = gettext(
-            "The moondrill fitted to %(structure_name)s at %(moon)s "
+            "The moon drill fitted to %(structure_name)s at %(moon)s "
             "in %(solar_system)s belonging to %(owner_link)s "
             "has been fired by %(character)s "
             "and the moon products are ready to be harvested.\n"
             "%(ore_text)s"
         ) % {
             "structure_name": Webhook.text_bold(self._structure_name),
             "moon": self._moon.name,
@@ -1165,15 +1164,15 @@
 
 class NotificationSovAllAnchoringMsg(NotificationBaseEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         corporation, _ = EveEntity.objects.get_or_create_esi(
             id=self._parsed_text.get("corpID")
         )
-        corp_link = self._gen_eveentity_link(corporation)
+        corp_link = self._gen_eve_entity_link(corporation)
         alliance_id = self._parsed_text.get("allianceID")
         if alliance_id:
             alliance, _ = EveEntity.objects.get_or_create_esi(id=alliance_id)
             structure_owner = f"{corp_link} ({alliance.name})"
         else:
             structure_owner = corp_link
         eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
@@ -1212,15 +1211,15 @@
         super().__init__(notification)
         self._character, _ = EveEntity.objects.get_or_create_esi(
             id=self._parsed_text["charID"]
         )
         self._corporation, _ = EveEntity.objects.get_or_create_esi(
             id=self._parsed_text["corpID"]
         )
-        self._character_link = self._gen_eveentity_link(self._character)
+        self._character_link = self._gen_eve_entity_link(self._character)
         self._corporation_link = self._gen_corporation_link(self._corporation.name)
         self._application_text = self._parsed_text.get("applicationText", "")
         self._thumbnail = dhooks_lite.Thumbnail(
             self._character.icon_url(size=self.ICON_DEFAULT_SIZE)
         )
 
 
@@ -1244,15 +1243,15 @@
 
 class NotificationCorpAppInvitedMsg(NotificationCorpCharEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         self._title = "%(character_name)s has been invited" % {
             "character_name": self._character.name
         }
-        inviting_character = self._gen_eveentity_link_from_id(
+        inviting_character = self._gen_eve_entity_link_from_id(
             self._parsed_text.get("invokingCharID")
         )
         self._description = (
             "%(character_name)s has been invited to join %(corporation_name)s "
             "by %(inviting_character)s.\n"
             "Application:\n"
             "> %(application_text)s"
@@ -1352,17 +1351,17 @@
             id=self._parsed_text["defenderID"]
         )
         start_time = ldap_time_2_datetime(self._parsed_text["startTime"])
         self._description = (
             "%(ally)s has joined %(defender)s in a war against %(aggressor)s. "
             "Their participation in the war will start at %(start_time)s."
         ) % {
-            "aggressor": self._gen_eveentity_link(aggressor),
-            "ally": self._gen_eveentity_link(ally),
-            "defender": self._gen_eveentity_link(defender),
+            "aggressor": self._gen_eve_entity_link(aggressor),
+            "ally": self._gen_eve_entity_link(ally),
+            "defender": self._gen_eve_entity_link(defender),
             "start_time": target_datetime_formatted(start_time),
         }
         self._thumbnail = dhooks_lite.Thumbnail(
             ally.icon_url(size=self.ICON_DEFAULT_SIZE)
         )
         self._color = Webhook.Color.WARNING
 
@@ -1386,16 +1385,16 @@
         super().__init__(notification)
         self._title = "One party has surrendered"
         self._description = (
             "The war between %(against)s and %(declared_by)s is coming to an end "
             "as one party has surrendered. "
             "The war will be declared as being over after approximately 24 hours."
         ) % {
-            "declared_by": self._gen_eveentity_link(self._declared_by),
-            "against": self._gen_eveentity_link(self._against),
+            "declared_by": self._gen_eve_entity_link(self._declared_by),
+            "against": self._gen_eve_entity_link(self._against),
         }
         self._color = Webhook.Color.WARNING
 
 
 class NotificationWarAdopted(NotificationWarEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
@@ -1408,17 +1407,17 @@
         }
         self._description = (
             "There has been a development in the war between %(declared_by)s "
             "and %(alliance)s.\n"
             "%(against)s is no longer a member of %(alliance)s, "
             "and therefore a new war between %(declared_by)s and %(against)s has begun."
         ) % {
-            "declared_by": self._gen_eveentity_link(self._declared_by),
-            "against": self._gen_eveentity_link(self._against),
-            "alliance": self._gen_eveentity_link(alliance),
+            "declared_by": self._gen_eve_entity_link(self._declared_by),
+            "against": self._gen_eve_entity_link(self._against),
+            "alliance": self._gen_eve_entity_link(alliance),
         }
         self._color = Webhook.Color.WARNING
 
 
 class NotificationWarDeclared(NotificationWarEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
@@ -1428,16 +1427,16 @@
         }
         self._description = (
             "%(declared_by)s has declared war on %(against)s with %(war_hq)s "
             "as the designated war headquarters.\n"
             "Within %(delay_hours)s hours fighting can legally occur "
             "between those involved."
         ) % {
-            "declared_by": self._gen_eveentity_link(self._declared_by),
-            "against": self._gen_eveentity_link(self._against),
+            "declared_by": self._gen_eve_entity_link(self._declared_by),
+            "against": self._gen_eve_entity_link(self._against),
             "war_hq": Webhook.text_bold(strip_tags(self._parsed_text["warHQ"])),
             "delay_hours": Webhook.text_bold(self._parsed_text["delayHours"]),
         }
         self._color = Webhook.Color.DANGER
 
 
 class NotificationWarInherited(NotificationWarEmbed):
@@ -1457,18 +1456,18 @@
             "opponent": opponent.name,
         }
         self._description = (
             "%(alliance)s has inherited the war between %(declared_by)s and "
             "%(against)s from newly joined %(quitter)s. "
             "Within **24** hours fighting can legally occur with %(alliance)s."
         ) % {
-            "declared_by": self._gen_eveentity_link(self._declared_by),
-            "against": self._gen_eveentity_link(self._against),
-            "alliance": self._gen_eveentity_link(alliance),
-            "quitter": self._gen_eveentity_link(quitter),
+            "declared_by": self._gen_eve_entity_link(self._declared_by),
+            "against": self._gen_eve_entity_link(self._against),
+            "alliance": self._gen_eve_entity_link(alliance),
+            "quitter": self._gen_eve_entity_link(quitter),
         }
         self._color = Webhook.Color.DANGER
 
 
 class NotificationWarRetractedByConcord(NotificationWarEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
@@ -1476,16 +1475,16 @@
         war_ends = ldap_time_2_datetime(self._parsed_text["endDate"])
         self._description = (
             "The war between %(declared_by)s and %(against)s "
             "has been retracted by CONCORD.\n"
             "After %(end_date)s CONCORD will again respond to any hostilities "
             "between those involved with full force."
         ) % {
-            "declared_by": self._gen_eveentity_link(self._declared_by),
-            "against": self._gen_eveentity_link(self._against),
+            "declared_by": self._gen_eve_entity_link(self._declared_by),
+            "against": self._gen_eve_entity_link(self._against),
             "end_date": target_datetime_formatted(war_ends),
         }
         self._color = Webhook.Color.WARNING
 
 
 class NotificationWarCorporationBecameEligible(NotificationBaseEmbed):
     def __init__(self, notification: Notification) -> None:
@@ -1522,38 +1521,39 @@
 class NotificationWarSurrenderOfferMsg(NotificationBaseEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         isk_value = self._parsed_text.get("iskValue", 0)
         owner_1, _ = EveEntity.objects.get_or_create_esi(
             id=self._parsed_text.get("ownerID1")
         )
-        owner_1_link = self._gen_eveentity_link(owner_1)
-        owner_2_link = self._gen_eveentity_link_from_id(
+        owner_1_link = self._gen_eve_entity_link(owner_1)
+        owner_2_link = self._gen_eve_entity_link_from_id(
             self._parsed_text.get("ownerID2")
         )
         self._title = gettext("%s has offered a surrender") % (owner_1,)
         self._description = gettext(
             "%s has offered to end the war with %s in the exchange for %s ISK. "
-            "If accepted, the war will end in 24 hours and your organizations will"
+            "If accepted, the war will end in 24 hours and your organizations will "
             "be unable to declare new wars against each other for the next 2 weeks."
         ) % (owner_1_link, owner_2_link, f"{isk_value:,.2f}")
         self._color = Webhook.Color.INFO
 
 
 class NotificationBillingBillOutOfMoneyMsg(NotificationBaseEmbed):
     def __init__(self, notification: Notification) -> None:
         super().__init__(notification)
         bill_type_id = self._parsed_text["billTypeID"]
         bill_type_str = BillType.to_enum(bill_type_id).label
         due_date = ldap_time_2_datetime(self._parsed_text["dueDate"])
         self._title = gettext("Insufficient Funds for Bill")
         self._description = gettext(
-            "The selected corporation wallet division for autopayments does not have "
-            "enough current funds available to pay the %(bill_type)s "
-            "due to be paid by %(due_date)s. Transfer additional funds to the selected wallet "
+            "The selected corporation wallet division for automatic payments "
+            "does not have enough current funds available to pay the %(bill_type)s "
+            "due to be paid by %(due_date)s. "
+            "Transfer additional funds to the selected wallet "
             "division in order to meet your pending automatic bills."
         ) % {
             "bill_type": bill_type_str,
             "due_date": target_datetime_formatted(due_date),
         }
         self._color = Webhook.Color.WARNING
```

### Comparing `aa_structures-2.2.0/structures/core/notification_timers.py` & `aa_structures-2.3.0/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/core/serializers.py` & `aa_structures-2.3.0/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/core/sovereignty.py` & `aa_structures-2.3.0/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/core/starbases.py` & `aa_structures-2.3.0/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/helpers/general.py` & `aa_structures-2.3.0/structures/helpers/general.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,37 @@
 # Erik Kalkoken <erik.kalkoken@gmail.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-17 02:47+0200\n"
+"POT-Creation-Date: 2023-04-24 23:05+0200\n"
 "PO-Revision-Date: 2020-03-09 19:25+0000\n"
 "Last-Translator: Erik Kalkoken <erik.kalkoken@gmail.com>, 2020\n"
 "Language-Team: German (Germany) (https://www.transifex.com/kalkoken-apps/"
 "teams/107978/de_DE/)\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:111
 msgid "Sent fuel notifications for selected configuration"
 msgstr ""
 
-#: admin.py:240 models/structures.py:162
+#: admin.py:137
+msgid ""
+"Timing configuration for sending fuel notifications. Note that the first "
+"notification will be sent at the exact start hour, and the last notification "
+"will be sent one repeat before the end hour."
+msgstr ""
+
+#: admin.py:240 models/structures.py:163
 msgid "N/A"
 msgstr "n.z."
 
 #: admin.py:255
 msgid "Not configured"
 msgstr ""
 
@@ -312,31 +319,31 @@
 #, python-format
 msgid ""
 "\n"
 "\n"
 "Change becomes effective at %s."
 msgstr ""
 
-#: core/notification_embeds.py:728 models/notifications.py:97
+#: core/notification_embeds.py:728 models/notifications.py:99
 msgid "Moon mining extraction started"
 msgstr "Mondmining Extraktion gestartet"
 
 #: core/notification_embeds.py:730
 #, fuzzy, python-format
 #| msgid ""
 #| "A moon mining extraction has been started for %(structure_name)s at "
 #| "%(moon)s in %(solar_system)s. Extraction was started by %(character)s.\n"
 #| "The chunk will be ready on location at %(ready_time)s, and will "
 #| "autofracture on %(auto_time)s.\n"
 msgid ""
 "A moon mining extraction has been started for %(structure_name)s at %(moon)s "
 "in %(solar_system)s belonging to %(owner_link)s. Extraction was started by "
 "%(character)s.\n"
-"The chunk will be ready on location at %(ready_time)s, and will autofracture "
-"on %(auto_time)s.\n"
+"The chunk will be ready on location at %(ready_time)s, and will fracture "
+"automatically on %(auto_time)s.\n"
 "%(ore_text)s"
 msgstr ""
 "Eine Mondmining Extraktion wurde begonnen auf %(structure_name)s an %(moon)s "
 "in %(solar_system)s. Extraktion wurde gestartet durch %(character)s. Der "
 "Brocken wird am %(ready_time)s bereit sein und wird automatisch am "
 "%(auto_time)s zerlegt.\n"
 
@@ -384,15 +391,15 @@
 #: core/notification_embeds.py:784
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has automatically been fired and the moon products are "
 #| "ready to be harvested.\n"
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has automatically been fired and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "Der Mondbohrer von %(structure_name)s bei %(moon)s in %(solar_system)s hat "
 "automatisch gefeuert und die Asteroiden können nun abgebaut werden.\n"
 
@@ -409,25 +416,27 @@
 "An ongoing extraction for %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been cancelled by %(character)s."
 msgstr ""
 "Die laufende Förderung durch %(structure_name)s bei %(moon)s in "
 "%(solar_system)s wurde abgebrochen von %(character)s."
 
 #: core/notification_embeds.py:831
-msgid "Moondrill fired"
+#, fuzzy
+#| msgid "Moondrill fired"
+msgid "Moon drill fired"
 msgstr "Mondbohrer hat gefeuert"
 
 #: core/notification_embeds.py:833
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has been fired by %(character)s and the moon products "
 #| "are ready to be harvested."
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been fired by %(character)s and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "Der Mondbohrer von %(structure_name)s bei %(moon)s in %(solar_system)s wurde "
 "abgefeuert von %(character)s und die Asteroiden sind bereit um abgebaut zu "
 "werden."
@@ -461,15 +470,15 @@
 "The %(structure_type)s at %(planet)s in %(solar_system)s belonging to "
 "%(owner_link)s has been reinforced by %(aggressor)s and will come out at: "
 "%(date)s."
 msgstr ""
 "Die %(structure_type)s bei %(planet)s in %(solar_system)s wurde beschädigt "
 "von %(aggressor)s und wird wieder verwundbar sein am %(date)s."
 
-#: core/notification_embeds.py:935 core/notification_embeds.py:1630
+#: core/notification_embeds.py:935 core/notification_embeds.py:1631
 #, fuzzy, python-format
 #| msgid ""
 #| "The starbase %(structure_name)s at %(moon)s in %(solar_system)s is low on "
 #| "fuel. It has %(quantity)d fuel blocks left."
 msgid ""
 "The starbase %(structure_name)s at %(moon)s in %(solar_system)s belonging to "
 "%(owner_link)s "
@@ -491,15 +500,15 @@
 "is under attack by %(aggressor)s.\n"
 "%(damage_text)s"
 msgstr ""
 "Die Sternenbasis %(structure_name)s an %(moon)s in %(solar_system)s wird "
 "angegriffen von %(aggressor)s\n"
 "%(damage_text)s"
 
-#: core/notification_embeds.py:982 models/notifications.py:91
+#: core/notification_embeds.py:982 models/notifications.py:93
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Starbase fuel alert"
 msgstr "Struktur Treibstoffalarm"
 
 #: core/notification_embeds.py:996
 #, fuzzy
@@ -628,62 +637,62 @@
 msgid "%s has offered a surrender"
 msgstr ""
 
 #: core/notification_embeds.py:1535
 #, python-format
 msgid ""
 "%s has offered to end the war with %s in the exchange for %s ISK. If "
-"accepted, the war will end in 24 hours and your organizations willbe unable "
+"accepted, the war will end in 24 hours and your organizations will be unable "
 "to declare new wars against each other for the next 2 weeks."
 msgstr ""
 
 #: core/notification_embeds.py:1548
 msgid "Insufficient Funds for Bill"
 msgstr ""
 
 #: core/notification_embeds.py:1550
 #, python-format
 msgid ""
-"The selected corporation wallet division for autopayments does not have "
-"enough current funds available to pay the %(bill_type)s due to be paid by "
-"%(due_date)s. Transfer additional funds to the selected wallet division in "
-"order to meet your pending automatic bills."
+"The selected corporation wallet division for automatic payments does not "
+"have enough current funds available to pay the %(bill_type)s due to be paid "
+"by %(due_date)s. Transfer additional funds to the selected wallet division "
+"in order to meet your pending automatic bills."
 msgstr ""
 
-#: core/notification_embeds.py:1569
+#: core/notification_embeds.py:1570
 msgid "IHub Bill About to Expire"
 msgstr ""
 
-#: core/notification_embeds.py:1571
+#: core/notification_embeds.py:1572
 #, python-format
 msgid ""
 "Maintenance bill for Infrastructure Hub in %(solar_system)s expires at "
 "%(due_date)s, if not paid in time this Infrastructure Hub will self-destruct."
 msgstr ""
 
-#: core/notification_embeds.py:1596
+#: core/notification_embeds.py:1597
 #, python-format
 msgid "%s has self-destructed due to unpaid maintenance bills"
 msgstr ""
 
-#: core/notification_embeds.py:1600
+#: core/notification_embeds.py:1601
 #, fuzzy, python-format
 #| msgid "%(structure_type)s in %(solar_system)s has entered reinforced mode"
 msgid ""
 "%(structure_type)s in %(solar_system)s has self-destructed, as the standard "
 "maintenance bills where not paid."
 msgstr "%(structure_type)s in %(solar_system)s wurde beschädigt"
 
-#: core/notification_embeds.py:1645
+#: core/notification_embeds.py:1646
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced"
 msgstr "Orbital beschädigt"
 
-#: core/notification_embeds.py:1653
+#: core/notification_embeds.py:1654
 #, python-format
 msgid "has been reinforced and will come out at: %s."
 msgstr ""
 
 #: core/notification_timers.py:89
 msgid "Armor timer"
 msgstr "Panzerungstimer"
@@ -705,1254 +714,1254 @@
 msgid "yes"
 msgstr "ja"
 
 #: core/serializers.py:496
 msgid "no"
 msgstr "nein"
 
-#: models/notifications.py:41
+#: models/notifications.py:43
 msgid "English"
 msgstr "Englisch"
 
-#: models/notifications.py:42
+#: models/notifications.py:44
 msgid "German"
 msgstr "Deutsch"
 
-#: models/notifications.py:43
+#: models/notifications.py:45
 msgid "Spanish"
 msgstr "Spanisch"
 
-#: models/notifications.py:44
+#: models/notifications.py:46
 msgid "Chinese Simplified"
 msgstr "Chinesisch"
 
-#: models/notifications.py:45
+#: models/notifications.py:47
 msgid "Russian"
 msgstr "Russisch"
 
-#: models/notifications.py:46
+#: models/notifications.py:48
 msgid "Korean"
 msgstr "Koreanisch"
 
-#: models/notifications.py:54
+#: models/notifications.py:56
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Upwell structure anchoring"
 msgstr "Struktur verankert"
 
-#: models/notifications.py:55
+#: models/notifications.py:57
 #, fuzzy
 #| msgid "Structure online"
 msgid "Upwell structure went online"
 msgstr "Struktur online"
 
-#: models/notifications.py:57
+#: models/notifications.py:59
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Upwell structure services went offline"
 msgstr "Struktur Services sind offline"
 
-#: models/notifications.py:60
+#: models/notifications.py:62
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went high power"
 msgstr "Struktur im Niedrigenergiemodus"
 
-#: models/notifications.py:63
+#: models/notifications.py:65
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went low power"
 msgstr "Struktur im Niedrigenergiemodus"
 
-#: models/notifications.py:65
+#: models/notifications.py:67
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Upwell structure unanchoring"
 msgstr "Struktur entankert"
 
-#: models/notifications.py:66
+#: models/notifications.py:68
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure fuel alert"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:67
+#: models/notifications.py:69
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure refueled"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:69
+#: models/notifications.py:71
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure jump fuel alert"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:72
+#: models/notifications.py:74
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "Upwell structure is under attack"
 msgstr "Struktur wird angegriffen"
 
-#: models/notifications.py:74
+#: models/notifications.py:76
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "Upwell structure lost shields"
 msgstr "Struktur hat die Schilde verloren"
 
-#: models/notifications.py:75
+#: models/notifications.py:77
 #, fuzzy
 #| msgid "Structure lost armor"
 msgid "Upwell structure lost armor"
 msgstr "Struktur hat die Panzerung verloren"
 
-#: models/notifications.py:76
+#: models/notifications.py:78
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Upwell structure destroyed"
 msgstr "Struktur zerstört"
 
-#: models/notifications.py:79
+#: models/notifications.py:81
 msgid "Upwell structure reinforcement time changed"
 msgstr ""
 
-#: models/notifications.py:82
+#: models/notifications.py:84
 #, fuzzy
 #| msgid "Ownership transferred"
 msgid "Upwell structure ownership transferred"
 msgstr "Besitzer geändert"
 
-#: models/notifications.py:86
+#: models/notifications.py:88
 msgid "Customs office attacked"
 msgstr ""
 
-#: models/notifications.py:87
+#: models/notifications.py:89
 #, fuzzy
 #| msgid "armor reinforce"
 msgid "Customs office reinforced"
 msgstr "Panzerung verwundet"
 
-#: models/notifications.py:90
+#: models/notifications.py:92
 #, fuzzy
 #| msgid "Starbase under attack"
 msgid "Starbase attacked"
 msgstr "Sternenbasis wird angegriffen"
 
-#: models/notifications.py:92
+#: models/notifications.py:94
 msgid "Starbase refueled (BETA)"
 msgstr ""
 
-#: models/notifications.py:93
+#: models/notifications.py:95
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced (BETA)"
 msgstr "Orbital beschädigt"
 
-#: models/notifications.py:99
+#: models/notifications.py:101
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moonmining laser fired"
 msgstr "Mondmining Extraktion gestartet"
 
-#: models/notifications.py:101
+#: models/notifications.py:103
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction cancelled"
 msgstr "Mondmining Extraktion gestartet"
 
-#: models/notifications.py:104
+#: models/notifications.py:106
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction finished"
 msgstr "Mondmining Extraktion gestartet"
 
-#: models/notifications.py:107
+#: models/notifications.py:109
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining automatic fracture triggered"
 msgstr "Mondmining Extraktion gestartet"
 
-#: models/notifications.py:112
+#: models/notifications.py:114
 msgid "Sovereignty structure reinforced"
 msgstr ""
 
-#: models/notifications.py:115
+#: models/notifications.py:117
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Sovereignty structure destroyed"
 msgstr "Struktur zerstört"
 
-#: models/notifications.py:118
+#: models/notifications.py:120
 msgid "Sovereignty entosis capture started"
 msgstr ""
 
-#: models/notifications.py:121
+#: models/notifications.py:123
 msgid "Sovereignty command node event started"
 msgstr ""
 
-#: models/notifications.py:124
+#: models/notifications.py:126
 #, fuzzy
 #| msgid "DED Sovereignty claim acknowledgment: %s"
 msgid "Sovereignty claim acknowledgment"
 msgstr "DED Souveränitätsanspruch anerkannt: %s "
 
-#: models/notifications.py:126
+#: models/notifications.py:128
 msgid "Sovereignty lost"
 msgstr ""
 
-#: models/notifications.py:128
+#: models/notifications.py:130
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Structure anchoring in alliance space"
 msgstr "Struktur verankert"
 
-#: models/notifications.py:132
+#: models/notifications.py:134
 msgid "War declared"
 msgstr ""
 
-#: models/notifications.py:134
+#: models/notifications.py:136
 msgid "War ally joined aggressor"
 msgstr ""
 
-#: models/notifications.py:136
+#: models/notifications.py:138
 msgid "War ally joined ally"
 msgstr ""
 
-#: models/notifications.py:138
+#: models/notifications.py:140
 msgid "War ally joined defender"
 msgstr ""
 
-#: models/notifications.py:140
+#: models/notifications.py:142
 msgid "War adopted"
 msgstr ""
 
-#: models/notifications.py:141
+#: models/notifications.py:143
 msgid "War inherited"
 msgstr ""
 
-#: models/notifications.py:142
+#: models/notifications.py:144
 msgid "War party surrendered"
 msgstr ""
 
-#: models/notifications.py:144
+#: models/notifications.py:146
 msgid "War retracted by Concord"
 msgstr ""
 
-#: models/notifications.py:147
+#: models/notifications.py:149
 msgid "War corporation became eligible"
 msgstr ""
 
-#: models/notifications.py:150
+#: models/notifications.py:152
 msgid "War corporation no longer eligible"
 msgstr ""
 
-#: models/notifications.py:152
+#: models/notifications.py:154
 msgid "War surrender offered"
 msgstr ""
 
-#: models/notifications.py:155
+#: models/notifications.py:157
 msgid "Character submitted application"
 msgstr ""
 
-#: models/notifications.py:157
+#: models/notifications.py:159
 msgid "Character invited to join corporation"
 msgstr ""
 
-#: models/notifications.py:160
+#: models/notifications.py:162
 msgid "Corp application rejected"
 msgstr ""
 
-#: models/notifications.py:162
+#: models/notifications.py:164
 msgid "Character withdrew application"
 msgstr ""
 
-#: models/notifications.py:163
+#: models/notifications.py:165
 msgid "Character joins corporation"
 msgstr ""
 
-#: models/notifications.py:164
+#: models/notifications.py:166
 msgid "Character leaves corporation"
 msgstr ""
 
-#: models/notifications.py:167
+#: models/notifications.py:169
 msgid "Bill out of money"
 msgstr ""
 
-#: models/notifications.py:170
+#: models/notifications.py:172
 msgid "I-HUB bill about to expire"
 msgstr ""
 
-#: models/notifications.py:174
+#: models/notifications.py:176
 msgid "I_HUB destroyed by bill failure"
 msgstr ""
 
-#: models/notifications.py:334
+#: models/notifications.py:336
 msgid "notification types"
 msgstr ""
 
-#: models/notifications.py:336
+#: models/notifications.py:338
 msgid "Select which type of notifications should be forwarded to this webhook"
 msgstr ""
 
-#: models/notifications.py:345
+#: models/notifications.py:347
 msgid "language"
 msgstr ""
 
-#: models/notifications.py:346
+#: models/notifications.py:348
 msgid "language of notifications send to this webhook"
 msgstr ""
 
-#: models/notifications.py:350 models/structures.py:91
+#: models/notifications.py:352 models/structures.py:92
 msgid "is default"
 msgstr ""
 
-#: models/notifications.py:352
+#: models/notifications.py:354
 msgid "Whether owners have this webhook automatically pre-set when created"
 msgstr ""
 
-#: models/notifications.py:357 models/owners.py:151
+#: models/notifications.py:359 models/owners.py:153
 msgid "has default pings enabled"
 msgstr ""
 
-#: models/notifications.py:368 models/owners.py:197
+#: models/notifications.py:370 models/owners.py:199
 msgid "ping groups"
 msgstr ""
 
-#: models/notifications.py:369
+#: models/notifications.py:371
 msgid "Groups to be pinged for each notification - "
 msgstr ""
 
-#: models/notifications.py:374
+#: models/notifications.py:376
 msgid "webhook"
 msgstr ""
 
-#: models/notifications.py:375 models/owners.py:212 models/structures.py:389
+#: models/notifications.py:377 models/owners.py:214 models/structures.py:390
 msgid "webhooks"
 msgstr ""
 
-#: models/notifications.py:388
+#: models/notifications.py:390
 msgid "is sent"
 msgstr ""
 
-#: models/notifications.py:389
+#: models/notifications.py:391
 msgid "True when this notification has been forwarded to Discord"
 msgstr ""
 
-#: models/notifications.py:394
+#: models/notifications.py:396
 msgid "is timer added"
 msgstr ""
 
-#: models/notifications.py:395
+#: models/notifications.py:397
 msgid "True when a timer has been added for this notification"
 msgstr ""
 
-#: models/notifications.py:401 models/structures.py:242
-#: models/structures.py:773
+#: models/notifications.py:403 models/structures.py:243
+#: models/structures.py:787
 msgid "type"
 msgstr ""
 
-#: models/notifications.py:402
+#: models/notifications.py:404
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "type of this notification"
 msgstr "%(ticker)s Benachrichtigungen"
 
-#: models/notifications.py:407 models/owners.py:219 models/owners.py:1278
-#: models/structures.py:312
+#: models/notifications.py:409 models/owners.py:221 models/owners.py:1287
+#: models/structures.py:313
 #, fuzzy
 #| msgid "Owner"
 msgid "owner"
 msgstr "Besitzer"
 
-#: models/notifications.py:408
+#: models/notifications.py:410
 msgid "Corporation that owns this notification"
 msgstr ""
 
-#: models/notifications.py:412 models/structures.py:402
+#: models/notifications.py:414 models/structures.py:403
 #, fuzzy
 #| msgid "Structure List"
 msgid "structures"
 msgstr "Strukturliste"
 
-#: models/notifications.py:413
+#: models/notifications.py:415
 msgid "Structures this notification is about (if any)"
 msgstr ""
 
-#: models/notifications.py:682 models/structures.py:202
-#: models/structures.py:759
+#: models/notifications.py:694 models/structures.py:203
+#: models/structures.py:773
 #, fuzzy
 #| msgid "d"
 msgid "id"
 msgstr "t"
 
-#: models/notifications.py:686
+#: models/notifications.py:698
 msgid "created"
 msgstr ""
 
-#: models/notifications.py:687
+#: models/notifications.py:699
 msgid "Date when this notification was first received from ESI"
 msgstr ""
 
-#: models/notifications.py:692
+#: models/notifications.py:704
 msgid "is read"
 msgstr ""
 
-#: models/notifications.py:693
+#: models/notifications.py:705
 msgid "True when this notification has read in the eve client"
 msgstr ""
 
-#: models/notifications.py:696
+#: models/notifications.py:708
 msgid "last updated"
 msgstr ""
 
-#: models/notifications.py:697
+#: models/notifications.py:709
 msgid "Date when this notification has last been updated from ESI"
 msgstr ""
 
-#: models/notifications.py:704
+#: models/notifications.py:716
 msgid "sender"
 msgstr ""
 
-#: models/notifications.py:711
+#: models/notifications.py:723
 msgid "text"
 msgstr ""
 
-#: models/notifications.py:712
+#: models/notifications.py:724
 msgid "Notification details in YAML"
 msgstr ""
 
-#: models/notifications.py:714 models/notifications.py:831
+#: models/notifications.py:726 models/notifications.py:843
 msgid "timestamp"
 msgstr ""
 
-#: models/notifications.py:719
+#: models/notifications.py:731
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "eve notification"
 msgstr "%(ticker)s Benachrichtigungen"
 
-#: models/notifications.py:720
+#: models/notifications.py:732
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "eve notifications"
 msgstr "%(ticker)s Benachrichtigungen"
 
-#: models/notifications.py:829
+#: models/notifications.py:841
 msgid "details"
 msgstr ""
 
-#: models/notifications.py:830
+#: models/notifications.py:842
 msgid "last_updated"
 msgstr ""
 
-#: models/notifications.py:836
+#: models/notifications.py:848
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "generated notification"
 msgstr "%(ticker)s Benachrichtigungen"
 
-#: models/notifications.py:837
+#: models/notifications.py:849
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "generated  notifications"
 msgstr "%(ticker)s Benachrichtigungen"
 
-#: models/notifications.py:866
+#: models/notifications.py:878
 msgid "channel pings"
 msgstr ""
 
-#: models/notifications.py:868
+#: models/notifications.py:880
 msgid ""
 "Option to ping every member of the channel. This setting can be overruled by "
 "the respective owner or webhook configuration"
 msgstr ""
 
-#: models/notifications.py:878
+#: models/notifications.py:890
 msgid "color"
 msgstr ""
 
-#: models/notifications.py:879
+#: models/notifications.py:891
 msgid "Context color of these notification on Discord"
 msgstr ""
 
-#: models/notifications.py:883
+#: models/notifications.py:895
 msgid "is_enabled"
 msgstr ""
 
-#: models/notifications.py:884
+#: models/notifications.py:896
 msgid "Disabled configurations will not create any new alerts."
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "end"
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "End of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:910
+#: models/notifications.py:922
 msgid "repeat"
 msgstr ""
 
-#: models/notifications.py:912
+#: models/notifications.py:924
 msgid "Notifications will be repeated every x hours. Set to 0 for no repeats"
 msgstr ""
 
-#: models/notifications.py:916
+#: models/notifications.py:928
 msgid "start"
 msgstr ""
 
-#: models/notifications.py:917
+#: models/notifications.py:929
 msgid "Start of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:921
+#: models/notifications.py:933
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert config"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:922
+#: models/notifications.py:934
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert configs"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:927
+#: models/notifications.py:941
 msgid "Start must be before end, i.e. have a larger value."
 msgstr ""
 
-#: models/notifications.py:931
+#: models/notifications.py:945
 msgid "Repeat can not be larger that the interval size."
 msgstr ""
 
-#: models/notifications.py:940
+#: models/notifications.py:954
 msgid "This configuration may not overlap with an existing configuration."
 msgstr ""
 
-#: models/notifications.py:1007
+#: models/notifications.py:1021
 msgid "threshold"
 msgstr ""
 
-#: models/notifications.py:1009
+#: models/notifications.py:1023
 msgid ""
 "Notifications will be sent once fuel level in units reaches this threshold"
 msgstr ""
 
-#: models/notifications.py:1014
+#: models/notifications.py:1028
 msgid "jump fuel alert config"
 msgstr ""
 
-#: models/notifications.py:1015
+#: models/notifications.py:1029
 msgid "jump fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:1064 models/notifications.py:1114
-#: models/structures.py:401 models/structures.py:765 models/structures.py:830
+#: models/notifications.py:1078 models/notifications.py:1128
+#: models/structures.py:402 models/structures.py:779 models/structures.py:844
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure"
 msgstr "Strukturliste"
 
-#: models/notifications.py:1070 models/notifications.py:1120
+#: models/notifications.py:1084 models/notifications.py:1134
 msgid "configuration"
 msgstr ""
 
-#: models/notifications.py:1074
+#: models/notifications.py:1088
 msgid "hours"
 msgstr ""
 
-#: models/notifications.py:1075
+#: models/notifications.py:1089
 msgid "number of hours before fuel expiration this alert was sent"
 msgstr ""
 
-#: models/notifications.py:1079
+#: models/notifications.py:1093
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:1080
+#: models/notifications.py:1094
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alerts"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:1124
+#: models/notifications.py:1138
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alert"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/notifications.py:1125
+#: models/notifications.py:1139
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alerts"
 msgstr "Struktur Treibstoffalarm"
 
-#: models/owners.py:117
+#: models/owners.py:119
 #, fuzzy
 #| msgid "Corporation"
 msgid "corporation"
 msgstr "Corporation"
 
-#: models/owners.py:118
+#: models/owners.py:120
 msgid "Corporation owning structures"
 msgstr ""
 
-#: models/owners.py:123
+#: models/owners.py:125
 msgid "are pocos public"
 msgstr ""
 
-#: models/owners.py:124
+#: models/owners.py:126
 msgid "whether pocos of this owner are shown on public POCO page"
 msgstr ""
 
-#: models/owners.py:130
+#: models/owners.py:132
 msgid "assets last update at"
 msgstr ""
 
-#: models/owners.py:131 models/owners.py:147 models/owners.py:190
-#: models/owners.py:205
+#: models/owners.py:133 models/owners.py:149 models/owners.py:192
+#: models/owners.py:207
 msgid "when the last successful update happened"
 msgstr ""
 
-#: models/owners.py:146
+#: models/owners.py:148
 msgid "forwarding last update at"
 msgstr ""
 
-#: models/owners.py:153
+#: models/owners.py:155
 msgid ""
 "to enable or disable pinging of notifications for this owner e.g. with "
 "@everyone and @here"
 msgstr ""
 
-#: models/owners.py:159
+#: models/owners.py:161
 msgid "is active"
 msgstr ""
 
-#: models/owners.py:160
+#: models/owners.py:162
 msgid "whether this owner is currently included in the sync process"
 msgstr ""
 
-#: models/owners.py:164
+#: models/owners.py:166
 #, fuzzy
 #| msgid "Alliance"
 msgid "is alliance main"
 msgstr "Allianz"
 
-#: models/owners.py:166
+#: models/owners.py:168
 msgid ""
 "whether alliance wide notifications are forwarded for this owner (e.g. sov "
 "notifications)"
 msgstr ""
 
-#: models/owners.py:172
+#: models/owners.py:174
 msgid "is included in service status"
 msgstr ""
 
-#: models/owners.py:174
+#: models/owners.py:176
 msgid ""
 "whether the sync status of this owner is included in the overall status of "
 "this services"
 msgstr ""
 
-#: models/owners.py:182
+#: models/owners.py:184
 msgid "is up"
 msgstr ""
 
-#: models/owners.py:183
+#: models/owners.py:185
 msgid "whether all services for this owner are currently up"
 msgstr ""
 
-#: models/owners.py:189
+#: models/owners.py:191
 msgid "notifications last update at"
 msgstr ""
 
-#: models/owners.py:198
+#: models/owners.py:200
 msgid "Groups to be pinged for each notification. "
 msgstr ""
 
-#: models/owners.py:204
+#: models/owners.py:206
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "structures last update at"
 msgstr "Struktur wird angegriffen"
 
-#: models/owners.py:213
+#: models/owners.py:215
 msgid "Notifications are sent to these webhooks."
 msgstr ""
 
-#: models/owners.py:220
+#: models/owners.py:222
 #, fuzzy
 #| msgid "Owner"
 msgid "owners"
 msgstr "Besitzer"
 
-#: models/owners.py:1139
+#: models/owners.py:1147
 #, fuzzy, python-format
 #| msgid ""
 #| "Syncing of %(topic)s for \"%(owner)s\" %(result)s.\n"
 #| "%(message_details)s"
 msgid ""
 "Syncing of %(topic)s for %(owner)s %(result)s.\n"
 " %(message_details)s"
 msgstr ""
 "Synchronisiere %(topic)s für \"%(owner)s\" %(result)s\n"
 "%(message_details)s"
 
-#: models/owners.py:1143
+#: models/owners.py:1151
 msgid "completed successfully"
 msgstr "erfolgreich beendet"
 
-#: models/owners.py:1148
+#: models/owners.py:1156
 #, python-format
 msgid "%(title)s: %(topic)s updated for %(owner)s: %(result)s"
 msgstr "%(title)s: %(topic)s aktualisiert für %(owner)s: %(result)s"
 
-#: models/owners.py:1153
+#: models/owners.py:1161
 msgid "OK"
 msgstr "OK"
 
-#: models/owners.py:1284
+#: models/owners.py:1293
 msgid "character_ownership"
 msgstr ""
 
-#: models/owners.py:1292
+#: models/owners.py:1301
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "structures last used at"
 msgstr "Struktur hat die Schilde verloren"
 
-#: models/owners.py:1300
+#: models/owners.py:1309
 msgid "notifications last used at"
 msgstr ""
 
-#: models/owners.py:1306
+#: models/owners.py:1315
 msgid "error count"
 msgstr ""
 
-#: models/owners.py:1312
+#: models/owners.py:1321
 msgid "owner character"
 msgstr ""
 
-#: models/owners.py:1313
+#: models/owners.py:1322
 msgid "owner characters"
 msgstr ""
 
-#: models/structures.py:37
+#: models/structures.py:38
 msgid "sov"
 msgstr ""
 
-#: models/structures.py:38
+#: models/structures.py:39
 msgid "highsec"
 msgstr ""
 
-#: models/structures.py:39
+#: models/structures.py:40
 msgid "lowsec"
 msgstr ""
 
-#: models/structures.py:40
+#: models/structures.py:41
 msgid "nullsec"
 msgstr ""
 
-#: models/structures.py:41
+#: models/structures.py:42
 msgid "w_space"
 msgstr ""
 
-#: models/structures.py:44
+#: models/structures.py:45
 msgid "grey"
 msgstr ""
 
-#: models/structures.py:45
+#: models/structures.py:46
 msgid "dark blue"
 msgstr ""
 
-#: models/structures.py:46
+#: models/structures.py:47
 msgid "green"
 msgstr ""
 
-#: models/structures.py:47
+#: models/structures.py:48
 msgid "light blue"
 msgstr ""
 
-#: models/structures.py:48
+#: models/structures.py:49
 msgid "orange"
 msgstr ""
 
-#: models/structures.py:49
+#: models/structures.py:50
 msgid "red"
 msgstr ""
 
-#: models/structures.py:61 models/structures.py:284 models/structures.py:834
+#: models/structures.py:62 models/structures.py:285 models/structures.py:848
 msgid "name"
 msgstr ""
 
-#: models/structures.py:62
+#: models/structures.py:63
 msgid "name of the tag - must be unique"
 msgstr ""
 
-#: models/structures.py:68
+#: models/structures.py:69
 msgid "description"
 msgstr ""
 
-#: models/structures.py:69
+#: models/structures.py:70
 msgid "description for this tag"
 msgstr ""
 
-#: models/structures.py:76
+#: models/structures.py:77
 msgid "style"
 msgstr ""
 
-#: models/structures.py:77
+#: models/structures.py:78
 msgid "color style of tag"
 msgstr ""
 
-#: models/structures.py:83
+#: models/structures.py:84
 msgid "order"
 msgstr ""
 
-#: models/structures.py:85
+#: models/structures.py:86
 msgid ""
 "number defining the order tags are shown. custom tags can not have an order "
 "below 100"
 msgstr ""
 
-#: models/structures.py:93
+#: models/structures.py:94
 msgid "if true this custom tag will automatically be added to new structures"
 msgstr ""
 
-#: models/structures.py:98
+#: models/structures.py:99
 msgid "is user managed"
 msgstr ""
 
-#: models/structures.py:100
+#: models/structures.py:101
 msgid ""
 "if False this tag is created and managed by the system and can not be "
 "modified by users"
 msgstr ""
 
-#: models/structures.py:108
+#: models/structures.py:109
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure tag"
 msgstr "Strukturliste"
 
-#: models/structures.py:109
+#: models/structures.py:110
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure tags"
 msgstr "Strukturliste"
 
-#: models/structures.py:143
+#: models/structures.py:144
 msgid "anchor vulnerable"
 msgstr "Stationierung verwundbar "
 
-#: models/structures.py:144
+#: models/structures.py:145
 msgid "anchoring"
 msgstr "verankert"
 
-#: models/structures.py:145
+#: models/structures.py:146
 msgid "armor reinforce"
 msgstr "Panzerung verwundet"
 
-#: models/structures.py:146
+#: models/structures.py:147
 msgid "armor vulnerable"
 msgstr "Panzerung verwundbar"
 
-#: models/structures.py:147
+#: models/structures.py:148
 msgid "deploy vulnerable"
 msgstr "Aufstellung verwundbar"
 
-#: models/structures.py:148
+#: models/structures.py:149
 msgid "fitting invulnerable"
 msgstr "Ausrüsten verwundbar"
 
-#: models/structures.py:149
+#: models/structures.py:150
 msgid "hull reinforce"
 msgstr "Rumpf verwundet"
 
-#: models/structures.py:150
+#: models/structures.py:151
 msgid "hull vulnerable"
 msgstr "Rumpf verwundbar"
 
-#: models/structures.py:151
+#: models/structures.py:152
 msgid "online deprecated"
 msgstr "online veraltet"
 
-#: models/structures.py:152
+#: models/structures.py:153
 msgid "onlining vulnerable"
 msgstr "Aktivierung verwundbar"
 
-#: models/structures.py:153
+#: models/structures.py:154
 msgid "shield vulnerable"
 msgstr "Schilde verwundbar"
 
-#: models/structures.py:154
+#: models/structures.py:155
 msgid "unanchored"
 msgstr "entankert"
 
-#: models/structures.py:156 models/structures.py:813
+#: models/structures.py:157 models/structures.py:827
 msgid "offline"
 msgstr "offline"
 
-#: models/structures.py:157 models/structures.py:814
+#: models/structures.py:158 models/structures.py:828
 msgid "online"
 msgstr "online"
 
-#: models/structures.py:158
+#: models/structures.py:159
 msgid "onlining"
 msgstr "Aktivierung"
 
-#: models/structures.py:159
+#: models/structures.py:160
 msgid "reinforced"
 msgstr "beschädigt"
 
-#: models/structures.py:160
+#: models/structures.py:161
 msgid "unanchoring "
 msgstr "entankert"
 
-#: models/structures.py:163
+#: models/structures.py:164
 msgid "unknown"
 msgstr "unbekannt"
 
-#: models/structures.py:194
+#: models/structures.py:195
 #, fuzzy
 #| msgid "Low Power"
 msgid "Full Power"
 msgstr "Niedrigenergie"
 
-#: models/structures.py:195
+#: models/structures.py:196
 msgid "Low Power"
 msgstr "Niedrigenergie"
 
-#: models/structures.py:196
+#: models/structures.py:197
 msgid "Abandoned"
 msgstr ""
 
-#: models/structures.py:197
+#: models/structures.py:198
 msgid "Abandoned?"
 msgstr ""
 
-#: models/structures.py:198
+#: models/structures.py:199
 #, fuzzy
 #| msgid "unknown"
 msgid "Unknown"
 msgstr "unbekannt"
 
-#: models/structures.py:203
+#: models/structures.py:204
 msgid "The Item ID of the structure"
 msgstr ""
 
-#: models/structures.py:208
+#: models/structures.py:209
 msgid "created at"
 msgstr ""
 
-#: models/structures.py:209
+#: models/structures.py:210
 msgid "date this structure was received from ESI for the first time"
 msgstr ""
 
-#: models/structures.py:218
+#: models/structures.py:219
 msgid "moon"
 msgstr ""
 
-#: models/structures.py:219
+#: models/structures.py:220
 msgid "Moon next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:228
+#: models/structures.py:229
 msgid "planet"
 msgstr ""
 
-#: models/structures.py:229
+#: models/structures.py:230
 msgid "Planet next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:235
+#: models/structures.py:236
 #, fuzzy
 #| msgid "Solar System"
 msgid "solar system"
 msgstr "Sonnensystem"
 
-#: models/structures.py:236
+#: models/structures.py:237
 msgid "Solar System the structure is located"
 msgstr ""
 
-#: models/structures.py:243
+#: models/structures.py:244
 msgid "Type of the structure"
 msgstr ""
 
-#: models/structures.py:249
+#: models/structures.py:250
 #, fuzzy
 #| msgid "Fuel Expires"
 msgid "fuel expires at"
 msgstr "Treibstoff verbraucht"
 
-#: models/structures.py:250
+#: models/structures.py:251
 msgid "Date on which the structure will run out of fuel"
 msgstr ""
 
-#: models/structures.py:257
+#: models/structures.py:258
 msgid "has fitting"
 msgstr ""
 
-#: models/structures.py:258
+#: models/structures.py:259
 msgid "bool indicating if the structure has a fitting"
 msgstr ""
 
-#: models/structures.py:265
+#: models/structures.py:266
 msgid "has core"
 msgstr ""
 
-#: models/structures.py:266
+#: models/structures.py:267
 msgid "bool indicating if the structure has a quantum core"
 msgstr ""
 
-#: models/structures.py:272
+#: models/structures.py:273
 #, fuzzy
 #| msgid "online"
 msgid "last online at"
 msgstr "online"
 
-#: models/structures.py:273
+#: models/structures.py:274
 msgid "date this structure had any of it's services online"
 msgstr ""
 
-#: models/structures.py:279 models/structures.py:778
+#: models/structures.py:280 models/structures.py:792
 msgid "last updated at"
 msgstr ""
 
-#: models/structures.py:280
+#: models/structures.py:281
 msgid "date this structure was last updated from the EVE server"
 msgstr ""
 
-#: models/structures.py:285
+#: models/structures.py:286
 msgid "The full name of the structure"
 msgstr ""
 
-#: models/structures.py:292
+#: models/structures.py:293
 #, fuzzy
 #| msgid "reinforced"
 msgid "next reinforce hour"
 msgstr "beschädigt"
 
-#: models/structures.py:294 models/structures.py:304
+#: models/structures.py:295 models/structures.py:305
 msgid ""
 "The requested change to reinforce_hour that will take effect at the time "
 "shown by next_reinforce_apply"
 msgstr ""
 
-#: models/structures.py:302
+#: models/structures.py:303
 #, fuzzy
 #| msgid "reinforced"
 msgid "next reinforce apply"
 msgstr "beschädigt"
 
-#: models/structures.py:313
+#: models/structures.py:314
 msgid "Corporation that owns the structure"
 msgstr ""
 
-#: models/structures.py:320
+#: models/structures.py:321
 #, fuzzy
 #| msgid "reinforced"
 msgid "reinforce hour"
 msgstr "beschädigt"
 
-#: models/structures.py:322
+#: models/structures.py:323
 msgid ""
 "The average hour of day that determines the time +/- some hours when the "
 "structure will randomly exit its reinforcement periods and become vulnerable "
 "to attack against its armor and/or hull. "
 msgstr ""
 
-#: models/structures.py:331
+#: models/structures.py:332
 msgid "position x"
 msgstr ""
 
-#: models/structures.py:332
+#: models/structures.py:333
 msgid "x position in the solar system"
 msgstr ""
 
-#: models/structures.py:338
+#: models/structures.py:339
 msgid "position y"
 msgstr ""
 
-#: models/structures.py:339
+#: models/structures.py:340
 msgid "y position in the solar system"
 msgstr ""
 
-#: models/structures.py:345
+#: models/structures.py:346
 msgid "position z"
 msgstr ""
 
-#: models/structures.py:346
+#: models/structures.py:347
 msgid "z position in the solar system"
 msgstr ""
 
-#: models/structures.py:352 models/structures.py:839
+#: models/structures.py:353 models/structures.py:853
 #, fuzzy
 #| msgid "State"
 msgid "state"
 msgstr "Status"
 
-#: models/structures.py:353
+#: models/structures.py:354
 msgid "Current state of the structure"
 msgstr ""
 
-#: models/structures.py:359
+#: models/structures.py:360
 msgid "state timer end"
 msgstr ""
 
-#: models/structures.py:360
+#: models/structures.py:361
 msgid "Date at which the structure entered it's current state"
 msgstr ""
 
-#: models/structures.py:366
+#: models/structures.py:367
 msgid "state timer start"
 msgstr ""
 
-#: models/structures.py:367
+#: models/structures.py:368
 msgid "Date at which the structure will move to it's next state"
 msgstr ""
 
-#: models/structures.py:374
+#: models/structures.py:375
 msgid "tags"
 msgstr ""
 
-#: models/structures.py:375
+#: models/structures.py:376
 msgid "List of tags for this structure. "
 msgstr ""
 
-#: models/structures.py:381
+#: models/structures.py:382
 #, fuzzy
 #| msgid "unanchoring "
 msgid "unanchors at"
 msgstr "entankert"
 
-#: models/structures.py:382
+#: models/structures.py:383
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Date at which the structure will unanchor"
 msgstr "Struktur entankert"
 
-#: models/structures.py:391
+#: models/structures.py:392
 msgid ""
 "Webhooks for sending notifications to. If any webhook is enabled, these will "
 "be used instead of the webhooks defined for the respective owner. If no "
 "webhook is enabled the owner's setting will be used. "
 msgstr ""
 
-#: models/structures.py:759
+#: models/structures.py:773
 msgid "The Eve item ID"
 msgstr ""
 
-#: models/structures.py:766
+#: models/structures.py:780
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this item is located in"
 msgstr "Struktur Services sind offline"
 
-#: models/structures.py:774
+#: models/structures.py:788
 msgid "type of the item"
 msgstr ""
 
-#: models/structures.py:776
+#: models/structures.py:790
 msgid "is singleton"
 msgstr ""
 
-#: models/structures.py:780
+#: models/structures.py:794
 #, fuzzy
 #| msgid "Location"
 msgid "location flag"
 msgstr "Ort"
 
-#: models/structures.py:781
+#: models/structures.py:795
 msgid "quantity"
 msgstr ""
 
-#: models/structures.py:784
+#: models/structures.py:798
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure item"
 msgstr "Strukturliste"
 
-#: models/structures.py:785
+#: models/structures.py:799
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure items"
 msgstr "Strukturliste"
 
-#: models/structures.py:831
+#: models/structures.py:845
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this service is installed to"
 msgstr "Struktur Services sind offline"
 
-#: models/structures.py:834
+#: models/structures.py:848
 msgid "Name of the service"
 msgstr ""
 
-#: models/structures.py:840
+#: models/structures.py:854
 msgid "Current state of this service"
 msgstr ""
 
-#: models/structures.py:844
+#: models/structures.py:858
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure service"
 msgstr "Strukturliste"
 
-#: models/structures.py:845
+#: models/structures.py:859
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "structure services"
 msgstr "Struktur Services sind offline"
 
-#: models/structures.py:861 webhooks/models.py:12
+#: models/structures.py:875 webhooks/models.py:12
 msgid "none"
 msgstr ""
 
-#: models/structures.py:862
+#: models/structures.py:876
 msgid "terrible"
 msgstr ""
 
-#: models/structures.py:863
+#: models/structures.py:877
 msgid "bad"
 msgstr ""
 
-#: models/structures.py:864
+#: models/structures.py:878
 msgid "neutral"
 msgstr ""
 
-#: models/structures.py:865
+#: models/structures.py:879
 msgid "good"
 msgstr ""
 
-#: models/structures.py:866
+#: models/structures.py:880
 msgid "excellent"
 msgstr ""
 
-#: models/structures.py:960
+#: models/structures.py:974
 #, fuzzy
 #| msgid "Alliance"
 msgid "alliance member"
 msgstr "Allianz"
 
-#: models/structures.py:961
+#: models/structures.py:975
 msgid "config starbase equipment role"
 msgstr ""
 
-#: models/structures.py:962
+#: models/structures.py:976
 #, fuzzy
 #| msgid "Corporation"
 msgid "corporation member"
 msgstr "Corporation"
 
-#: models/structures.py:963
+#: models/structures.py:977
 msgid "starbase fuel technician role"
 msgstr ""
 
 #: templates/structures/base.html:4
 #, fuzzy
 #| msgid "Structure List"
 msgid "Structures"
@@ -2390,78 +2399,78 @@
 msgid "No Access"
 msgstr ""
 
 #: templates/structures/templatetags/list_tax_item.html:11
 msgid "Has Access"
 msgstr ""
 
-#: views.py:255
+#: views.py:256
 msgid "Fuel blocks per day (est.)"
 msgstr ""
 
-#: views.py:406
+#: views.py:407
 #, python-format
 msgid ""
 "You can only use your main or alt characters to add corporations. However, "
 "character %s is neither. "
 msgstr ""
 "Du kannst nur deinen Hauptcharakter oder einen Deiner Zweitcharaketere "
 "nutzen um eine Corporation hinzu zu fügen. %s ist keines von beiden."
 
-#: views.py:439
+#: views.py:440
 #, fuzzy, python-format
 #| msgid ""
 #| "%(corporation)s has been added with %(character)s as sync character. We "
 #| "have started fetching structures for this corporation. You will receive a "
 #| "report once the process is finished."
 msgid ""
 "%(corporation)s has been added with %(character)s as sync character. We have "
 "started fetching structures and notifications for this corporation and you "
 "will receive a report once the process is finished."
 msgstr ""
 "%(corporation)s wurde hinzugefügt mit %(character)s als Charakter zum "
 "Synchronisieren. Strukturen werden eingelesen. Du erhältst eine "
 "Benachrichtigung sobald dieser Prozess abgeschlossen ist."
 
-#: views.py:455
+#: views.py:456
 #, python-format
 msgid "%(corporation)s was added as new structure owner by %(user)s."
 msgstr ""
 "%(corporation)s wurde als neuer Strukurenbesitzer hinzugefügt durch %(user)s."
 
-#: views.py:459
+#: views.py:460
 #, fuzzy, python-format
 #| msgid "Add Structure Owner"
 msgid "%s: Structure owner added: %s"
 msgstr "Strukturbesitzer hinzufügen"
 
-#: views.py:466
+#: views.py:467
 #, python-format
 msgid ""
 "%(character)s has been added to %(corporation)s as sync character. You now "
 "have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:481
+#: views.py:482
 #, python-format
 msgid ""
 "%(character)s was added as sync character to %(corporation)s by %(user)s.\n"
 "We now have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:491
+#: views.py:492
 #, python-format
 msgid "%s: Character added to: %s"
 msgstr ""
 
-#: views.py:508
+#: views.py:509
 msgid "service is up"
 msgstr "Service ist verfügbar"
 
-#: views.py:510
+#: views.py:511
 msgid "service is down"
 msgstr "Service ist nicht verfügbar"
 
 #: webhooks/models.py:13
 msgid "here"
 msgstr ""
```

### Comparing `aa_structures-2.2.0/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-17 02:47+0200\n"
+"POT-Creation-Date: 2023-04-24 23:05+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:111
 msgid "Sent fuel notifications for selected configuration"
 msgstr ""
 
-#: admin.py:240 models/structures.py:162
+#: admin.py:137
+msgid ""
+"Timing configuration for sending fuel notifications. Note that the first "
+"notification will be sent at the exact start hour, and the last notification "
+"will be sent one repeat before the end hour."
+msgstr ""
+
+#: admin.py:240 models/structures.py:163
 msgid "N/A"
 msgstr ""
 
 #: admin.py:255
 msgid "Not configured"
 msgstr ""
 
@@ -297,26 +304,26 @@
 #, python-format
 msgid ""
 "\n"
 "\n"
 "Change becomes effective at %s."
 msgstr ""
 
-#: core/notification_embeds.py:728 models/notifications.py:97
+#: core/notification_embeds.py:728 models/notifications.py:99
 msgid "Moon mining extraction started"
 msgstr ""
 
 #: core/notification_embeds.py:730
 #, python-format
 msgid ""
 "A moon mining extraction has been started for %(structure_name)s at %(moon)s "
 "in %(solar_system)s belonging to %(owner_link)s. Extraction was started by "
 "%(character)s.\n"
-"The chunk will be ready on location at %(ready_time)s, and will autofracture "
-"on %(auto_time)s.\n"
+"The chunk will be ready on location at %(ready_time)s, and will fracture "
+"automatically on %(auto_time)s.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:746
 #, python-format
 msgid ""
 "\n"
@@ -348,15 +355,15 @@
 #: core/notification_embeds.py:782
 msgid "Automatic Fracture"
 msgstr ""
 
 #: core/notification_embeds.py:784
 #, python-format
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has automatically been fired and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:810
 msgid "Extraction cancelled"
@@ -366,21 +373,21 @@
 #, python-format
 msgid ""
 "An ongoing extraction for %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been cancelled by %(character)s."
 msgstr ""
 
 #: core/notification_embeds.py:831
-msgid "Moondrill fired"
+msgid "Moon drill fired"
 msgstr ""
 
 #: core/notification_embeds.py:833
 #, python-format
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been fired by %(character)s and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:876
 msgid "Orbital under attack"
@@ -401,15 +408,15 @@
 #, python-format
 msgid ""
 "The %(structure_type)s at %(planet)s in %(solar_system)s belonging to "
 "%(owner_link)s has been reinforced by %(aggressor)s and will come out at: "
 "%(date)s."
 msgstr ""
 
-#: core/notification_embeds.py:935 core/notification_embeds.py:1630
+#: core/notification_embeds.py:935 core/notification_embeds.py:1631
 #, python-format
 msgid ""
 "The starbase %(structure_name)s at %(moon)s in %(solar_system)s belonging to "
 "%(owner_link)s "
 msgstr ""
 
 #: core/notification_embeds.py:952
@@ -419,15 +426,15 @@
 #: core/notification_embeds.py:954
 #, python-format
 msgid ""
 "is under attack by %(aggressor)s.\n"
 "%(damage_text)s"
 msgstr ""
 
-#: core/notification_embeds.py:982 models/notifications.py:91
+#: core/notification_embeds.py:982 models/notifications.py:93
 msgid "Starbase fuel alert"
 msgstr ""
 
 #: core/notification_embeds.py:996
 msgid "Starbase refueled"
 msgstr ""
 
@@ -528,59 +535,59 @@
 msgid "%s has offered a surrender"
 msgstr ""
 
 #: core/notification_embeds.py:1535
 #, python-format
 msgid ""
 "%s has offered to end the war with %s in the exchange for %s ISK. If "
-"accepted, the war will end in 24 hours and your organizations willbe unable "
+"accepted, the war will end in 24 hours and your organizations will be unable "
 "to declare new wars against each other for the next 2 weeks."
 msgstr ""
 
 #: core/notification_embeds.py:1548
 msgid "Insufficient Funds for Bill"
 msgstr ""
 
 #: core/notification_embeds.py:1550
 #, python-format
 msgid ""
-"The selected corporation wallet division for autopayments does not have "
-"enough current funds available to pay the %(bill_type)s due to be paid by "
-"%(due_date)s. Transfer additional funds to the selected wallet division in "
-"order to meet your pending automatic bills."
+"The selected corporation wallet division for automatic payments does not "
+"have enough current funds available to pay the %(bill_type)s due to be paid "
+"by %(due_date)s. Transfer additional funds to the selected wallet division "
+"in order to meet your pending automatic bills."
 msgstr ""
 
-#: core/notification_embeds.py:1569
+#: core/notification_embeds.py:1570
 msgid "IHub Bill About to Expire"
 msgstr ""
 
-#: core/notification_embeds.py:1571
+#: core/notification_embeds.py:1572
 #, python-format
 msgid ""
 "Maintenance bill for Infrastructure Hub in %(solar_system)s expires at "
 "%(due_date)s, if not paid in time this Infrastructure Hub will self-destruct."
 msgstr ""
 
-#: core/notification_embeds.py:1596
+#: core/notification_embeds.py:1597
 #, python-format
 msgid "%s has self-destructed due to unpaid maintenance bills"
 msgstr ""
 
-#: core/notification_embeds.py:1600
+#: core/notification_embeds.py:1601
 #, python-format
 msgid ""
 "%(structure_type)s in %(solar_system)s has self-destructed, as the standard "
 "maintenance bills where not paid."
 msgstr ""
 
-#: core/notification_embeds.py:1645
+#: core/notification_embeds.py:1646
 msgid "Starbase reinforced"
 msgstr ""
 
-#: core/notification_embeds.py:1653
+#: core/notification_embeds.py:1654
 #, python-format
 msgid "has been reinforced and will come out at: %s."
 msgstr ""
 
 #: core/notification_timers.py:89
 msgid "Armor timer"
 msgstr ""
@@ -602,1117 +609,1117 @@
 msgid "yes"
 msgstr ""
 
 #: core/serializers.py:496
 msgid "no"
 msgstr ""
 
-#: models/notifications.py:41
+#: models/notifications.py:43
 msgid "English"
 msgstr ""
 
-#: models/notifications.py:42
+#: models/notifications.py:44
 msgid "German"
 msgstr ""
 
-#: models/notifications.py:43
+#: models/notifications.py:45
 msgid "Spanish"
 msgstr ""
 
-#: models/notifications.py:44
+#: models/notifications.py:46
 msgid "Chinese Simplified"
 msgstr ""
 
-#: models/notifications.py:45
+#: models/notifications.py:47
 msgid "Russian"
 msgstr ""
 
-#: models/notifications.py:46
+#: models/notifications.py:48
 msgid "Korean"
 msgstr ""
 
-#: models/notifications.py:54
+#: models/notifications.py:56
 msgid "Upwell structure anchoring"
 msgstr ""
 
-#: models/notifications.py:55
+#: models/notifications.py:57
 msgid "Upwell structure went online"
 msgstr ""
 
-#: models/notifications.py:57
+#: models/notifications.py:59
 msgid "Upwell structure services went offline"
 msgstr ""
 
-#: models/notifications.py:60
+#: models/notifications.py:62
 msgid "Upwell structure went high power"
 msgstr ""
 
-#: models/notifications.py:63
+#: models/notifications.py:65
 msgid "Upwell structure went low power"
 msgstr ""
 
-#: models/notifications.py:65
+#: models/notifications.py:67
 msgid "Upwell structure unanchoring"
 msgstr ""
 
-#: models/notifications.py:66
+#: models/notifications.py:68
 msgid "Upwell structure fuel alert"
 msgstr ""
 
-#: models/notifications.py:67
+#: models/notifications.py:69
 msgid "Upwell structure refueled"
 msgstr ""
 
-#: models/notifications.py:69
+#: models/notifications.py:71
 msgid "Upwell structure jump fuel alert"
 msgstr ""
 
-#: models/notifications.py:72
+#: models/notifications.py:74
 msgid "Upwell structure is under attack"
 msgstr ""
 
-#: models/notifications.py:74
+#: models/notifications.py:76
 msgid "Upwell structure lost shields"
 msgstr ""
 
-#: models/notifications.py:75
+#: models/notifications.py:77
 msgid "Upwell structure lost armor"
 msgstr ""
 
-#: models/notifications.py:76
+#: models/notifications.py:78
 msgid "Upwell structure destroyed"
 msgstr ""
 
-#: models/notifications.py:79
+#: models/notifications.py:81
 msgid "Upwell structure reinforcement time changed"
 msgstr ""
 
-#: models/notifications.py:82
+#: models/notifications.py:84
 msgid "Upwell structure ownership transferred"
 msgstr ""
 
-#: models/notifications.py:86
+#: models/notifications.py:88
 msgid "Customs office attacked"
 msgstr ""
 
-#: models/notifications.py:87
+#: models/notifications.py:89
 msgid "Customs office reinforced"
 msgstr ""
 
-#: models/notifications.py:90
+#: models/notifications.py:92
 msgid "Starbase attacked"
 msgstr ""
 
-#: models/notifications.py:92
+#: models/notifications.py:94
 msgid "Starbase refueled (BETA)"
 msgstr ""
 
-#: models/notifications.py:93
+#: models/notifications.py:95
 msgid "Starbase reinforced (BETA)"
 msgstr ""
 
-#: models/notifications.py:99
+#: models/notifications.py:101
 msgid "Moonmining laser fired"
 msgstr ""
 
-#: models/notifications.py:101
+#: models/notifications.py:103
 msgid "Moon mining extraction cancelled"
 msgstr ""
 
-#: models/notifications.py:104
+#: models/notifications.py:106
 msgid "Moon mining extraction finished"
 msgstr ""
 
-#: models/notifications.py:107
+#: models/notifications.py:109
 msgid "Moon mining automatic fracture triggered"
 msgstr ""
 
-#: models/notifications.py:112
+#: models/notifications.py:114
 msgid "Sovereignty structure reinforced"
 msgstr ""
 
-#: models/notifications.py:115
+#: models/notifications.py:117
 msgid "Sovereignty structure destroyed"
 msgstr ""
 
-#: models/notifications.py:118
+#: models/notifications.py:120
 msgid "Sovereignty entosis capture started"
 msgstr ""
 
-#: models/notifications.py:121
+#: models/notifications.py:123
 msgid "Sovereignty command node event started"
 msgstr ""
 
-#: models/notifications.py:124
+#: models/notifications.py:126
 msgid "Sovereignty claim acknowledgment"
 msgstr ""
 
-#: models/notifications.py:126
+#: models/notifications.py:128
 msgid "Sovereignty lost"
 msgstr ""
 
-#: models/notifications.py:128
+#: models/notifications.py:130
 msgid "Structure anchoring in alliance space"
 msgstr ""
 
-#: models/notifications.py:132
+#: models/notifications.py:134
 msgid "War declared"
 msgstr ""
 
-#: models/notifications.py:134
+#: models/notifications.py:136
 msgid "War ally joined aggressor"
 msgstr ""
 
-#: models/notifications.py:136
+#: models/notifications.py:138
 msgid "War ally joined ally"
 msgstr ""
 
-#: models/notifications.py:138
+#: models/notifications.py:140
 msgid "War ally joined defender"
 msgstr ""
 
-#: models/notifications.py:140
+#: models/notifications.py:142
 msgid "War adopted"
 msgstr ""
 
-#: models/notifications.py:141
+#: models/notifications.py:143
 msgid "War inherited"
 msgstr ""
 
-#: models/notifications.py:142
+#: models/notifications.py:144
 msgid "War party surrendered"
 msgstr ""
 
-#: models/notifications.py:144
+#: models/notifications.py:146
 msgid "War retracted by Concord"
 msgstr ""
 
-#: models/notifications.py:147
+#: models/notifications.py:149
 msgid "War corporation became eligible"
 msgstr ""
 
-#: models/notifications.py:150
+#: models/notifications.py:152
 msgid "War corporation no longer eligible"
 msgstr ""
 
-#: models/notifications.py:152
+#: models/notifications.py:154
 msgid "War surrender offered"
 msgstr ""
 
-#: models/notifications.py:155
+#: models/notifications.py:157
 msgid "Character submitted application"
 msgstr ""
 
-#: models/notifications.py:157
+#: models/notifications.py:159
 msgid "Character invited to join corporation"
 msgstr ""
 
-#: models/notifications.py:160
+#: models/notifications.py:162
 msgid "Corp application rejected"
 msgstr ""
 
-#: models/notifications.py:162
+#: models/notifications.py:164
 msgid "Character withdrew application"
 msgstr ""
 
-#: models/notifications.py:163
+#: models/notifications.py:165
 msgid "Character joins corporation"
 msgstr ""
 
-#: models/notifications.py:164
+#: models/notifications.py:166
 msgid "Character leaves corporation"
 msgstr ""
 
-#: models/notifications.py:167
+#: models/notifications.py:169
 msgid "Bill out of money"
 msgstr ""
 
-#: models/notifications.py:170
+#: models/notifications.py:172
 msgid "I-HUB bill about to expire"
 msgstr ""
 
-#: models/notifications.py:174
+#: models/notifications.py:176
 msgid "I_HUB destroyed by bill failure"
 msgstr ""
 
-#: models/notifications.py:334
+#: models/notifications.py:336
 msgid "notification types"
 msgstr ""
 
-#: models/notifications.py:336
+#: models/notifications.py:338
 msgid "Select which type of notifications should be forwarded to this webhook"
 msgstr ""
 
-#: models/notifications.py:345
+#: models/notifications.py:347
 msgid "language"
 msgstr ""
 
-#: models/notifications.py:346
+#: models/notifications.py:348
 msgid "language of notifications send to this webhook"
 msgstr ""
 
-#: models/notifications.py:350 models/structures.py:91
+#: models/notifications.py:352 models/structures.py:92
 msgid "is default"
 msgstr ""
 
-#: models/notifications.py:352
+#: models/notifications.py:354
 msgid "Whether owners have this webhook automatically pre-set when created"
 msgstr ""
 
-#: models/notifications.py:357 models/owners.py:151
+#: models/notifications.py:359 models/owners.py:153
 msgid "has default pings enabled"
 msgstr ""
 
-#: models/notifications.py:368 models/owners.py:197
+#: models/notifications.py:370 models/owners.py:199
 msgid "ping groups"
 msgstr ""
 
-#: models/notifications.py:369
+#: models/notifications.py:371
 msgid "Groups to be pinged for each notification - "
 msgstr ""
 
-#: models/notifications.py:374
+#: models/notifications.py:376
 msgid "webhook"
 msgstr ""
 
-#: models/notifications.py:375 models/owners.py:212 models/structures.py:389
+#: models/notifications.py:377 models/owners.py:214 models/structures.py:390
 msgid "webhooks"
 msgstr ""
 
-#: models/notifications.py:388
+#: models/notifications.py:390
 msgid "is sent"
 msgstr ""
 
-#: models/notifications.py:389
+#: models/notifications.py:391
 msgid "True when this notification has been forwarded to Discord"
 msgstr ""
 
-#: models/notifications.py:394
+#: models/notifications.py:396
 msgid "is timer added"
 msgstr ""
 
-#: models/notifications.py:395
+#: models/notifications.py:397
 msgid "True when a timer has been added for this notification"
 msgstr ""
 
-#: models/notifications.py:401 models/structures.py:242
-#: models/structures.py:773
+#: models/notifications.py:403 models/structures.py:243
+#: models/structures.py:787
 msgid "type"
 msgstr ""
 
-#: models/notifications.py:402
+#: models/notifications.py:404
 msgid "type of this notification"
 msgstr ""
 
-#: models/notifications.py:407 models/owners.py:219 models/owners.py:1278
-#: models/structures.py:312
+#: models/notifications.py:409 models/owners.py:221 models/owners.py:1287
+#: models/structures.py:313
 msgid "owner"
 msgstr ""
 
-#: models/notifications.py:408
+#: models/notifications.py:410
 msgid "Corporation that owns this notification"
 msgstr ""
 
-#: models/notifications.py:412 models/structures.py:402
+#: models/notifications.py:414 models/structures.py:403
 msgid "structures"
 msgstr ""
 
-#: models/notifications.py:413
+#: models/notifications.py:415
 msgid "Structures this notification is about (if any)"
 msgstr ""
 
-#: models/notifications.py:682 models/structures.py:202
-#: models/structures.py:759
+#: models/notifications.py:694 models/structures.py:203
+#: models/structures.py:773
 msgid "id"
 msgstr ""
 
-#: models/notifications.py:686
+#: models/notifications.py:698
 msgid "created"
 msgstr ""
 
-#: models/notifications.py:687
+#: models/notifications.py:699
 msgid "Date when this notification was first received from ESI"
 msgstr ""
 
-#: models/notifications.py:692
+#: models/notifications.py:704
 msgid "is read"
 msgstr ""
 
-#: models/notifications.py:693
+#: models/notifications.py:705
 msgid "True when this notification has read in the eve client"
 msgstr ""
 
-#: models/notifications.py:696
+#: models/notifications.py:708
 msgid "last updated"
 msgstr ""
 
-#: models/notifications.py:697
+#: models/notifications.py:709
 msgid "Date when this notification has last been updated from ESI"
 msgstr ""
 
-#: models/notifications.py:704
+#: models/notifications.py:716
 msgid "sender"
 msgstr ""
 
-#: models/notifications.py:711
+#: models/notifications.py:723
 msgid "text"
 msgstr ""
 
-#: models/notifications.py:712
+#: models/notifications.py:724
 msgid "Notification details in YAML"
 msgstr ""
 
-#: models/notifications.py:714 models/notifications.py:831
+#: models/notifications.py:726 models/notifications.py:843
 msgid "timestamp"
 msgstr ""
 
-#: models/notifications.py:719
+#: models/notifications.py:731
 msgid "eve notification"
 msgstr ""
 
-#: models/notifications.py:720
+#: models/notifications.py:732
 msgid "eve notifications"
 msgstr ""
 
-#: models/notifications.py:829
+#: models/notifications.py:841
 msgid "details"
 msgstr ""
 
-#: models/notifications.py:830
+#: models/notifications.py:842
 msgid "last_updated"
 msgstr ""
 
-#: models/notifications.py:836
+#: models/notifications.py:848
 msgid "generated notification"
 msgstr ""
 
-#: models/notifications.py:837
+#: models/notifications.py:849
 msgid "generated  notifications"
 msgstr ""
 
-#: models/notifications.py:866
+#: models/notifications.py:878
 msgid "channel pings"
 msgstr ""
 
-#: models/notifications.py:868
+#: models/notifications.py:880
 msgid ""
 "Option to ping every member of the channel. This setting can be overruled by "
 "the respective owner or webhook configuration"
 msgstr ""
 
-#: models/notifications.py:878
+#: models/notifications.py:890
 msgid "color"
 msgstr ""
 
-#: models/notifications.py:879
+#: models/notifications.py:891
 msgid "Context color of these notification on Discord"
 msgstr ""
 
-#: models/notifications.py:883
+#: models/notifications.py:895
 msgid "is_enabled"
 msgstr ""
 
-#: models/notifications.py:884
+#: models/notifications.py:896
 msgid "Disabled configurations will not create any new alerts."
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "end"
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "End of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:910
+#: models/notifications.py:922
 msgid "repeat"
 msgstr ""
 
-#: models/notifications.py:912
+#: models/notifications.py:924
 msgid "Notifications will be repeated every x hours. Set to 0 for no repeats"
 msgstr ""
 
-#: models/notifications.py:916
+#: models/notifications.py:928
 msgid "start"
 msgstr ""
 
-#: models/notifications.py:917
+#: models/notifications.py:929
 msgid "Start of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:921
+#: models/notifications.py:933
 msgid "structure fuel alert config"
 msgstr ""
 
-#: models/notifications.py:922
+#: models/notifications.py:934
 msgid "structure fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:927
+#: models/notifications.py:941
 msgid "Start must be before end, i.e. have a larger value."
 msgstr ""
 
-#: models/notifications.py:931
+#: models/notifications.py:945
 msgid "Repeat can not be larger that the interval size."
 msgstr ""
 
-#: models/notifications.py:940
+#: models/notifications.py:954
 msgid "This configuration may not overlap with an existing configuration."
 msgstr ""
 
-#: models/notifications.py:1007
+#: models/notifications.py:1021
 msgid "threshold"
 msgstr ""
 
-#: models/notifications.py:1009
+#: models/notifications.py:1023
 msgid ""
 "Notifications will be sent once fuel level in units reaches this threshold"
 msgstr ""
 
-#: models/notifications.py:1014
+#: models/notifications.py:1028
 msgid "jump fuel alert config"
 msgstr ""
 
-#: models/notifications.py:1015
+#: models/notifications.py:1029
 msgid "jump fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:1064 models/notifications.py:1114
-#: models/structures.py:401 models/structures.py:765 models/structures.py:830
+#: models/notifications.py:1078 models/notifications.py:1128
+#: models/structures.py:402 models/structures.py:779 models/structures.py:844
 msgid "structure"
 msgstr ""
 
-#: models/notifications.py:1070 models/notifications.py:1120
+#: models/notifications.py:1084 models/notifications.py:1134
 msgid "configuration"
 msgstr ""
 
-#: models/notifications.py:1074
+#: models/notifications.py:1088
 msgid "hours"
 msgstr ""
 
-#: models/notifications.py:1075
+#: models/notifications.py:1089
 msgid "number of hours before fuel expiration this alert was sent"
 msgstr ""
 
-#: models/notifications.py:1079
+#: models/notifications.py:1093
 msgid "structure fuel alert"
 msgstr ""
 
-#: models/notifications.py:1080
+#: models/notifications.py:1094
 msgid "structure fuel alerts"
 msgstr ""
 
-#: models/notifications.py:1124
+#: models/notifications.py:1138
 msgid "jump fuel alert"
 msgstr ""
 
-#: models/notifications.py:1125
+#: models/notifications.py:1139
 msgid "jump fuel alerts"
 msgstr ""
 
-#: models/owners.py:117
+#: models/owners.py:119
 msgid "corporation"
 msgstr ""
 
-#: models/owners.py:118
+#: models/owners.py:120
 msgid "Corporation owning structures"
 msgstr ""
 
-#: models/owners.py:123
+#: models/owners.py:125
 msgid "are pocos public"
 msgstr ""
 
-#: models/owners.py:124
+#: models/owners.py:126
 msgid "whether pocos of this owner are shown on public POCO page"
 msgstr ""
 
-#: models/owners.py:130
+#: models/owners.py:132
 msgid "assets last update at"
 msgstr ""
 
-#: models/owners.py:131 models/owners.py:147 models/owners.py:190
-#: models/owners.py:205
+#: models/owners.py:133 models/owners.py:149 models/owners.py:192
+#: models/owners.py:207
 msgid "when the last successful update happened"
 msgstr ""
 
-#: models/owners.py:146
+#: models/owners.py:148
 msgid "forwarding last update at"
 msgstr ""
 
-#: models/owners.py:153
+#: models/owners.py:155
 msgid ""
 "to enable or disable pinging of notifications for this owner e.g. with "
 "@everyone and @here"
 msgstr ""
 
-#: models/owners.py:159
+#: models/owners.py:161
 msgid "is active"
 msgstr ""
 
-#: models/owners.py:160
+#: models/owners.py:162
 msgid "whether this owner is currently included in the sync process"
 msgstr ""
 
-#: models/owners.py:164
+#: models/owners.py:166
 msgid "is alliance main"
 msgstr ""
 
-#: models/owners.py:166
+#: models/owners.py:168
 msgid ""
 "whether alliance wide notifications are forwarded for this owner (e.g. sov "
 "notifications)"
 msgstr ""
 
-#: models/owners.py:172
+#: models/owners.py:174
 msgid "is included in service status"
 msgstr ""
 
-#: models/owners.py:174
+#: models/owners.py:176
 msgid ""
 "whether the sync status of this owner is included in the overall status of "
 "this services"
 msgstr ""
 
-#: models/owners.py:182
+#: models/owners.py:184
 msgid "is up"
 msgstr ""
 
-#: models/owners.py:183
+#: models/owners.py:185
 msgid "whether all services for this owner are currently up"
 msgstr ""
 
-#: models/owners.py:189
+#: models/owners.py:191
 msgid "notifications last update at"
 msgstr ""
 
-#: models/owners.py:198
+#: models/owners.py:200
 msgid "Groups to be pinged for each notification. "
 msgstr ""
 
-#: models/owners.py:204
+#: models/owners.py:206
 msgid "structures last update at"
 msgstr ""
 
-#: models/owners.py:213
+#: models/owners.py:215
 msgid "Notifications are sent to these webhooks."
 msgstr ""
 
-#: models/owners.py:220
+#: models/owners.py:222
 msgid "owners"
 msgstr ""
 
-#: models/owners.py:1139
+#: models/owners.py:1147
 #, python-format
 msgid ""
 "Syncing of %(topic)s for %(owner)s %(result)s.\n"
 " %(message_details)s"
 msgstr ""
 
-#: models/owners.py:1143
+#: models/owners.py:1151
 msgid "completed successfully"
 msgstr ""
 
-#: models/owners.py:1148
+#: models/owners.py:1156
 #, python-format
 msgid "%(title)s: %(topic)s updated for %(owner)s: %(result)s"
 msgstr ""
 
-#: models/owners.py:1153
+#: models/owners.py:1161
 msgid "OK"
 msgstr ""
 
-#: models/owners.py:1284
+#: models/owners.py:1293
 msgid "character_ownership"
 msgstr ""
 
-#: models/owners.py:1292
+#: models/owners.py:1301
 msgid "structures last used at"
 msgstr ""
 
-#: models/owners.py:1300
+#: models/owners.py:1309
 msgid "notifications last used at"
 msgstr ""
 
-#: models/owners.py:1306
+#: models/owners.py:1315
 msgid "error count"
 msgstr ""
 
-#: models/owners.py:1312
+#: models/owners.py:1321
 msgid "owner character"
 msgstr ""
 
-#: models/owners.py:1313
+#: models/owners.py:1322
 msgid "owner characters"
 msgstr ""
 
-#: models/structures.py:37
+#: models/structures.py:38
 msgid "sov"
 msgstr ""
 
-#: models/structures.py:38
+#: models/structures.py:39
 msgid "highsec"
 msgstr ""
 
-#: models/structures.py:39
+#: models/structures.py:40
 msgid "lowsec"
 msgstr ""
 
-#: models/structures.py:40
+#: models/structures.py:41
 msgid "nullsec"
 msgstr ""
 
-#: models/structures.py:41
+#: models/structures.py:42
 msgid "w_space"
 msgstr ""
 
-#: models/structures.py:44
+#: models/structures.py:45
 msgid "grey"
 msgstr ""
 
-#: models/structures.py:45
+#: models/structures.py:46
 msgid "dark blue"
 msgstr ""
 
-#: models/structures.py:46
+#: models/structures.py:47
 msgid "green"
 msgstr ""
 
-#: models/structures.py:47
+#: models/structures.py:48
 msgid "light blue"
 msgstr ""
 
-#: models/structures.py:48
+#: models/structures.py:49
 msgid "orange"
 msgstr ""
 
-#: models/structures.py:49
+#: models/structures.py:50
 msgid "red"
 msgstr ""
 
-#: models/structures.py:61 models/structures.py:284 models/structures.py:834
+#: models/structures.py:62 models/structures.py:285 models/structures.py:848
 msgid "name"
 msgstr ""
 
-#: models/structures.py:62
+#: models/structures.py:63
 msgid "name of the tag - must be unique"
 msgstr ""
 
-#: models/structures.py:68
+#: models/structures.py:69
 msgid "description"
 msgstr ""
 
-#: models/structures.py:69
+#: models/structures.py:70
 msgid "description for this tag"
 msgstr ""
 
-#: models/structures.py:76
+#: models/structures.py:77
 msgid "style"
 msgstr ""
 
-#: models/structures.py:77
+#: models/structures.py:78
 msgid "color style of tag"
 msgstr ""
 
-#: models/structures.py:83
+#: models/structures.py:84
 msgid "order"
 msgstr ""
 
-#: models/structures.py:85
+#: models/structures.py:86
 msgid ""
 "number defining the order tags are shown. custom tags can not have an order "
 "below 100"
 msgstr ""
 
-#: models/structures.py:93
+#: models/structures.py:94
 msgid "if true this custom tag will automatically be added to new structures"
 msgstr ""
 
-#: models/structures.py:98
+#: models/structures.py:99
 msgid "is user managed"
 msgstr ""
 
-#: models/structures.py:100
+#: models/structures.py:101
 msgid ""
 "if False this tag is created and managed by the system and can not be "
 "modified by users"
 msgstr ""
 
-#: models/structures.py:108
+#: models/structures.py:109
 msgid "structure tag"
 msgstr ""
 
-#: models/structures.py:109
+#: models/structures.py:110
 msgid "structure tags"
 msgstr ""
 
-#: models/structures.py:143
+#: models/structures.py:144
 msgid "anchor vulnerable"
 msgstr ""
 
-#: models/structures.py:144
+#: models/structures.py:145
 msgid "anchoring"
 msgstr ""
 
-#: models/structures.py:145
+#: models/structures.py:146
 msgid "armor reinforce"
 msgstr ""
 
-#: models/structures.py:146
+#: models/structures.py:147
 msgid "armor vulnerable"
 msgstr ""
 
-#: models/structures.py:147
+#: models/structures.py:148
 msgid "deploy vulnerable"
 msgstr ""
 
-#: models/structures.py:148
+#: models/structures.py:149
 msgid "fitting invulnerable"
 msgstr ""
 
-#: models/structures.py:149
+#: models/structures.py:150
 msgid "hull reinforce"
 msgstr ""
 
-#: models/structures.py:150
+#: models/structures.py:151
 msgid "hull vulnerable"
 msgstr ""
 
-#: models/structures.py:151
+#: models/structures.py:152
 msgid "online deprecated"
 msgstr ""
 
-#: models/structures.py:152
+#: models/structures.py:153
 msgid "onlining vulnerable"
 msgstr ""
 
-#: models/structures.py:153
+#: models/structures.py:154
 msgid "shield vulnerable"
 msgstr ""
 
-#: models/structures.py:154
+#: models/structures.py:155
 msgid "unanchored"
 msgstr ""
 
-#: models/structures.py:156 models/structures.py:813
+#: models/structures.py:157 models/structures.py:827
 msgid "offline"
 msgstr ""
 
-#: models/structures.py:157 models/structures.py:814
+#: models/structures.py:158 models/structures.py:828
 msgid "online"
 msgstr ""
 
-#: models/structures.py:158
+#: models/structures.py:159
 msgid "onlining"
 msgstr ""
 
-#: models/structures.py:159
+#: models/structures.py:160
 msgid "reinforced"
 msgstr ""
 
-#: models/structures.py:160
+#: models/structures.py:161
 msgid "unanchoring "
 msgstr ""
 
-#: models/structures.py:163
+#: models/structures.py:164
 msgid "unknown"
 msgstr ""
 
-#: models/structures.py:194
+#: models/structures.py:195
 msgid "Full Power"
 msgstr ""
 
-#: models/structures.py:195
+#: models/structures.py:196
 msgid "Low Power"
 msgstr ""
 
-#: models/structures.py:196
+#: models/structures.py:197
 msgid "Abandoned"
 msgstr ""
 
-#: models/structures.py:197
+#: models/structures.py:198
 msgid "Abandoned?"
 msgstr ""
 
-#: models/structures.py:198
+#: models/structures.py:199
 msgid "Unknown"
 msgstr ""
 
-#: models/structures.py:203
+#: models/structures.py:204
 msgid "The Item ID of the structure"
 msgstr ""
 
-#: models/structures.py:208
+#: models/structures.py:209
 msgid "created at"
 msgstr ""
 
-#: models/structures.py:209
+#: models/structures.py:210
 msgid "date this structure was received from ESI for the first time"
 msgstr ""
 
-#: models/structures.py:218
+#: models/structures.py:219
 msgid "moon"
 msgstr ""
 
-#: models/structures.py:219
+#: models/structures.py:220
 msgid "Moon next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:228
+#: models/structures.py:229
 msgid "planet"
 msgstr ""
 
-#: models/structures.py:229
+#: models/structures.py:230
 msgid "Planet next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:235
+#: models/structures.py:236
 msgid "solar system"
 msgstr ""
 
-#: models/structures.py:236
+#: models/structures.py:237
 msgid "Solar System the structure is located"
 msgstr ""
 
-#: models/structures.py:243
+#: models/structures.py:244
 msgid "Type of the structure"
 msgstr ""
 
-#: models/structures.py:249
+#: models/structures.py:250
 msgid "fuel expires at"
 msgstr ""
 
-#: models/structures.py:250
+#: models/structures.py:251
 msgid "Date on which the structure will run out of fuel"
 msgstr ""
 
-#: models/structures.py:257
+#: models/structures.py:258
 msgid "has fitting"
 msgstr ""
 
-#: models/structures.py:258
+#: models/structures.py:259
 msgid "bool indicating if the structure has a fitting"
 msgstr ""
 
-#: models/structures.py:265
+#: models/structures.py:266
 msgid "has core"
 msgstr ""
 
-#: models/structures.py:266
+#: models/structures.py:267
 msgid "bool indicating if the structure has a quantum core"
 msgstr ""
 
-#: models/structures.py:272
+#: models/structures.py:273
 msgid "last online at"
 msgstr ""
 
-#: models/structures.py:273
+#: models/structures.py:274
 msgid "date this structure had any of it's services online"
 msgstr ""
 
-#: models/structures.py:279 models/structures.py:778
+#: models/structures.py:280 models/structures.py:792
 msgid "last updated at"
 msgstr ""
 
-#: models/structures.py:280
+#: models/structures.py:281
 msgid "date this structure was last updated from the EVE server"
 msgstr ""
 
-#: models/structures.py:285
+#: models/structures.py:286
 msgid "The full name of the structure"
 msgstr ""
 
-#: models/structures.py:292
+#: models/structures.py:293
 msgid "next reinforce hour"
 msgstr ""
 
-#: models/structures.py:294 models/structures.py:304
+#: models/structures.py:295 models/structures.py:305
 msgid ""
 "The requested change to reinforce_hour that will take effect at the time "
 "shown by next_reinforce_apply"
 msgstr ""
 
-#: models/structures.py:302
+#: models/structures.py:303
 msgid "next reinforce apply"
 msgstr ""
 
-#: models/structures.py:313
+#: models/structures.py:314
 msgid "Corporation that owns the structure"
 msgstr ""
 
-#: models/structures.py:320
+#: models/structures.py:321
 msgid "reinforce hour"
 msgstr ""
 
-#: models/structures.py:322
+#: models/structures.py:323
 msgid ""
 "The average hour of day that determines the time +/- some hours when the "
 "structure will randomly exit its reinforcement periods and become vulnerable "
 "to attack against its armor and/or hull. "
 msgstr ""
 
-#: models/structures.py:331
+#: models/structures.py:332
 msgid "position x"
 msgstr ""
 
-#: models/structures.py:332
+#: models/structures.py:333
 msgid "x position in the solar system"
 msgstr ""
 
-#: models/structures.py:338
+#: models/structures.py:339
 msgid "position y"
 msgstr ""
 
-#: models/structures.py:339
+#: models/structures.py:340
 msgid "y position in the solar system"
 msgstr ""
 
-#: models/structures.py:345
+#: models/structures.py:346
 msgid "position z"
 msgstr ""
 
-#: models/structures.py:346
+#: models/structures.py:347
 msgid "z position in the solar system"
 msgstr ""
 
-#: models/structures.py:352 models/structures.py:839
+#: models/structures.py:353 models/structures.py:853
 msgid "state"
 msgstr ""
 
-#: models/structures.py:353
+#: models/structures.py:354
 msgid "Current state of the structure"
 msgstr ""
 
-#: models/structures.py:359
+#: models/structures.py:360
 msgid "state timer end"
 msgstr ""
 
-#: models/structures.py:360
+#: models/structures.py:361
 msgid "Date at which the structure entered it's current state"
 msgstr ""
 
-#: models/structures.py:366
+#: models/structures.py:367
 msgid "state timer start"
 msgstr ""
 
-#: models/structures.py:367
+#: models/structures.py:368
 msgid "Date at which the structure will move to it's next state"
 msgstr ""
 
-#: models/structures.py:374
+#: models/structures.py:375
 msgid "tags"
 msgstr ""
 
-#: models/structures.py:375
+#: models/structures.py:376
 msgid "List of tags for this structure. "
 msgstr ""
 
-#: models/structures.py:381
+#: models/structures.py:382
 msgid "unanchors at"
 msgstr ""
 
-#: models/structures.py:382
+#: models/structures.py:383
 msgid "Date at which the structure will unanchor"
 msgstr ""
 
-#: models/structures.py:391
+#: models/structures.py:392
 msgid ""
 "Webhooks for sending notifications to. If any webhook is enabled, these will "
 "be used instead of the webhooks defined for the respective owner. If no "
 "webhook is enabled the owner's setting will be used. "
 msgstr ""
 
-#: models/structures.py:759
+#: models/structures.py:773
 msgid "The Eve item ID"
 msgstr ""
 
-#: models/structures.py:766
+#: models/structures.py:780
 msgid "Structure this item is located in"
 msgstr ""
 
-#: models/structures.py:774
+#: models/structures.py:788
 msgid "type of the item"
 msgstr ""
 
-#: models/structures.py:776
+#: models/structures.py:790
 msgid "is singleton"
 msgstr ""
 
-#: models/structures.py:780
+#: models/structures.py:794
 msgid "location flag"
 msgstr ""
 
-#: models/structures.py:781
+#: models/structures.py:795
 msgid "quantity"
 msgstr ""
 
-#: models/structures.py:784
+#: models/structures.py:798
 msgid "structure item"
 msgstr ""
 
-#: models/structures.py:785
+#: models/structures.py:799
 msgid "structure items"
 msgstr ""
 
-#: models/structures.py:831
+#: models/structures.py:845
 msgid "Structure this service is installed to"
 msgstr ""
 
-#: models/structures.py:834
+#: models/structures.py:848
 msgid "Name of the service"
 msgstr ""
 
-#: models/structures.py:840
+#: models/structures.py:854
 msgid "Current state of this service"
 msgstr ""
 
-#: models/structures.py:844
+#: models/structures.py:858
 msgid "structure service"
 msgstr ""
 
-#: models/structures.py:845
+#: models/structures.py:859
 msgid "structure services"
 msgstr ""
 
-#: models/structures.py:861 webhooks/models.py:12
+#: models/structures.py:875 webhooks/models.py:12
 msgid "none"
 msgstr ""
 
-#: models/structures.py:862
+#: models/structures.py:876
 msgid "terrible"
 msgstr ""
 
-#: models/structures.py:863
+#: models/structures.py:877
 msgid "bad"
 msgstr ""
 
-#: models/structures.py:864
+#: models/structures.py:878
 msgid "neutral"
 msgstr ""
 
-#: models/structures.py:865
+#: models/structures.py:879
 msgid "good"
 msgstr ""
 
-#: models/structures.py:866
+#: models/structures.py:880
 msgid "excellent"
 msgstr ""
 
-#: models/structures.py:960
+#: models/structures.py:974
 msgid "alliance member"
 msgstr ""
 
-#: models/structures.py:961
+#: models/structures.py:975
 msgid "config starbase equipment role"
 msgstr ""
 
-#: models/structures.py:962
+#: models/structures.py:976
 msgid "corporation member"
 msgstr ""
 
-#: models/structures.py:963
+#: models/structures.py:977
 msgid "starbase fuel technician role"
 msgstr ""
 
 #: templates/structures/base.html:4
 msgid "Structures"
 msgstr ""
 
@@ -2132,67 +2139,67 @@
 msgid "No Access"
 msgstr ""
 
 #: templates/structures/templatetags/list_tax_item.html:11
 msgid "Has Access"
 msgstr ""
 
-#: views.py:255
+#: views.py:256
 msgid "Fuel blocks per day (est.)"
 msgstr ""
 
-#: views.py:406
+#: views.py:407
 #, python-format
 msgid ""
 "You can only use your main or alt characters to add corporations. However, "
 "character %s is neither. "
 msgstr ""
 
-#: views.py:439
+#: views.py:440
 #, python-format
 msgid ""
 "%(corporation)s has been added with %(character)s as sync character. We have "
 "started fetching structures and notifications for this corporation and you "
 "will receive a report once the process is finished."
 msgstr ""
 
-#: views.py:455
+#: views.py:456
 #, python-format
 msgid "%(corporation)s was added as new structure owner by %(user)s."
 msgstr ""
 
-#: views.py:459
+#: views.py:460
 #, python-format
 msgid "%s: Structure owner added: %s"
 msgstr ""
 
-#: views.py:466
+#: views.py:467
 #, python-format
 msgid ""
 "%(character)s has been added to %(corporation)s as sync character. You now "
 "have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:481
+#: views.py:482
 #, python-format
 msgid ""
 "%(character)s was added as sync character to %(corporation)s by %(user)s.\n"
 "We now have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:491
+#: views.py:492
 #, python-format
 msgid "%s: Character added to: %s"
 msgstr ""
 
-#: views.py:508
+#: views.py:509
 msgid "service is up"
 msgstr ""
 
-#: views.py:510
+#: views.py:511
 msgid "service is down"
 msgstr ""
 
 #: webhooks/models.py:13
 msgid "here"
 msgstr ""
```

### Comparing `aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,37 @@
 # frank1210 <francolopez_16@hotmail.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-17 02:47+0200\n"
+"POT-Creation-Date: 2023-04-24 23:05+0200\n"
 "PO-Revision-Date: 2020-03-09 19:25+0000\n"
 "Last-Translator: frank1210 <francolopez_16@hotmail.com>, 2020\n"
 "Language-Team: Spanish (Spain) (https://www.transifex.com/kalkoken-apps/"
 "teams/107978/es_ES/)\n"
 "Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:111
 msgid "Sent fuel notifications for selected configuration"
 msgstr ""
 
-#: admin.py:240 models/structures.py:162
+#: admin.py:137
+msgid ""
+"Timing configuration for sending fuel notifications. Note that the first "
+"notification will be sent at the exact start hour, and the last notification "
+"will be sent one repeat before the end hour."
+msgstr ""
+
+#: admin.py:240 models/structures.py:163
 msgid "N/A"
 msgstr ""
 
 #: admin.py:255
 msgid "Not configured"
 msgstr ""
 
@@ -311,31 +318,31 @@
 #, python-format
 msgid ""
 "\n"
 "\n"
 "Change becomes effective at %s."
 msgstr ""
 
-#: core/notification_embeds.py:728 models/notifications.py:97
+#: core/notification_embeds.py:728 models/notifications.py:99
 msgid "Moon mining extraction started"
 msgstr "Extraccion de luna iniciada"
 
 #: core/notification_embeds.py:730
 #, fuzzy, python-format
 #| msgid ""
 #| "A moon mining extraction has been started for %(structure_name)s at "
 #| "%(moon)s in %(solar_system)s. Extraction was started by %(character)s.\n"
 #| "The chunk will be ready on location at %(ready_time)s, and will "
 #| "autofracture on %(auto_time)s.\n"
 msgid ""
 "A moon mining extraction has been started for %(structure_name)s at %(moon)s "
 "in %(solar_system)s belonging to %(owner_link)s. Extraction was started by "
 "%(character)s.\n"
-"The chunk will be ready on location at %(ready_time)s, and will autofracture "
-"on %(auto_time)s.\n"
+"The chunk will be ready on location at %(ready_time)s, and will fracture "
+"automatically on %(auto_time)s.\n"
 "%(ore_text)s"
 msgstr ""
 "Una extraccion de luna a comenzado en la estructura %(structure_name)s  "
 "%(moon)s en %(solar_system)s. La extraccion fue iniciada por %(character)s.\n"
 "El fragmento estara listo para fracturarse el %(ready_time)s, y se "
 "autofracturara en %(auto_time)s.\n"
 
@@ -382,15 +389,15 @@
 #: core/notification_embeds.py:784
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has automatically been fired and the moon products are "
 #| "ready to be harvested.\n"
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has automatically been fired and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "El taladro lunar equipado en %(structure_name)s %(moon)s en%(solar_system)s "
 "fue activado automaticamente y los productos lunares estan listos para ser "
 "recogidos.\n"
@@ -408,25 +415,27 @@
 "An ongoing extraction for %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been cancelled by %(character)s."
 msgstr ""
 "Una extraccion en %(structure_name)s, %(moon)s  %(solar_system)s, fue "
 "cancelada por %(character)s."
 
 #: core/notification_embeds.py:831
-msgid "Moondrill fired"
+#, fuzzy
+#| msgid "Moondrill fired"
+msgid "Moon drill fired"
 msgstr "Extractor lunar encendido"
 
 #: core/notification_embeds.py:833
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has been fired by %(character)s and the moon products "
 #| "are ready to be harvested."
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been fired by %(character)s and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "El extractor lunar equipado en %(structure_name)s %(moon)s en el sistema "
 "%(solar_system)s fue iniciado por %(character)s y los productos lunares "
 "estan listo para ser recogidos."
@@ -460,15 +469,15 @@
 "The %(structure_type)s at %(planet)s in %(solar_system)s belonging to "
 "%(owner_link)s has been reinforced by %(aggressor)s and will come out at: "
 "%(date)s."
 msgstr ""
 "La %(structure_type)s en %(planet)s el sistema %(solar_system)s esta siendo "
 "atacada por %(aggressor)s."
 
-#: core/notification_embeds.py:935 core/notification_embeds.py:1630
+#: core/notification_embeds.py:935 core/notification_embeds.py:1631
 #, fuzzy, python-format
 #| msgid ""
 #| "An ongoing extraction for %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has been cancelled by %(character)s."
 msgid ""
 "The starbase %(structure_name)s at %(moon)s in %(solar_system)s belonging to "
 "%(owner_link)s "
@@ -484,15 +493,15 @@
 #, fuzzy, python-format
 #| msgid "is under attack by %s"
 msgid ""
 "is under attack by %(aggressor)s.\n"
 "%(damage_text)s"
 msgstr "se encuentra bajo ataque por %s"
 
-#: core/notification_embeds.py:982 models/notifications.py:91
+#: core/notification_embeds.py:982 models/notifications.py:93
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Starbase fuel alert"
 msgstr "Alerta de combustible de la estructura"
 
 #: core/notification_embeds.py:996
 msgid "Starbase refueled"
@@ -597,61 +606,61 @@
 msgid "%s has offered a surrender"
 msgstr ""
 
 #: core/notification_embeds.py:1535
 #, python-format
 msgid ""
 "%s has offered to end the war with %s in the exchange for %s ISK. If "
-"accepted, the war will end in 24 hours and your organizations willbe unable "
+"accepted, the war will end in 24 hours and your organizations will be unable "
 "to declare new wars against each other for the next 2 weeks."
 msgstr ""
 
 #: core/notification_embeds.py:1548
 msgid "Insufficient Funds for Bill"
 msgstr ""
 
 #: core/notification_embeds.py:1550
 #, python-format
 msgid ""
-"The selected corporation wallet division for autopayments does not have "
-"enough current funds available to pay the %(bill_type)s due to be paid by "
-"%(due_date)s. Transfer additional funds to the selected wallet division in "
-"order to meet your pending automatic bills."
+"The selected corporation wallet division for automatic payments does not "
+"have enough current funds available to pay the %(bill_type)s due to be paid "
+"by %(due_date)s. Transfer additional funds to the selected wallet division "
+"in order to meet your pending automatic bills."
 msgstr ""
 
-#: core/notification_embeds.py:1569
+#: core/notification_embeds.py:1570
 msgid "IHub Bill About to Expire"
 msgstr ""
 
-#: core/notification_embeds.py:1571
+#: core/notification_embeds.py:1572
 #, python-format
 msgid ""
 "Maintenance bill for Infrastructure Hub in %(solar_system)s expires at "
 "%(due_date)s, if not paid in time this Infrastructure Hub will self-destruct."
 msgstr ""
 
-#: core/notification_embeds.py:1596
+#: core/notification_embeds.py:1597
 #, python-format
 msgid "%s has self-destructed due to unpaid maintenance bills"
 msgstr ""
 
-#: core/notification_embeds.py:1600
+#: core/notification_embeds.py:1601
 #, python-format
 msgid ""
 "%(structure_type)s in %(solar_system)s has self-destructed, as the standard "
 "maintenance bills where not paid."
 msgstr ""
 
-#: core/notification_embeds.py:1645
+#: core/notification_embeds.py:1646
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced"
 msgstr "Orbital reinforzado"
 
-#: core/notification_embeds.py:1653
+#: core/notification_embeds.py:1654
 #, python-format
 msgid "has been reinforced and will come out at: %s."
 msgstr ""
 
 #: core/notification_timers.py:89
 msgid "Armor timer"
 msgstr ""
@@ -673,1199 +682,1199 @@
 msgid "yes"
 msgstr ""
 
 #: core/serializers.py:496
 msgid "no"
 msgstr ""
 
-#: models/notifications.py:41
+#: models/notifications.py:43
 msgid "English"
 msgstr "Ingles"
 
-#: models/notifications.py:42
+#: models/notifications.py:44
 msgid "German"
 msgstr "Aleman"
 
-#: models/notifications.py:43
+#: models/notifications.py:45
 msgid "Spanish"
 msgstr "Español"
 
-#: models/notifications.py:44
+#: models/notifications.py:46
 msgid "Chinese Simplified"
 msgstr "Chino Simplificado"
 
-#: models/notifications.py:45
+#: models/notifications.py:47
 msgid "Russian"
 msgstr "Ruso"
 
-#: models/notifications.py:46
+#: models/notifications.py:48
 msgid "Korean"
 msgstr "eano"
 
-#: models/notifications.py:54
+#: models/notifications.py:56
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Upwell structure anchoring"
 msgstr "estructura anclandose"
 
-#: models/notifications.py:55
+#: models/notifications.py:57
 #, fuzzy
 #| msgid "Structure online"
 msgid "Upwell structure went online"
 msgstr "Estructura en linea"
 
-#: models/notifications.py:57
+#: models/notifications.py:59
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Upwell structure services went offline"
 msgstr "Servicios de la estructura apagados"
 
-#: models/notifications.py:60
+#: models/notifications.py:62
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went high power"
 msgstr "La estructura se encuentra en modo low power"
 
-#: models/notifications.py:63
+#: models/notifications.py:65
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went low power"
 msgstr "La estructura se encuentra en modo low power"
 
-#: models/notifications.py:65
+#: models/notifications.py:67
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Upwell structure unanchoring"
 msgstr "Estructura en desanclado"
 
-#: models/notifications.py:66
+#: models/notifications.py:68
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure fuel alert"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:67
+#: models/notifications.py:69
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure refueled"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:69
+#: models/notifications.py:71
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure jump fuel alert"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:72
+#: models/notifications.py:74
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "Upwell structure is under attack"
 msgstr "Estructura bajo ataque"
 
-#: models/notifications.py:74
+#: models/notifications.py:76
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "Upwell structure lost shields"
 msgstr "La estructura perdió sus escudos"
 
-#: models/notifications.py:75
+#: models/notifications.py:77
 #, fuzzy
 #| msgid "Structure lost armor"
 msgid "Upwell structure lost armor"
 msgstr "La estructura perdio su armadura"
 
-#: models/notifications.py:76
+#: models/notifications.py:78
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Upwell structure destroyed"
 msgstr "Estructura destruida"
 
-#: models/notifications.py:79
+#: models/notifications.py:81
 msgid "Upwell structure reinforcement time changed"
 msgstr ""
 
-#: models/notifications.py:82
+#: models/notifications.py:84
 #, fuzzy
 #| msgid "Ownership transferred"
 msgid "Upwell structure ownership transferred"
 msgstr "propiedad transferida"
 
-#: models/notifications.py:86
+#: models/notifications.py:88
 msgid "Customs office attacked"
 msgstr ""
 
-#: models/notifications.py:87
+#: models/notifications.py:89
 msgid "Customs office reinforced"
 msgstr ""
 
-#: models/notifications.py:90
+#: models/notifications.py:92
 msgid "Starbase attacked"
 msgstr ""
 
-#: models/notifications.py:92
+#: models/notifications.py:94
 msgid "Starbase refueled (BETA)"
 msgstr ""
 
-#: models/notifications.py:93
+#: models/notifications.py:95
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced (BETA)"
 msgstr "Orbital reinforzado"
 
-#: models/notifications.py:99
+#: models/notifications.py:101
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moonmining laser fired"
 msgstr "Extraccion de luna iniciada"
 
-#: models/notifications.py:101
+#: models/notifications.py:103
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction cancelled"
 msgstr "Extraccion de luna iniciada"
 
-#: models/notifications.py:104
+#: models/notifications.py:106
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction finished"
 msgstr "Extraccion de luna iniciada"
 
-#: models/notifications.py:107
+#: models/notifications.py:109
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining automatic fracture triggered"
 msgstr "Extraccion de luna iniciada"
 
-#: models/notifications.py:112
+#: models/notifications.py:114
 msgid "Sovereignty structure reinforced"
 msgstr ""
 
-#: models/notifications.py:115
+#: models/notifications.py:117
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Sovereignty structure destroyed"
 msgstr "Estructura destruida"
 
-#: models/notifications.py:118
+#: models/notifications.py:120
 msgid "Sovereignty entosis capture started"
 msgstr ""
 
-#: models/notifications.py:121
+#: models/notifications.py:123
 msgid "Sovereignty command node event started"
 msgstr ""
 
-#: models/notifications.py:124
+#: models/notifications.py:126
 msgid "Sovereignty claim acknowledgment"
 msgstr ""
 
-#: models/notifications.py:126
+#: models/notifications.py:128
 msgid "Sovereignty lost"
 msgstr ""
 
-#: models/notifications.py:128
+#: models/notifications.py:130
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Structure anchoring in alliance space"
 msgstr "estructura anclandose"
 
-#: models/notifications.py:132
+#: models/notifications.py:134
 msgid "War declared"
 msgstr ""
 
-#: models/notifications.py:134
+#: models/notifications.py:136
 msgid "War ally joined aggressor"
 msgstr ""
 
-#: models/notifications.py:136
+#: models/notifications.py:138
 msgid "War ally joined ally"
 msgstr ""
 
-#: models/notifications.py:138
+#: models/notifications.py:140
 msgid "War ally joined defender"
 msgstr ""
 
-#: models/notifications.py:140
+#: models/notifications.py:142
 msgid "War adopted"
 msgstr ""
 
-#: models/notifications.py:141
+#: models/notifications.py:143
 msgid "War inherited"
 msgstr ""
 
-#: models/notifications.py:142
+#: models/notifications.py:144
 msgid "War party surrendered"
 msgstr ""
 
-#: models/notifications.py:144
+#: models/notifications.py:146
 msgid "War retracted by Concord"
 msgstr ""
 
-#: models/notifications.py:147
+#: models/notifications.py:149
 msgid "War corporation became eligible"
 msgstr ""
 
-#: models/notifications.py:150
+#: models/notifications.py:152
 msgid "War corporation no longer eligible"
 msgstr ""
 
-#: models/notifications.py:152
+#: models/notifications.py:154
 msgid "War surrender offered"
 msgstr ""
 
-#: models/notifications.py:155
+#: models/notifications.py:157
 msgid "Character submitted application"
 msgstr ""
 
-#: models/notifications.py:157
+#: models/notifications.py:159
 msgid "Character invited to join corporation"
 msgstr ""
 
-#: models/notifications.py:160
+#: models/notifications.py:162
 msgid "Corp application rejected"
 msgstr ""
 
-#: models/notifications.py:162
+#: models/notifications.py:164
 msgid "Character withdrew application"
 msgstr ""
 
-#: models/notifications.py:163
+#: models/notifications.py:165
 msgid "Character joins corporation"
 msgstr ""
 
-#: models/notifications.py:164
+#: models/notifications.py:166
 msgid "Character leaves corporation"
 msgstr ""
 
-#: models/notifications.py:167
+#: models/notifications.py:169
 msgid "Bill out of money"
 msgstr ""
 
-#: models/notifications.py:170
+#: models/notifications.py:172
 msgid "I-HUB bill about to expire"
 msgstr ""
 
-#: models/notifications.py:174
+#: models/notifications.py:176
 msgid "I_HUB destroyed by bill failure"
 msgstr ""
 
-#: models/notifications.py:334
+#: models/notifications.py:336
 msgid "notification types"
 msgstr ""
 
-#: models/notifications.py:336
+#: models/notifications.py:338
 msgid "Select which type of notifications should be forwarded to this webhook"
 msgstr ""
 
-#: models/notifications.py:345
+#: models/notifications.py:347
 msgid "language"
 msgstr ""
 
-#: models/notifications.py:346
+#: models/notifications.py:348
 msgid "language of notifications send to this webhook"
 msgstr ""
 
-#: models/notifications.py:350 models/structures.py:91
+#: models/notifications.py:352 models/structures.py:92
 msgid "is default"
 msgstr ""
 
-#: models/notifications.py:352
+#: models/notifications.py:354
 msgid "Whether owners have this webhook automatically pre-set when created"
 msgstr ""
 
-#: models/notifications.py:357 models/owners.py:151
+#: models/notifications.py:359 models/owners.py:153
 msgid "has default pings enabled"
 msgstr ""
 
-#: models/notifications.py:368 models/owners.py:197
+#: models/notifications.py:370 models/owners.py:199
 msgid "ping groups"
 msgstr ""
 
-#: models/notifications.py:369
+#: models/notifications.py:371
 msgid "Groups to be pinged for each notification - "
 msgstr ""
 
-#: models/notifications.py:374
+#: models/notifications.py:376
 msgid "webhook"
 msgstr ""
 
-#: models/notifications.py:375 models/owners.py:212 models/structures.py:389
+#: models/notifications.py:377 models/owners.py:214 models/structures.py:390
 msgid "webhooks"
 msgstr ""
 
-#: models/notifications.py:388
+#: models/notifications.py:390
 msgid "is sent"
 msgstr ""
 
-#: models/notifications.py:389
+#: models/notifications.py:391
 msgid "True when this notification has been forwarded to Discord"
 msgstr ""
 
-#: models/notifications.py:394
+#: models/notifications.py:396
 msgid "is timer added"
 msgstr ""
 
-#: models/notifications.py:395
+#: models/notifications.py:397
 msgid "True when a timer has been added for this notification"
 msgstr ""
 
-#: models/notifications.py:401 models/structures.py:242
-#: models/structures.py:773
+#: models/notifications.py:403 models/structures.py:243
+#: models/structures.py:787
 msgid "type"
 msgstr ""
 
-#: models/notifications.py:402
+#: models/notifications.py:404
 msgid "type of this notification"
 msgstr ""
 
-#: models/notifications.py:407 models/owners.py:219 models/owners.py:1278
-#: models/structures.py:312
+#: models/notifications.py:409 models/owners.py:221 models/owners.py:1287
+#: models/structures.py:313
 msgid "owner"
 msgstr ""
 
-#: models/notifications.py:408
+#: models/notifications.py:410
 msgid "Corporation that owns this notification"
 msgstr ""
 
-#: models/notifications.py:412 models/structures.py:402
+#: models/notifications.py:414 models/structures.py:403
 #, fuzzy
 #| msgid "Structure online"
 msgid "structures"
 msgstr "Estructura en linea"
 
-#: models/notifications.py:413
+#: models/notifications.py:415
 msgid "Structures this notification is about (if any)"
 msgstr ""
 
-#: models/notifications.py:682 models/structures.py:202
-#: models/structures.py:759
+#: models/notifications.py:694 models/structures.py:203
+#: models/structures.py:773
 msgid "id"
 msgstr ""
 
-#: models/notifications.py:686
+#: models/notifications.py:698
 msgid "created"
 msgstr ""
 
-#: models/notifications.py:687
+#: models/notifications.py:699
 msgid "Date when this notification was first received from ESI"
 msgstr ""
 
-#: models/notifications.py:692
+#: models/notifications.py:704
 msgid "is read"
 msgstr ""
 
-#: models/notifications.py:693
+#: models/notifications.py:705
 msgid "True when this notification has read in the eve client"
 msgstr ""
 
-#: models/notifications.py:696
+#: models/notifications.py:708
 msgid "last updated"
 msgstr ""
 
-#: models/notifications.py:697
+#: models/notifications.py:709
 msgid "Date when this notification has last been updated from ESI"
 msgstr ""
 
-#: models/notifications.py:704
+#: models/notifications.py:716
 msgid "sender"
 msgstr ""
 
-#: models/notifications.py:711
+#: models/notifications.py:723
 msgid "text"
 msgstr ""
 
-#: models/notifications.py:712
+#: models/notifications.py:724
 msgid "Notification details in YAML"
 msgstr ""
 
-#: models/notifications.py:714 models/notifications.py:831
+#: models/notifications.py:726 models/notifications.py:843
 msgid "timestamp"
 msgstr ""
 
-#: models/notifications.py:719
+#: models/notifications.py:731
 msgid "eve notification"
 msgstr ""
 
-#: models/notifications.py:720
+#: models/notifications.py:732
 msgid "eve notifications"
 msgstr ""
 
-#: models/notifications.py:829
+#: models/notifications.py:841
 msgid "details"
 msgstr ""
 
-#: models/notifications.py:830
+#: models/notifications.py:842
 msgid "last_updated"
 msgstr ""
 
-#: models/notifications.py:836
+#: models/notifications.py:848
 msgid "generated notification"
 msgstr ""
 
-#: models/notifications.py:837
+#: models/notifications.py:849
 msgid "generated  notifications"
 msgstr ""
 
-#: models/notifications.py:866
+#: models/notifications.py:878
 msgid "channel pings"
 msgstr ""
 
-#: models/notifications.py:868
+#: models/notifications.py:880
 msgid ""
 "Option to ping every member of the channel. This setting can be overruled by "
 "the respective owner or webhook configuration"
 msgstr ""
 
-#: models/notifications.py:878
+#: models/notifications.py:890
 msgid "color"
 msgstr ""
 
-#: models/notifications.py:879
+#: models/notifications.py:891
 msgid "Context color of these notification on Discord"
 msgstr ""
 
-#: models/notifications.py:883
+#: models/notifications.py:895
 msgid "is_enabled"
 msgstr ""
 
-#: models/notifications.py:884
+#: models/notifications.py:896
 msgid "Disabled configurations will not create any new alerts."
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "end"
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "End of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:910
+#: models/notifications.py:922
 msgid "repeat"
 msgstr ""
 
-#: models/notifications.py:912
+#: models/notifications.py:924
 msgid "Notifications will be repeated every x hours. Set to 0 for no repeats"
 msgstr ""
 
-#: models/notifications.py:916
+#: models/notifications.py:928
 msgid "start"
 msgstr ""
 
-#: models/notifications.py:917
+#: models/notifications.py:929
 msgid "Start of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:921
+#: models/notifications.py:933
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert config"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:922
+#: models/notifications.py:934
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert configs"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:927
+#: models/notifications.py:941
 msgid "Start must be before end, i.e. have a larger value."
 msgstr ""
 
-#: models/notifications.py:931
+#: models/notifications.py:945
 msgid "Repeat can not be larger that the interval size."
 msgstr ""
 
-#: models/notifications.py:940
+#: models/notifications.py:954
 msgid "This configuration may not overlap with an existing configuration."
 msgstr ""
 
-#: models/notifications.py:1007
+#: models/notifications.py:1021
 msgid "threshold"
 msgstr ""
 
-#: models/notifications.py:1009
+#: models/notifications.py:1023
 msgid ""
 "Notifications will be sent once fuel level in units reaches this threshold"
 msgstr ""
 
-#: models/notifications.py:1014
+#: models/notifications.py:1028
 msgid "jump fuel alert config"
 msgstr ""
 
-#: models/notifications.py:1015
+#: models/notifications.py:1029
 msgid "jump fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:1064 models/notifications.py:1114
-#: models/structures.py:401 models/structures.py:765 models/structures.py:830
+#: models/notifications.py:1078 models/notifications.py:1128
+#: models/structures.py:402 models/structures.py:779 models/structures.py:844
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure"
 msgstr "Estructura en linea"
 
-#: models/notifications.py:1070 models/notifications.py:1120
+#: models/notifications.py:1084 models/notifications.py:1134
 msgid "configuration"
 msgstr ""
 
-#: models/notifications.py:1074
+#: models/notifications.py:1088
 msgid "hours"
 msgstr ""
 
-#: models/notifications.py:1075
+#: models/notifications.py:1089
 msgid "number of hours before fuel expiration this alert was sent"
 msgstr ""
 
-#: models/notifications.py:1079
+#: models/notifications.py:1093
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:1080
+#: models/notifications.py:1094
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alerts"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:1124
+#: models/notifications.py:1138
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alert"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/notifications.py:1125
+#: models/notifications.py:1139
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alerts"
 msgstr "Alerta de combustible de la estructura"
 
-#: models/owners.py:117
+#: models/owners.py:119
 msgid "corporation"
 msgstr ""
 
-#: models/owners.py:118
+#: models/owners.py:120
 msgid "Corporation owning structures"
 msgstr ""
 
-#: models/owners.py:123
+#: models/owners.py:125
 msgid "are pocos public"
 msgstr ""
 
-#: models/owners.py:124
+#: models/owners.py:126
 msgid "whether pocos of this owner are shown on public POCO page"
 msgstr ""
 
-#: models/owners.py:130
+#: models/owners.py:132
 msgid "assets last update at"
 msgstr ""
 
-#: models/owners.py:131 models/owners.py:147 models/owners.py:190
-#: models/owners.py:205
+#: models/owners.py:133 models/owners.py:149 models/owners.py:192
+#: models/owners.py:207
 msgid "when the last successful update happened"
 msgstr ""
 
-#: models/owners.py:146
+#: models/owners.py:148
 msgid "forwarding last update at"
 msgstr ""
 
-#: models/owners.py:153
+#: models/owners.py:155
 msgid ""
 "to enable or disable pinging of notifications for this owner e.g. with "
 "@everyone and @here"
 msgstr ""
 
-#: models/owners.py:159
+#: models/owners.py:161
 msgid "is active"
 msgstr ""
 
-#: models/owners.py:160
+#: models/owners.py:162
 msgid "whether this owner is currently included in the sync process"
 msgstr ""
 
-#: models/owners.py:164
+#: models/owners.py:166
 msgid "is alliance main"
 msgstr ""
 
-#: models/owners.py:166
+#: models/owners.py:168
 msgid ""
 "whether alliance wide notifications are forwarded for this owner (e.g. sov "
 "notifications)"
 msgstr ""
 
-#: models/owners.py:172
+#: models/owners.py:174
 msgid "is included in service status"
 msgstr ""
 
-#: models/owners.py:174
+#: models/owners.py:176
 msgid ""
 "whether the sync status of this owner is included in the overall status of "
 "this services"
 msgstr ""
 
-#: models/owners.py:182
+#: models/owners.py:184
 msgid "is up"
 msgstr ""
 
-#: models/owners.py:183
+#: models/owners.py:185
 msgid "whether all services for this owner are currently up"
 msgstr ""
 
-#: models/owners.py:189
+#: models/owners.py:191
 msgid "notifications last update at"
 msgstr ""
 
-#: models/owners.py:198
+#: models/owners.py:200
 msgid "Groups to be pinged for each notification. "
 msgstr ""
 
-#: models/owners.py:204
+#: models/owners.py:206
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "structures last update at"
 msgstr "Estructura bajo ataque"
 
-#: models/owners.py:213
+#: models/owners.py:215
 msgid "Notifications are sent to these webhooks."
 msgstr ""
 
-#: models/owners.py:220
+#: models/owners.py:222
 msgid "owners"
 msgstr ""
 
-#: models/owners.py:1139
+#: models/owners.py:1147
 #, python-format
 msgid ""
 "Syncing of %(topic)s for %(owner)s %(result)s.\n"
 " %(message_details)s"
 msgstr ""
 
-#: models/owners.py:1143
+#: models/owners.py:1151
 msgid "completed successfully"
 msgstr ""
 
-#: models/owners.py:1148
+#: models/owners.py:1156
 #, python-format
 msgid "%(title)s: %(topic)s updated for %(owner)s: %(result)s"
 msgstr ""
 
-#: models/owners.py:1153
+#: models/owners.py:1161
 msgid "OK"
 msgstr ""
 
-#: models/owners.py:1284
+#: models/owners.py:1293
 msgid "character_ownership"
 msgstr ""
 
-#: models/owners.py:1292
+#: models/owners.py:1301
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "structures last used at"
 msgstr "La estructura perdió sus escudos"
 
-#: models/owners.py:1300
+#: models/owners.py:1309
 msgid "notifications last used at"
 msgstr ""
 
-#: models/owners.py:1306
+#: models/owners.py:1315
 msgid "error count"
 msgstr ""
 
-#: models/owners.py:1312
+#: models/owners.py:1321
 msgid "owner character"
 msgstr ""
 
-#: models/owners.py:1313
+#: models/owners.py:1322
 msgid "owner characters"
 msgstr ""
 
-#: models/structures.py:37
+#: models/structures.py:38
 msgid "sov"
 msgstr ""
 
-#: models/structures.py:38
+#: models/structures.py:39
 msgid "highsec"
 msgstr ""
 
-#: models/structures.py:39
+#: models/structures.py:40
 msgid "lowsec"
 msgstr ""
 
-#: models/structures.py:40
+#: models/structures.py:41
 msgid "nullsec"
 msgstr ""
 
-#: models/structures.py:41
+#: models/structures.py:42
 msgid "w_space"
 msgstr ""
 
-#: models/structures.py:44
+#: models/structures.py:45
 msgid "grey"
 msgstr ""
 
-#: models/structures.py:45
+#: models/structures.py:46
 msgid "dark blue"
 msgstr ""
 
-#: models/structures.py:46
+#: models/structures.py:47
 msgid "green"
 msgstr ""
 
-#: models/structures.py:47
+#: models/structures.py:48
 msgid "light blue"
 msgstr ""
 
-#: models/structures.py:48
+#: models/structures.py:49
 msgid "orange"
 msgstr ""
 
-#: models/structures.py:49
+#: models/structures.py:50
 msgid "red"
 msgstr ""
 
-#: models/structures.py:61 models/structures.py:284 models/structures.py:834
+#: models/structures.py:62 models/structures.py:285 models/structures.py:848
 msgid "name"
 msgstr ""
 
-#: models/structures.py:62
+#: models/structures.py:63
 msgid "name of the tag - must be unique"
 msgstr ""
 
-#: models/structures.py:68
+#: models/structures.py:69
 msgid "description"
 msgstr ""
 
-#: models/structures.py:69
+#: models/structures.py:70
 msgid "description for this tag"
 msgstr ""
 
-#: models/structures.py:76
+#: models/structures.py:77
 msgid "style"
 msgstr ""
 
-#: models/structures.py:77
+#: models/structures.py:78
 msgid "color style of tag"
 msgstr ""
 
-#: models/structures.py:83
+#: models/structures.py:84
 msgid "order"
 msgstr ""
 
-#: models/structures.py:85
+#: models/structures.py:86
 msgid ""
 "number defining the order tags are shown. custom tags can not have an order "
 "below 100"
 msgstr ""
 
-#: models/structures.py:93
+#: models/structures.py:94
 msgid "if true this custom tag will automatically be added to new structures"
 msgstr ""
 
-#: models/structures.py:98
+#: models/structures.py:99
 msgid "is user managed"
 msgstr ""
 
-#: models/structures.py:100
+#: models/structures.py:101
 msgid ""
 "if False this tag is created and managed by the system and can not be "
 "modified by users"
 msgstr ""
 
-#: models/structures.py:108
+#: models/structures.py:109
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure tag"
 msgstr "Estructura en linea"
 
-#: models/structures.py:109
+#: models/structures.py:110
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure tags"
 msgstr "Estructura en linea"
 
-#: models/structures.py:143
+#: models/structures.py:144
 msgid "anchor vulnerable"
 msgstr ""
 
-#: models/structures.py:144
+#: models/structures.py:145
 msgid "anchoring"
 msgstr ""
 
-#: models/structures.py:145
+#: models/structures.py:146
 msgid "armor reinforce"
 msgstr ""
 
-#: models/structures.py:146
+#: models/structures.py:147
 msgid "armor vulnerable"
 msgstr ""
 
-#: models/structures.py:147
+#: models/structures.py:148
 msgid "deploy vulnerable"
 msgstr ""
 
-#: models/structures.py:148
+#: models/structures.py:149
 msgid "fitting invulnerable"
 msgstr ""
 
-#: models/structures.py:149
+#: models/structures.py:150
 msgid "hull reinforce"
 msgstr ""
 
-#: models/structures.py:150
+#: models/structures.py:151
 msgid "hull vulnerable"
 msgstr ""
 
-#: models/structures.py:151
+#: models/structures.py:152
 msgid "online deprecated"
 msgstr ""
 
-#: models/structures.py:152
+#: models/structures.py:153
 msgid "onlining vulnerable"
 msgstr ""
 
-#: models/structures.py:153
+#: models/structures.py:154
 msgid "shield vulnerable"
 msgstr ""
 
-#: models/structures.py:154
+#: models/structures.py:155
 msgid "unanchored"
 msgstr ""
 
-#: models/structures.py:156 models/structures.py:813
+#: models/structures.py:157 models/structures.py:827
 msgid "offline"
 msgstr ""
 
-#: models/structures.py:157 models/structures.py:814
+#: models/structures.py:158 models/structures.py:828
 msgid "online"
 msgstr ""
 
-#: models/structures.py:158
+#: models/structures.py:159
 msgid "onlining"
 msgstr ""
 
-#: models/structures.py:159
+#: models/structures.py:160
 msgid "reinforced"
 msgstr ""
 
-#: models/structures.py:160
+#: models/structures.py:161
 msgid "unanchoring "
 msgstr ""
 
-#: models/structures.py:163
+#: models/structures.py:164
 msgid "unknown"
 msgstr ""
 
-#: models/structures.py:194
+#: models/structures.py:195
 msgid "Full Power"
 msgstr ""
 
-#: models/structures.py:195
+#: models/structures.py:196
 msgid "Low Power"
 msgstr ""
 
-#: models/structures.py:196
+#: models/structures.py:197
 msgid "Abandoned"
 msgstr ""
 
-#: models/structures.py:197
+#: models/structures.py:198
 msgid "Abandoned?"
 msgstr ""
 
-#: models/structures.py:198
+#: models/structures.py:199
 #, fuzzy
 #| msgid "(unknown)"
 msgid "Unknown"
 msgstr "(desconocido)"
 
-#: models/structures.py:203
+#: models/structures.py:204
 msgid "The Item ID of the structure"
 msgstr ""
 
-#: models/structures.py:208
+#: models/structures.py:209
 msgid "created at"
 msgstr ""
 
-#: models/structures.py:209
+#: models/structures.py:210
 msgid "date this structure was received from ESI for the first time"
 msgstr ""
 
-#: models/structures.py:218
+#: models/structures.py:219
 msgid "moon"
 msgstr ""
 
-#: models/structures.py:219
+#: models/structures.py:220
 msgid "Moon next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:228
+#: models/structures.py:229
 msgid "planet"
 msgstr ""
 
-#: models/structures.py:229
+#: models/structures.py:230
 msgid "Planet next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:235
+#: models/structures.py:236
 msgid "solar system"
 msgstr ""
 
-#: models/structures.py:236
+#: models/structures.py:237
 msgid "Solar System the structure is located"
 msgstr ""
 
-#: models/structures.py:243
+#: models/structures.py:244
 msgid "Type of the structure"
 msgstr ""
 
-#: models/structures.py:249
+#: models/structures.py:250
 msgid "fuel expires at"
 msgstr ""
 
-#: models/structures.py:250
+#: models/structures.py:251
 msgid "Date on which the structure will run out of fuel"
 msgstr ""
 
-#: models/structures.py:257
+#: models/structures.py:258
 msgid "has fitting"
 msgstr ""
 
-#: models/structures.py:258
+#: models/structures.py:259
 msgid "bool indicating if the structure has a fitting"
 msgstr ""
 
-#: models/structures.py:265
+#: models/structures.py:266
 msgid "has core"
 msgstr ""
 
-#: models/structures.py:266
+#: models/structures.py:267
 msgid "bool indicating if the structure has a quantum core"
 msgstr ""
 
-#: models/structures.py:272
+#: models/structures.py:273
 msgid "last online at"
 msgstr ""
 
-#: models/structures.py:273
+#: models/structures.py:274
 msgid "date this structure had any of it's services online"
 msgstr ""
 
-#: models/structures.py:279 models/structures.py:778
+#: models/structures.py:280 models/structures.py:792
 msgid "last updated at"
 msgstr ""
 
-#: models/structures.py:280
+#: models/structures.py:281
 msgid "date this structure was last updated from the EVE server"
 msgstr ""
 
-#: models/structures.py:285
+#: models/structures.py:286
 msgid "The full name of the structure"
 msgstr ""
 
-#: models/structures.py:292
+#: models/structures.py:293
 msgid "next reinforce hour"
 msgstr ""
 
-#: models/structures.py:294 models/structures.py:304
+#: models/structures.py:295 models/structures.py:305
 msgid ""
 "The requested change to reinforce_hour that will take effect at the time "
 "shown by next_reinforce_apply"
 msgstr ""
 
-#: models/structures.py:302
+#: models/structures.py:303
 msgid "next reinforce apply"
 msgstr ""
 
-#: models/structures.py:313
+#: models/structures.py:314
 msgid "Corporation that owns the structure"
 msgstr ""
 
-#: models/structures.py:320
+#: models/structures.py:321
 msgid "reinforce hour"
 msgstr ""
 
-#: models/structures.py:322
+#: models/structures.py:323
 msgid ""
 "The average hour of day that determines the time +/- some hours when the "
 "structure will randomly exit its reinforcement periods and become vulnerable "
 "to attack against its armor and/or hull. "
 msgstr ""
 
-#: models/structures.py:331
+#: models/structures.py:332
 msgid "position x"
 msgstr ""
 
-#: models/structures.py:332
+#: models/structures.py:333
 msgid "x position in the solar system"
 msgstr ""
 
-#: models/structures.py:338
+#: models/structures.py:339
 msgid "position y"
 msgstr ""
 
-#: models/structures.py:339
+#: models/structures.py:340
 msgid "y position in the solar system"
 msgstr ""
 
-#: models/structures.py:345
+#: models/structures.py:346
 msgid "position z"
 msgstr ""
 
-#: models/structures.py:346
+#: models/structures.py:347
 msgid "z position in the solar system"
 msgstr ""
 
-#: models/structures.py:352 models/structures.py:839
+#: models/structures.py:353 models/structures.py:853
 msgid "state"
 msgstr ""
 
-#: models/structures.py:353
+#: models/structures.py:354
 msgid "Current state of the structure"
 msgstr ""
 
-#: models/structures.py:359
+#: models/structures.py:360
 msgid "state timer end"
 msgstr ""
 
-#: models/structures.py:360
+#: models/structures.py:361
 msgid "Date at which the structure entered it's current state"
 msgstr ""
 
-#: models/structures.py:366
+#: models/structures.py:367
 msgid "state timer start"
 msgstr ""
 
-#: models/structures.py:367
+#: models/structures.py:368
 msgid "Date at which the structure will move to it's next state"
 msgstr ""
 
-#: models/structures.py:374
+#: models/structures.py:375
 msgid "tags"
 msgstr ""
 
-#: models/structures.py:375
+#: models/structures.py:376
 msgid "List of tags for this structure. "
 msgstr ""
 
-#: models/structures.py:381
+#: models/structures.py:382
 msgid "unanchors at"
 msgstr ""
 
-#: models/structures.py:382
+#: models/structures.py:383
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Date at which the structure will unanchor"
 msgstr "Estructura en desanclado"
 
-#: models/structures.py:391
+#: models/structures.py:392
 msgid ""
 "Webhooks for sending notifications to. If any webhook is enabled, these will "
 "be used instead of the webhooks defined for the respective owner. If no "
 "webhook is enabled the owner's setting will be used. "
 msgstr ""
 
-#: models/structures.py:759
+#: models/structures.py:773
 msgid "The Eve item ID"
 msgstr ""
 
-#: models/structures.py:766
+#: models/structures.py:780
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this item is located in"
 msgstr "Servicios de la estructura apagados"
 
-#: models/structures.py:774
+#: models/structures.py:788
 msgid "type of the item"
 msgstr ""
 
-#: models/structures.py:776
+#: models/structures.py:790
 msgid "is singleton"
 msgstr ""
 
-#: models/structures.py:780
+#: models/structures.py:794
 msgid "location flag"
 msgstr ""
 
-#: models/structures.py:781
+#: models/structures.py:795
 msgid "quantity"
 msgstr ""
 
-#: models/structures.py:784
+#: models/structures.py:798
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure item"
 msgstr "Estructura en linea"
 
-#: models/structures.py:785
+#: models/structures.py:799
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure items"
 msgstr "Estructura en linea"
 
-#: models/structures.py:831
+#: models/structures.py:845
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this service is installed to"
 msgstr "Servicios de la estructura apagados"
 
-#: models/structures.py:834
+#: models/structures.py:848
 msgid "Name of the service"
 msgstr ""
 
-#: models/structures.py:840
+#: models/structures.py:854
 msgid "Current state of this service"
 msgstr ""
 
-#: models/structures.py:844
+#: models/structures.py:858
 #, fuzzy
 #| msgid "Structure online"
 msgid "structure service"
 msgstr "Estructura en linea"
 
-#: models/structures.py:845
+#: models/structures.py:859
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "structure services"
 msgstr "Servicios de la estructura apagados"
 
-#: models/structures.py:861 webhooks/models.py:12
+#: models/structures.py:875 webhooks/models.py:12
 msgid "none"
 msgstr ""
 
-#: models/structures.py:862
+#: models/structures.py:876
 msgid "terrible"
 msgstr ""
 
-#: models/structures.py:863
+#: models/structures.py:877
 msgid "bad"
 msgstr ""
 
-#: models/structures.py:864
+#: models/structures.py:878
 msgid "neutral"
 msgstr ""
 
-#: models/structures.py:865
+#: models/structures.py:879
 msgid "good"
 msgstr ""
 
-#: models/structures.py:866
+#: models/structures.py:880
 msgid "excellent"
 msgstr ""
 
-#: models/structures.py:960
+#: models/structures.py:974
 msgid "alliance member"
 msgstr ""
 
-#: models/structures.py:961
+#: models/structures.py:975
 msgid "config starbase equipment role"
 msgstr ""
 
-#: models/structures.py:962
+#: models/structures.py:976
 msgid "corporation member"
 msgstr ""
 
-#: models/structures.py:963
+#: models/structures.py:977
 msgid "starbase fuel technician role"
 msgstr ""
 
 #: templates/structures/base.html:4
 #, fuzzy
 #| msgid "Structure online"
 msgid "Structures"
@@ -2289,67 +2298,67 @@
 msgid "No Access"
 msgstr ""
 
 #: templates/structures/templatetags/list_tax_item.html:11
 msgid "Has Access"
 msgstr ""
 
-#: views.py:255
+#: views.py:256
 msgid "Fuel blocks per day (est.)"
 msgstr ""
 
-#: views.py:406
+#: views.py:407
 #, python-format
 msgid ""
 "You can only use your main or alt characters to add corporations. However, "
 "character %s is neither. "
 msgstr ""
 
-#: views.py:439
+#: views.py:440
 #, python-format
 msgid ""
 "%(corporation)s has been added with %(character)s as sync character. We have "
 "started fetching structures and notifications for this corporation and you "
 "will receive a report once the process is finished."
 msgstr ""
 
-#: views.py:455
+#: views.py:456
 #, python-format
 msgid "%(corporation)s was added as new structure owner by %(user)s."
 msgstr ""
 
-#: views.py:459
+#: views.py:460
 #, python-format
 msgid "%s: Structure owner added: %s"
 msgstr ""
 
-#: views.py:466
+#: views.py:467
 #, python-format
 msgid ""
 "%(character)s has been added to %(corporation)s as sync character. You now "
 "have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:481
+#: views.py:482
 #, python-format
 msgid ""
 "%(character)s was added as sync character to %(corporation)s by %(user)s.\n"
 "We now have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:491
+#: views.py:492
 #, python-format
 msgid "%s: Character added to: %s"
 msgstr ""
 
-#: views.py:508
+#: views.py:509
 msgid "service is up"
 msgstr ""
 
-#: views.py:510
+#: views.py:511
 msgid "service is down"
 msgstr ""
 
 #: webhooks/models.py:13
 msgid "here"
 msgstr ""
```

### Comparing `aa_structures-2.2.0/structures/locale/ko/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-17 02:47+0200\n"
-"PO-Revision-Date: 2020-03-09 19:25+0000\n"
-"Language-Team: Russian (Russia) (https://www.transifex.com/kalkoken-apps/"
-"teams/107978/ru_RU/)\n"
-"Language: ru_RU\n"
+"POT-Creation-Date: 2023-04-24 23:05+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin.py:111
 msgid "Sent fuel notifications for selected configuration"
 msgstr ""
 
-#: admin.py:240 models/structures.py:162
+#: admin.py:137
+msgid ""
+"Timing configuration for sending fuel notifications. Note that the first "
+"notification will be sent at the exact start hour, and the last notification "
+"will be sent one repeat before the end hour."
+msgstr ""
+
+#: admin.py:240 models/structures.py:163
 msgid "N/A"
 msgstr ""
 
 #: admin.py:255
 msgid "Not configured"
 msgstr ""
 
@@ -299,26 +304,26 @@
 #, python-format
 msgid ""
 "\n"
 "\n"
 "Change becomes effective at %s."
 msgstr ""
 
-#: core/notification_embeds.py:728 models/notifications.py:97
+#: core/notification_embeds.py:728 models/notifications.py:99
 msgid "Moon mining extraction started"
 msgstr ""
 
 #: core/notification_embeds.py:730
 #, python-format
 msgid ""
 "A moon mining extraction has been started for %(structure_name)s at %(moon)s "
 "in %(solar_system)s belonging to %(owner_link)s. Extraction was started by "
 "%(character)s.\n"
-"The chunk will be ready on location at %(ready_time)s, and will autofracture "
-"on %(auto_time)s.\n"
+"The chunk will be ready on location at %(ready_time)s, and will fracture "
+"automatically on %(auto_time)s.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:746
 #, python-format
 msgid ""
 "\n"
@@ -350,15 +355,15 @@
 #: core/notification_embeds.py:782
 msgid "Automatic Fracture"
 msgstr ""
 
 #: core/notification_embeds.py:784
 #, python-format
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has automatically been fired and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:810
 msgid "Extraction cancelled"
@@ -368,21 +373,21 @@
 #, python-format
 msgid ""
 "An ongoing extraction for %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been cancelled by %(character)s."
 msgstr ""
 
 #: core/notification_embeds.py:831
-msgid "Moondrill fired"
+msgid "Moon drill fired"
 msgstr ""
 
 #: core/notification_embeds.py:833
 #, python-format
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been fired by %(character)s and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 
 #: core/notification_embeds.py:876
 msgid "Orbital under attack"
@@ -403,15 +408,15 @@
 #, python-format
 msgid ""
 "The %(structure_type)s at %(planet)s in %(solar_system)s belonging to "
 "%(owner_link)s has been reinforced by %(aggressor)s and will come out at: "
 "%(date)s."
 msgstr ""
 
-#: core/notification_embeds.py:935 core/notification_embeds.py:1630
+#: core/notification_embeds.py:935 core/notification_embeds.py:1631
 #, python-format
 msgid ""
 "The starbase %(structure_name)s at %(moon)s in %(solar_system)s belonging to "
 "%(owner_link)s "
 msgstr ""
 
 #: core/notification_embeds.py:952
@@ -421,15 +426,15 @@
 #: core/notification_embeds.py:954
 #, python-format
 msgid ""
 "is under attack by %(aggressor)s.\n"
 "%(damage_text)s"
 msgstr ""
 
-#: core/notification_embeds.py:982 models/notifications.py:91
+#: core/notification_embeds.py:982 models/notifications.py:93
 msgid "Starbase fuel alert"
 msgstr ""
 
 #: core/notification_embeds.py:996
 msgid "Starbase refueled"
 msgstr ""
 
@@ -530,59 +535,59 @@
 msgid "%s has offered a surrender"
 msgstr ""
 
 #: core/notification_embeds.py:1535
 #, python-format
 msgid ""
 "%s has offered to end the war with %s in the exchange for %s ISK. If "
-"accepted, the war will end in 24 hours and your organizations willbe unable "
+"accepted, the war will end in 24 hours and your organizations will be unable "
 "to declare new wars against each other for the next 2 weeks."
 msgstr ""
 
 #: core/notification_embeds.py:1548
 msgid "Insufficient Funds for Bill"
 msgstr ""
 
 #: core/notification_embeds.py:1550
 #, python-format
 msgid ""
-"The selected corporation wallet division for autopayments does not have "
-"enough current funds available to pay the %(bill_type)s due to be paid by "
-"%(due_date)s. Transfer additional funds to the selected wallet division in "
-"order to meet your pending automatic bills."
+"The selected corporation wallet division for automatic payments does not "
+"have enough current funds available to pay the %(bill_type)s due to be paid "
+"by %(due_date)s. Transfer additional funds to the selected wallet division "
+"in order to meet your pending automatic bills."
 msgstr ""
 
-#: core/notification_embeds.py:1569
+#: core/notification_embeds.py:1570
 msgid "IHub Bill About to Expire"
 msgstr ""
 
-#: core/notification_embeds.py:1571
+#: core/notification_embeds.py:1572
 #, python-format
 msgid ""
 "Maintenance bill for Infrastructure Hub in %(solar_system)s expires at "
 "%(due_date)s, if not paid in time this Infrastructure Hub will self-destruct."
 msgstr ""
 
-#: core/notification_embeds.py:1596
+#: core/notification_embeds.py:1597
 #, python-format
 msgid "%s has self-destructed due to unpaid maintenance bills"
 msgstr ""
 
-#: core/notification_embeds.py:1600
+#: core/notification_embeds.py:1601
 #, python-format
 msgid ""
 "%(structure_type)s in %(solar_system)s has self-destructed, as the standard "
 "maintenance bills where not paid."
 msgstr ""
 
-#: core/notification_embeds.py:1645
+#: core/notification_embeds.py:1646
 msgid "Starbase reinforced"
 msgstr ""
 
-#: core/notification_embeds.py:1653
+#: core/notification_embeds.py:1654
 #, python-format
 msgid "has been reinforced and will come out at: %s."
 msgstr ""
 
 #: core/notification_timers.py:89
 msgid "Armor timer"
 msgstr ""
@@ -604,1117 +609,1117 @@
 msgid "yes"
 msgstr ""
 
 #: core/serializers.py:496
 msgid "no"
 msgstr ""
 
-#: models/notifications.py:41
+#: models/notifications.py:43
 msgid "English"
 msgstr ""
 
-#: models/notifications.py:42
+#: models/notifications.py:44
 msgid "German"
 msgstr ""
 
-#: models/notifications.py:43
+#: models/notifications.py:45
 msgid "Spanish"
 msgstr ""
 
-#: models/notifications.py:44
+#: models/notifications.py:46
 msgid "Chinese Simplified"
 msgstr ""
 
-#: models/notifications.py:45
+#: models/notifications.py:47
 msgid "Russian"
 msgstr ""
 
-#: models/notifications.py:46
+#: models/notifications.py:48
 msgid "Korean"
 msgstr ""
 
-#: models/notifications.py:54
+#: models/notifications.py:56
 msgid "Upwell structure anchoring"
 msgstr ""
 
-#: models/notifications.py:55
+#: models/notifications.py:57
 msgid "Upwell structure went online"
 msgstr ""
 
-#: models/notifications.py:57
+#: models/notifications.py:59
 msgid "Upwell structure services went offline"
 msgstr ""
 
-#: models/notifications.py:60
+#: models/notifications.py:62
 msgid "Upwell structure went high power"
 msgstr ""
 
-#: models/notifications.py:63
+#: models/notifications.py:65
 msgid "Upwell structure went low power"
 msgstr ""
 
-#: models/notifications.py:65
+#: models/notifications.py:67
 msgid "Upwell structure unanchoring"
 msgstr ""
 
-#: models/notifications.py:66
+#: models/notifications.py:68
 msgid "Upwell structure fuel alert"
 msgstr ""
 
-#: models/notifications.py:67
+#: models/notifications.py:69
 msgid "Upwell structure refueled"
 msgstr ""
 
-#: models/notifications.py:69
+#: models/notifications.py:71
 msgid "Upwell structure jump fuel alert"
 msgstr ""
 
-#: models/notifications.py:72
+#: models/notifications.py:74
 msgid "Upwell structure is under attack"
 msgstr ""
 
-#: models/notifications.py:74
+#: models/notifications.py:76
 msgid "Upwell structure lost shields"
 msgstr ""
 
-#: models/notifications.py:75
+#: models/notifications.py:77
 msgid "Upwell structure lost armor"
 msgstr ""
 
-#: models/notifications.py:76
+#: models/notifications.py:78
 msgid "Upwell structure destroyed"
 msgstr ""
 
-#: models/notifications.py:79
+#: models/notifications.py:81
 msgid "Upwell structure reinforcement time changed"
 msgstr ""
 
-#: models/notifications.py:82
+#: models/notifications.py:84
 msgid "Upwell structure ownership transferred"
 msgstr ""
 
-#: models/notifications.py:86
+#: models/notifications.py:88
 msgid "Customs office attacked"
 msgstr ""
 
-#: models/notifications.py:87
+#: models/notifications.py:89
 msgid "Customs office reinforced"
 msgstr ""
 
-#: models/notifications.py:90
+#: models/notifications.py:92
 msgid "Starbase attacked"
 msgstr ""
 
-#: models/notifications.py:92
+#: models/notifications.py:94
 msgid "Starbase refueled (BETA)"
 msgstr ""
 
-#: models/notifications.py:93
+#: models/notifications.py:95
 msgid "Starbase reinforced (BETA)"
 msgstr ""
 
-#: models/notifications.py:99
+#: models/notifications.py:101
 msgid "Moonmining laser fired"
 msgstr ""
 
-#: models/notifications.py:101
+#: models/notifications.py:103
 msgid "Moon mining extraction cancelled"
 msgstr ""
 
-#: models/notifications.py:104
+#: models/notifications.py:106
 msgid "Moon mining extraction finished"
 msgstr ""
 
-#: models/notifications.py:107
+#: models/notifications.py:109
 msgid "Moon mining automatic fracture triggered"
 msgstr ""
 
-#: models/notifications.py:112
+#: models/notifications.py:114
 msgid "Sovereignty structure reinforced"
 msgstr ""
 
-#: models/notifications.py:115
+#: models/notifications.py:117
 msgid "Sovereignty structure destroyed"
 msgstr ""
 
-#: models/notifications.py:118
+#: models/notifications.py:120
 msgid "Sovereignty entosis capture started"
 msgstr ""
 
-#: models/notifications.py:121
+#: models/notifications.py:123
 msgid "Sovereignty command node event started"
 msgstr ""
 
-#: models/notifications.py:124
+#: models/notifications.py:126
 msgid "Sovereignty claim acknowledgment"
 msgstr ""
 
-#: models/notifications.py:126
+#: models/notifications.py:128
 msgid "Sovereignty lost"
 msgstr ""
 
-#: models/notifications.py:128
+#: models/notifications.py:130
 msgid "Structure anchoring in alliance space"
 msgstr ""
 
-#: models/notifications.py:132
+#: models/notifications.py:134
 msgid "War declared"
 msgstr ""
 
-#: models/notifications.py:134
+#: models/notifications.py:136
 msgid "War ally joined aggressor"
 msgstr ""
 
-#: models/notifications.py:136
+#: models/notifications.py:138
 msgid "War ally joined ally"
 msgstr ""
 
-#: models/notifications.py:138
+#: models/notifications.py:140
 msgid "War ally joined defender"
 msgstr ""
 
-#: models/notifications.py:140
+#: models/notifications.py:142
 msgid "War adopted"
 msgstr ""
 
-#: models/notifications.py:141
+#: models/notifications.py:143
 msgid "War inherited"
 msgstr ""
 
-#: models/notifications.py:142
+#: models/notifications.py:144
 msgid "War party surrendered"
 msgstr ""
 
-#: models/notifications.py:144
+#: models/notifications.py:146
 msgid "War retracted by Concord"
 msgstr ""
 
-#: models/notifications.py:147
+#: models/notifications.py:149
 msgid "War corporation became eligible"
 msgstr ""
 
-#: models/notifications.py:150
+#: models/notifications.py:152
 msgid "War corporation no longer eligible"
 msgstr ""
 
-#: models/notifications.py:152
+#: models/notifications.py:154
 msgid "War surrender offered"
 msgstr ""
 
-#: models/notifications.py:155
+#: models/notifications.py:157
 msgid "Character submitted application"
 msgstr ""
 
-#: models/notifications.py:157
+#: models/notifications.py:159
 msgid "Character invited to join corporation"
 msgstr ""
 
-#: models/notifications.py:160
+#: models/notifications.py:162
 msgid "Corp application rejected"
 msgstr ""
 
-#: models/notifications.py:162
+#: models/notifications.py:164
 msgid "Character withdrew application"
 msgstr ""
 
-#: models/notifications.py:163
+#: models/notifications.py:165
 msgid "Character joins corporation"
 msgstr ""
 
-#: models/notifications.py:164
+#: models/notifications.py:166
 msgid "Character leaves corporation"
 msgstr ""
 
-#: models/notifications.py:167
+#: models/notifications.py:169
 msgid "Bill out of money"
 msgstr ""
 
-#: models/notifications.py:170
+#: models/notifications.py:172
 msgid "I-HUB bill about to expire"
 msgstr ""
 
-#: models/notifications.py:174
+#: models/notifications.py:176
 msgid "I_HUB destroyed by bill failure"
 msgstr ""
 
-#: models/notifications.py:334
+#: models/notifications.py:336
 msgid "notification types"
 msgstr ""
 
-#: models/notifications.py:336
+#: models/notifications.py:338
 msgid "Select which type of notifications should be forwarded to this webhook"
 msgstr ""
 
-#: models/notifications.py:345
+#: models/notifications.py:347
 msgid "language"
 msgstr ""
 
-#: models/notifications.py:346
+#: models/notifications.py:348
 msgid "language of notifications send to this webhook"
 msgstr ""
 
-#: models/notifications.py:350 models/structures.py:91
+#: models/notifications.py:352 models/structures.py:92
 msgid "is default"
 msgstr ""
 
-#: models/notifications.py:352
+#: models/notifications.py:354
 msgid "Whether owners have this webhook automatically pre-set when created"
 msgstr ""
 
-#: models/notifications.py:357 models/owners.py:151
+#: models/notifications.py:359 models/owners.py:153
 msgid "has default pings enabled"
 msgstr ""
 
-#: models/notifications.py:368 models/owners.py:197
+#: models/notifications.py:370 models/owners.py:199
 msgid "ping groups"
 msgstr ""
 
-#: models/notifications.py:369
+#: models/notifications.py:371
 msgid "Groups to be pinged for each notification - "
 msgstr ""
 
-#: models/notifications.py:374
+#: models/notifications.py:376
 msgid "webhook"
 msgstr ""
 
-#: models/notifications.py:375 models/owners.py:212 models/structures.py:389
+#: models/notifications.py:377 models/owners.py:214 models/structures.py:390
 msgid "webhooks"
 msgstr ""
 
-#: models/notifications.py:388
+#: models/notifications.py:390
 msgid "is sent"
 msgstr ""
 
-#: models/notifications.py:389
+#: models/notifications.py:391
 msgid "True when this notification has been forwarded to Discord"
 msgstr ""
 
-#: models/notifications.py:394
+#: models/notifications.py:396
 msgid "is timer added"
 msgstr ""
 
-#: models/notifications.py:395
+#: models/notifications.py:397
 msgid "True when a timer has been added for this notification"
 msgstr ""
 
-#: models/notifications.py:401 models/structures.py:242
-#: models/structures.py:773
+#: models/notifications.py:403 models/structures.py:243
+#: models/structures.py:787
 msgid "type"
 msgstr ""
 
-#: models/notifications.py:402
+#: models/notifications.py:404
 msgid "type of this notification"
 msgstr ""
 
-#: models/notifications.py:407 models/owners.py:219 models/owners.py:1278
-#: models/structures.py:312
+#: models/notifications.py:409 models/owners.py:221 models/owners.py:1287
+#: models/structures.py:313
 msgid "owner"
 msgstr ""
 
-#: models/notifications.py:408
+#: models/notifications.py:410
 msgid "Corporation that owns this notification"
 msgstr ""
 
-#: models/notifications.py:412 models/structures.py:402
+#: models/notifications.py:414 models/structures.py:403
 msgid "structures"
 msgstr ""
 
-#: models/notifications.py:413
+#: models/notifications.py:415
 msgid "Structures this notification is about (if any)"
 msgstr ""
 
-#: models/notifications.py:682 models/structures.py:202
-#: models/structures.py:759
+#: models/notifications.py:694 models/structures.py:203
+#: models/structures.py:773
 msgid "id"
 msgstr ""
 
-#: models/notifications.py:686
+#: models/notifications.py:698
 msgid "created"
 msgstr ""
 
-#: models/notifications.py:687
+#: models/notifications.py:699
 msgid "Date when this notification was first received from ESI"
 msgstr ""
 
-#: models/notifications.py:692
+#: models/notifications.py:704
 msgid "is read"
 msgstr ""
 
-#: models/notifications.py:693
+#: models/notifications.py:705
 msgid "True when this notification has read in the eve client"
 msgstr ""
 
-#: models/notifications.py:696
+#: models/notifications.py:708
 msgid "last updated"
 msgstr ""
 
-#: models/notifications.py:697
+#: models/notifications.py:709
 msgid "Date when this notification has last been updated from ESI"
 msgstr ""
 
-#: models/notifications.py:704
+#: models/notifications.py:716
 msgid "sender"
 msgstr ""
 
-#: models/notifications.py:711
+#: models/notifications.py:723
 msgid "text"
 msgstr ""
 
-#: models/notifications.py:712
+#: models/notifications.py:724
 msgid "Notification details in YAML"
 msgstr ""
 
-#: models/notifications.py:714 models/notifications.py:831
+#: models/notifications.py:726 models/notifications.py:843
 msgid "timestamp"
 msgstr ""
 
-#: models/notifications.py:719
+#: models/notifications.py:731
 msgid "eve notification"
 msgstr ""
 
-#: models/notifications.py:720
+#: models/notifications.py:732
 msgid "eve notifications"
 msgstr ""
 
-#: models/notifications.py:829
+#: models/notifications.py:841
 msgid "details"
 msgstr ""
 
-#: models/notifications.py:830
+#: models/notifications.py:842
 msgid "last_updated"
 msgstr ""
 
-#: models/notifications.py:836
+#: models/notifications.py:848
 msgid "generated notification"
 msgstr ""
 
-#: models/notifications.py:837
+#: models/notifications.py:849
 msgid "generated  notifications"
 msgstr ""
 
-#: models/notifications.py:866
+#: models/notifications.py:878
 msgid "channel pings"
 msgstr ""
 
-#: models/notifications.py:868
+#: models/notifications.py:880
 msgid ""
 "Option to ping every member of the channel. This setting can be overruled by "
 "the respective owner or webhook configuration"
 msgstr ""
 
-#: models/notifications.py:878
+#: models/notifications.py:890
 msgid "color"
 msgstr ""
 
-#: models/notifications.py:879
+#: models/notifications.py:891
 msgid "Context color of these notification on Discord"
 msgstr ""
 
-#: models/notifications.py:883
+#: models/notifications.py:895
 msgid "is_enabled"
 msgstr ""
 
-#: models/notifications.py:884
+#: models/notifications.py:896
 msgid "Disabled configurations will not create any new alerts."
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "end"
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "End of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:910
+#: models/notifications.py:922
 msgid "repeat"
 msgstr ""
 
-#: models/notifications.py:912
+#: models/notifications.py:924
 msgid "Notifications will be repeated every x hours. Set to 0 for no repeats"
 msgstr ""
 
-#: models/notifications.py:916
+#: models/notifications.py:928
 msgid "start"
 msgstr ""
 
-#: models/notifications.py:917
+#: models/notifications.py:929
 msgid "Start of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:921
+#: models/notifications.py:933
 msgid "structure fuel alert config"
 msgstr ""
 
-#: models/notifications.py:922
+#: models/notifications.py:934
 msgid "structure fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:927
+#: models/notifications.py:941
 msgid "Start must be before end, i.e. have a larger value."
 msgstr ""
 
-#: models/notifications.py:931
+#: models/notifications.py:945
 msgid "Repeat can not be larger that the interval size."
 msgstr ""
 
-#: models/notifications.py:940
+#: models/notifications.py:954
 msgid "This configuration may not overlap with an existing configuration."
 msgstr ""
 
-#: models/notifications.py:1007
+#: models/notifications.py:1021
 msgid "threshold"
 msgstr ""
 
-#: models/notifications.py:1009
+#: models/notifications.py:1023
 msgid ""
 "Notifications will be sent once fuel level in units reaches this threshold"
 msgstr ""
 
-#: models/notifications.py:1014
+#: models/notifications.py:1028
 msgid "jump fuel alert config"
 msgstr ""
 
-#: models/notifications.py:1015
+#: models/notifications.py:1029
 msgid "jump fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:1064 models/notifications.py:1114
-#: models/structures.py:401 models/structures.py:765 models/structures.py:830
+#: models/notifications.py:1078 models/notifications.py:1128
+#: models/structures.py:402 models/structures.py:779 models/structures.py:844
 msgid "structure"
 msgstr ""
 
-#: models/notifications.py:1070 models/notifications.py:1120
+#: models/notifications.py:1084 models/notifications.py:1134
 msgid "configuration"
 msgstr ""
 
-#: models/notifications.py:1074
+#: models/notifications.py:1088
 msgid "hours"
 msgstr ""
 
-#: models/notifications.py:1075
+#: models/notifications.py:1089
 msgid "number of hours before fuel expiration this alert was sent"
 msgstr ""
 
-#: models/notifications.py:1079
+#: models/notifications.py:1093
 msgid "structure fuel alert"
 msgstr ""
 
-#: models/notifications.py:1080
+#: models/notifications.py:1094
 msgid "structure fuel alerts"
 msgstr ""
 
-#: models/notifications.py:1124
+#: models/notifications.py:1138
 msgid "jump fuel alert"
 msgstr ""
 
-#: models/notifications.py:1125
+#: models/notifications.py:1139
 msgid "jump fuel alerts"
 msgstr ""
 
-#: models/owners.py:117
+#: models/owners.py:119
 msgid "corporation"
 msgstr ""
 
-#: models/owners.py:118
+#: models/owners.py:120
 msgid "Corporation owning structures"
 msgstr ""
 
-#: models/owners.py:123
+#: models/owners.py:125
 msgid "are pocos public"
 msgstr ""
 
-#: models/owners.py:124
+#: models/owners.py:126
 msgid "whether pocos of this owner are shown on public POCO page"
 msgstr ""
 
-#: models/owners.py:130
+#: models/owners.py:132
 msgid "assets last update at"
 msgstr ""
 
-#: models/owners.py:131 models/owners.py:147 models/owners.py:190
-#: models/owners.py:205
+#: models/owners.py:133 models/owners.py:149 models/owners.py:192
+#: models/owners.py:207
 msgid "when the last successful update happened"
 msgstr ""
 
-#: models/owners.py:146
+#: models/owners.py:148
 msgid "forwarding last update at"
 msgstr ""
 
-#: models/owners.py:153
+#: models/owners.py:155
 msgid ""
 "to enable or disable pinging of notifications for this owner e.g. with "
 "@everyone and @here"
 msgstr ""
 
-#: models/owners.py:159
+#: models/owners.py:161
 msgid "is active"
 msgstr ""
 
-#: models/owners.py:160
+#: models/owners.py:162
 msgid "whether this owner is currently included in the sync process"
 msgstr ""
 
-#: models/owners.py:164
+#: models/owners.py:166
 msgid "is alliance main"
 msgstr ""
 
-#: models/owners.py:166
+#: models/owners.py:168
 msgid ""
 "whether alliance wide notifications are forwarded for this owner (e.g. sov "
 "notifications)"
 msgstr ""
 
-#: models/owners.py:172
+#: models/owners.py:174
 msgid "is included in service status"
 msgstr ""
 
-#: models/owners.py:174
+#: models/owners.py:176
 msgid ""
 "whether the sync status of this owner is included in the overall status of "
 "this services"
 msgstr ""
 
-#: models/owners.py:182
+#: models/owners.py:184
 msgid "is up"
 msgstr ""
 
-#: models/owners.py:183
+#: models/owners.py:185
 msgid "whether all services for this owner are currently up"
 msgstr ""
 
-#: models/owners.py:189
+#: models/owners.py:191
 msgid "notifications last update at"
 msgstr ""
 
-#: models/owners.py:198
+#: models/owners.py:200
 msgid "Groups to be pinged for each notification. "
 msgstr ""
 
-#: models/owners.py:204
+#: models/owners.py:206
 msgid "structures last update at"
 msgstr ""
 
-#: models/owners.py:213
+#: models/owners.py:215
 msgid "Notifications are sent to these webhooks."
 msgstr ""
 
-#: models/owners.py:220
+#: models/owners.py:222
 msgid "owners"
 msgstr ""
 
-#: models/owners.py:1139
+#: models/owners.py:1147
 #, python-format
 msgid ""
 "Syncing of %(topic)s for %(owner)s %(result)s.\n"
 " %(message_details)s"
 msgstr ""
 
-#: models/owners.py:1143
+#: models/owners.py:1151
 msgid "completed successfully"
 msgstr ""
 
-#: models/owners.py:1148
+#: models/owners.py:1156
 #, python-format
 msgid "%(title)s: %(topic)s updated for %(owner)s: %(result)s"
 msgstr ""
 
-#: models/owners.py:1153
+#: models/owners.py:1161
 msgid "OK"
 msgstr ""
 
-#: models/owners.py:1284
+#: models/owners.py:1293
 msgid "character_ownership"
 msgstr ""
 
-#: models/owners.py:1292
+#: models/owners.py:1301
 msgid "structures last used at"
 msgstr ""
 
-#: models/owners.py:1300
+#: models/owners.py:1309
 msgid "notifications last used at"
 msgstr ""
 
-#: models/owners.py:1306
+#: models/owners.py:1315
 msgid "error count"
 msgstr ""
 
-#: models/owners.py:1312
+#: models/owners.py:1321
 msgid "owner character"
 msgstr ""
 
-#: models/owners.py:1313
+#: models/owners.py:1322
 msgid "owner characters"
 msgstr ""
 
-#: models/structures.py:37
+#: models/structures.py:38
 msgid "sov"
 msgstr ""
 
-#: models/structures.py:38
+#: models/structures.py:39
 msgid "highsec"
 msgstr ""
 
-#: models/structures.py:39
+#: models/structures.py:40
 msgid "lowsec"
 msgstr ""
 
-#: models/structures.py:40
+#: models/structures.py:41
 msgid "nullsec"
 msgstr ""
 
-#: models/structures.py:41
+#: models/structures.py:42
 msgid "w_space"
 msgstr ""
 
-#: models/structures.py:44
+#: models/structures.py:45
 msgid "grey"
 msgstr ""
 
-#: models/structures.py:45
+#: models/structures.py:46
 msgid "dark blue"
 msgstr ""
 
-#: models/structures.py:46
+#: models/structures.py:47
 msgid "green"
 msgstr ""
 
-#: models/structures.py:47
+#: models/structures.py:48
 msgid "light blue"
 msgstr ""
 
-#: models/structures.py:48
+#: models/structures.py:49
 msgid "orange"
 msgstr ""
 
-#: models/structures.py:49
+#: models/structures.py:50
 msgid "red"
 msgstr ""
 
-#: models/structures.py:61 models/structures.py:284 models/structures.py:834
+#: models/structures.py:62 models/structures.py:285 models/structures.py:848
 msgid "name"
 msgstr ""
 
-#: models/structures.py:62
+#: models/structures.py:63
 msgid "name of the tag - must be unique"
 msgstr ""
 
-#: models/structures.py:68
+#: models/structures.py:69
 msgid "description"
 msgstr ""
 
-#: models/structures.py:69
+#: models/structures.py:70
 msgid "description for this tag"
 msgstr ""
 
-#: models/structures.py:76
+#: models/structures.py:77
 msgid "style"
 msgstr ""
 
-#: models/structures.py:77
+#: models/structures.py:78
 msgid "color style of tag"
 msgstr ""
 
-#: models/structures.py:83
+#: models/structures.py:84
 msgid "order"
 msgstr ""
 
-#: models/structures.py:85
+#: models/structures.py:86
 msgid ""
 "number defining the order tags are shown. custom tags can not have an order "
 "below 100"
 msgstr ""
 
-#: models/structures.py:93
+#: models/structures.py:94
 msgid "if true this custom tag will automatically be added to new structures"
 msgstr ""
 
-#: models/structures.py:98
+#: models/structures.py:99
 msgid "is user managed"
 msgstr ""
 
-#: models/structures.py:100
+#: models/structures.py:101
 msgid ""
 "if False this tag is created and managed by the system and can not be "
 "modified by users"
 msgstr ""
 
-#: models/structures.py:108
+#: models/structures.py:109
 msgid "structure tag"
 msgstr ""
 
-#: models/structures.py:109
+#: models/structures.py:110
 msgid "structure tags"
 msgstr ""
 
-#: models/structures.py:143
+#: models/structures.py:144
 msgid "anchor vulnerable"
 msgstr ""
 
-#: models/structures.py:144
+#: models/structures.py:145
 msgid "anchoring"
 msgstr ""
 
-#: models/structures.py:145
+#: models/structures.py:146
 msgid "armor reinforce"
 msgstr ""
 
-#: models/structures.py:146
+#: models/structures.py:147
 msgid "armor vulnerable"
 msgstr ""
 
-#: models/structures.py:147
+#: models/structures.py:148
 msgid "deploy vulnerable"
 msgstr ""
 
-#: models/structures.py:148
+#: models/structures.py:149
 msgid "fitting invulnerable"
 msgstr ""
 
-#: models/structures.py:149
+#: models/structures.py:150
 msgid "hull reinforce"
 msgstr ""
 
-#: models/structures.py:150
+#: models/structures.py:151
 msgid "hull vulnerable"
 msgstr ""
 
-#: models/structures.py:151
+#: models/structures.py:152
 msgid "online deprecated"
 msgstr ""
 
-#: models/structures.py:152
+#: models/structures.py:153
 msgid "onlining vulnerable"
 msgstr ""
 
-#: models/structures.py:153
+#: models/structures.py:154
 msgid "shield vulnerable"
 msgstr ""
 
-#: models/structures.py:154
+#: models/structures.py:155
 msgid "unanchored"
 msgstr ""
 
-#: models/structures.py:156 models/structures.py:813
+#: models/structures.py:157 models/structures.py:827
 msgid "offline"
 msgstr ""
 
-#: models/structures.py:157 models/structures.py:814
+#: models/structures.py:158 models/structures.py:828
 msgid "online"
 msgstr ""
 
-#: models/structures.py:158
+#: models/structures.py:159
 msgid "onlining"
 msgstr ""
 
-#: models/structures.py:159
+#: models/structures.py:160
 msgid "reinforced"
 msgstr ""
 
-#: models/structures.py:160
+#: models/structures.py:161
 msgid "unanchoring "
 msgstr ""
 
-#: models/structures.py:163
+#: models/structures.py:164
 msgid "unknown"
 msgstr ""
 
-#: models/structures.py:194
+#: models/structures.py:195
 msgid "Full Power"
 msgstr ""
 
-#: models/structures.py:195
+#: models/structures.py:196
 msgid "Low Power"
 msgstr ""
 
-#: models/structures.py:196
+#: models/structures.py:197
 msgid "Abandoned"
 msgstr ""
 
-#: models/structures.py:197
+#: models/structures.py:198
 msgid "Abandoned?"
 msgstr ""
 
-#: models/structures.py:198
+#: models/structures.py:199
 msgid "Unknown"
 msgstr ""
 
-#: models/structures.py:203
+#: models/structures.py:204
 msgid "The Item ID of the structure"
 msgstr ""
 
-#: models/structures.py:208
+#: models/structures.py:209
 msgid "created at"
 msgstr ""
 
-#: models/structures.py:209
+#: models/structures.py:210
 msgid "date this structure was received from ESI for the first time"
 msgstr ""
 
-#: models/structures.py:218
+#: models/structures.py:219
 msgid "moon"
 msgstr ""
 
-#: models/structures.py:219
+#: models/structures.py:220
 msgid "Moon next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:228
+#: models/structures.py:229
 msgid "planet"
 msgstr ""
 
-#: models/structures.py:229
+#: models/structures.py:230
 msgid "Planet next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:235
+#: models/structures.py:236
 msgid "solar system"
 msgstr ""
 
-#: models/structures.py:236
+#: models/structures.py:237
 msgid "Solar System the structure is located"
 msgstr ""
 
-#: models/structures.py:243
+#: models/structures.py:244
 msgid "Type of the structure"
 msgstr ""
 
-#: models/structures.py:249
+#: models/structures.py:250
 msgid "fuel expires at"
 msgstr ""
 
-#: models/structures.py:250
+#: models/structures.py:251
 msgid "Date on which the structure will run out of fuel"
 msgstr ""
 
-#: models/structures.py:257
+#: models/structures.py:258
 msgid "has fitting"
 msgstr ""
 
-#: models/structures.py:258
+#: models/structures.py:259
 msgid "bool indicating if the structure has a fitting"
 msgstr ""
 
-#: models/structures.py:265
+#: models/structures.py:266
 msgid "has core"
 msgstr ""
 
-#: models/structures.py:266
+#: models/structures.py:267
 msgid "bool indicating if the structure has a quantum core"
 msgstr ""
 
-#: models/structures.py:272
+#: models/structures.py:273
 msgid "last online at"
 msgstr ""
 
-#: models/structures.py:273
+#: models/structures.py:274
 msgid "date this structure had any of it's services online"
 msgstr ""
 
-#: models/structures.py:279 models/structures.py:778
+#: models/structures.py:280 models/structures.py:792
 msgid "last updated at"
 msgstr ""
 
-#: models/structures.py:280
+#: models/structures.py:281
 msgid "date this structure was last updated from the EVE server"
 msgstr ""
 
-#: models/structures.py:285
+#: models/structures.py:286
 msgid "The full name of the structure"
 msgstr ""
 
-#: models/structures.py:292
+#: models/structures.py:293
 msgid "next reinforce hour"
 msgstr ""
 
-#: models/structures.py:294 models/structures.py:304
+#: models/structures.py:295 models/structures.py:305
 msgid ""
 "The requested change to reinforce_hour that will take effect at the time "
 "shown by next_reinforce_apply"
 msgstr ""
 
-#: models/structures.py:302
+#: models/structures.py:303
 msgid "next reinforce apply"
 msgstr ""
 
-#: models/structures.py:313
+#: models/structures.py:314
 msgid "Corporation that owns the structure"
 msgstr ""
 
-#: models/structures.py:320
+#: models/structures.py:321
 msgid "reinforce hour"
 msgstr ""
 
-#: models/structures.py:322
+#: models/structures.py:323
 msgid ""
 "The average hour of day that determines the time +/- some hours when the "
 "structure will randomly exit its reinforcement periods and become vulnerable "
 "to attack against its armor and/or hull. "
 msgstr ""
 
-#: models/structures.py:331
+#: models/structures.py:332
 msgid "position x"
 msgstr ""
 
-#: models/structures.py:332
+#: models/structures.py:333
 msgid "x position in the solar system"
 msgstr ""
 
-#: models/structures.py:338
+#: models/structures.py:339
 msgid "position y"
 msgstr ""
 
-#: models/structures.py:339
+#: models/structures.py:340
 msgid "y position in the solar system"
 msgstr ""
 
-#: models/structures.py:345
+#: models/structures.py:346
 msgid "position z"
 msgstr ""
 
-#: models/structures.py:346
+#: models/structures.py:347
 msgid "z position in the solar system"
 msgstr ""
 
-#: models/structures.py:352 models/structures.py:839
+#: models/structures.py:353 models/structures.py:853
 msgid "state"
 msgstr ""
 
-#: models/structures.py:353
+#: models/structures.py:354
 msgid "Current state of the structure"
 msgstr ""
 
-#: models/structures.py:359
+#: models/structures.py:360
 msgid "state timer end"
 msgstr ""
 
-#: models/structures.py:360
+#: models/structures.py:361
 msgid "Date at which the structure entered it's current state"
 msgstr ""
 
-#: models/structures.py:366
+#: models/structures.py:367
 msgid "state timer start"
 msgstr ""
 
-#: models/structures.py:367
+#: models/structures.py:368
 msgid "Date at which the structure will move to it's next state"
 msgstr ""
 
-#: models/structures.py:374
+#: models/structures.py:375
 msgid "tags"
 msgstr ""
 
-#: models/structures.py:375
+#: models/structures.py:376
 msgid "List of tags for this structure. "
 msgstr ""
 
-#: models/structures.py:381
+#: models/structures.py:382
 msgid "unanchors at"
 msgstr ""
 
-#: models/structures.py:382
+#: models/structures.py:383
 msgid "Date at which the structure will unanchor"
 msgstr ""
 
-#: models/structures.py:391
+#: models/structures.py:392
 msgid ""
 "Webhooks for sending notifications to. If any webhook is enabled, these will "
 "be used instead of the webhooks defined for the respective owner. If no "
 "webhook is enabled the owner's setting will be used. "
 msgstr ""
 
-#: models/structures.py:759
+#: models/structures.py:773
 msgid "The Eve item ID"
 msgstr ""
 
-#: models/structures.py:766
+#: models/structures.py:780
 msgid "Structure this item is located in"
 msgstr ""
 
-#: models/structures.py:774
+#: models/structures.py:788
 msgid "type of the item"
 msgstr ""
 
-#: models/structures.py:776
+#: models/structures.py:790
 msgid "is singleton"
 msgstr ""
 
-#: models/structures.py:780
+#: models/structures.py:794
 msgid "location flag"
 msgstr ""
 
-#: models/structures.py:781
+#: models/structures.py:795
 msgid "quantity"
 msgstr ""
 
-#: models/structures.py:784
+#: models/structures.py:798
 msgid "structure item"
 msgstr ""
 
-#: models/structures.py:785
+#: models/structures.py:799
 msgid "structure items"
 msgstr ""
 
-#: models/structures.py:831
+#: models/structures.py:845
 msgid "Structure this service is installed to"
 msgstr ""
 
-#: models/structures.py:834
+#: models/structures.py:848
 msgid "Name of the service"
 msgstr ""
 
-#: models/structures.py:840
+#: models/structures.py:854
 msgid "Current state of this service"
 msgstr ""
 
-#: models/structures.py:844
+#: models/structures.py:858
 msgid "structure service"
 msgstr ""
 
-#: models/structures.py:845
+#: models/structures.py:859
 msgid "structure services"
 msgstr ""
 
-#: models/structures.py:861 webhooks/models.py:12
+#: models/structures.py:875 webhooks/models.py:12
 msgid "none"
 msgstr ""
 
-#: models/structures.py:862
+#: models/structures.py:876
 msgid "terrible"
 msgstr ""
 
-#: models/structures.py:863
+#: models/structures.py:877
 msgid "bad"
 msgstr ""
 
-#: models/structures.py:864
+#: models/structures.py:878
 msgid "neutral"
 msgstr ""
 
-#: models/structures.py:865
+#: models/structures.py:879
 msgid "good"
 msgstr ""
 
-#: models/structures.py:866
+#: models/structures.py:880
 msgid "excellent"
 msgstr ""
 
-#: models/structures.py:960
+#: models/structures.py:974
 msgid "alliance member"
 msgstr ""
 
-#: models/structures.py:961
+#: models/structures.py:975
 msgid "config starbase equipment role"
 msgstr ""
 
-#: models/structures.py:962
+#: models/structures.py:976
 msgid "corporation member"
 msgstr ""
 
-#: models/structures.py:963
+#: models/structures.py:977
 msgid "starbase fuel technician role"
 msgstr ""
 
 #: templates/structures/base.html:4
 msgid "Structures"
 msgstr ""
 
@@ -2134,67 +2139,67 @@
 msgid "No Access"
 msgstr ""
 
 #: templates/structures/templatetags/list_tax_item.html:11
 msgid "Has Access"
 msgstr ""
 
-#: views.py:255
+#: views.py:256
 msgid "Fuel blocks per day (est.)"
 msgstr ""
 
-#: views.py:406
+#: views.py:407
 #, python-format
 msgid ""
 "You can only use your main or alt characters to add corporations. However, "
 "character %s is neither. "
 msgstr ""
 
-#: views.py:439
+#: views.py:440
 #, python-format
 msgid ""
 "%(corporation)s has been added with %(character)s as sync character. We have "
 "started fetching structures and notifications for this corporation and you "
 "will receive a report once the process is finished."
 msgstr ""
 
-#: views.py:455
+#: views.py:456
 #, python-format
 msgid "%(corporation)s was added as new structure owner by %(user)s."
 msgstr ""
 
-#: views.py:459
+#: views.py:460
 #, python-format
 msgid "%s: Structure owner added: %s"
 msgstr ""
 
-#: views.py:466
+#: views.py:467
 #, python-format
 msgid ""
 "%(character)s has been added to %(corporation)s as sync character. You now "
 "have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:481
+#: views.py:482
 #, python-format
 msgid ""
 "%(character)s was added as sync character to %(corporation)s by %(user)s.\n"
 "We now have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:491
+#: views.py:492
 #, python-format
 msgid "%s: Character added to: %s"
 msgstr ""
 
-#: views.py:508
+#: views.py:509
 msgid "service is up"
 msgstr ""
 
-#: views.py:510
+#: views.py:511
 msgid "service is down"
 msgstr ""
 
 #: webhooks/models.py:13
 msgid "here"
 msgstr ""
```

### Comparing `aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,37 @@
 # Erik Kalkoken <erik.kalkoken@gmail.com>, 2020
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-17 02:47+0200\n"
+"POT-Creation-Date: 2023-04-24 23:05+0200\n"
 "PO-Revision-Date: 2020-03-09 19:25+0000\n"
 "Last-Translator: Erik Kalkoken <erik.kalkoken@gmail.com>, 2020\n"
 "Language-Team: Chinese (China) (https://www.transifex.com/kalkoken-apps/"
 "teams/107978/zh_CN/)\n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: admin.py:111
 msgid "Sent fuel notifications for selected configuration"
 msgstr ""
 
-#: admin.py:240 models/structures.py:162
+#: admin.py:137
+msgid ""
+"Timing configuration for sending fuel notifications. Note that the first "
+"notification will be sent at the exact start hour, and the last notification "
+"will be sent one repeat before the end hour."
+msgstr ""
+
+#: admin.py:240 models/structures.py:163
 msgid "N/A"
 msgstr "N/A"
 
 #: admin.py:255
 msgid "Not configured"
 msgstr ""
 
@@ -310,31 +317,31 @@
 #, python-format
 msgid ""
 "\n"
 "\n"
 "Change becomes effective at %s."
 msgstr ""
 
-#: core/notification_embeds.py:728 models/notifications.py:97
+#: core/notification_embeds.py:728 models/notifications.py:99
 msgid "Moon mining extraction started"
 msgstr "月矿采集开始"
 
 #: core/notification_embeds.py:730
 #, fuzzy, python-format
 #| msgid ""
 #| "A moon mining extraction has been started for %(structure_name)s at "
 #| "%(moon)s in %(solar_system)s. Extraction was started by %(character)s.\n"
 #| "The chunk will be ready on location at %(ready_time)s, and will "
 #| "autofracture on %(auto_time)s.\n"
 msgid ""
 "A moon mining extraction has been started for %(structure_name)s at %(moon)s "
 "in %(solar_system)s belonging to %(owner_link)s. Extraction was started by "
 "%(character)s.\n"
-"The chunk will be ready on location at %(ready_time)s, and will autofracture "
-"on %(auto_time)s.\n"
+"The chunk will be ready on location at %(ready_time)s, and will fracture "
+"automatically on %(auto_time)s.\n"
 "%(ore_text)s"
 msgstr ""
 "%(structure_name)s开始了在%(solar_system)s的%(moon)s月球的月矿采集。"
 "是%(character)s启动的采集。\n"
 "月矿将在%(ready_time)s开采完毕，并在%(auto_time)s自动裂解。\n"
 
 #: core/notification_embeds.py:746
@@ -379,15 +386,15 @@
 #: core/notification_embeds.py:784
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has automatically been fired and the moon products are "
 #| "ready to be harvested.\n"
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has automatically been fired and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "在%(solar_system)s的%(moon)s月球的%(structure_name)s矿枪已自动开火，月矿已准"
 "备可开采\n"
 
@@ -403,25 +410,27 @@
 msgid ""
 "An ongoing extraction for %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been cancelled by %(character)s."
 msgstr ""
 "在%(solar_system)s的%(moon)s月球的%(structure_name)s已被%(character)s取消"
 
 #: core/notification_embeds.py:831
-msgid "Moondrill fired"
+#, fuzzy
+#| msgid "Moondrill fired"
+msgid "Moon drill fired"
 msgstr "月球矿枪已开火"
 
 #: core/notification_embeds.py:833
 #, fuzzy, python-format
 #| msgid ""
 #| "The moondrill fitted to %(structure_name)s at %(moon)s in "
 #| "%(solar_system)s has been fired by %(character)s and the moon products "
 #| "are ready to be harvested."
 msgid ""
-"The moondrill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
+"The moon drill fitted to %(structure_name)s at %(moon)s in %(solar_system)s "
 "belonging to %(owner_link)s has been fired by %(character)s and the moon "
 "products are ready to be harvested.\n"
 "%(ore_text)s"
 msgstr ""
 "%(solar_system)s%(moon)s月球的%(structure_name)s的矿枪已被%(character)s启用，"
 "月矿已可采集。"
 
@@ -453,15 +462,15 @@
 "The %(structure_type)s at %(planet)s in %(solar_system)s belonging to "
 "%(owner_link)s has been reinforced by %(aggressor)s and will come out at: "
 "%(date)s."
 msgstr ""
 "在%(solar_system)s%(planet)s的%(structure_type)s已被%(aggressor)s增强，将会"
 "在%(date)s退出增强"
 
-#: core/notification_embeds.py:935 core/notification_embeds.py:1630
+#: core/notification_embeds.py:935 core/notification_embeds.py:1631
 #, fuzzy, python-format
 #| msgid ""
 #| "The starbase %(structure_name)s at %(moon)s in %(solar_system)s is low on "
 #| "fuel. It has %(quantity)d fuel blocks left."
 msgid ""
 "The starbase %(structure_name)s at %(moon)s in %(solar_system)s belonging to "
 "%(owner_link)s "
@@ -482,15 +491,15 @@
 msgid ""
 "is under attack by %(aggressor)s.\n"
 "%(damage_text)s"
 msgstr ""
 "在%(solar_system)s%(moon)s的POS%(structure_name)s正在遭到%(aggressor)s攻击\n"
 "%(damage_text)s"
 
-#: core/notification_embeds.py:982 models/notifications.py:91
+#: core/notification_embeds.py:982 models/notifications.py:93
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Starbase fuel alert"
 msgstr "建筑燃料警报"
 
 #: core/notification_embeds.py:996
 #, fuzzy
@@ -613,62 +622,62 @@
 msgid "%s has offered a surrender"
 msgstr ""
 
 #: core/notification_embeds.py:1535
 #, python-format
 msgid ""
 "%s has offered to end the war with %s in the exchange for %s ISK. If "
-"accepted, the war will end in 24 hours and your organizations willbe unable "
+"accepted, the war will end in 24 hours and your organizations will be unable "
 "to declare new wars against each other for the next 2 weeks."
 msgstr ""
 
 #: core/notification_embeds.py:1548
 msgid "Insufficient Funds for Bill"
 msgstr ""
 
 #: core/notification_embeds.py:1550
 #, python-format
 msgid ""
-"The selected corporation wallet division for autopayments does not have "
-"enough current funds available to pay the %(bill_type)s due to be paid by "
-"%(due_date)s. Transfer additional funds to the selected wallet division in "
-"order to meet your pending automatic bills."
+"The selected corporation wallet division for automatic payments does not "
+"have enough current funds available to pay the %(bill_type)s due to be paid "
+"by %(due_date)s. Transfer additional funds to the selected wallet division "
+"in order to meet your pending automatic bills."
 msgstr ""
 
-#: core/notification_embeds.py:1569
+#: core/notification_embeds.py:1570
 msgid "IHub Bill About to Expire"
 msgstr ""
 
-#: core/notification_embeds.py:1571
+#: core/notification_embeds.py:1572
 #, python-format
 msgid ""
 "Maintenance bill for Infrastructure Hub in %(solar_system)s expires at "
 "%(due_date)s, if not paid in time this Infrastructure Hub will self-destruct."
 msgstr ""
 
-#: core/notification_embeds.py:1596
+#: core/notification_embeds.py:1597
 #, python-format
 msgid "%s has self-destructed due to unpaid maintenance bills"
 msgstr ""
 
-#: core/notification_embeds.py:1600
+#: core/notification_embeds.py:1601
 #, fuzzy, python-format
 #| msgid "%(structure_type)s in %(solar_system)s has entered reinforced mode"
 msgid ""
 "%(structure_type)s in %(solar_system)s has self-destructed, as the standard "
 "maintenance bills where not paid."
 msgstr "在%(solar_system)s的%(structure_type)s已进入增强模式"
 
-#: core/notification_embeds.py:1645
+#: core/notification_embeds.py:1646
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced"
 msgstr "轨道 增强"
 
-#: core/notification_embeds.py:1653
+#: core/notification_embeds.py:1654
 #, python-format
 msgid "has been reinforced and will come out at: %s."
 msgstr ""
 
 #: core/notification_timers.py:89
 msgid "Armor timer"
 msgstr "装甲timer"
@@ -690,1246 +699,1246 @@
 msgid "yes"
 msgstr "是"
 
 #: core/serializers.py:496
 msgid "no"
 msgstr "没有"
 
-#: models/notifications.py:41
+#: models/notifications.py:43
 msgid "English"
 msgstr "英语"
 
-#: models/notifications.py:42
+#: models/notifications.py:44
 msgid "German"
 msgstr "德语"
 
-#: models/notifications.py:43
+#: models/notifications.py:45
 msgid "Spanish"
 msgstr "西班牙文"
 
-#: models/notifications.py:44
+#: models/notifications.py:46
 msgid "Chinese Simplified"
 msgstr "简体中文"
 
-#: models/notifications.py:45
+#: models/notifications.py:47
 msgid "Russian"
 msgstr "俄语"
 
-#: models/notifications.py:46
+#: models/notifications.py:48
 msgid "Korean"
 msgstr " 韩语"
 
-#: models/notifications.py:54
+#: models/notifications.py:56
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Upwell structure anchoring"
 msgstr "建筑正在铆钉"
 
-#: models/notifications.py:55
+#: models/notifications.py:57
 #, fuzzy
 #| msgid "Structure online"
 msgid "Upwell structure went online"
 msgstr "建筑上线"
 
-#: models/notifications.py:57
+#: models/notifications.py:59
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Upwell structure services went offline"
 msgstr "建筑服务下线"
 
-#: models/notifications.py:60
+#: models/notifications.py:62
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went high power"
 msgstr "建筑低能量"
 
-#: models/notifications.py:63
+#: models/notifications.py:65
 #, fuzzy
 #| msgid "Structure low power"
 msgid "Upwell structure went low power"
 msgstr "建筑低能量"
 
-#: models/notifications.py:65
+#: models/notifications.py:67
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Upwell structure unanchoring"
 msgstr "建筑解铆中"
 
-#: models/notifications.py:66
+#: models/notifications.py:68
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure fuel alert"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:67
+#: models/notifications.py:69
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure refueled"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:69
+#: models/notifications.py:71
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "Upwell structure jump fuel alert"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:72
+#: models/notifications.py:74
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "Upwell structure is under attack"
 msgstr "建筑收到攻击"
 
-#: models/notifications.py:74
+#: models/notifications.py:76
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "Upwell structure lost shields"
 msgstr "建筑失去护盾"
 
-#: models/notifications.py:75
+#: models/notifications.py:77
 #, fuzzy
 #| msgid "Structure lost armor"
 msgid "Upwell structure lost armor"
 msgstr "建筑失去护甲"
 
-#: models/notifications.py:76
+#: models/notifications.py:78
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Upwell structure destroyed"
 msgstr "建筑已被击毁"
 
-#: models/notifications.py:79
+#: models/notifications.py:81
 msgid "Upwell structure reinforcement time changed"
 msgstr ""
 
-#: models/notifications.py:82
+#: models/notifications.py:84
 #, fuzzy
 #| msgid "Ownership transferred"
 msgid "Upwell structure ownership transferred"
 msgstr "所有权已转移"
 
-#: models/notifications.py:86
+#: models/notifications.py:88
 msgid "Customs office attacked"
 msgstr ""
 
-#: models/notifications.py:87
+#: models/notifications.py:89
 msgid "Customs office reinforced"
 msgstr ""
 
-#: models/notifications.py:90
+#: models/notifications.py:92
 #, fuzzy
 #| msgid "Starbase under attack"
 msgid "Starbase attacked"
 msgstr "POS正在被攻击"
 
-#: models/notifications.py:92
+#: models/notifications.py:94
 msgid "Starbase refueled (BETA)"
 msgstr ""
 
-#: models/notifications.py:93
+#: models/notifications.py:95
 #, fuzzy
 #| msgid "Orbital reinforced"
 msgid "Starbase reinforced (BETA)"
 msgstr "轨道 增强"
 
-#: models/notifications.py:99
+#: models/notifications.py:101
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moonmining laser fired"
 msgstr "月矿采集开始"
 
-#: models/notifications.py:101
+#: models/notifications.py:103
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction cancelled"
 msgstr "月矿采集开始"
 
-#: models/notifications.py:104
+#: models/notifications.py:106
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining extraction finished"
 msgstr "月矿采集开始"
 
-#: models/notifications.py:107
+#: models/notifications.py:109
 #, fuzzy
 #| msgid "Moon mining extraction started"
 msgid "Moon mining automatic fracture triggered"
 msgstr "月矿采集开始"
 
-#: models/notifications.py:112
+#: models/notifications.py:114
 msgid "Sovereignty structure reinforced"
 msgstr ""
 
-#: models/notifications.py:115
+#: models/notifications.py:117
 #, fuzzy
 #| msgid "Structure destroyed"
 msgid "Sovereignty structure destroyed"
 msgstr "建筑已被击毁"
 
-#: models/notifications.py:118
+#: models/notifications.py:120
 msgid "Sovereignty entosis capture started"
 msgstr ""
 
-#: models/notifications.py:121
+#: models/notifications.py:123
 msgid "Sovereignty command node event started"
 msgstr ""
 
-#: models/notifications.py:124
+#: models/notifications.py:126
 #, fuzzy
 #| msgid "DED Sovereignty claim acknowledgment: %s"
 msgid "Sovereignty claim acknowledgment"
 msgstr "DED主权夺取通知：%s"
 
-#: models/notifications.py:126
+#: models/notifications.py:128
 msgid "Sovereignty lost"
 msgstr ""
 
-#: models/notifications.py:128
+#: models/notifications.py:130
 #, fuzzy
 #| msgid "Structure anchoring"
 msgid "Structure anchoring in alliance space"
 msgstr "建筑正在铆钉"
 
-#: models/notifications.py:132
+#: models/notifications.py:134
 msgid "War declared"
 msgstr ""
 
-#: models/notifications.py:134
+#: models/notifications.py:136
 msgid "War ally joined aggressor"
 msgstr ""
 
-#: models/notifications.py:136
+#: models/notifications.py:138
 msgid "War ally joined ally"
 msgstr ""
 
-#: models/notifications.py:138
+#: models/notifications.py:140
 msgid "War ally joined defender"
 msgstr ""
 
-#: models/notifications.py:140
+#: models/notifications.py:142
 msgid "War adopted"
 msgstr ""
 
-#: models/notifications.py:141
+#: models/notifications.py:143
 msgid "War inherited"
 msgstr ""
 
-#: models/notifications.py:142
+#: models/notifications.py:144
 msgid "War party surrendered"
 msgstr ""
 
-#: models/notifications.py:144
+#: models/notifications.py:146
 msgid "War retracted by Concord"
 msgstr ""
 
-#: models/notifications.py:147
+#: models/notifications.py:149
 msgid "War corporation became eligible"
 msgstr ""
 
-#: models/notifications.py:150
+#: models/notifications.py:152
 msgid "War corporation no longer eligible"
 msgstr ""
 
-#: models/notifications.py:152
+#: models/notifications.py:154
 msgid "War surrender offered"
 msgstr ""
 
-#: models/notifications.py:155
+#: models/notifications.py:157
 msgid "Character submitted application"
 msgstr ""
 
-#: models/notifications.py:157
+#: models/notifications.py:159
 msgid "Character invited to join corporation"
 msgstr ""
 
-#: models/notifications.py:160
+#: models/notifications.py:162
 msgid "Corp application rejected"
 msgstr ""
 
-#: models/notifications.py:162
+#: models/notifications.py:164
 msgid "Character withdrew application"
 msgstr ""
 
-#: models/notifications.py:163
+#: models/notifications.py:165
 msgid "Character joins corporation"
 msgstr ""
 
-#: models/notifications.py:164
+#: models/notifications.py:166
 msgid "Character leaves corporation"
 msgstr ""
 
-#: models/notifications.py:167
+#: models/notifications.py:169
 msgid "Bill out of money"
 msgstr ""
 
-#: models/notifications.py:170
+#: models/notifications.py:172
 msgid "I-HUB bill about to expire"
 msgstr ""
 
-#: models/notifications.py:174
+#: models/notifications.py:176
 msgid "I_HUB destroyed by bill failure"
 msgstr ""
 
-#: models/notifications.py:334
+#: models/notifications.py:336
 msgid "notification types"
 msgstr ""
 
-#: models/notifications.py:336
+#: models/notifications.py:338
 msgid "Select which type of notifications should be forwarded to this webhook"
 msgstr ""
 
-#: models/notifications.py:345
+#: models/notifications.py:347
 msgid "language"
 msgstr ""
 
-#: models/notifications.py:346
+#: models/notifications.py:348
 msgid "language of notifications send to this webhook"
 msgstr ""
 
-#: models/notifications.py:350 models/structures.py:91
+#: models/notifications.py:352 models/structures.py:92
 msgid "is default"
 msgstr ""
 
-#: models/notifications.py:352
+#: models/notifications.py:354
 msgid "Whether owners have this webhook automatically pre-set when created"
 msgstr ""
 
-#: models/notifications.py:357 models/owners.py:151
+#: models/notifications.py:359 models/owners.py:153
 msgid "has default pings enabled"
 msgstr ""
 
-#: models/notifications.py:368 models/owners.py:197
+#: models/notifications.py:370 models/owners.py:199
 msgid "ping groups"
 msgstr ""
 
-#: models/notifications.py:369
+#: models/notifications.py:371
 msgid "Groups to be pinged for each notification - "
 msgstr ""
 
-#: models/notifications.py:374
+#: models/notifications.py:376
 msgid "webhook"
 msgstr ""
 
-#: models/notifications.py:375 models/owners.py:212 models/structures.py:389
+#: models/notifications.py:377 models/owners.py:214 models/structures.py:390
 msgid "webhooks"
 msgstr ""
 
-#: models/notifications.py:388
+#: models/notifications.py:390
 msgid "is sent"
 msgstr ""
 
-#: models/notifications.py:389
+#: models/notifications.py:391
 msgid "True when this notification has been forwarded to Discord"
 msgstr ""
 
-#: models/notifications.py:394
+#: models/notifications.py:396
 msgid "is timer added"
 msgstr ""
 
-#: models/notifications.py:395
+#: models/notifications.py:397
 msgid "True when a timer has been added for this notification"
 msgstr ""
 
-#: models/notifications.py:401 models/structures.py:242
-#: models/structures.py:773
+#: models/notifications.py:403 models/structures.py:243
+#: models/structures.py:787
 msgid "type"
 msgstr ""
 
-#: models/notifications.py:402
+#: models/notifications.py:404
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "type of this notification"
 msgstr "%(ticker)s提示"
 
-#: models/notifications.py:407 models/owners.py:219 models/owners.py:1278
-#: models/structures.py:312
+#: models/notifications.py:409 models/owners.py:221 models/owners.py:1287
+#: models/structures.py:313
 #, fuzzy
 #| msgid "Owner"
 msgid "owner"
 msgstr "所有人"
 
-#: models/notifications.py:408
+#: models/notifications.py:410
 msgid "Corporation that owns this notification"
 msgstr ""
 
-#: models/notifications.py:412 models/structures.py:402
+#: models/notifications.py:414 models/structures.py:403
 #, fuzzy
 #| msgid "Structure List"
 msgid "structures"
 msgstr "建筑列表"
 
-#: models/notifications.py:413
+#: models/notifications.py:415
 msgid "Structures this notification is about (if any)"
 msgstr ""
 
-#: models/notifications.py:682 models/structures.py:202
-#: models/structures.py:759
+#: models/notifications.py:694 models/structures.py:203
+#: models/structures.py:773
 #, fuzzy
 #| msgid "d"
 msgid "id"
 msgstr "日"
 
-#: models/notifications.py:686
+#: models/notifications.py:698
 msgid "created"
 msgstr ""
 
-#: models/notifications.py:687
+#: models/notifications.py:699
 msgid "Date when this notification was first received from ESI"
 msgstr ""
 
-#: models/notifications.py:692
+#: models/notifications.py:704
 msgid "is read"
 msgstr ""
 
-#: models/notifications.py:693
+#: models/notifications.py:705
 msgid "True when this notification has read in the eve client"
 msgstr ""
 
-#: models/notifications.py:696
+#: models/notifications.py:708
 msgid "last updated"
 msgstr ""
 
-#: models/notifications.py:697
+#: models/notifications.py:709
 msgid "Date when this notification has last been updated from ESI"
 msgstr ""
 
-#: models/notifications.py:704
+#: models/notifications.py:716
 msgid "sender"
 msgstr ""
 
-#: models/notifications.py:711
+#: models/notifications.py:723
 msgid "text"
 msgstr ""
 
-#: models/notifications.py:712
+#: models/notifications.py:724
 msgid "Notification details in YAML"
 msgstr ""
 
-#: models/notifications.py:714 models/notifications.py:831
+#: models/notifications.py:726 models/notifications.py:843
 msgid "timestamp"
 msgstr ""
 
-#: models/notifications.py:719
+#: models/notifications.py:731
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "eve notification"
 msgstr "%(ticker)s提示"
 
-#: models/notifications.py:720
+#: models/notifications.py:732
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "eve notifications"
 msgstr "%(ticker)s提示"
 
-#: models/notifications.py:829
+#: models/notifications.py:841
 msgid "details"
 msgstr ""
 
-#: models/notifications.py:830
+#: models/notifications.py:842
 msgid "last_updated"
 msgstr ""
 
-#: models/notifications.py:836
+#: models/notifications.py:848
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "generated notification"
 msgstr "%(ticker)s提示"
 
-#: models/notifications.py:837
+#: models/notifications.py:849
 #, fuzzy
 #| msgid "%(ticker)s Notification"
 msgid "generated  notifications"
 msgstr "%(ticker)s提示"
 
-#: models/notifications.py:866
+#: models/notifications.py:878
 msgid "channel pings"
 msgstr ""
 
-#: models/notifications.py:868
+#: models/notifications.py:880
 msgid ""
 "Option to ping every member of the channel. This setting can be overruled by "
 "the respective owner or webhook configuration"
 msgstr ""
 
-#: models/notifications.py:878
+#: models/notifications.py:890
 msgid "color"
 msgstr ""
 
-#: models/notifications.py:879
+#: models/notifications.py:891
 msgid "Context color of these notification on Discord"
 msgstr ""
 
-#: models/notifications.py:883
+#: models/notifications.py:895
 msgid "is_enabled"
 msgstr ""
 
-#: models/notifications.py:884
+#: models/notifications.py:896
 msgid "Disabled configurations will not create any new alerts."
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "end"
 msgstr ""
 
-#: models/notifications.py:907
+#: models/notifications.py:919
 msgid "End of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:910
+#: models/notifications.py:922
 msgid "repeat"
 msgstr ""
 
-#: models/notifications.py:912
+#: models/notifications.py:924
 msgid "Notifications will be repeated every x hours. Set to 0 for no repeats"
 msgstr ""
 
-#: models/notifications.py:916
+#: models/notifications.py:928
 msgid "start"
 msgstr ""
 
-#: models/notifications.py:917
+#: models/notifications.py:929
 msgid "Start of alerts in hours before fuel expires"
 msgstr ""
 
-#: models/notifications.py:921
+#: models/notifications.py:933
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert config"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:922
+#: models/notifications.py:934
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert configs"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:927
+#: models/notifications.py:941
 msgid "Start must be before end, i.e. have a larger value."
 msgstr ""
 
-#: models/notifications.py:931
+#: models/notifications.py:945
 msgid "Repeat can not be larger that the interval size."
 msgstr ""
 
-#: models/notifications.py:940
+#: models/notifications.py:954
 msgid "This configuration may not overlap with an existing configuration."
 msgstr ""
 
-#: models/notifications.py:1007
+#: models/notifications.py:1021
 msgid "threshold"
 msgstr ""
 
-#: models/notifications.py:1009
+#: models/notifications.py:1023
 msgid ""
 "Notifications will be sent once fuel level in units reaches this threshold"
 msgstr ""
 
-#: models/notifications.py:1014
+#: models/notifications.py:1028
 msgid "jump fuel alert config"
 msgstr ""
 
-#: models/notifications.py:1015
+#: models/notifications.py:1029
 msgid "jump fuel alert configs"
 msgstr ""
 
-#: models/notifications.py:1064 models/notifications.py:1114
-#: models/structures.py:401 models/structures.py:765 models/structures.py:830
+#: models/notifications.py:1078 models/notifications.py:1128
+#: models/structures.py:402 models/structures.py:779 models/structures.py:844
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure"
 msgstr "建筑列表"
 
-#: models/notifications.py:1070 models/notifications.py:1120
+#: models/notifications.py:1084 models/notifications.py:1134
 msgid "configuration"
 msgstr ""
 
-#: models/notifications.py:1074
+#: models/notifications.py:1088
 msgid "hours"
 msgstr ""
 
-#: models/notifications.py:1075
+#: models/notifications.py:1089
 msgid "number of hours before fuel expiration this alert was sent"
 msgstr ""
 
-#: models/notifications.py:1079
+#: models/notifications.py:1093
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alert"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:1080
+#: models/notifications.py:1094
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "structure fuel alerts"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:1124
+#: models/notifications.py:1138
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alert"
 msgstr "建筑燃料警报"
 
-#: models/notifications.py:1125
+#: models/notifications.py:1139
 #, fuzzy
 #| msgid "Structure fuel alert"
 msgid "jump fuel alerts"
 msgstr "建筑燃料警报"
 
-#: models/owners.py:117
+#: models/owners.py:119
 #, fuzzy
 #| msgid "Corporation"
 msgid "corporation"
 msgstr "公司"
 
-#: models/owners.py:118
+#: models/owners.py:120
 msgid "Corporation owning structures"
 msgstr ""
 
-#: models/owners.py:123
+#: models/owners.py:125
 msgid "are pocos public"
 msgstr ""
 
-#: models/owners.py:124
+#: models/owners.py:126
 msgid "whether pocos of this owner are shown on public POCO page"
 msgstr ""
 
-#: models/owners.py:130
+#: models/owners.py:132
 msgid "assets last update at"
 msgstr ""
 
-#: models/owners.py:131 models/owners.py:147 models/owners.py:190
-#: models/owners.py:205
+#: models/owners.py:133 models/owners.py:149 models/owners.py:192
+#: models/owners.py:207
 msgid "when the last successful update happened"
 msgstr ""
 
-#: models/owners.py:146
+#: models/owners.py:148
 msgid "forwarding last update at"
 msgstr ""
 
-#: models/owners.py:153
+#: models/owners.py:155
 msgid ""
 "to enable or disable pinging of notifications for this owner e.g. with "
 "@everyone and @here"
 msgstr ""
 
-#: models/owners.py:159
+#: models/owners.py:161
 msgid "is active"
 msgstr ""
 
-#: models/owners.py:160
+#: models/owners.py:162
 msgid "whether this owner is currently included in the sync process"
 msgstr ""
 
-#: models/owners.py:164
+#: models/owners.py:166
 #, fuzzy
 #| msgid "Alliance"
 msgid "is alliance main"
 msgstr "联盟"
 
-#: models/owners.py:166
+#: models/owners.py:168
 msgid ""
 "whether alliance wide notifications are forwarded for this owner (e.g. sov "
 "notifications)"
 msgstr ""
 
-#: models/owners.py:172
+#: models/owners.py:174
 msgid "is included in service status"
 msgstr ""
 
-#: models/owners.py:174
+#: models/owners.py:176
 msgid ""
 "whether the sync status of this owner is included in the overall status of "
 "this services"
 msgstr ""
 
-#: models/owners.py:182
+#: models/owners.py:184
 msgid "is up"
 msgstr ""
 
-#: models/owners.py:183
+#: models/owners.py:185
 msgid "whether all services for this owner are currently up"
 msgstr ""
 
-#: models/owners.py:189
+#: models/owners.py:191
 msgid "notifications last update at"
 msgstr ""
 
-#: models/owners.py:198
+#: models/owners.py:200
 msgid "Groups to be pinged for each notification. "
 msgstr ""
 
-#: models/owners.py:204
+#: models/owners.py:206
 #, fuzzy
 #| msgid "Structure under attack"
 msgid "structures last update at"
 msgstr "建筑收到攻击"
 
-#: models/owners.py:213
+#: models/owners.py:215
 msgid "Notifications are sent to these webhooks."
 msgstr ""
 
-#: models/owners.py:220
+#: models/owners.py:222
 #, fuzzy
 #| msgid "Owner"
 msgid "owners"
 msgstr "所有人"
 
-#: models/owners.py:1139
+#: models/owners.py:1147
 #, fuzzy, python-format
 #| msgid ""
 #| "Syncing of %(topic)s for \"%(owner)s\" %(result)s.\n"
 #| "%(message_details)s"
 msgid ""
 "Syncing of %(topic)s for %(owner)s %(result)s.\n"
 " %(message_details)s"
 msgstr ""
 "正在同步 %(topic)s 对于 %(owner)s %(result)s.\n"
 "%(message_details)s"
 
-#: models/owners.py:1143
+#: models/owners.py:1151
 msgid "completed successfully"
 msgstr "成功完成"
 
-#: models/owners.py:1148
+#: models/owners.py:1156
 #, python-format
 msgid "%(title)s: %(topic)s updated for %(owner)s: %(result)s"
 msgstr "%(title)s: %(topic)s 更新为 %(owner)s: %(result)s"
 
-#: models/owners.py:1153
+#: models/owners.py:1161
 msgid "OK"
 msgstr "好"
 
-#: models/owners.py:1284
+#: models/owners.py:1293
 msgid "character_ownership"
 msgstr ""
 
-#: models/owners.py:1292
+#: models/owners.py:1301
 #, fuzzy
 #| msgid "Structure lost shield"
 msgid "structures last used at"
 msgstr "建筑失去护盾"
 
-#: models/owners.py:1300
+#: models/owners.py:1309
 msgid "notifications last used at"
 msgstr ""
 
-#: models/owners.py:1306
+#: models/owners.py:1315
 msgid "error count"
 msgstr ""
 
-#: models/owners.py:1312
+#: models/owners.py:1321
 msgid "owner character"
 msgstr ""
 
-#: models/owners.py:1313
+#: models/owners.py:1322
 msgid "owner characters"
 msgstr ""
 
-#: models/structures.py:37
+#: models/structures.py:38
 msgid "sov"
 msgstr ""
 
-#: models/structures.py:38
+#: models/structures.py:39
 msgid "highsec"
 msgstr ""
 
-#: models/structures.py:39
+#: models/structures.py:40
 msgid "lowsec"
 msgstr ""
 
-#: models/structures.py:40
+#: models/structures.py:41
 msgid "nullsec"
 msgstr ""
 
-#: models/structures.py:41
+#: models/structures.py:42
 msgid "w_space"
 msgstr ""
 
-#: models/structures.py:44
+#: models/structures.py:45
 msgid "grey"
 msgstr ""
 
-#: models/structures.py:45
+#: models/structures.py:46
 msgid "dark blue"
 msgstr ""
 
-#: models/structures.py:46
+#: models/structures.py:47
 msgid "green"
 msgstr ""
 
-#: models/structures.py:47
+#: models/structures.py:48
 msgid "light blue"
 msgstr ""
 
-#: models/structures.py:48
+#: models/structures.py:49
 msgid "orange"
 msgstr ""
 
-#: models/structures.py:49
+#: models/structures.py:50
 msgid "red"
 msgstr ""
 
-#: models/structures.py:61 models/structures.py:284 models/structures.py:834
+#: models/structures.py:62 models/structures.py:285 models/structures.py:848
 msgid "name"
 msgstr ""
 
-#: models/structures.py:62
+#: models/structures.py:63
 msgid "name of the tag - must be unique"
 msgstr ""
 
-#: models/structures.py:68
+#: models/structures.py:69
 msgid "description"
 msgstr ""
 
-#: models/structures.py:69
+#: models/structures.py:70
 msgid "description for this tag"
 msgstr ""
 
-#: models/structures.py:76
+#: models/structures.py:77
 msgid "style"
 msgstr ""
 
-#: models/structures.py:77
+#: models/structures.py:78
 msgid "color style of tag"
 msgstr ""
 
-#: models/structures.py:83
+#: models/structures.py:84
 msgid "order"
 msgstr ""
 
-#: models/structures.py:85
+#: models/structures.py:86
 msgid ""
 "number defining the order tags are shown. custom tags can not have an order "
 "below 100"
 msgstr ""
 
-#: models/structures.py:93
+#: models/structures.py:94
 msgid "if true this custom tag will automatically be added to new structures"
 msgstr ""
 
-#: models/structures.py:98
+#: models/structures.py:99
 msgid "is user managed"
 msgstr ""
 
-#: models/structures.py:100
+#: models/structures.py:101
 msgid ""
 "if False this tag is created and managed by the system and can not be "
 "modified by users"
 msgstr ""
 
-#: models/structures.py:108
+#: models/structures.py:109
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure tag"
 msgstr "建筑列表"
 
-#: models/structures.py:109
+#: models/structures.py:110
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure tags"
 msgstr "建筑列表"
 
-#: models/structures.py:143
+#: models/structures.py:144
 msgid "anchor vulnerable"
 msgstr ""
 
-#: models/structures.py:144
+#: models/structures.py:145
 msgid "anchoring"
 msgstr ""
 
-#: models/structures.py:145
+#: models/structures.py:146
 msgid "armor reinforce"
 msgstr ""
 
-#: models/structures.py:146
+#: models/structures.py:147
 msgid "armor vulnerable"
 msgstr ""
 
-#: models/structures.py:147
+#: models/structures.py:148
 msgid "deploy vulnerable"
 msgstr ""
 
-#: models/structures.py:148
+#: models/structures.py:149
 msgid "fitting invulnerable"
 msgstr ""
 
-#: models/structures.py:149
+#: models/structures.py:150
 msgid "hull reinforce"
 msgstr ""
 
-#: models/structures.py:150
+#: models/structures.py:151
 msgid "hull vulnerable"
 msgstr ""
 
-#: models/structures.py:151
+#: models/structures.py:152
 msgid "online deprecated"
 msgstr ""
 
-#: models/structures.py:152
+#: models/structures.py:153
 msgid "onlining vulnerable"
 msgstr ""
 
-#: models/structures.py:153
+#: models/structures.py:154
 msgid "shield vulnerable"
 msgstr ""
 
-#: models/structures.py:154
+#: models/structures.py:155
 msgid "unanchored"
 msgstr ""
 
-#: models/structures.py:156 models/structures.py:813
+#: models/structures.py:157 models/structures.py:827
 msgid "offline"
 msgstr "离线"
 
-#: models/structures.py:157 models/structures.py:814
+#: models/structures.py:158 models/structures.py:828
 msgid "online"
 msgstr "线上"
 
-#: models/structures.py:158
+#: models/structures.py:159
 msgid "onlining"
 msgstr ""
 
-#: models/structures.py:159
+#: models/structures.py:160
 msgid "reinforced"
 msgstr ""
 
-#: models/structures.py:160
+#: models/structures.py:161
 msgid "unanchoring "
 msgstr ""
 
-#: models/structures.py:163
+#: models/structures.py:164
 msgid "unknown"
 msgstr "未知"
 
-#: models/structures.py:194
+#: models/structures.py:195
 #, fuzzy
 #| msgid "Low Power"
 msgid "Full Power"
 msgstr "低能量"
 
-#: models/structures.py:195
+#: models/structures.py:196
 msgid "Low Power"
 msgstr "低能量"
 
-#: models/structures.py:196
+#: models/structures.py:197
 msgid "Abandoned"
 msgstr ""
 
-#: models/structures.py:197
+#: models/structures.py:198
 msgid "Abandoned?"
 msgstr ""
 
-#: models/structures.py:198
+#: models/structures.py:199
 #, fuzzy
 #| msgid "unknown"
 msgid "Unknown"
 msgstr "未知"
 
-#: models/structures.py:203
+#: models/structures.py:204
 msgid "The Item ID of the structure"
 msgstr ""
 
-#: models/structures.py:208
+#: models/structures.py:209
 msgid "created at"
 msgstr ""
 
-#: models/structures.py:209
+#: models/structures.py:210
 msgid "date this structure was received from ESI for the first time"
 msgstr ""
 
-#: models/structures.py:218
+#: models/structures.py:219
 msgid "moon"
 msgstr ""
 
-#: models/structures.py:219
+#: models/structures.py:220
 msgid "Moon next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:228
+#: models/structures.py:229
 msgid "planet"
 msgstr ""
 
-#: models/structures.py:229
+#: models/structures.py:230
 msgid "Planet next to this structure - if any"
 msgstr ""
 
-#: models/structures.py:235
+#: models/structures.py:236
 #, fuzzy
 #| msgid "Solar System"
 msgid "solar system"
 msgstr "星系"
 
-#: models/structures.py:236
+#: models/structures.py:237
 msgid "Solar System the structure is located"
 msgstr ""
 
-#: models/structures.py:243
+#: models/structures.py:244
 msgid "Type of the structure"
 msgstr ""
 
-#: models/structures.py:249
+#: models/structures.py:250
 #, fuzzy
 #| msgid "Fuel Expires"
 msgid "fuel expires at"
 msgstr "燃料消耗"
 
-#: models/structures.py:250
+#: models/structures.py:251
 msgid "Date on which the structure will run out of fuel"
 msgstr ""
 
-#: models/structures.py:257
+#: models/structures.py:258
 msgid "has fitting"
 msgstr ""
 
-#: models/structures.py:258
+#: models/structures.py:259
 msgid "bool indicating if the structure has a fitting"
 msgstr ""
 
-#: models/structures.py:265
+#: models/structures.py:266
 msgid "has core"
 msgstr ""
 
-#: models/structures.py:266
+#: models/structures.py:267
 msgid "bool indicating if the structure has a quantum core"
 msgstr ""
 
-#: models/structures.py:272
+#: models/structures.py:273
 #, fuzzy
 #| msgid "online"
 msgid "last online at"
 msgstr "线上"
 
-#: models/structures.py:273
+#: models/structures.py:274
 msgid "date this structure had any of it's services online"
 msgstr ""
 
-#: models/structures.py:279 models/structures.py:778
+#: models/structures.py:280 models/structures.py:792
 msgid "last updated at"
 msgstr ""
 
-#: models/structures.py:280
+#: models/structures.py:281
 msgid "date this structure was last updated from the EVE server"
 msgstr ""
 
-#: models/structures.py:285
+#: models/structures.py:286
 msgid "The full name of the structure"
 msgstr ""
 
-#: models/structures.py:292
+#: models/structures.py:293
 msgid "next reinforce hour"
 msgstr ""
 
-#: models/structures.py:294 models/structures.py:304
+#: models/structures.py:295 models/structures.py:305
 msgid ""
 "The requested change to reinforce_hour that will take effect at the time "
 "shown by next_reinforce_apply"
 msgstr ""
 
-#: models/structures.py:302
+#: models/structures.py:303
 msgid "next reinforce apply"
 msgstr ""
 
-#: models/structures.py:313
+#: models/structures.py:314
 msgid "Corporation that owns the structure"
 msgstr ""
 
-#: models/structures.py:320
+#: models/structures.py:321
 #, fuzzy
 #| msgid "Reinforced?"
 msgid "reinforce hour"
 msgstr "增强？"
 
-#: models/structures.py:322
+#: models/structures.py:323
 msgid ""
 "The average hour of day that determines the time +/- some hours when the "
 "structure will randomly exit its reinforcement periods and become vulnerable "
 "to attack against its armor and/or hull. "
 msgstr ""
 
-#: models/structures.py:331
+#: models/structures.py:332
 msgid "position x"
 msgstr ""
 
-#: models/structures.py:332
+#: models/structures.py:333
 msgid "x position in the solar system"
 msgstr ""
 
-#: models/structures.py:338
+#: models/structures.py:339
 msgid "position y"
 msgstr ""
 
-#: models/structures.py:339
+#: models/structures.py:340
 msgid "y position in the solar system"
 msgstr ""
 
-#: models/structures.py:345
+#: models/structures.py:346
 msgid "position z"
 msgstr ""
 
-#: models/structures.py:346
+#: models/structures.py:347
 msgid "z position in the solar system"
 msgstr ""
 
-#: models/structures.py:352 models/structures.py:839
+#: models/structures.py:353 models/structures.py:853
 #, fuzzy
 #| msgid "State"
 msgid "state"
 msgstr "状态"
 
-#: models/structures.py:353
+#: models/structures.py:354
 msgid "Current state of the structure"
 msgstr ""
 
-#: models/structures.py:359
+#: models/structures.py:360
 msgid "state timer end"
 msgstr ""
 
-#: models/structures.py:360
+#: models/structures.py:361
 msgid "Date at which the structure entered it's current state"
 msgstr ""
 
-#: models/structures.py:366
+#: models/structures.py:367
 msgid "state timer start"
 msgstr ""
 
-#: models/structures.py:367
+#: models/structures.py:368
 msgid "Date at which the structure will move to it's next state"
 msgstr ""
 
-#: models/structures.py:374
+#: models/structures.py:375
 msgid "tags"
 msgstr ""
 
-#: models/structures.py:375
+#: models/structures.py:376
 msgid "List of tags for this structure. "
 msgstr ""
 
-#: models/structures.py:381
+#: models/structures.py:382
 msgid "unanchors at"
 msgstr ""
 
-#: models/structures.py:382
+#: models/structures.py:383
 #, fuzzy
 #| msgid "Structure un-anchoring"
 msgid "Date at which the structure will unanchor"
 msgstr "建筑解铆中"
 
-#: models/structures.py:391
+#: models/structures.py:392
 msgid ""
 "Webhooks for sending notifications to. If any webhook is enabled, these will "
 "be used instead of the webhooks defined for the respective owner. If no "
 "webhook is enabled the owner's setting will be used. "
 msgstr ""
 
-#: models/structures.py:759
+#: models/structures.py:773
 msgid "The Eve item ID"
 msgstr ""
 
-#: models/structures.py:766
+#: models/structures.py:780
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this item is located in"
 msgstr "建筑服务下线"
 
-#: models/structures.py:774
+#: models/structures.py:788
 msgid "type of the item"
 msgstr ""
 
-#: models/structures.py:776
+#: models/structures.py:790
 msgid "is singleton"
 msgstr ""
 
-#: models/structures.py:780
+#: models/structures.py:794
 #, fuzzy
 #| msgid "Location"
 msgid "location flag"
 msgstr "位置"
 
-#: models/structures.py:781
+#: models/structures.py:795
 msgid "quantity"
 msgstr ""
 
-#: models/structures.py:784
+#: models/structures.py:798
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure item"
 msgstr "建筑列表"
 
-#: models/structures.py:785
+#: models/structures.py:799
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure items"
 msgstr "建筑列表"
 
-#: models/structures.py:831
+#: models/structures.py:845
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "Structure this service is installed to"
 msgstr "建筑服务下线"
 
-#: models/structures.py:834
+#: models/structures.py:848
 msgid "Name of the service"
 msgstr ""
 
-#: models/structures.py:840
+#: models/structures.py:854
 msgid "Current state of this service"
 msgstr ""
 
-#: models/structures.py:844
+#: models/structures.py:858
 #, fuzzy
 #| msgid "Structure List"
 msgid "structure service"
 msgstr "建筑列表"
 
-#: models/structures.py:845
+#: models/structures.py:859
 #, fuzzy
 #| msgid "Structure services off-line"
 msgid "structure services"
 msgstr "建筑服务下线"
 
-#: models/structures.py:861 webhooks/models.py:12
+#: models/structures.py:875 webhooks/models.py:12
 msgid "none"
 msgstr ""
 
-#: models/structures.py:862
+#: models/structures.py:876
 msgid "terrible"
 msgstr ""
 
-#: models/structures.py:863
+#: models/structures.py:877
 msgid "bad"
 msgstr ""
 
-#: models/structures.py:864
+#: models/structures.py:878
 msgid "neutral"
 msgstr ""
 
-#: models/structures.py:865
+#: models/structures.py:879
 msgid "good"
 msgstr ""
 
-#: models/structures.py:866
+#: models/structures.py:880
 msgid "excellent"
 msgstr ""
 
-#: models/structures.py:960
+#: models/structures.py:974
 #, fuzzy
 #| msgid "Alliance"
 msgid "alliance member"
 msgstr "联盟"
 
-#: models/structures.py:961
+#: models/structures.py:975
 msgid "config starbase equipment role"
 msgstr ""
 
-#: models/structures.py:962
+#: models/structures.py:976
 #, fuzzy
 #| msgid "Corporation"
 msgid "corporation member"
 msgstr "公司"
 
-#: models/structures.py:963
+#: models/structures.py:977
 msgid "starbase fuel technician role"
 msgstr ""
 
 #: templates/structures/base.html:4
 #, fuzzy
 #| msgid "Structure List"
 msgid "Structures"
@@ -2365,74 +2374,74 @@
 msgid "No Access"
 msgstr ""
 
 #: templates/structures/templatetags/list_tax_item.html:11
 msgid "Has Access"
 msgstr ""
 
-#: views.py:255
+#: views.py:256
 msgid "Fuel blocks per day (est.)"
 msgstr ""
 
-#: views.py:406
+#: views.py:407
 #, python-format
 msgid ""
 "You can only use your main or alt characters to add corporations. However, "
 "character %s is neither. "
 msgstr "你只能用你的大号或小号注册公司，但是%s不属于以上两种。"
 
-#: views.py:439
+#: views.py:440
 #, fuzzy, python-format
 #| msgid ""
 #| "%(corporation)s has been added with %(character)s as sync character. We "
 #| "have started fetching structures for this corporation. You will receive a "
 #| "report once the process is finished."
 msgid ""
 "%(corporation)s has been added with %(character)s as sync character. We have "
 "started fetching structures and notifications for this corporation and you "
 "will receive a report once the process is finished."
 msgstr ""
 "%(corporation)s已将%(character)s添加为同步人物。我们正在获取这个公司的建筑"
 "物。你将在这个过程结束后收到一份报告"
 
-#: views.py:455
+#: views.py:456
 #, python-format
 msgid "%(corporation)s was added as new structure owner by %(user)s."
 msgstr "%(corporation)s已被%(user)s添加为新建筑持有者"
 
-#: views.py:459
+#: views.py:460
 #, fuzzy, python-format
 #| msgid "Add Structure Owner"
 msgid "%s: Structure owner added: %s"
 msgstr "添加建筑持有人"
 
-#: views.py:466
+#: views.py:467
 #, python-format
 msgid ""
 "%(character)s has been added to %(corporation)s as sync character. You now "
 "have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:481
+#: views.py:482
 #, python-format
 msgid ""
 "%(character)s was added as sync character to %(corporation)s by %(user)s.\n"
 "We now have %(characters_count)d sync character(s) configured."
 msgstr ""
 
-#: views.py:491
+#: views.py:492
 #, python-format
 msgid "%s: Character added to: %s"
 msgstr ""
 
-#: views.py:508
+#: views.py:509
 msgid "service is up"
 msgstr "服务已上线"
 
-#: views.py:510
+#: views.py:511
 msgid "service is down"
 msgstr "服务已离线"
 
 #: webhooks/models.py:13
 msgid "here"
 msgstr ""
```

### Comparing `aa_structures-2.2.0/structures/management/commands/structures_load_eve.py` & `aa_structures-2.3.0/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.3.0/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/migrations/0001_initial_new.py` & `aa_structures-2.3.0/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.3.0/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.3.0/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/models/eveuniverse.py` & `aa_structures-2.3.0/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/models/notifications.py` & `aa_structures-2.3.0/structures/models/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Notification related models."""
 
 import math
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Set, Tuple, Union
 
 import dhooks_lite
 import yaml
 from multiselectfield import MultiSelectField
 from requests.exceptions import HTTPError
 
 from django.contrib.auth.models import Group
@@ -173,28 +173,28 @@
     )
     BILLING_I_HUB_DESTROYED_BY_BILL_FAILURE = (
         "IHubDestroyedByBillFailure",
         _("I_HUB destroyed by bill failure"),
     )
 
     @classproperty
-    def esi_notifications(cls) -> set:
-        return set(cls.values) - cls.generated_notifications
+    def esi_notifications(cls) -> Set["NotificationType"]:
+        return set(cls.values) - cls.generated_notifications  # type: ignore
 
     @classproperty
-    def generated_notifications(cls) -> set:
+    def generated_notifications(cls) -> Set["NotificationType"]:
         return {
             cls.STRUCTURE_JUMP_FUEL_ALERT,
             cls.STRUCTURE_REFUELED_EXTRA,
             cls.TOWER_REFUELED_EXTRA,
             cls.TOWER_REINFORCED_EXTRA,
         }
 
     @classproperty
-    def webhook_defaults(cls) -> list:
+    def webhook_defaults(cls) -> List["NotificationType"]:
         """List of default notifications for new webhooks."""
         return [
             cls.STRUCTURE_ANCHORING,
             cls.STRUCTURE_DESTROYED,
             cls.STRUCTURE_FUEL_ALERT,
             cls.STRUCTURE_LOST_ARMOR,
             cls.STRUCTURE_LOST_SHIELD,
@@ -208,28 +208,28 @@
             cls.TOWER_ALERT_MSG,
             cls.TOWER_RESOURCE_ALERT_MSG,
             cls.SOV_STRUCTURE_REINFORCED,
             cls.SOV_STRUCTURE_DESTROYED,
         ]
 
     @classproperty
-    def relevant_for_timerboard(cls) -> set:
+    def relevant_for_timerboard(cls) -> Set["NotificationType"]:
         """Notification types that can create timers."""
         return {
             cls.STRUCTURE_LOST_SHIELD,
             cls.STRUCTURE_LOST_ARMOR,
             cls.ORBITAL_REINFORCED,
             cls.MOONMINING_EXTRACTION_STARTED,
             cls.MOONMINING_EXTRACTION_CANCELLED,
             cls.SOV_STRUCTURE_REINFORCED,
             cls.TOWER_REINFORCED_EXTRA,
         }
 
     @classproperty
-    def relevant_for_alliance_level(cls) -> set:
+    def relevant_for_alliance_level(cls) -> Set["NotificationType"]:
         """Notification types that require the alliance level flag."""
         return {
             # billing
             cls.BILLING_BILL_OUT_OF_MONEY_MSG,
             cls.BILLING_I_HUB_DESTROYED_BY_BILL_FAILURE,
             cls.BILLING_I_HUB_BILL_ABOUT_TO_EXPIRE,
             # sov
@@ -251,26 +251,26 @@
             cls.WAR_WAR_DECLARED,
             cls.WAR_WAR_INHERITED,
             cls.WAR_WAR_RETRACTED_BY_CONCORD,
             cls.WAR_WAR_SURRENDER_OFFER_MSG,
         }
 
     @classproperty
-    def relevant_for_moonmining(cls) -> set:
+    def relevant_for_moonmining(cls) -> Set["NotificationType"]:
         """Notification types about moon mining."""
         return {
             cls.MOONMINING_EXTRACTION_STARTED,
             cls.MOONMINING_EXTRACTION_CANCELLED,
             cls.MOONMINING_LASER_FIRED,
             cls.MOONMINING_EXTRACTION_FINISHED,
             cls.MOONMINING_AUTOMATIC_FRACTURE,
         }
 
     @classproperty
-    def structure_related(cls) -> set:
+    def structure_related(cls) -> Set["NotificationType"]:
         """Notification types that are related to a structure."""
         return {
             cls.STRUCTURE_ONLINE,
             cls.STRUCTURE_FUEL_ALERT,
             cls.STRUCTURE_JUMP_FUEL_ALERT,
             cls.STRUCTURE_REFUELED_EXTRA,
             cls.STRUCTURE_SERVICES_OFFLINE,
@@ -294,26 +294,26 @@
             cls.TOWER_ALERT_MSG,
             cls.TOWER_RESOURCE_ALERT_MSG,
             cls.TOWER_REFUELED_EXTRA,
             cls.TOWER_REINFORCED_EXTRA,
         }
 
     @classproperty
-    def relevant_for_forwarding(cls) -> set:
+    def relevant_for_forwarding(cls) -> Set["NotificationType"]:
         """Notification types that are forwarded to Discord."""
-        my_set = set(cls.values_enabled)
+        my_set = set(cls.values_enabled)  # type: ignore
         # if STRUCTURES_NOTIFICATION_DISABLE_ESI_FUEL_ALERTS:
         #     my_set.discard(cls.STRUCTURE_FUEL_ALERT)
         #     my_set.discard(cls.TOWER_RESOURCE_ALERT_MSG)
         return my_set
 
     @classproperty
-    def values_enabled(cls) -> set:
+    def values_enabled(cls) -> Set["NotificationType"]:
         """Values of enabled notif types only."""
-        my_set = set(cls.values)
+        my_set = set(cls.values)  # type: ignore
         if not STRUCTURES_FEATURE_REFUELED_NOTIFICATIONS:
             my_set.discard(cls.STRUCTURE_REFUELED_EXTRA)
             my_set.discard(cls.TOWER_REFUELED_EXTRA)
         return my_set
 
     @classproperty
     def choices_enabled(cls) -> list:
@@ -510,18 +510,21 @@
             and self.owner.corporation.alliance is not None
             and not self.owner.is_alliance_main
         )
 
     def relevant_webhooks(self) -> models.QuerySet:
         """Determine relevant webhooks matching this notification type."""
         if not self.is_structure_related:
-            structures_qs = None
+            structures_qs = Structure.objects.none()
         else:
             structures_qs = self.calc_related_structures()
-        if structures_qs and structures_qs.filter(webhooks__isnull=False).count() == 1:
+        if (
+            structures_qs.exists()
+            and structures_qs.filter(webhooks__isnull=False).count() == 1
+        ):
             webhooks_qs = structures_qs.first().webhooks.filter(
                 notification_types__contains=self.notif_type, is_active=True
             )
         else:
             webhooks_qs = self.owner.webhooks.filter(
                 notification_types__contains=self.notif_type, is_active=True
             )
@@ -627,15 +630,15 @@
         if success and not self.is_temporary:
             self.is_sent = True
             self.save()
         return success
 
     def _generate_embed(
         self, language_code: Optional[str]
-    ) -> Tuple[dhooks_lite.Embed, Webhook.PingType]:
+    ) -> Tuple[dhooks_lite.Embed, Optional[Webhook.PingType]]:
         """Generates a Discord embed for this notification."""
         from ..core.notification_embeds import NotificationBaseEmbed
 
         logger.info("Creating embed with language = %s" % language_code)
         with translation.override(language_code):
             notification_embed = NotificationBaseEmbed.create(self)
             embed = notification_embed.generate_embed()
```

### Comparing `aa_structures-2.2.0/structures/models/owners.py` & `aa_structures-2.3.0/structures/models/owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,17 +901,15 @@
             except HTTPNotFound:
                 pass
             else:
                 names_data += names_data_chunk
         names = {x["item_id"]: x["name"] for x in names_data}
         return names
 
-    def _update_starbase_detail(
-        self, structure: object, token: Token
-    ) -> StarbaseDetail:
+    def _update_starbase_detail(self, structure, token: Token) -> StarbaseDetail:
         """Update detail for the starbase from ESI."""
         operation = esi.client.Corporation.get_corporations_corporation_id_starbases_starbase_id(
             corporation_id=structure.owner.corporation.corporation_id,
             starbase_id=structure.id,
             system_id=structure.eve_solar_system.id,
             token=token.valid_access_token(),
         )
```

### Comparing `aa_structures-2.2.0/structures/models/structures.py` & `aa_structures-2.3.0/structures/models/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
     )
     unanchor_role = models.CharField(max_length=2, choices=Role.choices)
     use_alliance_standings = models.BooleanField()
 
     def __str__(self) -> str:
         return str(self.structure)
 
-    def calc_fuel_expires(self) -> dt.datetime:
+    def calc_fuel_expires(self) -> Optional[dt.datetime]:
         """Estimate when fuel will expire for this starbase.
 
         Estimate will vary due to server caching of remaining fuel blocks.
         """
         if self.structure.state is Structure.State.POS_OFFLINE:
             return None
         fuel = self.fuels.filter(eve_type__eve_group_id=EveGroupId.FUEL_BLOCK).first()
```

### Comparing `aa_structures-2.2.0/structures/static/structures/css/global.css` & `aa_structures-2.3.0/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/css/main.css` & `aa_structures-2.3.0/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.3.0/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/0h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/0l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/0m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/0r.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/0s.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/1h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/1l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/1m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/1r.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/2h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/2l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/2m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/2r.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/3h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/3l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/3m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/3r.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/4h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/4l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/4m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/4s.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/5h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/5l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/5m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/5s.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/6h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/6l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/6m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/7h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/7l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/7m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/8h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/8l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/8m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/circle.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/h.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/l.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/m.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/noship.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/r.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/main.html` & `aa_structures-2.3.0/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.3.0/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.3.0/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.3.0/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.3.0/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.3.0/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.3.0/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.3.0/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.3.0/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.3.0/structures/templates/structures/partials/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.3.0/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/templatetags/structures.py` & `aa_structures-2.3.0/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_admin.py` & `aa_structures-2.3.0/structures/tests/test_admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,38 @@
 from django.test import RequestFactory, TestCase
 from django.urls import reverse
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
 from allianceauth.eveonline.models import EveCorporationInfo
 
-from ..admin import (
+from structures.admin import (
     NotificationAdmin,
     OwnerAdmin,
     OwnerAllianceFilter,
     OwnerCorporationsFilter,
     StructureAdmin,
+    StructureFuelAlertConfigAdmin,
     WebhookAdmin,
 )
-from ..models import (
+from structures.models import (
     FuelAlertConfig,
     Notification,
     Owner,
     Structure,
     StructureTag,
     Webhook,
 )
+
+from .testdata.factories_2 import (
+    FuelAlertConfigFactory,
+    NotificationFactory,
+    OwnerFactory,
+    StructureFactory,
+)
 from .testdata.helpers import (
     create_structures,
     create_user,
     load_entities,
     load_notification_entities,
     set_owner_character,
 )
@@ -40,26 +48,25 @@
 
 
 class MockRequest(object):
     def __init__(self, user=None):
         self.user = user
 
 
-class TestFuelNotificationConfigAdmin(TestCase):
+class TestFuelNotificationConfigAdminView(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.defaults = {
             "is_enabled": True,
             "channel_ping_type": Webhook.PingType.HERE,
             "color": Webhook.Color.WARNING,
         }
         cls.user = User.objects.create_superuser("Clark Kent")
         load_eveuniverse()
-        create_structures()
 
     def test_should_create_new_config(self):
         # given
         self.client.force_login(self.user)
         # when
         response = self.client.post(
             reverse("admin:structures_fuelalertconfig_add"),
@@ -70,31 +77,31 @@
             response, reverse("admin:structures_fuelalertconfig_changelist")
         )
         self.assertEqual(FuelAlertConfig.objects.count(), 1)
 
     def test_should_update_existing_config(self):
         # given
         self.client.force_login(self.user)
-        config = FuelAlertConfig.objects.create(start=48, end=24, repeat=12)
+        config = FuelAlertConfigFactory(start=48, end=24, repeat=12)
         # when
         response = self.client.post(
             reverse("admin:structures_fuelalertconfig_change", args=[config.pk]),
             data={**self.defaults, **{"start": 48, "end": 0, "repeat": 2}},
         )
         # then
         self.assertRedirects(
             response, reverse("admin:structures_fuelalertconfig_changelist")
         )
         self.assertEqual(FuelAlertConfig.objects.count(), 1)
 
     def test_should_remove_existing_fuel_notifications_when_timing_changed(self):
         # given
         self.client.force_login(self.user)
-        config = FuelAlertConfig.objects.create(start=48, end=24, repeat=12)
-        structure = Structure.objects.get(id=1000000000001)
+        config = FuelAlertConfigFactory(start=48, end=24, repeat=12)
+        structure = StructureFactory()
         structure.structure_fuel_alerts.create(
             config=config, structure=structure, hours=5
         )
         # when
         response = self.client.post(
             reverse("admin:structures_fuelalertconfig_change", args=[config.pk]),
             data={**self.defaults, **{"start": 48, "end": 0, "repeat": 2}},
@@ -104,16 +111,16 @@
             response, reverse("admin:structures_fuelalertconfig_changelist")
         )
         self.assertEqual(structure.structure_fuel_alerts.count(), 0)
 
     def test_should_not_remove_existing_fuel_notifications_on_other_changes(self):
         # given
         self.client.force_login(self.user)
-        config = FuelAlertConfig.objects.create(start=48, end=24, repeat=12)
-        structure = Structure.objects.get(id=1000000000001)
+        config = FuelAlertConfigFactory(start=48, end=24, repeat=12)
+        structure = StructureFactory()
         structure.structure_fuel_alerts.create(
             config=config, structure=structure, hours=5
         )
         # when
         response = self.client.post(
             reverse("admin:structures_fuelalertconfig_change", args=[config.pk]),
             data={
@@ -152,15 +159,15 @@
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "errornote")
         self.assertEqual(FuelAlertConfig.objects.count(), 0)
 
     def test_should_not_allow_creating_overlapping(self):
         # given
         self.client.force_login(self.user)
-        FuelAlertConfig.objects.create(start=48, end=24, repeat=12)
+        FuelAlertConfigFactory(start=48, end=24, repeat=12)
         # when
         response = self.client.post(
             reverse("admin:structures_fuelalertconfig_add"),
             data={**self.defaults, **{"start": 36, "end": 0, "repeat": 8}},
         )
         # then
         self.assertEqual(response.status_code, 200)
@@ -203,14 +210,37 @@
         )
         # then
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "errornote")
         self.assertEqual(FuelAlertConfig.objects.count(), 0)
 
 
+class TestStructureFuelAlertAdmin(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        cls.modeladmin = StructureFuelAlertConfigAdmin(
+            model=FuelAlertConfig, admin_site=AdminSite()
+        )
+        load_eveuniverse()
+
+    @patch(MODULE_PATH + ".StructureFuelAlertConfigAdmin.message_user", spec=True)
+    @patch(MODULE_PATH + ".tasks", spec=True)
+    def test_should_send_fuel_notifications(self, mock_tasks, mock_message_user):
+        # given
+        config = FuelAlertConfigFactory()
+        request = MockRequest()
+        queryset = FuelAlertConfig.objects.filter(pk=config.pk)
+        # when
+        self.modeladmin.send_fuel_notifications(request, queryset)
+        # then
+        self.assertTrue(mock_tasks.send_queued_messages_for_webhooks.called)
+        self.assertTrue(mock_message_user.called)
+
+
 class TestNotificationAdmin(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.modeladmin = NotificationAdmin(model=Notification, admin_site=AdminSite())
         load_eveuniverse()
         create_structures()
@@ -333,28 +363,28 @@
     @patch(MODULE_PATH + ".app_settings.STRUCTURES_NOTIFICATION_TURNAROUND_MEDIUM", 15)
     @patch(MODULE_PATH + ".app_settings.STRUCTURES_NOTIFICATION_TURNAROUND_LONG", 50)
     @patch(
         MODULE_PATH + ".app_settings.STRUCTURES_NOTIFICATION_TURNAROUND_MAX_VALID", 3600
     )
     def test_should_return_correct_turnaround_times(self):
         # given
-        my_owner = Owner.objects.get(corporation__corporation_id=2001)
+        my_owner = OwnerFactory()
         my_sender = EveEntity.objects.get(id=1001)
         my_now = now()
-        Notification.objects.create(
+        NotificationFactory(
             owner=my_owner,
             notification_id=1,
             sender=my_sender,
             last_updated=my_now,
             timestamp=my_now,
             created=my_now + dt.timedelta(seconds=3601),
         )
         for i in range(50):
             timestamp = my_now + dt.timedelta(minutes=i)
-            Notification.objects.create(
+            NotificationFactory(
                 owner=my_owner,
                 notification_id=2 + i,
                 sender=my_sender,
                 last_updated=my_now,
                 timestamp=timestamp,
                 created=timestamp + dt.timedelta(seconds=2),
             )
@@ -418,20 +448,18 @@
         self.assertTrue(mock_message_user.called)
 
     def test_owner_corporations_status_filter(self):
         class StructureAdminTest(admin.ModelAdmin):
             list_filter = (OwnerCorporationsFilter,)
 
         Owner.objects.all().delete()
-        owner_2001 = Owner.objects.create(
+        owner_2001 = OwnerFactory(
             corporation=EveCorporationInfo.objects.get(corporation_id=2001)
         )
-        Owner.objects.create(
-            corporation=EveCorporationInfo.objects.get(corporation_id=2002)
-        )
+        OwnerFactory(corporation=EveCorporationInfo.objects.get(corporation_id=2002))
         my_modeladmin = StructureAdminTest(Structure, AdminSite())
 
         # Make sure the lookups are correct
         request = self.factory.get("/")
         request.user = self.user
         changelist = my_modeladmin.get_changelist_instance(request)
         filterspec = changelist.get_filters(request)[0][0]
@@ -447,23 +475,21 @@
         self.assertSetEqual(set(queryset), set(expected))
 
     def test_owner_alliance_status_filter(self):
         class StructureAdminTest(admin.ModelAdmin):
             list_filter = (OwnerAllianceFilter,)
 
         Owner.objects.all().delete()
-        owner_2001 = Owner.objects.create(
+        owner_2001 = OwnerFactory(
             corporation=EveCorporationInfo.objects.get(corporation_id=2001)
         )
-        owner_2002 = Owner.objects.create(
+        owner_2002 = OwnerFactory(
             corporation=EveCorporationInfo.objects.get(corporation_id=2002)
         )
-        Owner.objects.create(
-            corporation=EveCorporationInfo.objects.get(corporation_id=2102)
-        )
+        OwnerFactory(corporation=EveCorporationInfo.objects.get(corporation_id=2102))
         modeladmin = StructureAdminTest(Structure, AdminSite())
 
         # Make sure the lookups are correct
         request = self.factory.get("/")
         request.user = self.user
         changelist = modeladmin.get_changelist_instance(request)
         filterspec = changelist.get_filters(request)[0][0]
```

### Comparing `aa_structures-2.2.0/structures/tests/test_checks.py` & `aa_structures-2.3.0/structures/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_helpers.py` & `aa_structures-2.3.0/structures/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_integration.py` & `aa_structures-2.3.0/structures/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_managers_1.py` & `aa_structures-2.3.0/structures/tests/test_managers_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_managers_3.py` & `aa_structures-2.3.0/structures/tests/test_managers_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_tasks.py` & `aa_structures-2.3.0/structures/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/test_views.py` & `aa_structures-2.3.0/structures/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/core/test_notification_embeds.py` & `aa_structures-2.3.0/structures/tests/core/test_notification_embeds.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,45 +4,68 @@
 
 from django.test import TestCase, override_settings
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ...core import notification_embeds as ne
-from ...models.notifications import Notification, NotificationType, Structure, Webhook
+from structures.core import notification_embeds as ne
+from structures.core.notification_embeds import (
+    NotificationBaseEmbed,
+    NotificationTowerReinforcedExtra,
+)
+from structures.models.notifications import (
+    Notification,
+    NotificationType,
+    Structure,
+    Webhook,
+)
+
 from ..testdata.factories import (
     create_notification,
     create_owner_from_user,
     create_starbase,
 )
+from ..testdata.factories_2 import (
+    EveEntityAllianceFactory,
+    GeneratedNotificationFactory,
+    NotificationFactory,
+    OwnerFactory,
+    WebhookFactory,
+)
 from ..testdata.helpers import (
     create_structures,
     load_entities,
     load_notification_entities,
     markdown_to_plain,
     set_owner_character,
 )
 from ..testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.core.notification_embeds"
 
 
+class TestBilType(TestCase):
+    def test_should_create_from_valid_id(self):
+        self.assertEqual(ne.BillType.to_enum(7), ne.BillType.INFRASTRUCTURE_HUB)
+
+    def test_should_create_from_invalid_id(self):
+        for bill_id in range(7):
+            with self.subTest(bill_id=bill_id):
+                self.assertEqual(ne.BillType.to_enum(bill_id), ne.BillType.UNKNOWN)
+
+
 class TestNotificationEmbeds(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         create_structures()
         _, cls.owner = set_owner_character(character_id=1001)
         load_notification_entities(cls.owner)
-        cls.webhook = Webhook.objects.create(
-            name="Test", url="http://www.example.com/dummy/"
-        )
-        cls.owner.webhooks.add(cls.webhook)
 
     def test_should_create_obj_from_notification(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
         # when
         notification_embed = ne.NotificationBaseEmbed.create(notification)
         # then
@@ -55,14 +78,48 @@
         self.assertEqual(
             repr(notification_embed),
             "NotificationMoonminningExtractionFinished(notification=Notification("
             "notification_id=1000000403, owner='Wayne Technologies', "
             "notif_type='MoonminingExtractionFinished'))",
         )
 
+    def test_should_raise_exception_for_unsupported_notif_types(self):
+        # given
+        notification = Notification.objects.create(
+            notification_id=666,
+            owner=self.owner,
+            sender=EveEntity.objects.get(id=2001),
+            timestamp=now(),
+            notif_type="XXXUnsupportedNotificationTypeXXX",
+            last_updated=now(),
+        )
+        # when / then
+        with self.assertRaises(NotImplementedError):
+            ne.NotificationBaseEmbed.create(notification)
+
+    def test_should_require_notification_for_init(self):
+        with self.assertRaises(TypeError):
+            ne.NotificationBaseEmbed(notification="dummy")
+
+    def test_should_require_notification_for_factory(self):
+        with self.assertRaises(TypeError):
+            ne.NotificationBaseEmbed.create(notification="dummy")
+
+
+class TestNotificationEmbedsGenerate(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+        create_structures()
+        _, cls.owner = set_owner_character(character_id=1001)
+        load_notification_entities(cls.owner)
+        cls.webhook = WebhookFactory()
+        cls.owner.webhooks.add(cls.webhook)
+
     def test_should_generate_embed_from_notification(self):
         # given
         notification = Notification.objects.get(notification_id=1000000403)
         notification_embed = ne.NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
@@ -112,44 +169,14 @@
                 # when
                 discord_embed = notification_embed.generate_embed()
                 # then
                 self.assertIsInstance(discord_embed, dhooks_lite.Embed)
                 types_tested.add(notification.notif_type)
         self.assertSetEqual(NotificationType.esi_notifications, types_tested)
 
-    def test_should_raise_exception_for_unsupported_notif_types(self):
-        # given
-        notification = Notification.objects.create(
-            notification_id=666,
-            owner=self.owner,
-            sender=EveEntity.objects.get(id=2001),
-            timestamp=now(),
-            notif_type="XXXUnsupportedNotificationTypeXXX",
-            last_updated=now(),
-        )
-        # when / then
-        with self.assertRaises(NotImplementedError):
-            ne.NotificationBaseEmbed.create(notification)
-
-    def test_should_require_notification_for_init(self):
-        with self.assertRaises(TypeError):
-            ne.NotificationBaseEmbed(notification="dummy")
-
-    def test_should_require_notification_for_factory(self):
-        with self.assertRaises(TypeError):
-            ne.NotificationBaseEmbed.create(notification="dummy")
-
-    def test_should_not_allow_generating_embed_for_base_class(self):
-        # given
-        notification = Notification.objects.get(notification_id=1000000403)
-        notification_embed = ne.NotificationBaseEmbed(notification=notification)
-        # when
-        with self.assertRaises(ValueError):
-            notification_embed.generate_embed()
-
     def test_should_set_ping_everyone_for_color_danger(self):
         # given
         notification = Notification.objects.get(notification_id=1000000513)
         notification_embed = ne.NotificationBaseEmbed.create(notification)
         notification_embed._color = Webhook.Color.DANGER
         # when
         notification_embed.generate_embed()
@@ -265,7 +292,69 @@
         )
         notification_embed = ne.NotificationBaseEmbed.create(notification)
         # when
         discord_embed = notification_embed.generate_embed()
         # then
         description = markdown_to_plain(discord_embed.description)
         self.assertIn("is running out of fuel in 2 hours", description)
+
+
+class TestGeneratedNotification(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+
+    def test_should_create_tower_reinforced_embed(self):
+        # given
+        notif = GeneratedNotificationFactory()
+        # when
+        obj = NotificationBaseEmbed.create(notif)
+        # then
+        self.assertIsInstance(obj, NotificationTowerReinforcedExtra)
+
+    def test_should_generate_embed(self):
+        # given
+        notif = GeneratedNotificationFactory()
+        embed = NotificationBaseEmbed.create(notif)
+        # when
+        obj = embed.generate_embed()
+        # then
+        self.assertIsInstance(obj, dhooks_lite.Embed)
+        starbase = notif.structures.first()
+        self.assertIn(starbase.name, obj.description)
+
+
+class TestEveNotificationEmbeds(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+        cls.owner = OwnerFactory()
+
+    def test_should_create_sov_embed(self):
+        # given
+        notif = NotificationFactory(
+            owner=self.owner,
+            sender=EveEntityAllianceFactory(),
+            notif_type=NotificationType.SOV_ENTOSIS_CAPTURE_STARTED,
+            text_from_dict={"solarSystemID": 30000474, "structureTypeID": 32226},
+        )
+        embed = NotificationBaseEmbed.create(notif)
+        # when
+        obj = embed.generate_embed()
+        # then
+        self.assertIsInstance(obj, dhooks_lite.Embed)
+
+    def test_should_create_sov_embed_without_sender(self):
+        # given
+        notif = NotificationFactory(
+            owner=self.owner,
+            sender=None,
+            notif_type=NotificationType.SOV_ENTOSIS_CAPTURE_STARTED,
+            text_from_dict={"solarSystemID": 30000474, "structureTypeID": 32226},
+        )
+        embed = NotificationBaseEmbed.create(notif)
+        # when
+        obj = embed.generate_embed()
+        # then
+        self.assertIsInstance(obj, dhooks_lite.Embed)
```

### Comparing `aa_structures-2.2.0/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.3.0/structures/tests/core/test_notification_structuretimers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.3.0/structures/tests/core/test_notifications_timerboard.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/core/test_serializers.py` & `aa_structures-2.3.0/structures/tests/core/test_serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/core/test_sovereignty.py` & `aa_structures-2.3.0/structures/tests/core/test_sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/core/test_starbases.py` & `aa_structures-2.3.0/structures/tests/core/test_starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.3.0/structures/tests/models/test_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_notifications_1.py` & `aa_structures-2.3.0/structures/tests/models/test_notifications_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_notifications_2.py` & `aa_structures-2.3.0/structures/tests/models/test_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_notifications_3.py` & `aa_structures-2.3.0/structures/tests/models/test_notifications_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.3.0/structures/tests/models/test_notifications_discord.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_owners_1.py` & `aa_structures-2.3.0/structures/tests/models/test_owners_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_owners_2.py` & `aa_structures-2.3.0/structures/tests/models/test_owners_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_owners_3.py` & `aa_structures-2.3.0/structures/tests/models/test_owners_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/models/test_structures.py` & `aa_structures-2.3.0/structures/tests/models/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.3.0/structures/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/entities.json` & `aa_structures-2.3.0/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/esi_data.json` & `aa_structures-2.3.0/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.3.0/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/factories.py` & `aa_structures-2.3.0/structures/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/factories_2.py` & `aa_structures-2.3.0/structures/tests/testdata/factories_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.3.0/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.3.0/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/generate_structures.py` & `aa_structures-2.3.0/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/helpers.py` & `aa_structures-2.3.0/structures/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.3.0/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/webhooks/core.py` & `aa_structures-2.3.0/structures/webhooks/core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/webhooks/managers.py` & `aa_structures-2.3.0/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/webhooks/models.py` & `aa_structures-2.3.0/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/structures/webhooks/tests/test_core.py` & `aa_structures-2.3.0/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/LICENSE` & `aa_structures-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/README.md` & `aa_structures-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/pyproject.toml` & `aa_structures-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_structures-2.2.0/PKG-INFO` & `aa_structures-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.2.0
+Version: 2.3.0
 Summary: App for managing Eve Online structures with Alliance Auth
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Documentation, https://aa-structures.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structures/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
```

