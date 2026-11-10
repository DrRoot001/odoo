# Module: test_mail_full

- **Module ID:** MOD-576
- **Path:** `addons/test_mail_full`
- **Manifest:** `addons/test_mail_full/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Mail Tests: performances and tests specific to mail with all sub-modules

This module contains tests related to various mail features
and mail-related sub modules. Those tests are present in a separate module as it
contains models used only to perform tests independently to functional aspects of
real applications. 

Declared dependencies: `mail`, `mail_bot`, `mail_tracking_mass_mailing`, `mass_mailing`, `mass_mailing_sms`, `phone_validation`, `portal`, `rating`, `sms`, `test_mail`, `test_mail_sms`, `test_mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 16 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "mail_bot",
    "mail_tracking_mass_mailing",
    "mass_mailing",
    "mass_mailing_sms",
    "phone_validation",
    "portal",
    "rating",
    "sms",
    "test_mail",
    "test_mail_sms",
    "test_mass_mailing"
  ],
  "data": [
    "data/mail_message_subtype_data.xml",
    "views/test_portal_template.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_unit_tests": [
      "test_mail_full/static/tests/**/*",
      [
        "remove",
        "test_mail_full/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "test_mail_full/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_mail_full/__init__.py` (2 lines)
- `addons/test_mail_full/__manifest__.py` (42 lines)
- `addons/test_mail_full/controllers/__init__.py` (4 lines)
- `addons/test_mail_full/controllers/portal.py` (49 lines)
- `addons/test_mail_full/data/mail_message_subtype_data.xml` (10 lines)
- `addons/test_mail_full/i18n/test_mail_full.pot` (291 lines)
- `addons/test_mail_full/models/__init__.py` (3 lines)
- `addons/test_mail_full/models/test_mail_models_mail.py` (162 lines)
- `addons/test_mail_full/security/ir.access.csv` (14 lines)
- `addons/test_mail_full/static/tests/messaging_menu_patch.test.js` (68 lines)
- `addons/test_mail_full/static/tests/mock_server/models/mail_test_rating.js` (5 lines)
- `addons/test_mail_full/static/tests/test_mail_full_test_helpers.js` (9 lines)
- `addons/test_mail_full/static/tests/tours/load_more_tour.js` (19 lines)
- `addons/test_mail_full/static/tests/tours/message_actions_tour.js` (88 lines)
- `addons/test_mail_full/static/tests/tours/portal_composer_actions_tour.js` (32 lines)
- `addons/test_mail_full/static/tests/tours/portal_copy_link_tour.js` (13 lines)
- `addons/test_mail_full/static/tests/tours/portal_message_highlight_tour.js` (9 lines)
- `addons/test_mail_full/static/tests/tours/portal_no_copy_link_tour.js` (28 lines)
- `addons/test_mail_full/static/tests/tours/portal_rating_pagination_tour.js` (45 lines)
- `addons/test_mail_full/static/tests/tours/portal_rating_tour.js.js` (50 lines)
- `addons/test_mail_full/tests/__init__.py` (15 lines)
- `addons/test_mail_full/tests/common.py` (8 lines)
- `addons/test_mail_full/tests/test_controller_attachment.py` (39 lines)
- `addons/test_mail_full/tests/test_controller_reaction.py` (80 lines)
- `addons/test_mail_full/tests/test_controller_thread.py` (209 lines)
- `addons/test_mail_full/tests/test_controller_update.py` (48 lines)
- `addons/test_mail_full/tests/test_ir_mail_server.py` (123 lines)
- `addons/test_mail_full/tests/test_mail_bot.py` (154 lines)
- `addons/test_mail_full/tests/test_mail_performance.py` (465 lines)
- `addons/test_mail_full/tests/test_mail_thread_internals.py` (91 lines)
- `addons/test_mail_full/tests/test_mass_mailing.py` (156 lines)
- `addons/test_mail_full/tests/test_portal.py` (477 lines)
- `addons/test_mail_full/tests/test_rating.py` (288 lines)
- `addons/test_mail_full/tests/test_res_users.py` (89 lines)
- `addons/test_mail_full/tests/test_ui.py` (167 lines)
- `addons/test_mail_full/views/test_portal_template.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
