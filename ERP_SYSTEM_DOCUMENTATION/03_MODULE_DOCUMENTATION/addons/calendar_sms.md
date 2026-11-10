# Module: calendar_sms

- **Module ID:** MOD-047
- **Path:** `addons/calendar_sms`
- **Manifest:** `addons/calendar_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Send text messages as event reminders

Send text messages as event reminders

Declared dependencies: `calendar`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "calendar",
    "sms"
  ],
  "data": [
    "data/sms_data.xml",
    "views/calendar_alarm_views.xml",
    "views/calendar_views.xml"
  ]
}
```

### Representative source files

- `addons/calendar_sms/__init__.py` (4 lines)
- `addons/calendar_sms/__manifest__.py` (18 lines)
- `addons/calendar_sms/data/sms_data.xml` (10 lines)
- `addons/calendar_sms/i18n/af.po` (117 lines)
- `addons/calendar_sms/i18n/ar.po` (125 lines)
- `addons/calendar_sms/i18n/az.po` (121 lines)
- `addons/calendar_sms/i18n/bg.po` (124 lines)
- `addons/calendar_sms/i18n/bs.po` (121 lines)
- `addons/calendar_sms/i18n/ca.po` (130 lines)
- `addons/calendar_sms/i18n/calendar_sms.pot` (114 lines)
- `addons/calendar_sms/i18n/cs.po` (124 lines)
- `addons/calendar_sms/i18n/da.po` (124 lines)
- `addons/calendar_sms/i18n/de.po` (126 lines)
- `addons/calendar_sms/i18n/el.po` (122 lines)
- `addons/calendar_sms/i18n/es.po` (127 lines)
- `addons/calendar_sms/i18n/es_419.po` (123 lines)
- `addons/calendar_sms/i18n/et.po` (129 lines)
- `addons/calendar_sms/i18n/fa.po` (127 lines)
- `addons/calendar_sms/i18n/fi.po` (127 lines)
- `addons/calendar_sms/i18n/fr.po` (126 lines)
- `addons/calendar_sms/i18n/gu.po` (116 lines)
- `addons/calendar_sms/i18n/he.po` (127 lines)
- `addons/calendar_sms/i18n/hi.po` (118 lines)
- `addons/calendar_sms/i18n/hr.po` (123 lines)
- `addons/calendar_sms/i18n/hu.po` (122 lines)
- `addons/calendar_sms/i18n/id.po` (123 lines)
- `addons/calendar_sms/i18n/is.po` (113 lines)
- `addons/calendar_sms/i18n/it.po` (126 lines)
- `addons/calendar_sms/i18n/ja.po` (125 lines)
- `addons/calendar_sms/i18n/kab.po` (117 lines)
- `addons/calendar_sms/i18n/km.po` (118 lines)
- `addons/calendar_sms/i18n/ko.po` (124 lines)
- `addons/calendar_sms/i18n/ku.po` (118 lines)
- `addons/calendar_sms/i18n/lo.po` (117 lines)
- `addons/calendar_sms/i18n/lt.po` (128 lines)
- `addons/calendar_sms/i18n/lv.po` (121 lines)
- `addons/calendar_sms/i18n/mn.po` (123 lines)
- `addons/calendar_sms/i18n/my.po` (118 lines)
- `addons/calendar_sms/i18n/nb.po` (123 lines)
- `addons/calendar_sms/i18n/nl.po` (125 lines)
- `addons/calendar_sms/i18n/pl.po` (132 lines)
- `addons/calendar_sms/i18n/pt.po` (127 lines)
- `addons/calendar_sms/i18n/pt_BR.po` (125 lines)
- `addons/calendar_sms/i18n/ro.po` (128 lines)
- `addons/calendar_sms/i18n/ru.po` (124 lines)
- `addons/calendar_sms/i18n/sk.po` (122 lines)
- `addons/calendar_sms/i18n/sl.po` (124 lines)
- `addons/calendar_sms/i18n/sr@latin.po` (123 lines)
- `addons/calendar_sms/i18n/sv.po` (129 lines)
- `addons/calendar_sms/i18n/th.po` (124 lines)
- `addons/calendar_sms/i18n/tr.po` (131 lines)
- `addons/calendar_sms/i18n/uk.po` (127 lines)
- `addons/calendar_sms/i18n/uz.po` (142 lines)
- `addons/calendar_sms/i18n/vi.po` (123 lines)
- `addons/calendar_sms/i18n/zh_CN.po` (124 lines)
- `addons/calendar_sms/i18n/zh_TW.po` (124 lines)
- `addons/calendar_sms/models/__init__.py` (6 lines)
- `addons/calendar_sms/models/calendar_alarm.py` (25 lines)
- `addons/calendar_sms/models/calendar_alarm_manager.py` (24 lines)
- `addons/calendar_sms/models/calendar_event.py` (52 lines)
- `addons/calendar_sms/tests/__init__.py` (4 lines)
- `addons/calendar_sms/tests/test_calendar_sms.py` (142 lines)
- `addons/calendar_sms/views/calendar_alarm_views.xml` (12 lines)
- `addons/calendar_sms/views/calendar_views.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
