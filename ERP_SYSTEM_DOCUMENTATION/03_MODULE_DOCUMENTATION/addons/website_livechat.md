# Module: website_livechat

- **Module ID:** MOD-623
- **Path:** `addons/website_livechat`
- **Manifest:** `addons/website_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Chat with your website visitors

Allow website visitors to chat with the collaborators.

Declared dependencies: `website`, `im_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 28 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 5 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 37 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "im_livechat"
  ],
  "data": [
    "views/website_livechat.xml",
    "views/res_config_settings_views.xml",
    "views/im_livechat_chatbot_script_view.xml",
    "views/website_visitor_views.xml",
    "views/im_livechat_channel_add.xml",
    "data/website_livechat_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/website_livechat_chatbot_demo.xml",
    "demo/im_livechat_session_11.xml"
  ],
  "assets": {
    "im_livechat.assets_embed_core": [
      "website_livechat/static/src/core/common/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      [
        "remove",
        "website_livechat/static/**"
      ],
      "web/static/tests/public/helpers.js",
      "website/static/tests/helpers.js",
      "website_livechat/static/tests/website_livechat_test_helpers.js",
      "website/static/tests/mock_server/**/*",
      "website_livechat/static/tests/mock_server/**/*"
    ],
    "mail.assets_public": [
      "website_livechat/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "website_livechat/static/src/core/common/**/*"
    ],
    "website.assets_editor": [
      "website_livechat/static/src/js/**/*"
    ],
    "web.assets_frontend": [
      "website_livechat/static/src/core/common/**/*"
    ],
    "web.assets_backend": [
      "website_livechat/static/src/core/common/**/*",
      "website_livechat/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "website_livechat/static/tests/**/*",
      [
        "remove",
        "website_livechat/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "website_livechat/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_livechat/__init__.py` (3 lines)
- `addons/website_livechat/__manifest__.py` (59 lines)
- `addons/website_livechat/controllers/__init__.py` (7 lines)
- `addons/website_livechat/controllers/chatbot.py` (61 lines)
- `addons/website_livechat/controllers/main.py` (12 lines)
- `addons/website_livechat/controllers/webclient.py` (60 lines)
- `addons/website_livechat/controllers/website.py` (16 lines)
- `addons/website_livechat/data/website_livechat_chatbot_demo.xml` (15 lines)
- `addons/website_livechat/data/website_livechat_data.xml` (14 lines)
- `addons/website_livechat/demo/im_livechat_session_11.xml` (13 lines)
- `addons/website_livechat/i18n/af.po` (297 lines)
- `addons/website_livechat/i18n/ar.po` (306 lines)
- `addons/website_livechat/i18n/az.po` (301 lines)
- `addons/website_livechat/i18n/bg.po` (305 lines)
- `addons/website_livechat/i18n/bs.po` (301 lines)
- `addons/website_livechat/i18n/ca.po` (316 lines)
- `addons/website_livechat/i18n/cs.po` (311 lines)
- `addons/website_livechat/i18n/da.po` (310 lines)
- `addons/website_livechat/i18n/de.po` (312 lines)
- `addons/website_livechat/i18n/el.po` (302 lines)
- `addons/website_livechat/i18n/es.po` (309 lines)
- `addons/website_livechat/i18n/es_419.po` (307 lines)
- `addons/website_livechat/i18n/et.po` (316 lines)
- `addons/website_livechat/i18n/fa.po` (308 lines)
- `addons/website_livechat/i18n/fi.po` (315 lines)
- `addons/website_livechat/i18n/fr.po` (312 lines)
- `addons/website_livechat/i18n/fr_BE.po` (281 lines)
- `addons/website_livechat/i18n/gl.po` (295 lines)
- `addons/website_livechat/i18n/gu.po` (296 lines)
- `addons/website_livechat/i18n/he.po` (311 lines)
- `addons/website_livechat/i18n/hi.po` (298 lines)
- `addons/website_livechat/i18n/hr.po` (309 lines)
- `addons/website_livechat/i18n/hu.po` (307 lines)
- `addons/website_livechat/i18n/id.po` (308 lines)
- `addons/website_livechat/i18n/is.po` (293 lines)
- `addons/website_livechat/i18n/it.po` (312 lines)
- `addons/website_livechat/i18n/ja.po` (311 lines)
- `addons/website_livechat/i18n/kab.po` (297 lines)
- `addons/website_livechat/i18n/km.po` (297 lines)
- `addons/website_livechat/i18n/ko.po` (306 lines)
- `addons/website_livechat/i18n/ku.po` (297 lines)
- `addons/website_livechat/i18n/lo.po` (300 lines)
- `addons/website_livechat/i18n/lt.po` (306 lines)
- `addons/website_livechat/i18n/lv.po` (303 lines)
- `addons/website_livechat/i18n/mk.po` (301 lines)
- `addons/website_livechat/i18n/mn.po` (306 lines)
- `addons/website_livechat/i18n/my.po` (298 lines)
- `addons/website_livechat/i18n/nb.po` (303 lines)
- `addons/website_livechat/i18n/nl.po` (311 lines)
- `addons/website_livechat/i18n/pl.po` (321 lines)
- `addons/website_livechat/i18n/pt.po` (313 lines)
- `addons/website_livechat/i18n/pt_BR.po` (314 lines)
- `addons/website_livechat/i18n/ro.po` (311 lines)
- `addons/website_livechat/i18n/ru.po` (306 lines)
- `addons/website_livechat/i18n/sk.po` (306 lines)
- `addons/website_livechat/i18n/sl.po` (307 lines)
- `addons/website_livechat/i18n/sr@latin.po` (306 lines)
- `addons/website_livechat/i18n/sv.po` (313 lines)
- `addons/website_livechat/i18n/ta.po` (295 lines)
- `addons/website_livechat/i18n/th.po` (304 lines)
- `addons/website_livechat/i18n/tr.po` (321 lines)
- `addons/website_livechat/i18n/uk.po` (309 lines)
- `addons/website_livechat/i18n/uz.po` (350 lines)
- `addons/website_livechat/i18n/vi.po` (309 lines)
- `addons/website_livechat/i18n/website_livechat.pot` (293 lines)
- `addons/website_livechat/i18n/zh_CN.po` (304 lines)
- `addons/website_livechat/i18n/zh_TW.po` (303 lines)
- `addons/website_livechat/models/__init__.py` (11 lines)
- `addons/website_livechat/models/chatbot_script.py` (16 lines)
- `addons/website_livechat/models/chatbot_script_step.py` (20 lines)
- `addons/website_livechat/models/discuss_channel.py` (80 lines)
- `addons/website_livechat/models/discuss_channel_member.py` (20 lines)
- `addons/website_livechat/models/im_livechat_channel.py` (67 lines)
- `addons/website_livechat/models/ir_http.py` (13 lines)
- `addons/website_livechat/models/res_config_settings.py` (10 lines)
- `addons/website_livechat/models/website.py` (30 lines)
- `addons/website_livechat/models/website_visitor.py` (177 lines)
- `addons/website_livechat/security/ir.access.csv` (3 lines)
- `addons/website_livechat/static/description/icon.png` (26 lines)
- `addons/website_livechat/static/description/icon.svg` (1 lines)
- `addons/website_livechat/static/description/icon_hi.png` (79 lines)
- `addons/website_livechat/static/src/core/common/@types/models.d.ts` (12 lines)
- `addons/website_livechat/static/src/core/common/discuss_channel_model_patch.js` (16 lines)
- `addons/website_livechat/static/src/core/common/thread_model_patch.js` (10 lines)
- `addons/website_livechat/static/src/core/common/website_livechat_edit_mode.scss` (10 lines)
- `addons/website_livechat/static/src/core/common/website_visitor_model_patch.js` (15 lines)
- `addons/website_livechat/static/src/core/web/@types/models.d.ts` (5 lines)
- `addons/website_livechat/static/src/core/web/channel_member_model_patch.js` (13 lines)
- `addons/website_livechat/static/src/core/web/livechat_channel_info_list_patch.js` (23 lines)
- `addons/website_livechat/static/src/core/web/livechat_channel_info_list_patch.xml` (42 lines)
- `addons/website_livechat/static/src/core/web/website_visitor_model_patch.js` (21 lines)
- `addons/website_livechat/static/src/js/systray_items/new_content.js` (19 lines)
- `addons/website_livechat/static/tests/discuss_content_patch.test.js` (36 lines)
- `addons/website_livechat/static/tests/livechat_channel_info_list_patch.test.js` (109 lines)
- `addons/website_livechat/static/tests/messaging_service_patch.test.js` (30 lines)
- `addons/website_livechat/static/tests/mock_server/mock_models/discuss_channel.js` (49 lines)
- `addons/website_livechat/static/tests/mock_server/mock_models/website_visitor.js` (97 lines)
- `addons/website_livechat/static/tests/thread_patch.test.js` (37 lines)
- `addons/website_livechat/static/tests/tours/lazy_frontend_bus_tour.js` (55 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_as_portal.js` (14 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_after_reload.js` (44 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_continue.js` (24 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_continue_after_login.js` (55 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_flow.js` (151 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_forward.js` (29 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_fw_operator_matching_lang.js` (17 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_redirect.js` (65 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_restart.js` (90 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_stops_when_agent_joins_tour.js` (28 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_test_page_tour.js` (57 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_trigger_selection_tour.js` (34 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_chatbot_user_input_tour.js` (48 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_common.js` (136 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_no_new_session_with_hide_rule.js` (53 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_question_selection_overlapping_answers.js` (49 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_rating.js` (43 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_request.js` (38 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_session_user_changes.js` (32 lines)
- `addons/website_livechat/static/tests/tours/website_livechat_user_known_after_reload.js` (22 lines)
- `addons/website_livechat/static/tests/website_livechat_test_helpers.js` (17 lines)
- `addons/website_livechat/tests/__init__.py` (10 lines)
- `addons/website_livechat/tests/common.py` (122 lines)
- `addons/website_livechat/tests/test_chatbot_ui.py` (519 lines)
- `addons/website_livechat/tests/test_cors_livechat.py` (24 lines)
- `addons/website_livechat/tests/test_fw_operator.py` (79 lines)
- `addons/website_livechat/tests/test_lazy_frontend_bus.py` (9 lines)
- `addons/website_livechat/tests/test_livechat_basic_flow.py` (461 lines)
- `addons/website_livechat/tests/test_livechat_request.py` (132 lines)
- `addons/website_livechat/tests/test_livechat_session_user_changes.py` (9 lines)
- `addons/website_livechat/tests/test_ui.py` (96 lines)
- `addons/website_livechat/tests/test_website_visitor.py` (127 lines)
- `addons/website_livechat/views/im_livechat_channel_add.xml` (25 lines)
- `addons/website_livechat/views/im_livechat_chatbot_script_view.xml` (16 lines)
- `addons/website_livechat/views/res_config_settings_views.xml` (18 lines)
- `addons/website_livechat/views/website_livechat.xml` (18 lines)
- `addons/website_livechat/views/website_visitor_views.xml` (134 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
