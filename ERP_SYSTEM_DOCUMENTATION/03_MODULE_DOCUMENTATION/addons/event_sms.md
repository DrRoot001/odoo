# Module: event_sms

- **Module ID:** MOD-071
- **Path:** `addons/event_sms`
- **Manifest:** `addons/event_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Schedule SMS in event management

Declared dependencies: `event`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "sms"
  ],
  "data": [
    "data/sms_data.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "event_sms/static/src/template_reference_field/*"
    ]
  }
}
```

### Representative source files

- `addons/event_sms/__init__.py` (4 lines)
- `addons/event_sms/__manifest__.py` (20 lines)
- `addons/event_sms/data/sms_data.xml` (17 lines)
- `addons/event_sms/i18n/ar.po` (127 lines)
- `addons/event_sms/i18n/az.po` (120 lines)
- `addons/event_sms/i18n/bg.po` (120 lines)
- `addons/event_sms/i18n/bs.po` (121 lines)
- `addons/event_sms/i18n/ca.po` (124 lines)
- `addons/event_sms/i18n/cs.po` (128 lines)
- `addons/event_sms/i18n/da.po` (127 lines)
- `addons/event_sms/i18n/de.po` (138 lines)
- `addons/event_sms/i18n/el.po` (121 lines)
- `addons/event_sms/i18n/es.po` (138 lines)
- `addons/event_sms/i18n/es_419.po` (134 lines)
- `addons/event_sms/i18n/et.po` (123 lines)
- `addons/event_sms/i18n/event_sms.pot` (109 lines)
- `addons/event_sms/i18n/fa.po` (123 lines)
- `addons/event_sms/i18n/fi.po` (134 lines)
- `addons/event_sms/i18n/fr.po` (140 lines)
- `addons/event_sms/i18n/he.po` (129 lines)
- `addons/event_sms/i18n/hi.po` (120 lines)
- `addons/event_sms/i18n/hr.po` (124 lines)
- `addons/event_sms/i18n/hu.po` (124 lines)
- `addons/event_sms/i18n/id.po` (124 lines)
- `addons/event_sms/i18n/it.po` (138 lines)
- `addons/event_sms/i18n/ja.po` (134 lines)
- `addons/event_sms/i18n/kab.po` (120 lines)
- `addons/event_sms/i18n/ko.po` (124 lines)
- `addons/event_sms/i18n/ku.po` (120 lines)
- `addons/event_sms/i18n/lo.po` (119 lines)
- `addons/event_sms/i18n/lt.po` (127 lines)
- `addons/event_sms/i18n/lv.po` (120 lines)
- `addons/event_sms/i18n/mn.po` (123 lines)
- `addons/event_sms/i18n/my.po` (121 lines)
- `addons/event_sms/i18n/nb.po` (123 lines)
- `addons/event_sms/i18n/nl.po` (137 lines)
- `addons/event_sms/i18n/pl.po` (133 lines)
- `addons/event_sms/i18n/pt.po` (129 lines)
- `addons/event_sms/i18n/pt_BR.po` (137 lines)
- `addons/event_sms/i18n/ro.po` (129 lines)
- `addons/event_sms/i18n/ru.po` (128 lines)
- `addons/event_sms/i18n/sk.po` (119 lines)
- `addons/event_sms/i18n/sl.po` (125 lines)
- `addons/event_sms/i18n/sr@latin.po` (124 lines)
- `addons/event_sms/i18n/sv.po` (125 lines)
- `addons/event_sms/i18n/th.po` (124 lines)
- `addons/event_sms/i18n/tr.po` (132 lines)
- `addons/event_sms/i18n/uk.po` (129 lines)
- `addons/event_sms/i18n/uz.po` (142 lines)
- `addons/event_sms/i18n/vi.po` (127 lines)
- `addons/event_sms/i18n/zh_CN.po` (127 lines)
- `addons/event_sms/i18n/zh_TW.po` (127 lines)
- `addons/event_sms/models/__init__.py` (7 lines)
- `addons/event_sms/models/event_mail.py` (30 lines)
- `addons/event_sms/models/event_mail_registration.py` (15 lines)
- `addons/event_sms/models/event_type_mail.py` (13 lines)
- `addons/event_sms/models/sms_template.py` (28 lines)
- `addons/event_sms/security/ir.access.csv` (3 lines)
- `addons/event_sms/static/src/template_reference_field/field_event_mail_template_reference.scss` (8 lines)
- `addons/event_sms/static/src/template_reference_field/field_event_mail_template_reference.xml` (11 lines)
- `addons/event_sms/tests/__init__.py` (3 lines)
- `addons/event_sms/tests/test_sms_schedule.py` (113 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
