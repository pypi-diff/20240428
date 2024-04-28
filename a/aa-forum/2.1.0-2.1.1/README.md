# Comparing `tmp/aa_forum-2.1.0.tar.gz` & `tmp/aa_forum-2.1.1.tar.gz`

## Comparing `aa_forum-2.1.0.tar` & `aa_forum-2.1.1.tar`

### file list

```diff
@@ -1,204 +1,203 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/admin.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/app_settings.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/apps.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/auth_hooks.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/constants.py
--rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/forms.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/managers.py
--rw-r--r--   0        0        0    30320 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/models.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/signals.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/urls.py
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/discord_messages.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/eve_images.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/forms.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/pagination.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/text.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/user.py
--rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/django.pot
--rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44946 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41205 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    39473 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39830 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    39551 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40498 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39849 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0001_initial.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0002_default_settings.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0003_board_discord_webhook.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0005_announcement_boards.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0006_reset_default_settings.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0007_change_settings_to_singleton.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0008_populate_default_settings.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0009_add_related_names.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0010_better_setting_names.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0011_userprofile.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0012_personal_messages.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0016_fix_quotation_marks.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/drop_tables.sql
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/fake_messages.py
--rw-r--r--   0        0        0    13044 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.css
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css
--rw-r--r--   0        0        0    15567 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
--rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
--rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
--rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
--rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
--rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
--rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
--rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
--rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
--rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/base.html
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor-js.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/select2-css.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/select2-js.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/breadcrumb.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu.html
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/categories.html
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/new-category.html
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/forum-index.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board.html
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/profile/form.html
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/pagination.html
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-form.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-result.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/forum-settings.html
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/board.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/index.html
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-message.html
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/new-topic.html
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/topic.html
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/profile/index.html
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/search/results.html
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templatetags/__init__.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templatetags/aa_forum.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_app_settings.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_helpers.py
--rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_integration.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_managers.py
--rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_models.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_signals.py
--rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_templatetags.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_views_admin.py
--rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_views_forum.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/__init__.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/admin.py
--rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/forum.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/personal_messages.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/profile.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/search.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/widgets.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.1.0/LICENSE
--rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.1.0/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/admin.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/app_settings.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/apps.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/auth_hooks.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/constants.py
+-rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/forms.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/managers.py
+-rw-r--r--   0        0        0    30251 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/models.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/signals.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/urls.py
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/discord_messages.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/eve_images.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/forms.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/pagination.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/text.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/helper/user.py
+-rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/django.pot
+-rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44946 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40664 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41205 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    39473 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39830 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    39551 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40498 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39849 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0002_default_settings.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0003_board_discord_webhook.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0005_announcement_boards.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0006_reset_default_settings.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0007_change_settings_to_singleton.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0008_populate_default_settings.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0009_add_related_names.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0010_better_setting_names.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0011_userprofile.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0012_personal_messages.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0016_fix_quotation_marks.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/migrations/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/scripts/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/scripts/fake_messages.py
+-rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.css
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.min.css
+-rw-r--r--   0        0        0    16294 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
+-rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
+-rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
+-rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
+-rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
+-rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
+-rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
+-rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/base.html
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/select2-css.html
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/select2-js.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/breadcrumb.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/menu.html
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/categories.html
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/new-category.html
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/forum-index.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/board.html
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/profile/form.html
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/search/pagination.html
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/search/search-form.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/search/search-result.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/administration/forum-settings.html
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/board.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/modify-message.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/new-topic.html
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/topic.html
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/profile/index.html
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/search/results.html
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templatetags/__init__.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/templatetags/aa_forum.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_helpers.py
+-rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_integration.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_managers.py
+-rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_models.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_signals.py
+-rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_templatetags.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_views_admin.py
+-rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/test_views_forum.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/__init__.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/admin.py
+-rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/forum.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/personal_messages.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/profile.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/search.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.1.1/aa_forum/views/widgets.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.1.1/LICENSE
+-rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.1.1/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.1.1/PKG-INFO
```

### Comparing `aa_forum-2.1.0/aa_forum/admin.py` & `aa_forum-2.1.1/aa_forum/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/app_settings.py` & `aa_forum-2.1.1/aa_forum/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/apps.py` & `aa_forum-2.1.1/aa_forum/apps.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/auth_hooks.py` & `aa_forum-2.1.1/aa_forum/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/constants.py` & `aa_forum-2.1.1/aa_forum/constants.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/forms.py` & `aa_forum-2.1.1/aa_forum/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/managers.py` & `aa_forum-2.1.1/aa_forum/managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/models.py` & `aa_forum-2.1.1/aa_forum/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,23 +448,21 @@
 
         :param user:
         :type user:
         :return:
         :rtype:
         """
 
-        user_can_start_topic = True
-
         if self.is_announcement_board:
-            user_can_start_topic = bool(
+            return bool(
                 user.has_perm(perm="aa_forum.manage_forum")
                 or user.groups.filter(pk__in=self.announcement_groups.all()).exists()
             )
 
-        return user_can_start_topic
+        return True
 
     def _update_message_references(self):
         """
         Update the first and last message for this board.
 
         :return:
         :rtype:
```

### Comparing `aa_forum-2.1.0/aa_forum/signals.py` & `aa_forum-2.1.1/aa_forum/signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/urls.py` & `aa_forum-2.1.1/aa_forum/urls.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/discord_messages.py` & `aa_forum-2.1.1/aa_forum/helper/discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/eve_images.py` & `aa_forum-2.1.1/aa_forum/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/forms.py` & `aa_forum-2.1.1/aa_forum/helper/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/pagination.py` & `aa_forum-2.1.1/aa_forum/helper/pagination.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/text.py` & `aa_forum-2.1.1/aa_forum/helper/text.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/helper/user.py` & `aa_forum-2.1.1/aa_forum/helper/user.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/django.pot` & `aa_forum-2.1.1/aa_forum/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/cs/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/ja/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/nl/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/sk/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_forum-2.1.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_forum-2.1.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0001_initial.py` & `aa_forum-2.1.1/aa_forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0002_default_settings.py` & `aa_forum-2.1.1/aa_forum/migrations/0002_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py` & `aa_forum-2.1.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0005_announcement_boards.py` & `aa_forum-2.1.1/aa_forum/migrations/0005_announcement_boards.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0006_reset_default_settings.py` & `aa_forum-2.1.1/aa_forum/migrations/0006_reset_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0007_change_settings_to_singleton.py` & `aa_forum-2.1.1/aa_forum/migrations/0007_change_settings_to_singleton.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0008_populate_default_settings.py` & `aa_forum-2.1.1/aa_forum/migrations/0008_populate_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0009_add_related_names.py` & `aa_forum-2.1.1/aa_forum/migrations/0009_add_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0010_better_setting_names.py` & `aa_forum-2.1.1/aa_forum/migrations/0010_better_setting_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0011_userprofile.py` & `aa_forum-2.1.1/aa_forum/migrations/0011_userprofile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0012_personal_messages.py` & `aa_forum-2.1.1/aa_forum/migrations/0012_personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py` & `aa_forum-2.1.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py` & `aa_forum-2.1.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0016_fix_quotation_marks.py` & `aa_forum-2.1.1/aa_forum/migrations/0016_fix_quotation_marks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py` & `aa_forum-2.1.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/scripts/drop_tables.sql` & `aa_forum-2.1.1/aa_forum/scripts/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/scripts/fake_messages.py` & `aa_forum-2.1.1/aa_forum/scripts/fake_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.css`

 * *Files 4% similar despite different names*

```diff
@@ -392,14 +392,37 @@
     }
 
     .aa-forum .ck-word-count {
         color: var(--bs-secondary-color) !important;
 
         --bs-text-opacity: 1;
     }
+
+    /* Image alignment
+    --------------------------------------------------------------------------------- */
+    .aa-forum .ck-content .image {
+        margin: 0.9em 0;
+    }
+
+    .aa-forum .ck-content .image-style-align-center {
+        margin-left: auto;
+        margin-right: auto;
+    }
+
+    .aa-forum .ck-content .image-style-align-left {
+        margin-right: var(--ck-image-style-spacing);
+    }
+
+    .aa-forum .ck-content .image-style-align-right {
+        margin-left: var(--ck-image-style-spacing);
+    }
+
+    .aa-forum .ck-content .image-style-side {
+        margin-left: var(--ck-image-style-spacing);
+    }
 }
 
 /*
 ----------------------------------------------------------------------------------------
                 Responsive (@media all and (min-width: 768px))
 ----------------------------------------------------------------------------------------
 */
```

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-:root{--bg-hover-transition:background-color 0.25s linear}@media all{.aa-forum .aa-forum-svg-wrapper{height:0;width:0}.aa-forum .aa-forum-body #aa-forum-form-search-results .input-group{margin-bottom:1rem}.aa-forum .aa-forum-ui-placeholder{outline:1px dashed rgb(0 0 0)}.aa-forum .boards-sortable,.aa-forum .categories-sortable{list-style-type:none}.aa-forum .boards-sortable>li:first-child{margin-top:1rem}.aa-forum [data-bs-toggle=collapse].collapsed .if-expanded{display:none}.aa-forum [data-bs-toggle=collapse]:not(.collapsed) .if-collapsed{display:none}.aa-forum .category-sortable{cursor:move}.aa-forum .aa-forum-breadcrumb ul{list-style-type:none;padding:0}.aa-forum .aa-forum-breadcrumb ul li{display:inline}.aa-forum .aa-forum-breadcrumb ul li:first-child{padding-left:0}.aa-forum .card-aa-forum-category .aa-forum-board{flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-category .aa-forum-board:last-child{margin-bottom:0}.aa-forum .card-aa-forum-category .aa-forum-board:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-category .aa-forum-board-image svg{height:65px;margin-top:-1rem;width:65px}.aa-forum .card-aa-forum-category .aa-forum-board-name{width:100%}.aa-forum .aa-forum-board-name p:last-child{margin:0}.aa-forum .aa-forum-board-group-restrictions{list-style-type:none;margin:0;padding:0}.aa-forum .aa-forum-board-last-post .img-last-post-avatar{float:left;height:55px;margin-right:1rem;width:55px}.aa-forum .aa-forum-board-last-post .last-post-information{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;word-wrap:normal}.aa-forum .aa-forum-legend>span{display:flex;margin-right:5rem}.aa-forum .aa-forum-legend .aa-forum-legend-image svg{height:30px;width:30px}.aa-forum .aa-forum-legend .aa-forum-legend-text{display:inline-block}.aa-forum .aa-forum-legend span:last-child{margin-right:0}.aa-forum .aa-forum-topic-row .aa-forum-topic{align-content:center;align-items:center;display:flex;flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child,.aa-forum .aa-forum-topic-row:last-child .aa-forum-topic{margin-bottom:0}.aa-forum .aa-forum-topic-row .aa-forum-topic:hover{background:rgb(0 0 0/5%)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image{width:40px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg{height:35px;margin-top:-1rem;width:35px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name{width:auto}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats{text-align:center;width:15%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post{width:25%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions{width:70px}.aa-forum .aa-forum-topic-locked{background-color:rgb(185 199 219/25%)}.aa-forum .aa-forum-topic-sticky{background-color:rgb(255 220 104/25%)}.aa-forum .label-aa-forum-topic-new-message{font-size:55%}.aa-forum .label-aa-forum-child-board-new-message{font-size:55%;margin-left:.25rem;padding:.3em .6em;vertical-align:middle}.aa-forum .aa-forum-message-author .img-author-avatar{max-width:100%}.aa-forum .aa-forum-message-wrapper{width:auto}.aa-forum .aa-forum-message-body{border-top:1px solid rgb(236 240 241)}.aa-forum .aa-forum-message-body-author-signature{border-top:1px solid rgb(236 240 241);margin-top:3em}.aa-forum .aa-forum-message-body-last-edited{margin-top:5rem}.aa-forum .aa-forum-message-body img{height:auto!important;max-width:100%}.aa-forum .aa-forum-search-result-inner{align-items:flex-start;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-search-results-total-number{font-size:2rem;font-weight:bolder;margin-bottom:2rem}.aa-forum .aa-forum-search-result-counter{font-size:3rem;font-weight:bolder;margin-right:1rem;min-width:50px;padding:1rem}.aa-forum .aa-forum-search-result-details{width:100%}.aa-forum .aa-forum-search-term-highlight{color:rgb(255 114 0)!important;font-size:1.1em;font-weight:700}.aa-forum .card-aa-forum-personal-messages-item{padding:1rem;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-personal-messages-item:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-personal-messages-item-header{border-bottom:1px solid rgb(236 240 241);font-weight:700}.aa-forum .card-aa-forum-personal-messages-item-unread{font-weight:700}.aa-forum .aa-forum-personal-messages-message .card{margin-top:2rem}.aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active){background-color:var(--bs-secondary-bg-subtle)}.aa-forum li.aa-forum-messages-sidebar-menu-item>a.active{color:rgb(var(--bs-primary-rgb))}.aa-forum .aa-forum-lightbox-modal{align-items:center;display:flex!important;justify-content:center;z-index:-1}.aa-forum .aa-forum-lightbox-modal .modal-dialog{display:inline-block;height:auto!important;max-height:95%;max-width:95%;width:auto!important}.aa-forum .aa-forum-lightbox-modal.fade.in{z-index:1050}.aa-forum .btn-aa-forum-topic-moderation{background:0 0}.aa-forum .btn-aa-forum-topic-moderation.focus,.aa-forum .btn-aa-forum-topic-moderation:focus,.aa-forum .btn-aa-forum-topic-moderation:hover{color:inherit;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.aa-forum .btn-aa-forum-delete{color:rgb(255 0 0)}.aa-forum .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-forum .SumoSelect{color:rgb(54 54 54);display:block}.aa-forum .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-forum .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}.aa-forum .select2-container--bootstrap-5{max-width:100%!important}.aa-forum .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-forum .ck-editor__editable{color:initial}.aa-forum .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}}@media all and (min-width:768px){.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name,.aa-forum .card-aa-forum-category .aa-forum-board-name{width:60%}.aa-forum .card-aa-forum-category .aa-forum-board-stats{text-align:center;width:15%}.aa-forum .card-aa-forum-category .aa-forum-board-last-post{width:25%}.aa-forum .aa-forum-legend{display:flex}.aa-forum .aa-forum-message{align-items:flex-start;display:flex;flex-wrap:nowrap}.aa-forum .aa-forum-message-author figure{width:auto}.aa-forum .aa-forum-message-author{min-width:150px;width:150px}.aa-forum .aa-forum-message-wrapper{width:100%}}@media all and (min-width:992px){.aa-forum .card-aa-forum-personal-messages-item,.aa-forum .card-aa-forum-personal-messages-item-header{align-items:center;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-personal-message-date,.aa-forum .aa-forum-personal-message-recipient,.aa-forum .aa-forum-personal-message-sender{min-width:200px}.aa-forum .aa-forum-personal-message-subject{width:100%}}@media all{.aa-forum figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-forum figure.media .oembed-video>iframe{height:100%;left:0;position:absolute;top:0;width:100%}}
+:root{--bg-hover-transition:background-color 0.25s linear}@media all{.aa-forum .aa-forum-svg-wrapper{height:0;width:0}.aa-forum .aa-forum-body #aa-forum-form-search-results .input-group{margin-bottom:1rem}.aa-forum .aa-forum-ui-placeholder{outline:1px dashed rgb(0 0 0)}.aa-forum .boards-sortable,.aa-forum .categories-sortable{list-style-type:none}.aa-forum .boards-sortable>li:first-child{margin-top:1rem}.aa-forum [data-bs-toggle=collapse].collapsed .if-expanded{display:none}.aa-forum [data-bs-toggle=collapse]:not(.collapsed) .if-collapsed{display:none}.aa-forum .category-sortable{cursor:move}.aa-forum .aa-forum-breadcrumb ul{list-style-type:none;padding:0}.aa-forum .aa-forum-breadcrumb ul li{display:inline}.aa-forum .aa-forum-breadcrumb ul li:first-child{padding-left:0}.aa-forum .card-aa-forum-category .aa-forum-board{flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-category .aa-forum-board:last-child{margin-bottom:0}.aa-forum .card-aa-forum-category .aa-forum-board:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-category .aa-forum-board-image svg{height:65px;margin-top:-1rem;width:65px}.aa-forum .card-aa-forum-category .aa-forum-board-name{width:100%}.aa-forum .aa-forum-board-name p:last-child{margin:0}.aa-forum .aa-forum-board-group-restrictions{list-style-type:none;margin:0;padding:0}.aa-forum .aa-forum-board-last-post .img-last-post-avatar{float:left;height:55px;margin-right:1rem;width:55px}.aa-forum .aa-forum-board-last-post .last-post-information{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;word-wrap:normal}.aa-forum .aa-forum-legend>span{display:flex;margin-right:5rem}.aa-forum .aa-forum-legend .aa-forum-legend-image svg{height:30px;width:30px}.aa-forum .aa-forum-legend .aa-forum-legend-text{display:inline-block}.aa-forum .aa-forum-legend span:last-child{margin-right:0}.aa-forum .aa-forum-topic-row .aa-forum-topic{align-content:center;align-items:center;display:flex;flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child,.aa-forum .aa-forum-topic-row:last-child .aa-forum-topic{margin-bottom:0}.aa-forum .aa-forum-topic-row .aa-forum-topic:hover{background:rgb(0 0 0/5%)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image{width:40px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg{height:35px;margin-top:-1rem;width:35px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name{width:auto}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats{text-align:center;width:15%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post{width:25%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions{width:70px}.aa-forum .aa-forum-topic-locked{background-color:rgb(185 199 219/25%)}.aa-forum .aa-forum-topic-sticky{background-color:rgb(255 220 104/25%)}.aa-forum .label-aa-forum-topic-new-message{font-size:55%}.aa-forum .label-aa-forum-child-board-new-message{font-size:55%;margin-left:.25rem;padding:.3em .6em;vertical-align:middle}.aa-forum .aa-forum-message-author .img-author-avatar{max-width:100%}.aa-forum .aa-forum-message-wrapper{width:auto}.aa-forum .aa-forum-message-body{border-top:1px solid rgb(236 240 241)}.aa-forum .aa-forum-message-body-author-signature{border-top:1px solid rgb(236 240 241);margin-top:3em}.aa-forum .aa-forum-message-body-last-edited{margin-top:5rem}.aa-forum .aa-forum-message-body img{height:auto!important;max-width:100%}.aa-forum .aa-forum-search-result-inner{align-items:flex-start;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-search-results-total-number{font-size:2rem;font-weight:bolder;margin-bottom:2rem}.aa-forum .aa-forum-search-result-counter{font-size:3rem;font-weight:bolder;margin-right:1rem;min-width:50px;padding:1rem}.aa-forum .aa-forum-search-result-details{width:100%}.aa-forum .aa-forum-search-term-highlight{color:rgb(255 114 0)!important;font-size:1.1em;font-weight:700}.aa-forum .card-aa-forum-personal-messages-item{padding:1rem;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-personal-messages-item:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-personal-messages-item-header{border-bottom:1px solid rgb(236 240 241);font-weight:700}.aa-forum .card-aa-forum-personal-messages-item-unread{font-weight:700}.aa-forum .aa-forum-personal-messages-message .card{margin-top:2rem}.aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active){background-color:var(--bs-secondary-bg-subtle)}.aa-forum li.aa-forum-messages-sidebar-menu-item>a.active{color:rgb(var(--bs-primary-rgb))}.aa-forum .aa-forum-lightbox-modal{align-items:center;display:flex!important;justify-content:center;z-index:-1}.aa-forum .aa-forum-lightbox-modal .modal-dialog{display:inline-block;height:auto!important;max-height:95%;max-width:95%;width:auto!important}.aa-forum .aa-forum-lightbox-modal.fade.in{z-index:1050}.aa-forum .btn-aa-forum-topic-moderation{background:0 0}.aa-forum .btn-aa-forum-topic-moderation.focus,.aa-forum .btn-aa-forum-topic-moderation:focus,.aa-forum .btn-aa-forum-topic-moderation:hover{color:inherit;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.aa-forum .btn-aa-forum-delete{color:rgb(255 0 0)}.aa-forum .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-forum .SumoSelect{color:rgb(54 54 54);display:block}.aa-forum .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-forum .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}.aa-forum .select2-container--bootstrap-5{max-width:100%!important}.aa-forum .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-forum .ck-editor__editable{color:initial}.aa-forum .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}.aa-forum .ck-content .image{margin:.9em 0}.aa-forum .ck-content .image-style-align-center{margin-left:auto;margin-right:auto}.aa-forum .ck-content .image-style-align-left{margin-right:var(--ck-image-style-spacing)}.aa-forum .ck-content .image-style-align-right,.aa-forum .ck-content .image-style-side{margin-left:var(--ck-image-style-spacing)}}@media all and (min-width:768px){.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name,.aa-forum .card-aa-forum-category .aa-forum-board-name{width:60%}.aa-forum .card-aa-forum-category .aa-forum-board-stats{text-align:center;width:15%}.aa-forum .card-aa-forum-category .aa-forum-board-last-post{width:25%}.aa-forum .aa-forum-legend{display:flex}.aa-forum .aa-forum-message{align-items:flex-start;display:flex;flex-wrap:nowrap}.aa-forum .aa-forum-message-author figure{width:auto}.aa-forum .aa-forum-message-author{min-width:150px;width:150px}.aa-forum .aa-forum-message-wrapper{width:100%}}@media all and (min-width:992px){.aa-forum .card-aa-forum-personal-messages-item,.aa-forum .card-aa-forum-personal-messages-item-header{align-items:center;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-personal-message-date,.aa-forum .aa-forum-personal-message-recipient,.aa-forum .aa-forum-personal-message-sender{min-width:200px}.aa-forum .aa-forum-personal-message-subject{width:100%}}@media all{.aa-forum figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-forum figure.media .oembed-video>iframe{height:100%;left:0;position:absolute;top:0;width:100%}}
 /*# sourceMappingURL=aa-forum.min.css.map */
```

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map` & `aa_forum-2.1.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'mappings'": "'AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CA […]*

```diff
@@ -1,12 +1,12 @@
 {
     "file": "aa-forum.css",
-    "mappings": "AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CACI,oB,CAGJ,0C,CACI,c,CAOJ,6C,CACI,oB,CACA,kB,CACA,Y,CACA,kB,CACA,qC,CAyBJ,+E,CAtBA,wD,CACI,e,CAGJ,mD,CACI,wB,CAGJ,mE,CACI,U,CAGJ,uE,CACI,W,CACA,gB,CACA,U,CAGJ,kE,CACI,U,CAOJ,mE,CACI,iB,CACA,S,CAGJ,uE,CACI,S,CAGJ,qE,CACI,U,CAGJ,gC,CACI,qC,CAGJ,gC,CACI,qC,CAGJ,2C,CACI,a,CAGJ,iD,CACI,a,CACA,kB,CACA,iB,CACA,qB,CAOJ,qD,CACI,c,CAGJ,mC,CACI,U,CAGJ,gC,CACI,qC,CAGJ,iD,CACI,qC,CACA,c,CAGJ,4C,CACI,e,CAGJ,oC,CACI,qB,CACA,c,CAOJ,uC,CACI,sB,CACA,Y,CACA,oB,CACA,mC,CAGJ,+C,CACI,c,CACA,kB,CACA,kB,CAGJ,yC,CACI,c,CACA,kB,CACA,iB,CACA,c,CACA,Y,CAGJ,yC,CACI,U,CAGJ,yC,CACI,8B,CACA,e,CACA,e,CAOJ,+C,CACI,Y,CACA,qC,CAGJ,qD,CACI,wB,CAGJ,sD,CACI,wC,CACA,e,CAGJ,sD,CACI,e,CAGJ,mD,CACI,e,CAGJ,qDAAqD,S,CACjD,8C,CAGJ,yD,CACI,gC,CAOJ,kC,CACI,kB,CACA,sB,CACA,sB,CACA,U,CAGJ,gD,CACI,oB,CACA,qB,CACA,c,CACA,a,CACA,oB,CAGJ,0C,CACI,Y,CAOJ,wC,CACI,c,CAGJ,8C,CACA,8C,CACA,8C,CACI,a,CACA,yC,CACA,mB,CAGJ,8B,CACI,kB,CAOJ,uB,CACI,qC,CACA,W,CAGJ,qB,CACI,mB,CACA,a,CAGJ,0C,CACI,qB,CAGJ,mD,CACI,4B,CACA,mB,CACA,S,CAOJ,yC,CACI,wB,CAOJ,6B,CACI,0C,CAGJ,8B,CACI,a,CAGJ,wB,CACI,yC,CAEA,qBAYR,A,iCAsBI,kE,CArBA,sD,CACI,S,CAGJ,uD,CACI,iB,CACA,S,CAGJ,2D,CACI,S,CAGJ,0B,CACI,Y,CAeJ,2B,CACI,sB,CACA,Y,CACA,gB,CAGJ,yC,CACI,U,CAGJ,kC,CACI,e,CACA,W,CAGJ,mC,CACI,YAYR,A,iCAEI,+C,CADA,sD,CAEI,kB,CACA,Y,CACA,oB,CACA,mC,CAGJ,yC,CAKA,8C,CADA,2C,CAHI,e,CAQJ,4C,CACI,YAMR,A,WACI,oC,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,2C,CACI,W,CACA,M,CACA,iB,CACA,K,CACA,Y",
+    "mappings": "AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CACI,oB,CAGJ,0C,CACI,c,CAOJ,6C,CACI,oB,CACA,kB,CACA,Y,CACA,kB,CACA,qC,CAyBJ,+E,CAtBA,wD,CACI,e,CAGJ,mD,CACI,wB,CAGJ,mE,CACI,U,CAGJ,uE,CACI,W,CACA,gB,CACA,U,CAGJ,kE,CACI,U,CAOJ,mE,CACI,iB,CACA,S,CAGJ,uE,CACI,S,CAGJ,qE,CACI,U,CAGJ,gC,CACI,qC,CAGJ,gC,CACI,qC,CAGJ,2C,CACI,a,CAGJ,iD,CACI,a,CACA,kB,CACA,iB,CACA,qB,CAOJ,qD,CACI,c,CAGJ,mC,CACI,U,CAGJ,gC,CACI,qC,CAGJ,iD,CACI,qC,CACA,c,CAGJ,4C,CACI,e,CAGJ,oC,CACI,qB,CACA,c,CAOJ,uC,CACI,sB,CACA,Y,CACA,oB,CACA,mC,CAGJ,+C,CACI,c,CACA,kB,CACA,kB,CAGJ,yC,CACI,c,CACA,kB,CACA,iB,CACA,c,CACA,Y,CAGJ,yC,CACI,U,CAGJ,yC,CACI,8B,CACA,e,CACA,e,CAOJ,+C,CACI,Y,CACA,qC,CAGJ,qD,CACI,wB,CAGJ,sD,CACI,wC,CACA,e,CAGJ,sD,CACI,e,CAGJ,mD,CACI,e,CAGJ,qDAAqD,S,CACjD,8C,CAGJ,yD,CACI,gC,CAOJ,kC,CACI,kB,CACA,sB,CACA,sB,CACA,U,CAGJ,gD,CACI,oB,CACA,qB,CACA,c,CACA,a,CACA,oB,CAGJ,0C,CACI,Y,CAOJ,wC,CACI,c,CAGJ,8C,CACA,8C,CACA,8C,CACI,a,CACA,yC,CACA,mB,CAGJ,8B,CACI,kB,CAOJ,uB,CACI,qC,CACA,W,CAGJ,qB,CACI,mB,CACA,a,CAGJ,0C,CACI,qB,CAGJ,mD,CACI,4B,CACA,mB,CACA,S,CAOJ,yC,CACI,wB,CAOJ,6B,CACI,0C,CAGJ,8B,CACI,a,CAGJ,wB,CACI,yC,CAEA,mB,CAKJ,4B,CACI,a,CAGJ,+C,CACI,gB,CACA,iB,CAGJ,6C,CACI,0C,CAGJ,8C,CAIA,uC,CAHI,2CAgBR,A,iCAsBI,kE,CArBA,sD,CACI,S,CAGJ,uD,CACI,iB,CACA,S,CAGJ,2D,CACI,S,CAGJ,0B,CACI,Y,CAeJ,2B,CACI,sB,CACA,Y,CACA,gB,CAGJ,yC,CACI,U,CAGJ,kC,CACI,e,CACA,W,CAGJ,mC,CACI,YAYR,A,iCAEI,+C,CADA,sD,CAEI,kB,CACA,Y,CACA,oB,CACA,mC,CAGJ,yC,CAKA,8C,CADA,2C,CAHI,e,CAQJ,4C,CACI,YAMR,A,WACI,oC,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,2C,CACI,W,CACA,M,CACA,iB,CACA,K,CACA,Y",
     "names": [],
     "sources": [
         "aa-forum.css"
     ],
     "sourcesContent": [
-        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
+        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n\n    /* Image alignment\n    --------------------------------------------------------------------------------- */\n    .aa-forum .ck-content .image {\n        margin: 0.9em 0;\n    }\n\n    .aa-forum .ck-content .image-style-align-center {\n        margin-left: auto;\n        margin-right: auto;\n    }\n\n    .aa-forum .ck-content .image-style-align-left {\n        margin-right: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-align-right {\n        margin-left: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-side {\n        margin-left: var(--ck-image-style-spacing);\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,39 @@
 "use strict";
-const aaForumDashboardWidgets = document.getElementById("aa-forum-dashboard-widgets"),
-    aaForumUnreadTopicsWidget = document.getElementById("aa-forum-dashboard-widget-unread-topics");
-if (aaForumUnreadTopicsWidget) {
-    const a = aaForumUnreadTopicsWidget.querySelector(".aa-forum-dashboard-widget-unread-topics-content");
-    fetch(aaForumDashboardWidgetsSettings.unreadTopics.ajaxUrl).then(o => {
-        if (o.ok) return o.text();
+const mergeOptions = (...e) => {
+        const s = e => e && "object" == typeof e;
+        return e.reduce((o, r) => (Object.keys(r).forEach(e => {
+            const a = o[e],
+                t = r[e];
+            Array.isArray(a) && Array.isArray(t) ? o[e] = [...new Set([...t, ...a])] : s(a) && s(t) ? o[e] = mergeOptions(a, t) : o[e] = t
+        }), o), {})
+    },
+    aaForumDashboardWidgetsDefaults = {
+        wrapper: {
+            element: document.getElementById("aa-forum-dashboard-widgets")
+        },
+        unreadTopicsWidget: {
+            element: document.getElementById("aa-forum-dashboard-widget-unread-topics"),
+            contentElementClass: "aa-forum-dashboard-widget-unread-topics-content"
+        }
+    },
+    aaForumDashboardWidgets = mergeOptions(aaForumDashboardWidgetsDefaults, aaForumDashboardWidgetsSettings);
+if (null !== aaForumDashboardWidgets.unreadTopicsWidget.element) {
+    const i = aaForumDashboardWidgets.unreadTopicsWidget.element.querySelector(`.${aaForumDashboardWidgets.unreadTopicsWidget.contentElementClass}`);
+    fetch(aaForumDashboardWidgetsSettings.unreadTopicsWidget.ajaxUrl).then(e => {
+        if (e.ok) return e.text();
         throw new Error("Something went wrong")
-    }).then(o => {
-        if ("" !== o) {
-            a.innerHTML = o;
-            new bootstrap.Collapse(aaForumDashboardWidgets, {
+    }).then(e => {
+        if ("" !== e) {
+            i.innerHTML = e;
+            new bootstrap.Collapse(aaForumDashboardWidgets.wrapper.element, {
                 show: !0
-            }), new bootstrap.Collapse(aaForumUnreadTopicsWidget, {
+            }), new bootstrap.Collapse(aaForumDashboardWidgets.unreadTopicsWidget.element, {
                 show: !0
             });
-            [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-forum"]')).map(o => new bootstrap.Tooltip(o))
+            [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-forum"]')).map(e => new bootstrap.Tooltip(e))
         }
-    }).catch(o => {
-        console.log(o)
+    }).catch(e => {
+        console.log(e)
     })
 }
 //# sourceMappingURL=aa-forum-desktop-widgets.min.js.map
```

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map` & `aa_forum-2.1.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_forum-2.1.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/base.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/base.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/breadcrumb.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/categories.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/categories.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/new-category.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/new-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/profile/form.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/profile/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/pagination.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/search/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-form.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/partials/search/search-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/board.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/index.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/new-topic.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/new-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/topic.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/profile/index.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/profile/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/search/results.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/search/results.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html` & `aa_forum-2.1.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
         <div class="aa-forum-svg-wrapper">
             {% include "aa_forum/bundles/svg/aa-forum-icons.svg" %}
         </div>
 
         <script>
             const aaForumDashboardWidgetsSettings = {
-                unreadPersonalMessages: {
-                },
-                unreadTopics: {
+                unreadTopicsWidget: {
                     ajaxUrl: '{% url "aa_forum:widgets_ajax_unread_topics" %}',
                 },
             };
         </script>
 
         {% include "aa_forum/bundles/aa-forum-css.html" %}
         {% include "aa_forum/bundles/aa-forum-dashboard-widgets-js.html" %}
```

### Comparing `aa_forum-2.1.0/aa_forum/templatetags/aa_forum.py` & `aa_forum-2.1.1/aa_forum/templatetags/aa_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_app_settings.py` & `aa_forum-2.1.1/aa_forum/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_auth_hooks.py` & `aa_forum-2.1.1/aa_forum/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_helpers.py` & `aa_forum-2.1.1/aa_forum/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_integration.py` & `aa_forum-2.1.1/aa_forum/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_managers.py` & `aa_forum-2.1.1/aa_forum/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_models.py` & `aa_forum-2.1.1/aa_forum/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_signals.py` & `aa_forum-2.1.1/aa_forum/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_templatetags.py` & `aa_forum-2.1.1/aa_forum/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_views_admin.py` & `aa_forum-2.1.1/aa_forum/tests/test_views_admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/test_views_forum.py` & `aa_forum-2.1.1/aa_forum/tests/test_views_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/tests/utils.py` & `aa_forum-2.1.1/aa_forum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/admin.py` & `aa_forum-2.1.1/aa_forum/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/forum.py` & `aa_forum-2.1.1/aa_forum/views/forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/personal_messages.py` & `aa_forum-2.1.1/aa_forum/views/personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/profile.py` & `aa_forum-2.1.1/aa_forum/views/profile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/search.py` & `aa_forum-2.1.1/aa_forum/views/search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/aa_forum/views/widgets.py` & `aa_forum-2.1.1/aa_forum/views/widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/LICENSE` & `aa_forum-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/README.md` & `aa_forum-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/pyproject.toml` & `aa_forum-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_forum-2.1.0/PKG-INFO` & `aa_forum-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-forum
-Version: 2.1.0
+Version: 2.1.1
 Summary: Simple forum for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-forum/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-forum/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-forum
 Project-URL: Source, https://github.com/ppfeufer/aa-forum.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-forum/issues
```

