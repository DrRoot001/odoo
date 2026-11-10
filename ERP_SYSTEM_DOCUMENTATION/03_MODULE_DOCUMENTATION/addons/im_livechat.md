# Module: im_livechat

- **Module ID:** MOD-111
- **Path:** `addons/im_livechat`
- **Manifest:** `addons/im_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Chat with your website visitors


Live Chat Support
==========================

Allow to drop instant messaging widgets on any web page that will communicate
with the current server and dispatch visitors request amongst several live
chat operators.
Help your customers with this chat, and analyse their feedback.

        

Declared dependencies: `mail`, `digest`, `utm`, `phone_validation`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 70 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 22 | Files under `models/` or `models.py`. |
| Controller-path Python files | 20 | Files under `controllers/` or `controllers.py`. |
| XML files | 78 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 185 | Client behavior/assets. |
| Tests | 24 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 38 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "digest",
    "utm",
    "phone_validation"
  ],
  "data": [
    "security/im_livechat_channel_security.xml",
    "data/mail_templates.xml",
    "data/im_livechat_channel_data.xml",
    "data/im_livechat_chatbot_data.xml",
    "data/digest_data.xml",
    "data/utm_data.xml",
    "views/chatbot_script_answer_views.xml",
    "views/chatbot_script_step_views.xml",
    "views/chatbot_script_views.xml",
    "views/discuss_channel_views.xml",
    "views/res_partner_views.xml",
    "views/im_livechat_channel_views.xml",
    "views/im_livechat_channel_templates.xml",
    "views/im_livechat_chatbot_templates.xml",
    "views/im_livechat_channel_config_views.xml",
    "views/im_livechat_expertise_views.xml",
    "views/im_livechat_channel_member_history_views.xml",
    "views/res_users_views.xml",
    "views/digest_views.xml",
    "views/webclient_templates.xml",
    "report/im_livechat_report_channel_views.xml",
    "report/im_livechat_conversation_report.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/im_livechat_channel/im_livechat_channel.xml",
    "demo/im_livechat_channel/im_livechat_chatbot.xml",
    "demo/im_livechat_channel/im_livechat_chatbot_session_1.xml",
    "demo/im_livechat_channel/im_livechat_chatbot_session_2.xml",
    "demo/im_livechat_channel/im_livechat_chatbot_session_3.xml",
    "demo/im_livechat_channel/im_livechat_session_1.xml",
    "demo/im_livechat_channel/im_livechat_session_2.xml",
    "demo/im_livechat_channel/im_livechat_session_3.xml",
    "demo/im_livechat_channel/im_livechat_session_4.xml",
    "demo/im_livechat_channel/im_livechat_session_5.xml",
    "demo/im_livechat_channel/im_livechat_session_6.xml",
    "demo/im_livechat_channel/im_livechat_session_7.xml",
    "demo/im_livechat_channel/im_livechat_session_8.xml",
    "demo/im_livechat_channel/im_livechat_session_9.xml",
    "demo/im_livechat_channel/im_livechat_session_10.xml",
    "demo/im_livechat_channel/im_livechat_session_11.xml",
    "demo/im_livechat_channel/im_livechat_session_12.xml",
    "demo/im_livechat_channel/im_livechat_session_13.xml",
    "demo/im_livechat_channel/im_livechat_session_14.xml",
    "demo/im_livechat_channel/im_livechat_session_15.xml",
    "demo/im_livechat_channel/im_livechat_support_bot.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_1.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_2.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_3.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_4.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_5.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_6.xml",
    "demo/im_livechat_channel/im_livechat_support_bot_session_7.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "web/static/src/views/fields/file_handler.*",
      "web/static/src/views/fields/formatters.js",
      [
        "include",
        "im_livechat.assets_embed_core"
      ],
      "im_livechat/static/src/embed/frontend/**/*"
    ],
    "web.assets_backend": [
      "im_livechat/static/src/js/colors_reset_button/*",
      "im_livechat/static/src/js/im_livechat_chatbot_steps_one2many.js",
      "im_livechat/static/src/views/**/*",
      [
        "remove",
        "im_livechat/static/src/views/lazy/**/*"
      ],
      "im_livechat/static/src/scss/im_livechat_history.scss",
      "im_livechat/static/src/scss/im_livechat_form.scss",
      "im_livechat/static/src/core/common/**/*",
      "im_livechat/static/src/core/public_web/**/*",
      "im_livechat/static/src/core/web/**/*",
      [
        "remove",
        "im_livechat/static/src/**/*.dark.scss"
      ]
    ],
    "web.assets_backend_lazy": [
      "im_livechat/static/src/views/lazy/**/*"
    ],
    "web.assets_web_dark": [
      "im_livechat/static/src/**/*.dark.scss"
    ],
    "web.assets_unit_tests": [
      "im_livechat/static/tests/**/*",
      [
        "remove",
        "im_livechat/static/tests/embed/**/*"
      ],
      [
        "remove",
        "im_livechat/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "im_livechat/static/tests/tours/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "im_livechat/static/src/core/common/**/*",
      "im_livechat/static/src/embed/common/**/*"
    ],
    "im_livechat.assets_embed_external": [
      "im_livechat/static/src/embed/external/**/*"
    ],
    "im_livechat.assets_embed_cors": [
      "im_livechat/static/src/embed/cors/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      [
        "remove",
        "im_livechat/static/**"
      ],
      [
        "include",
        "im_livechat.assets_embed_external"
      ],
      [
        "remove",
        "im_livechat/static/src/embed/external/boot.js"
      ],
      "im_livechat/static/tests/livechat_test_helpers.js",
      "im_livechat/static/tests/mock_server/**/*"
    ],
    "im_livechat.assets_livechat_support_tours": [
      [
        "include",
        "web_tour.assets"
      ],
      "im_livechat/static/tests/tours/livechat_tour_utils.js",
      "im_livechat/static/tests/tours/support/*"
    ],
    "im_livechat.embed_assets_unit_tests": [
      "web/static/tests/_framework/**/*",
      "im_livechat/static/tests/embed/**/*"
    ],
    "mail.assets_public": [
      "im_livechat/static/src/core/common/**/*",
      "im_livechat/static/src/core/public_web/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "im_livechat/static/src/core/common/**/*",
      [
        "remove",
        "im_livechat/static/src/core/common/**/*.scss"
      ]
    ]
  }
}
```

### Representative source files

- `addons/im_livechat/__init__.py` (5 lines)
- `addons/im_livechat/__manifest__.py` (145 lines)
- `addons/im_livechat/controllers/__init__.py` (11 lines)
- `addons/im_livechat/controllers/attachment.py` (25 lines)
- `addons/im_livechat/controllers/channel.py` (69 lines)
- `addons/im_livechat/controllers/chatbot.py` (171 lines)
- `addons/im_livechat/controllers/cors/__init__.py` (12 lines)
- `addons/im_livechat/controllers/cors/attachment.py` (13 lines)
- `addons/im_livechat/controllers/cors/channel.py` (15 lines)
- `addons/im_livechat/controllers/cors/chatbot.py` (23 lines)
- `addons/im_livechat/controllers/cors/google_translate.py` (16 lines)
- `addons/im_livechat/controllers/cors/link_preview.py` (15 lines)
- `addons/im_livechat/controllers/cors/main.py` (35 lines)
- `addons/im_livechat/controllers/cors/message_reaction.py` (11 lines)
- `addons/im_livechat/controllers/cors/rtc.py` (27 lines)
- `addons/im_livechat/controllers/cors/thread.py` (15 lines)
- `addons/im_livechat/controllers/cors/webclient.py` (13 lines)
- `addons/im_livechat/controllers/main.py` (278 lines)
- `addons/im_livechat/controllers/messaging_menu.py` (41 lines)
- `addons/im_livechat/controllers/rtc.py` (20 lines)
- `addons/im_livechat/controllers/thread.py` (12 lines)
- `addons/im_livechat/controllers/webclient.py` (96 lines)
- `addons/im_livechat/data/digest_data.xml` (25 lines)
- `addons/im_livechat/data/im_livechat_channel_data.xml` (9 lines)
- `addons/im_livechat/data/im_livechat_chatbot_data.xml` (103 lines)
- `addons/im_livechat/data/mail_templates.xml` (78 lines)
- `addons/im_livechat/data/utm_data.xml` (6 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_channel.xml` (25 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_chatbot.xml` (92 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_chatbot_session_1.xml` (81 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_chatbot_session_2.xml` (81 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_chatbot_session_3.xml` (112 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_1.xml` (123 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_10.xml` (117 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_11.xml` (79 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_12.xml` (51 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_13.xml` (73 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_14.xml` (92 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_15.xml` (49 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_2.xml` (120 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_3.xml` (82 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_4.xml` (82 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_5.xml` (90 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_6.xml` (90 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_7.xml` (82 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_8.xml` (88 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_session_9.xml` (126 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot.xml` (117 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_1.xml` (206 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_2.xml` (106 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_3.xml` (106 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_4.xml` (194 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_5.xml` (105 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_6.xml` (149 lines)
- `addons/im_livechat/demo/im_livechat_channel/im_livechat_support_bot_session_7.xml` (72 lines)
- `addons/im_livechat/i18n/af.po` (3,030 lines)
- `addons/im_livechat/i18n/ar.po` (3,137 lines)
- `addons/im_livechat/i18n/az.po` (3,071 lines)
- `addons/im_livechat/i18n/bg.po` (3,103 lines)
- `addons/im_livechat/i18n/bs.po` (3,079 lines)
- `addons/im_livechat/i18n/ca.po` (3,143 lines)
- `addons/im_livechat/i18n/cs.po` (3,141 lines)
- `addons/im_livechat/i18n/da.po` (3,086 lines)
- `addons/im_livechat/i18n/de.po` (3,231 lines)
- `addons/im_livechat/i18n/el.po` (3,084 lines)
- `addons/im_livechat/i18n/es.po` (3,189 lines)
- `addons/im_livechat/i18n/es_419.po` (3,216 lines)
- `addons/im_livechat/i18n/es_CL.po` (120 lines)
- `addons/im_livechat/i18n/et.po` (3,105 lines)
- `addons/im_livechat/i18n/eu.po` (3,029 lines)
- `addons/im_livechat/i18n/fa.po` (3,122 lines)
- `addons/im_livechat/i18n/fi.po` (3,186 lines)
- `addons/im_livechat/i18n/fo.po` (3,029 lines)
- `addons/im_livechat/i18n/fr.po` (3,223 lines)
- `addons/im_livechat/i18n/fr_CA.po` (120 lines)
- `addons/im_livechat/i18n/gl.po` (3,029 lines)
- `addons/im_livechat/i18n/gu.po` (3,033 lines)
- `addons/im_livechat/i18n/he.po` (3,086 lines)
- `addons/im_livechat/i18n/hi.po` (3,070 lines)
- `addons/im_livechat/i18n/hr.po` (3,091 lines)
- `addons/im_livechat/i18n/hu.po` (3,122 lines)
- `addons/im_livechat/i18n/id.po` (3,167 lines)
- `addons/im_livechat/i18n/im_livechat.pot` (3,051 lines)
- `addons/im_livechat/i18n/is.po` (3,026 lines)
- `addons/im_livechat/i18n/it.po` (3,206 lines)
- `addons/im_livechat/i18n/ja.po` (3,164 lines)
- `addons/im_livechat/i18n/ka.po` (3,029 lines)
- `addons/im_livechat/i18n/kab.po` (3,069 lines)
- `addons/im_livechat/i18n/km.po` (3,032 lines)
- `addons/im_livechat/i18n/ko.po` (3,132 lines)
- `addons/im_livechat/i18n/ku.po` (3,068 lines)
- `addons/im_livechat/i18n/lb.po` (3,031 lines)
- `addons/im_livechat/i18n/lo.po` (3,149 lines)
- `addons/im_livechat/i18n/lt.po` (3,095 lines)
- `addons/im_livechat/i18n/lv.po` (3,075 lines)
- `addons/im_livechat/i18n/mk.po` (3,029 lines)
- `addons/im_livechat/i18n/mn.po` (3,086 lines)
- `addons/im_livechat/i18n/my.po` (3,069 lines)
- `addons/im_livechat/i18n/nb.po` (3,075 lines)
- `addons/im_livechat/i18n/nl.po` (3,213 lines)
- `addons/im_livechat/i18n/pl.po` (3,232 lines)
- `addons/im_livechat/i18n/pt.po` (3,164 lines)
- `addons/im_livechat/i18n/pt_BR.po` (3,219 lines)
- `addons/im_livechat/i18n/ro.po` (3,128 lines)
- `addons/im_livechat/i18n/ru.po` (3,168 lines)
- `addons/im_livechat/i18n/sk.po` (3,087 lines)
- `addons/im_livechat/i18n/sl.po` (3,137 lines)
- `addons/im_livechat/i18n/sq.po` (3,029 lines)
- `addons/im_livechat/i18n/sr@latin.po` (3,113 lines)
- `addons/im_livechat/i18n/sv.po` (3,125 lines)
- `addons/im_livechat/i18n/ta.po` (3,030 lines)
- `addons/im_livechat/i18n/th.po` (3,106 lines)
- `addons/im_livechat/i18n/tr.po` (3,174 lines)
- `addons/im_livechat/i18n/uk.po` (3,118 lines)
- `addons/im_livechat/i18n/uz.po` (3,594 lines)
- `addons/im_livechat/i18n/vi.po` (3,152 lines)
- `addons/im_livechat/i18n/zh_CN.po` (3,136 lines)
- `addons/im_livechat/i18n/zh_TW.po` (3,105 lines)
- `addons/im_livechat/models/__init__.py` (23 lines)
- `addons/im_livechat/models/chatbot_message.py` (38 lines)
- `addons/im_livechat/models/chatbot_script.py` (238 lines)
- `addons/im_livechat/models/chatbot_script_answer.py` (47 lines)
- `addons/im_livechat/models/chatbot_script_step.py` (367 lines)
- `addons/im_livechat/models/digest.py` (68 lines)
- `addons/im_livechat/models/discuss_call_history.py` (10 lines)
- `addons/im_livechat/models/discuss_channel.py` (1,147 lines)
- `addons/im_livechat/models/discuss_channel_member.py` (223 lines)
- `addons/im_livechat/models/discuss_channel_rtc_session.py` (21 lines)
- `addons/im_livechat/models/im_livechat_channel.py` (731 lines)
- `addons/im_livechat/models/im_livechat_channel_member_history.py` (277 lines)
- `addons/im_livechat/models/im_livechat_expertise.py` (52 lines)
- `addons/im_livechat/models/ir_http.py` (50 lines)
- `addons/im_livechat/models/ir_qweb.py` (11 lines)
- `addons/im_livechat/models/ir_websocket.py` (21 lines)
- `addons/im_livechat/models/mail_message.py` (52 lines)
- `addons/im_livechat/models/res_groups.py` (25 lines)
- `addons/im_livechat/models/res_partner.py` (125 lines)
- `addons/im_livechat/models/res_users.py` (209 lines)
- `addons/im_livechat/models/res_users_settings.py` (22 lines)
- `addons/im_livechat/models/utm.py` (13 lines)
- `addons/im_livechat/report/__init__.py` (2 lines)
- `addons/im_livechat/report/im_livechat_conversation_report.xml` (20 lines)
- `addons/im_livechat/report/im_livechat_report_channel.py` (336 lines)
- `addons/im_livechat/report/im_livechat_report_channel_views.xml` (149 lines)
- `addons/im_livechat/security/im_livechat_channel_security.xml` (25 lines)
- `addons/im_livechat/security/ir.access.csv` (16 lines)
- `addons/im_livechat/static/description/icon.png` (23 lines)
- `addons/im_livechat/static/description/icon.svg` (1 lines)
- `addons/im_livechat/static/description/icon_hi.png` (85 lines)
- `addons/im_livechat/static/src/core/common/@types/models.d.ts` (107 lines)
- `addons/im_livechat/static/src/core/common/channel_member_list_patch.js` (10 lines)
- `addons/im_livechat/static/src/core/common/chat_window_model_patch.js` (44 lines)
- `addons/im_livechat/static/src/core/common/chat_window_patch.js` (5 lines)
- `addons/im_livechat/static/src/core/common/chat_window_patch.xml` (9 lines)
- `addons/im_livechat/static/src/core/common/chatbot_message_model.js` (32 lines)
- `addons/im_livechat/static/src/core/common/chatbot_model.js` (307 lines)
- `addons/im_livechat/static/src/core/common/chatbot_script_model.js` (13 lines)
- `addons/im_livechat/static/src/core/common/chatbot_script_step_answer_model.js` (13 lines)
- `addons/im_livechat/static/src/core/common/chatbot_script_step_model.js` (28 lines)
- `addons/im_livechat/static/src/core/common/chatbot_step_model.js` (55 lines)

Additional files not expanded here: 263. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
