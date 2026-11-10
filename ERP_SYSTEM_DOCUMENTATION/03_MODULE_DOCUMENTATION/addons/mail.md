# Module: mail

- **Module ID:** MOD-351
- **Path:** `addons/mail`
- **Manifest:** `addons/mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Chat, mail gateway and private channels



Chat, mail gateway and private channel.
=======================================

Communicate with your colleagues/customers/guest within Odoo.

Discuss/Chat
------------
User-friendly "Discuss" features that allows one 2 one or group communication
(text chat/voice call/video call), invite guests and share documents with
them, all real-time.

Mail gateway
------------
Sending information and documents made simplified. You can send emails
from Odoo itself, and that too with great possibilities. For example,
design a beautiful email template for the invoices, and use the same
for all your customers, no need to do the same exercise every time.

Chatter
-------
Do all the contextual conversation on a document. For example on an
applicant, directly post an update to send email to the applicant,
schedule the next interview call, attach the contract, add HR officer
to the follower list to notify them for important events(with help of
subtypes),...


Retrieve incoming email on POP/IMAP servers.
============================================
Enter the parameters of your POP/IMAP account(s), and any incoming emails on
these accounts will be automatically downloaded into your Odoo system. All
POP3/IMAP-compatible servers are supported, included those that require an
encrypted SSL/TLS connection.
This can be used to easily create email-based workflows for many email-enabled Odoo documents, such as:

* CRM Leads/Opportunities
* CRM Claims
* Project Issues
* Project Tasks
* Human Resource Recruitment (Applicants)

Just install the relevant application, and you can assign any of these document
types (Leads, Project Issues) to your incoming email accounts. New emails will
automatically spawn new documents of the chosen type, so it's a snap to create a
mailbox-to-Odoo integration. Even better: these documents directly act as mini
conversations synchronized by email. You can reply from within Odoo, and the
answers will automatically be collected when they come back, and attached to the
same *conversation* document.
For more specific needs, you may also assign custom-defined actions
(technically: Server Actions) to be triggered for each incoming mail.
    

Declared dependencies: `base`, `base_setup`, `bus`, `web_tour`, `html_editor`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 201 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 87 | Files under `models/` or `models.py`. |
| Controller-path Python files | 26 | Files under `controllers/` or `controllers.py`. |
| XML files | 271 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 688 | Client behavior/assets. |
| Tests | 66 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 20 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "base_setup",
    "bus",
    "web_tour",
    "html_editor"
  ],
  "data": [
    "data/mail_groups.xml",
    "wizard/mail_activity_schedule_views.xml",
    "wizard/mail_blacklist_remove_views.xml",
    "wizard/mail_compose_message_views.xml",
    "wizard/mail_template_preview_views.xml",
    "wizard/mail_followers_edit_views.xml",
    "wizard/mail_template_reset_views.xml",
    "views/fetchmail_views.xml",
    "views/ir_access_views.xml",
    "views/ir_cron_views.xml",
    "views/ir_filters_views.xml",
    "views/ir_mail_server_views.xml",
    "views/ir_ui_view_views.xml",
    "views/mail_message_subtype_views.xml",
    "views/mail_notification_views.xml",
    "views/mail_message_views.xml",
    "views/mail_message_schedule_views.xml",
    "views/mail_mail_views.xml",
    "views/mail_followers_views.xml",
    "views/mail_ice_server_views.xml",
    "views/discuss_category_views.xml",
    "views/discuss_channel_member_views.xml",
    "views/discuss_channel_rtc_session_views.xml",
    "views/mail_link_preview_views.xml",
    "views/discuss/discuss_gif_favorite_views.xml",
    "views/discuss_channel_views.xml",
    "views/mail_canned_response_views.xml",
    "views/res_role_views.xml",
    "views/mail_activity_views.xml",
    "views/mail_activity_plan_views.xml",
    "views/mail_activity_plan_template_views.xml",
    "views/res_config_settings_views.xml",
    "data/mail_templates_chatter.xml",
    "data/ir_config_parameter_data.xml",
    "data/res_partner_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_templates_email_layouts.xml",
    "data/mail_templates_mailgateway.xml",
    "data/discuss_channel_data.xml",
    "data/mail_activity_type_data.xml",
    "data/security_notifications_templates.xml",
    "data/ir_cron_data.xml",
    "data/ir_actions_data.xml",
    "views/discuss_public_templates.xml",
    "views/mail_alias_domain_views.xml",
    "views/mail_alias_views.xml",
    "views/mail_attachment_views.xml",
    "views/mail_gateway_allowed_views.xml",
    "views/mail_guest_views.xml",
    "views/mail_message_reaction_views.xml",
    "views/mail_templates_public.xml",
    "views/res_users_views.xml",
    "views/res_users_settings_views.xml",
    "views/mail_template_views.xml",
    "views/ir_actions_server_views.xml",
    "views/ir_model_views.xml",
    "views/res_partner_views.xml",
    "views/mail_blacklist_views.xml",
    "views/mail_menus.xml",
    "views/discuss/discuss_call_history_views.xml",
    "views/res_company_views.xml",
    "views/mail_scheduled_message_views.xml",
    "data/mail_canned_response_data.xml",
    "data/mail_templates_invite.xml",
    "data/web_tour_tour.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/res_role_demo.xml",
    "demo/mail_activity_demo.xml",
    "demo/discuss_channel_demo.xml",
    "demo/discuss_channel_chat_demo.xml",
    "demo/discuss/public_channel_demo.xml",
    "demo/discuss/readonly_channel_demo.xml",
    "demo/discuss/call_debrief_discuss_demo.xml",
    "demo/mail_poll_demo.xml",
    "demo/mail_canned_response_demo.xml"
  ],
  "assets": {
    "web._assets_primary_variables": [
      "mail/static/src/**/primary_variables.scss"
    ],
    "web.assets_backend": [
      "mail/static/src/scss/variables/derived_variables.scss",
      "mail/static/src/scss/*.scss",
      "mail/static/lib/idb-keyval/idb-keyval.js",
      "mail/static/lib/selfie_segmentation/selfie_segmentation.js",
      "mail/static/src/js/**/*",
      "mail/static/src/model/**/*",
      "mail/static/src/core/common/core.scss",
      "mail/static/src/core/common/**/*",
      "mail/static/src/core/public_web/**/*",
      "mail/static/src/core/web_portal_project/**/*",
      "mail/static/src/core/web/**/*",
      "mail/static/src/**/common/**/*",
      "mail/static/src/**/public_web/**/*",
      "mail/static/src/**/web_portal_project/**/*",
      "mail/static/src/**/web/**/*",
      [
        "remove",
        "mail/static/src/**/*.dark.scss"
      ],
      [
        "remove",
        "mail/static/src/discuss/**/*"
      ],
      "mail/static/src/discuss/core/common/**/*",
      "mail/static/src/discuss/core/public_web/**/*",
      "mail/static/src/discuss/core/web/**/*",
      "mail/static/src/discuss/**/common/**/*",
      "mail/static/src/discuss/**/public_web/**/*",
      "mail/static/src/discuss/**/web/**/*",
      [
        "remove",
        "mail/static/src/discuss/**/*.dark.scss"
      ],
      "mail/static/src/views/fields/**/*",
      [
        "remove",
        "mail/static/src/views/web/activity/**"
      ],
      "mail/static/src/convert_inline/**/*"
    ],
    "web.assets_backend_lazy": [
      "mail/static/src/views/web/activity/**"
    ],
    "web.assets_web_dark": [
      "mail/static/src/core/common/core.dark.scss",
      "mail/static/src/**/*.dark.scss"
    ],
    "web.assets_frontend": [
      "mail/static/src/html_editor/common/state_file_model_patch.js",
      "mail/static/src/utils/common/format.js",
      "mail/static/src/utils/common/html.js"
    ],
    "web.assets_web_print": [
      "mail/static/src/scss/discuss_print.scss"
    ],
    "mail.assets_discuss_public_test_tours": [
      [
        "include",
        "web_tour.assets"
      ],
      "mail/static/tests/tours/discuss_channel_public_tour.js",
      "mail/static/tests/tours/discuss_channel_as_guest_tour.js",
      "mail/static/tests/tours/discuss_channel_call_action.js",
      "mail/static/tests/tours/discuss_channel_call_public_tour.js",
      "mail/static/tests/tours/discuss_sidebar_in_public_page_tour.js",
      "mail/static/tests/tours/discuss_channel_meeting_view_tour.js",
      "mail/static/tests/tours/discuss_channel_welcome_page_tour.js"
    ],
    "web.assets_unit_tests": [
      "mail/static/tests/**/*",
      [
        "remove",
        "mail/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "mail/static/tests/tours/**/*"
    ],
    "mail.assets_odoo_sfu": [
      "mail/static/lib/odoo_sfu/odoo_sfu.js"
    ],
    "mail.assets_lamejs": [
      "mail/static/lib/lame/lame.js"
    ],
    "mail.assets_message_email": [
      [
        "include",
        "web.icons_fonts"
      ]
    ],
    "mail.assets_public": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      "web/static/src/scss/bootstrap_overridden.scss",
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/scss/animation.scss",
      "web/static/src/webclient/webclient.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      [
        "include",
        "web._assets_core"
      ],
      "web/static/src/views/fields/formatters.js",
      "web/static/src/views/fields/file_handler.*",
      "bus/static/src/*.js",
      "bus/static/src/services/**/*.js",
      "bus/static/src/workers/*.js",
      [
        "remove",
        "bus/static/src/workers/bus_worker_script.js"
      ],
      [
        "include",
        "html_editor.assets_editor"
      ],
      "mail/static/src/model/**/*",
      "mail/static/src/core/common/core.scss",
      "mail/static/src/core/common/**/*",
      "mail/static/src/core/public_web/**/*",
      "mail/static/src/**/common/**/*",
      "mail/static/src/**/public_web/**/*",
      "mail/static/src/**/public/**/*",
      "mail/static/lib/selfie_segmentation/selfie_segmentation.js",
      [
        "remove",
        "mail/static/src/**/*.dark.scss"
      ],
      [
        "remove",
        "mail/static/src/discuss/**/*"
      ],
      "mail/static/src/discuss/core/common/**/*",
      "mail/static/src/discuss/core/public_web/**/*",
      "mail/static/src/discuss/core/public/**/*",
      "mail/static/src/discuss/**/common/**/*",
      "mail/static/src/discuss/**/public_web/**/*",
      "mail/static/src/discuss/**/public/**/*",
      [
        "remove",
        "mail/static/src/discuss/**/*.dark.scss"
      ],
      [
        "remove",
        "web/static/src/**/*.dark.scss"
      ]
    ],
    "mail.assets_markdown": [
      "mail/static/src/markdown_assets/mail_markdown_assets.scss"
    ],
    "im_livechat.assets_embed_core": [
      [
        "include",
        "html_editor.assets_editor"
      ],
      "mail/static/src/model/**/*",
      "mail/static/src/core/common/core.scss",
      "mail/static/src/core/common/**/*",
      "mail/static/src/**/common/**/*",
      [
        "remove",
        "mail/static/src/**/*.dark.scss"
      ]
    ],
    "im_livechat.assets_embed_external": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      "web/static/src/scss/bootstrap_overridden.scss",
      "web/static/src/scss/ui.scss",
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/scss/animation.scss",
      "web/static/src/webclient/webclient.scss",
      [
        "include",
        "web._assets_core"
      ],
      "web/static/src/views/fields/formatters.js",
      "web/static/src/views/fields/file_handler.*",
      "web/static/src/scss/mimetypes.scss",
      [
        "remove",
        "web/static/src/**/*.dark.scss"
      ],
      "bus/static/src/*.js",
      "bus/static/src/services/**/*.js",
      "bus/static/src/workers/*.js",
      [
        "remove",
        "bus/static/src/workers/bus_worker_script.js"
      ],
      [
        "remove",
        "bus/static/src/services/assets_watchdog_plugin.js"
      ],
      [
        "remove",
        "bus/static/src/simple_notification_plugin.js"
      ],
      [
        "include",
        "im_livechat.assets_embed_core"
      ]
    ],
    "im_livechat.assets_embed_cors": [
      [
        "include",
        "im_livechat.assets_embed_external"
      ],
      [
        "remove",
        "mail/static/src/core/common/out_of_focus_service_patch.js"
      ],
      [
        "remove",
        "web/static/src/core/browser/title_plugin.js"
      ]
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      [
        "include",
        "web.assets_unit_tests_setup"
      ],
      "web/static/tests/web_test_helpers.js",
      "bus/static/tests/bus_test_helpers.js",
      "mail/static/tests/mail_test_helpers.js",
      "mail/static/tests/mail_test_helpers_contains.js",
      "bus/static/tests/mock_server/**/*",
      "mail/static/tests/mock_server/**/*",
      "bus/static/tests/mock_*.js"
    ]
  }
}
```

### Representative source files

- `addons/mail/README.md` (54 lines)
- `addons/mail/__init__.py` (10 lines)
- `addons/mail/__manifest__.py` (361 lines)
- `addons/mail/controllers/__init__.py` (21 lines)
- `addons/mail/controllers/attachment.py` (344 lines)
- `addons/mail/controllers/discuss/__init__.py` (10 lines)
- `addons/mail/controllers/discuss/channel.py` (372 lines)
- `addons/mail/controllers/discuss/gif.py` (122 lines)
- `addons/mail/controllers/discuss/messaging_menu.py` (184 lines)
- `addons/mail/controllers/discuss/public_page.py` (155 lines)
- `addons/mail/controllers/discuss/rtc.py` (269 lines)
- `addons/mail/controllers/discuss/search.py` (56 lines)
- `addons/mail/controllers/discuss/settings.py` (50 lines)
- `addons/mail/controllers/discuss/voice.py` (19 lines)
- `addons/mail/controllers/google_translate.py` (86 lines)
- `addons/mail/controllers/guest.py` (19 lines)
- `addons/mail/controllers/home.py` (13 lines)
- `addons/mail/controllers/im_status.py` (17 lines)
- `addons/mail/controllers/link_preview.py` (33 lines)
- `addons/mail/controllers/mail.py` (468 lines)
- `addons/mail/controllers/mailbox.py` (45 lines)
- `addons/mail/controllers/message_reaction.py` (31 lines)
- `addons/mail/controllers/messaging_menu.py` (119 lines)
- `addons/mail/controllers/poll.py` (113 lines)
- `addons/mail/controllers/store.py` (36 lines)
- `addons/mail/controllers/thread.py` (300 lines)
- `addons/mail/controllers/webclient.py` (236 lines)
- `addons/mail/controllers/webmanifest.py` (19 lines)
- `addons/mail/controllers/websocket.py` (25 lines)
- `addons/mail/data/discuss_channel_data.xml` (49 lines)
- `addons/mail/data/ir_actions_data.xml` (22 lines)
- `addons/mail/data/ir_config_parameter_data.xml` (13 lines)
- `addons/mail/data/ir_cron_data.xml` (106 lines)
- `addons/mail/data/mail_activity_type_data.xml` (48 lines)
- `addons/mail/data/mail_canned_response_data.xml` (12 lines)
- `addons/mail/data/mail_groups.xml` (29 lines)
- `addons/mail/data/mail_message_subtype_data.xml` (30 lines)
- `addons/mail/data/mail_templates_chatter.xml` (108 lines)
- `addons/mail/data/mail_templates_email_layouts.xml` (188 lines)
- `addons/mail/data/mail_templates_invite.xml` (39 lines)
- `addons/mail/data/mail_templates_mailgateway.xml` (59 lines)
- `addons/mail/data/neutralize.sql` (15 lines)
- `addons/mail/data/res_partner_data.xml` (14 lines)
- `addons/mail/data/security_notifications_templates.xml` (37 lines)
- `addons/mail/data/web_tour_tour.xml` (8 lines)
- `addons/mail/demo/discuss/call_debrief_discuss_demo.xml` (95 lines)
- `addons/mail/demo/discuss/fixtures/audio_opus_60s_long_3s_content.webm` (351 lines)
- `addons/mail/demo/discuss/fixtures/audio_physics_0s_20s_16k.mp3` (419 lines)
- `addons/mail/demo/discuss/fixtures/audio_physics_40s_60s_16k.mp3` (443 lines)
- `addons/mail/demo/discuss/fixtures/video_60s_long_3s_content_av1_opus.webm` (887 lines)
- `addons/mail/demo/discuss/public_channel_demo.xml` (88 lines)
- `addons/mail/demo/discuss/readonly_channel_demo.xml` (46 lines)
- `addons/mail/demo/discuss_channel_chat_demo.xml` (32 lines)
- `addons/mail/demo/discuss_channel_demo.xml` (263 lines)
- `addons/mail/demo/mail_activity_demo.xml` (17 lines)
- `addons/mail/demo/mail_canned_response_demo.xml` (12 lines)
- `addons/mail/demo/mail_poll_demo.xml` (38 lines)
- `addons/mail/demo/res_role_demo.xml` (9 lines)
- `addons/mail/i18n/af.po` (15,916 lines)
- `addons/mail/i18n/am.po` (15,912 lines)
- `addons/mail/i18n/ar.po` (16,938 lines)
- `addons/mail/i18n/az.po` (16,571 lines)
- `addons/mail/i18n/bg.po` (16,672 lines)
- `addons/mail/i18n/bs.po` (16,562 lines)
- `addons/mail/i18n/ca.po` (16,773 lines)
- `addons/mail/i18n/cs.po` (16,962 lines)
- `addons/mail/i18n/da.po` (16,678 lines)
- `addons/mail/i18n/de.po` (17,489 lines)
- `addons/mail/i18n/el.po` (16,659 lines)
- `addons/mail/i18n/es.po` (17,122 lines)
- `addons/mail/i18n/es_419.po` (17,330 lines)
- `addons/mail/i18n/es_CL.po` (440 lines)
- `addons/mail/i18n/et.po` (16,764 lines)
- `addons/mail/i18n/eu.po` (15,915 lines)
- `addons/mail/i18n/fa.po` (16,815 lines)
- `addons/mail/i18n/fi.po` (17,145 lines)
- `addons/mail/i18n/fo.po` (15,915 lines)
- `addons/mail/i18n/fr.po` (17,270 lines)
- `addons/mail/i18n/fr_CA.po` (435 lines)
- `addons/mail/i18n/gl.po` (15,915 lines)
- `addons/mail/i18n/gu.po` (15,944 lines)
- `addons/mail/i18n/he.po` (16,584 lines)
- `addons/mail/i18n/hi.po` (16,532 lines)
- `addons/mail/i18n/hr.po` (16,619 lines)
- `addons/mail/i18n/hu.po` (16,600 lines)
- `addons/mail/i18n/id.po` (17,279 lines)
- `addons/mail/i18n/is.po` (15,952 lines)
- `addons/mail/i18n/it.po` (17,326 lines)
- `addons/mail/i18n/ja.po` (17,086 lines)
- `addons/mail/i18n/ka.po` (15,915 lines)
- `addons/mail/i18n/kab.po` (16,480 lines)
- `addons/mail/i18n/km.po` (15,931 lines)
- `addons/mail/i18n/ko.po` (16,879 lines)
- `addons/mail/i18n/ku.po` (16,484 lines)
- `addons/mail/i18n/lo.po` (16,930 lines)
- `addons/mail/i18n/lt.po` (16,662 lines)
- `addons/mail/i18n/lv.po` (16,598 lines)
- `addons/mail/i18n/mail.pot` (16,441 lines)
- `addons/mail/i18n/mk.po` (15,915 lines)
- `addons/mail/i18n/mn.po` (16,641 lines)
- `addons/mail/i18n/my.po` (16,508 lines)
- `addons/mail/i18n/nb.po` (16,568 lines)
- `addons/mail/i18n/nl.po` (17,366 lines)
- `addons/mail/i18n/pl.po` (17,169 lines)
- `addons/mail/i18n/pt.po` (16,994 lines)
- `addons/mail/i18n/pt_BR.po` (17,334 lines)
- `addons/mail/i18n/ro.po` (17,012 lines)
- `addons/mail/i18n/ru.po` (17,318 lines)
- `addons/mail/i18n/sk.po` (16,650 lines)
- `addons/mail/i18n/sl.po` (16,938 lines)
- `addons/mail/i18n/sq.po` (15,915 lines)
- `addons/mail/i18n/sr@latin.po` (16,539 lines)
- `addons/mail/i18n/sv.po` (16,971 lines)
- `addons/mail/i18n/th.po` (16,784 lines)
- `addons/mail/i18n/tr.po` (17,208 lines)
- `addons/mail/i18n/uk.po` (16,851 lines)
- `addons/mail/i18n/uz.po` (18,897 lines)
- `addons/mail/i18n/vi.po` (17,047 lines)
- `addons/mail/i18n/zh_CN.po` (16,856 lines)
- `addons/mail/i18n/zh_TW.po` (16,716 lines)
- `addons/mail/models/__init__.py` (81 lines)
- `addons/mail/models/discuss/__init__.py` (27 lines)
- `addons/mail/models/discuss/bus.py` (17 lines)
- `addons/mail/models/discuss/bus_listener_mixin.py` (36 lines)
- `addons/mail/models/discuss/bus_sync_mixin.py` (48 lines)
- `addons/mail/models/discuss/discuss_call_history.py` (87 lines)
- `addons/mail/models/discuss/discuss_category.py` (48 lines)
- `addons/mail/models/discuss/discuss_channel.py` (2,173 lines)
- `addons/mail/models/discuss/discuss_channel_last_interest_update.py` (28 lines)
- `addons/mail/models/discuss/discuss_channel_member.py` (852 lines)
- `addons/mail/models/discuss/discuss_channel_rtc_session.py` (173 lines)
- `addons/mail/models/discuss/discuss_gif_favorite.py` (15 lines)
- `addons/mail/models/discuss/discuss_voice_metadata.py` (12 lines)
- `addons/mail/models/discuss/ir_attachment.py` (33 lines)
- `addons/mail/models/discuss/ir_websocket.py` (57 lines)
- `addons/mail/models/discuss/mail_guest.py` (187 lines)
- `addons/mail/models/discuss/mail_message.py` (82 lines)
- `addons/mail/models/discuss/res_groups.py` (13 lines)
- `addons/mail/models/discuss/res_partner.py` (209 lines)
- `addons/mail/models/discuss/res_users.py` (80 lines)
- `addons/mail/models/discuss/res_users_settings.py` (67 lines)
- `addons/mail/models/discuss/res_users_settings_volumes.py` (55 lines)
- `addons/mail/models/fetchmail.py` (365 lines)
- `addons/mail/models/ir_access.py` (12 lines)
- `addons/mail/models/ir_action_act_window.py` (10 lines)
- `addons/mail/models/ir_actions_server.py` (470 lines)
- `addons/mail/models/ir_attachment.py` (131 lines)
- `addons/mail/models/ir_config_parameter.py` (129 lines)
- `addons/mail/models/ir_cron.py` (21 lines)
- `addons/mail/models/ir_http.py` (28 lines)
- `addons/mail/models/ir_mail_server.py` (106 lines)
- `addons/mail/models/ir_model.py` (112 lines)
- `addons/mail/models/ir_model_fields.py` (32 lines)
- `addons/mail/models/ir_qweb.py` (55 lines)
- `addons/mail/models/ir_ui_menu.py` (63 lines)
- `addons/mail/models/ir_ui_view.py` (15 lines)
- `addons/mail/models/ir_websocket.py` (100 lines)
- `addons/mail/models/kpi_provider.py` (43 lines)
- `addons/mail/models/mail_activity.py` (1,037 lines)
- `addons/mail/models/mail_activity_mixin.py` (519 lines)

Additional files not expanded here: 1284. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
