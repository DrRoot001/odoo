# Module: test_event_full

- **Module ID:** MOD-572
- **Path:** `addons/test_event_full`
- **Manifest:** `addons/test_event_full/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module will test the main event flows of Odoo, both frontend and backend.
It installs sale capabilities, front-end flow, eCommerce, questions and
automatic lead generation, full Online support, ...


Declared dependencies: `event`, `event_booth`, `event_crm`, `event_crm_sale`, `event_sale`, `event_sms`, `payment_demo`, `website_event_booth_sale_exhibitor`, `website_event_exhibitor`, `website_event_sale`, `website_event_track`, `website_event_track_live`, `website_event_track_quiz`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "event_booth",
    "event_crm",
    "event_crm_sale",
    "event_sale",
    "event_sms",
    "payment_demo",
    "website_event_booth_sale_exhibitor",
    "website_event_exhibitor",
    "website_event_sale",
    "website_event_track",
    "website_event_track_live",
    "website_event_track_quiz"
  ],
  "data": [
    "data/ir_actions_report_data.xml",
    "views/event_registration_templates_reports.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "test_event_full/static/src/js/tours/*"
    ],
    "web.assets_unit_tests": [
      "test_event_full/static/src/js/tests/*"
    ]
  }
}
```

### Representative source files

- `addons/test_event_full/__init__.py` (2 lines)
- `addons/test_event_full/__manifest__.py` (41 lines)
- `addons/test_event_full/data/ir_actions_report_data.xml` (12 lines)
- `addons/test_event_full/static/src/js/tests/test_template_reference_field_widget.test.js` (128 lines)
- `addons/test_event_full/static/src/js/tours/event_portal_tour.js` (48 lines)
- `addons/test_event_full/static/src/js/tours/wevent_performance_tour.js` (70 lines)
- `addons/test_event_full/static/src/js/tours/wevent_register_tour.js` (204 lines)
- `addons/test_event_full/tests/__init__.py` (12 lines)
- `addons/test_event_full/tests/common.py` (538 lines)
- `addons/test_event_full/tests/test_event_crm.py` (179 lines)
- `addons/test_event_full/tests/test_event_event.py` (171 lines)
- `addons/test_event_full/tests/test_event_mail.py` (353 lines)
- `addons/test_event_full/tests/test_event_portal.py` (34 lines)
- `addons/test_event_full/tests/test_event_security.py` (292 lines)
- `addons/test_event_full/tests/test_performance.py` (482 lines)
- `addons/test_event_full/tests/test_wevent_menu.py` (41 lines)
- `addons/test_event_full/tests/test_wevent_register.py` (51 lines)
- `addons/test_event_full/views/event_registration_templates_reports.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
