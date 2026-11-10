# Module: test_discuss_full

- **Module ID:** MOD-571
- **Path:** `addons/test_discuss_full`
- **Manifest:** `addons/test_discuss_full/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Test of Discuss with all possible overrides installed.

Test of Discuss with all possible overrides installed, including feature and performance tests.

Declared dependencies: `calendar`, `crm`, `crm_livechat`, `hr_attendance`, `hr_fleet`, `hr_holidays`, `im_livechat`, `mail`, `mail_bot`, `microsoft_calendar`, `project_todo`, `website_livechat`, `website_sale`, `website_slides`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "calendar",
    "crm",
    "crm_livechat",
    "hr_attendance",
    "hr_fleet",
    "hr_holidays",
    "im_livechat",
    "mail",
    "mail_bot",
    "microsoft_calendar",
    "project_todo",
    "website_livechat",
    "website_sale",
    "website_slides"
  ],
  "assets": {
    "web.assets_tests": [
      "test_discuss_full/static/tests/tours/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      "test_discuss_full/static/tests/test_discuss_full_test_helpers.js"
    ],
    "im_livechat.embed_assets_unit_tests": [
      "test_discuss_full/static/tests/embed/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_discuss_full/__init__.py` (2 lines)
- `addons/test_discuss_full/__manifest__.py` (38 lines)
- `addons/test_discuss_full/static/tests/embed/livechat_button.test.js` (20 lines)
- `addons/test_discuss_full/static/tests/test_discuss_full_test_helpers.js` (17 lines)
- `addons/test_discuss_full/static/tests/tours/avatar_card_tour.js` (56 lines)
- `addons/test_discuss_full/static/tests/tours/chatbot_redirect_to_portal_tour.js` (40 lines)
- `addons/test_discuss_full/static/tests/tours/im_livechat_session_open_tour.js` (17 lines)
- `addons/test_discuss_full/tests/__init__.py` (9 lines)
- `addons/test_discuss_full/tests/test_avatar_card_tour.py` (193 lines)
- `addons/test_discuss_full/tests/test_im_livechat_portal.py` (53 lines)
- `addons/test_discuss_full/tests/test_livechat_hr_holidays.py` (58 lines)
- `addons/test_discuss_full/tests/test_livechat_session_open.py` (27 lines)
- `addons/test_discuss_full/tests/test_performance.py` (2,196 lines)
- `addons/test_discuss_full/tests/test_performance_inbox.py` (91 lines)
- `addons/test_discuss_full/tests/test_res_partner.py` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
