# Module: test_mail

- **Module ID:** MOD-575
- **Path:** `addons/test_mail`
- **Manifest:** `addons/test_mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Mail Tests: performances and tests specific to mail

This module contains tests related to mail. Those are
present in a separate module as it contains models used only to perform
tests independently to functional aspects of other models. 

Declared dependencies: `mail`, `test_base`, `phone_validation`, `mail_tracking`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 43 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 17 | Client behavior/assets. |
| Tests | 36 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail",
    "test_base",
    "phone_validation",
    "mail_tracking"
  ],
  "data": [
    "data/data.xml",
    "data/mail_template_data.xml",
    "data/subtype_data.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_unit_tests": [
      "test_mail/static/tests/**/*"
    ],
    "web.assets_tests": [
      "test_mail/static/tests/tours/*"
    ]
  }
}
```

### Representative source files

- `addons/test_mail/__init__.py` (4 lines)
- `addons/test_mail/__manifest__.py` (32 lines)
- `addons/test_mail/data/__init__.py` (3 lines)
- `addons/test_mail/data/data.xml` (36 lines)
- `addons/test_mail/data/mail_template_data.xml` (64 lines)
- `addons/test_mail/data/subtype_data.xml` (64 lines)
- `addons/test_mail/data/test_mail_data.py` (1,451 lines)
- `addons/test_mail/models/__init__.py` (6 lines)
- `addons/test_mail/models/mail_test_access.py` (97 lines)
- `addons/test_mail/models/mail_test_lead.py` (54 lines)
- `addons/test_mail/models/mail_test_ticket.py` (262 lines)
- `addons/test_mail/models/test_mail_corner_case_models.py` (333 lines)
- `addons/test_mail/models/test_mail_feature_models.py` (96 lines)
- `addons/test_mail/models/test_mail_models.py` (212 lines)
- `addons/test_mail/security/ir.access.csv` (88 lines)
- `addons/test_mail/static/tests/activity.test.js` (1,208 lines)
- `addons/test_mail/static/tests/activity_mobile.test.js` (35 lines)
- `addons/test_mail/static/tests/attachment_view.test.js` (368 lines)
- `addons/test_mail/static/tests/chatter.test.js` (201 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_activity.js` (6 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_multi_company.js` (5 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_multi_company_read.js` (6 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_properties.js` (5 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_simple.js` (5 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_simple_main_attachment.js` (5 lines)
- `addons/test_mail/static/tests/mock_server/models/mail_test_track_all.js` (10 lines)
- `addons/test_mail/static/tests/mock_server/models/res_currency.js` (5 lines)
- `addons/test_mail/static/tests/properties_field.test.js` (71 lines)
- `addons/test_mail/static/tests/systray_activity_menu.test.js` (154 lines)
- `addons/test_mail/static/tests/test_mail_test_helpers.js` (32 lines)
- `addons/test_mail/static/tests/tours/access_inbox_records_tour.js` (36 lines)
- `addons/test_mail/static/tests/tours/mail_activity_view_tour.js` (68 lines)
- `addons/test_mail/tests/__init__.py` (32 lines)
- `addons/test_mail/tests/common.py` (27 lines)
- `addons/test_mail/tests/test_controller_attachment.py` (433 lines)
- `addons/test_mail/tests/test_controller_binary.py` (47 lines)
- `addons/test_mail/tests/test_controller_thread.py` (219 lines)
- `addons/test_mail/tests/test_invite.py` (53 lines)
- `addons/test_mail/tests/test_ir_actions.py` (470 lines)
- `addons/test_mail/tests/test_ir_attachment.py` (59 lines)
- `addons/test_mail/tests/test_mail_activity.py` (1,020 lines)
- `addons/test_mail/tests/test_mail_activity_mixin.py` (867 lines)
- `addons/test_mail/tests/test_mail_activity_plan.py` (452 lines)
- `addons/test_mail/tests/test_mail_alias.py` (1,060 lines)
- `addons/test_mail/tests/test_mail_composer.py` (4,003 lines)
- `addons/test_mail/tests/test_mail_composer_mixin.py` (203 lines)
- `addons/test_mail/tests/test_mail_flow.py` (565 lines)
- `addons/test_mail/tests/test_mail_followers.py` (1,113 lines)
- `addons/test_mail/tests/test_mail_gateway.py` (2,868 lines)
- `addons/test_mail/tests/test_mail_mail.py` (1,220 lines)
- `addons/test_mail/tests/test_mail_management.py` (59 lines)
- `addons/test_mail/tests/test_mail_message.py` (478 lines)
- `addons/test_mail/tests/test_mail_message_security.py` (1,027 lines)
- `addons/test_mail/tests/test_mail_multicompany.py` (503 lines)
- `addons/test_mail/tests/test_mail_push.py` (707 lines)
- `addons/test_mail/tests/test_mail_scheduled_message.py` (243 lines)
- `addons/test_mail/tests/test_mail_security.py` (58 lines)
- `addons/test_mail/tests/test_mail_template.py` (472 lines)
- `addons/test_mail/tests/test_mail_template_preview.py` (134 lines)
- `addons/test_mail/tests/test_mail_thread_internals.py` (1,802 lines)
- `addons/test_mail/tests/test_mail_thread_mixins.py` (260 lines)
- `addons/test_mail/tests/test_message_post.py` (2,666 lines)
- `addons/test_mail/tests/test_message_track.py` (1,758 lines)
- `addons/test_mail/tests/test_performance.py` (2,091 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
