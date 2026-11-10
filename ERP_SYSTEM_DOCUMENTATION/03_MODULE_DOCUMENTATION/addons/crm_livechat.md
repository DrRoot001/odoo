# Module: crm_livechat

- **Module ID:** MOD-057
- **Path:** `addons/crm_livechat`
- **Manifest:** `addons/crm_livechat/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Create lead from livechat conversation

Create new lead with using /lead command in the channel

Declared dependencies: `crm`, `im_livechat`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 14 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "crm",
    "im_livechat"
  ],
  "data": [
    "data/crm_livechat_chatbot_data.xml",
    "views/chatbot_script_views.xml",
    "views/chatbot_script_step_views.xml",
    "views/crm_lead_views.xml",
    "views/discuss_channel_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": "{'crm_livechat/static/src/core/**/*'}",
    "mail.assets_public": [
      "crm_livechat/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "crm_livechat/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "crm_livechat/static/tests/**/*",
      [
        "remove",
        "crm_livechat/static/tests/tours/**/*"
      ]
    ],
    "im_livechat.assets_livechat_support_tours": [
      "crm_livechat/static/tests/tours/support/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      [
        "remove",
        "crm_livechat/static/src/core/web/**/*"
      ]
    ],
    "im_livechat.assets_embed_core": [
      "crm_livechat/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/crm_livechat/__init__.py` (5 lines)
- `addons/crm_livechat/__manifest__.py` (47 lines)
- `addons/crm_livechat/data/crm_livechat_chatbot_data.xml` (49 lines)
- `addons/crm_livechat/i18n/ar.po` (244 lines)
- `addons/crm_livechat/i18n/az.po` (235 lines)
- `addons/crm_livechat/i18n/bg.po` (238 lines)
- `addons/crm_livechat/i18n/bs.po` (236 lines)
- `addons/crm_livechat/i18n/ca.po` (246 lines)
- `addons/crm_livechat/i18n/crm_livechat.pot` (229 lines)
- `addons/crm_livechat/i18n/cs.po` (254 lines)
- `addons/crm_livechat/i18n/da.po` (245 lines)
- `addons/crm_livechat/i18n/de.po` (251 lines)
- `addons/crm_livechat/i18n/el.po` (237 lines)
- `addons/crm_livechat/i18n/es.po` (248 lines)
- `addons/crm_livechat/i18n/es_419.po` (241 lines)
- `addons/crm_livechat/i18n/et.po` (248 lines)
- `addons/crm_livechat/i18n/fa.po` (239 lines)
- `addons/crm_livechat/i18n/fi.po` (248 lines)
- `addons/crm_livechat/i18n/fr.po` (252 lines)
- `addons/crm_livechat/i18n/he.po` (245 lines)
- `addons/crm_livechat/i18n/hi.po` (233 lines)
- `addons/crm_livechat/i18n/hr.po` (238 lines)
- `addons/crm_livechat/i18n/hu.po` (240 lines)
- `addons/crm_livechat/i18n/id.po` (249 lines)
- `addons/crm_livechat/i18n/it.po` (250 lines)
- `addons/crm_livechat/i18n/ja.po` (246 lines)
- `addons/crm_livechat/i18n/kab.po` (232 lines)
- `addons/crm_livechat/i18n/ko.po` (242 lines)
- `addons/crm_livechat/i18n/ku.po` (233 lines)
- `addons/crm_livechat/i18n/lo.po` (240 lines)
- `addons/crm_livechat/i18n/lt.po` (240 lines)
- `addons/crm_livechat/i18n/lv.po` (235 lines)
- `addons/crm_livechat/i18n/mn.po` (238 lines)
- `addons/crm_livechat/i18n/my.po` (233 lines)
- `addons/crm_livechat/i18n/nb.po` (236 lines)
- `addons/crm_livechat/i18n/nl.po` (249 lines)
- `addons/crm_livechat/i18n/pl.po` (251 lines)
- `addons/crm_livechat/i18n/pt.po` (244 lines)
- `addons/crm_livechat/i18n/pt_BR.po` (250 lines)
- `addons/crm_livechat/i18n/ro.po` (249 lines)
- `addons/crm_livechat/i18n/ru.po` (249 lines)
- `addons/crm_livechat/i18n/sk.po` (238 lines)
- `addons/crm_livechat/i18n/sl.po` (246 lines)
- `addons/crm_livechat/i18n/sr@latin.po` (240 lines)
- `addons/crm_livechat/i18n/sv.po` (250 lines)
- `addons/crm_livechat/i18n/th.po` (242 lines)
- `addons/crm_livechat/i18n/tr.po` (251 lines)
- `addons/crm_livechat/i18n/uk.po` (242 lines)
- `addons/crm_livechat/i18n/uz.po` (281 lines)
- `addons/crm_livechat/i18n/vi.po` (246 lines)
- `addons/crm_livechat/i18n/zh_CN.po` (242 lines)
- `addons/crm_livechat/i18n/zh_TW.po` (239 lines)
- `addons/crm_livechat/models/__init__.py` (7 lines)
- `addons/crm_livechat/models/chatbot_script.py` (27 lines)
- `addons/crm_livechat/models/chatbot_script_step.py` (71 lines)
- `addons/crm_livechat/models/crm_lead.py` (39 lines)
- `addons/crm_livechat/models/discuss_channel.py` (76 lines)
- `addons/crm_livechat/models/res_users.py` (10 lines)
- `addons/crm_livechat/report/__init__.py` (1 lines)
- `addons/crm_livechat/report/im_livechat_report_channel.py` (26 lines)
- `addons/crm_livechat/security/ir.access.csv` (3 lines)
- `addons/crm_livechat/static/src/core/channel_commands.js` (8 lines)
- `addons/crm_livechat/static/src/core/common/@types/models.d.ts` (5 lines)
- `addons/crm_livechat/static/src/core/common/message_model_patch.js` (12 lines)
- `addons/crm_livechat/static/src/core/common/store_service_patch.js` (12 lines)
- `addons/crm_livechat/static/src/core/thread_action_patch.js` (16 lines)
- `addons/crm_livechat/static/src/core/thread_actions.js` (42 lines)
- `addons/crm_livechat/static/src/core/web/livechat_channel_info_list_patch.xml` (14 lines)
- `addons/crm_livechat/static/tests/composer.test.js` (32 lines)
- `addons/crm_livechat/static/tests/create_lead.test.js` (55 lines)
- `addons/crm_livechat/static/tests/crm_livechat_test_helpers.js` (11 lines)
- `addons/crm_livechat/static/tests/livechat_channel_info_list_patch.test.js` (26 lines)
- `addons/crm_livechat/static/tests/message.test.js` (39 lines)
- `addons/crm_livechat/static/tests/mock_server/mock_models/discuss_channel.js` (36 lines)
- `addons/crm_livechat/static/tests/mock_server/mock_models/res_users.js` (12 lines)
- `addons/crm_livechat/static/tests/tours/support/crm_livechat_create_lead_from_chatbot.js` (17 lines)
- `addons/crm_livechat/tests/__init__.py` (7 lines)
- `addons/crm_livechat/tests/chatbot_common.py` (53 lines)
- `addons/crm_livechat/tests/test_chatbot_lead.py` (135 lines)
- `addons/crm_livechat/tests/test_crm_lead.py` (161 lines)
- `addons/crm_livechat/tests/test_discuss_channel_access.py` (65 lines)
- `addons/crm_livechat/views/chatbot_script_step_views.xml` (19 lines)
- `addons/crm_livechat/views/chatbot_script_views.xml` (18 lines)
- `addons/crm_livechat/views/crm_lead_views.xml` (15 lines)
- `addons/crm_livechat/views/discuss_channel_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
