# Module: event_crm

- **Module ID:** MOD-067
- **Path:** `addons/event_crm`
- **Manifest:** `addons/event_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Create leads from event registrations.

Declared dependencies: `event`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "crm"
  ],
  "data": [
    "data/crm_lead_merge_template.xml",
    "data/ir_action_data.xml",
    "data/ir_cron_data.xml",
    "views/crm_lead_views.xml",
    "views/event_registration_views.xml",
    "views/event_lead_rule_views.xml",
    "views/event_event_views.xml",
    "views/event_question_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_crm_demo.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "event_crm/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/event_crm/__init__.py` (4 lines)
- `addons/event_crm/__manifest__.py` (31 lines)
- `addons/event_crm/data/crm_lead_merge_template.xml` (20 lines)
- `addons/event_crm/data/event_crm_demo.xml` (27 lines)
- `addons/event_crm/data/ir_action_data.xml` (17 lines)
- `addons/event_crm/data/ir_cron_data.xml` (16 lines)
- `addons/event_crm/i18n/ar.po` (563 lines)
- `addons/event_crm/i18n/az.po` (542 lines)
- `addons/event_crm/i18n/bg.po` (544 lines)
- `addons/event_crm/i18n/bs.po` (567 lines)
- `addons/event_crm/i18n/ca.po` (554 lines)
- `addons/event_crm/i18n/cs.po` (544 lines)
- `addons/event_crm/i18n/da.po` (564 lines)
- `addons/event_crm/i18n/de.po` (570 lines)
- `addons/event_crm/i18n/el.po` (542 lines)
- `addons/event_crm/i18n/es.po` (562 lines)
- `addons/event_crm/i18n/es_419.po` (561 lines)
- `addons/event_crm/i18n/et.po` (555 lines)
- `addons/event_crm/i18n/event_crm.pot` (536 lines)
- `addons/event_crm/i18n/fa.po` (553 lines)
- `addons/event_crm/i18n/fi.po` (562 lines)
- `addons/event_crm/i18n/fr.po` (573 lines)
- `addons/event_crm/i18n/he.po` (555 lines)
- `addons/event_crm/i18n/hi.po` (551 lines)
- `addons/event_crm/i18n/hr.po` (544 lines)
- `addons/event_crm/i18n/hu.po` (542 lines)
- `addons/event_crm/i18n/id.po` (566 lines)
- `addons/event_crm/i18n/it.po` (566 lines)
- `addons/event_crm/i18n/ja.po` (560 lines)
- `addons/event_crm/i18n/kab.po` (560 lines)
- `addons/event_crm/i18n/ko.po` (556 lines)
- `addons/event_crm/i18n/ku.po` (541 lines)
- `addons/event_crm/i18n/lo.po` (555 lines)
- `addons/event_crm/i18n/lt.po` (567 lines)
- `addons/event_crm/i18n/lv.po` (579 lines)
- `addons/event_crm/i18n/mn.po` (541 lines)
- `addons/event_crm/i18n/my.po` (546 lines)
- `addons/event_crm/i18n/nb.po` (542 lines)
- `addons/event_crm/i18n/nl.po` (565 lines)
- `addons/event_crm/i18n/pl.po` (567 lines)
- `addons/event_crm/i18n/pt.po` (564 lines)
- `addons/event_crm/i18n/pt_BR.po` (564 lines)
- `addons/event_crm/i18n/ro.po` (563 lines)
- `addons/event_crm/i18n/ru.po` (567 lines)
- `addons/event_crm/i18n/sk.po` (576 lines)
- `addons/event_crm/i18n/sl.po` (564 lines)
- `addons/event_crm/i18n/sr@latin.po` (561 lines)
- `addons/event_crm/i18n/sv.po` (563 lines)
- `addons/event_crm/i18n/th.po` (553 lines)
- `addons/event_crm/i18n/tr.po` (562 lines)
- `addons/event_crm/i18n/uk.po` (570 lines)
- `addons/event_crm/i18n/uz.po` (668 lines)
- `addons/event_crm/i18n/vi.po` (556 lines)
- `addons/event_crm/i18n/zh_CN.po` (552 lines)
- `addons/event_crm/i18n/zh_TW.po` (556 lines)
- `addons/event_crm/models/__init__.py` (9 lines)
- `addons/event_crm/models/crm_lead.py` (35 lines)
- `addons/event_crm/models/event_event.py` (82 lines)
- `addons/event_crm/models/event_lead_request.py` (79 lines)
- `addons/event_crm/models/event_lead_rule.py` (229 lines)
- `addons/event_crm/models/event_question_answer.py` (20 lines)
- `addons/event_crm/models/event_registration.py` (398 lines)
- `addons/event_crm/security/ir.access.csv` (5 lines)
- `addons/event_crm/static/tests/tours/event_question_answers_rule_creation_tour.js` (42 lines)
- `addons/event_crm/tests/__init__.py` (6 lines)
- `addons/event_crm/tests/common.py` (143 lines)
- `addons/event_crm/tests/test_crm_lead_merge.py` (84 lines)
- `addons/event_crm/tests/test_event_crm_flow.py` (241 lines)
- `addons/event_crm/tests/test_event_crm_http.py` (39 lines)
- `addons/event_crm/views/crm_lead_views.xml` (33 lines)
- `addons/event_crm/views/event_event_views.xml` (33 lines)
- `addons/event_crm/views/event_lead_rule_views.xml` (107 lines)
- `addons/event_crm/views/event_question_views.xml` (16 lines)
- `addons/event_crm/views/event_registration_views.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
