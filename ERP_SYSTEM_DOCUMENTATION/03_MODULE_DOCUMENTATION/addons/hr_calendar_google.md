# Module: hr_calendar_google

- **Module ID:** MOD-085
- **Path:** `addons/hr_calendar_google`
- **Manifest:** `addons/hr_calendar_google/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `hr_calendar`, `google_calendar`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_calendar",
    "google_calendar"
  ],
  "data": [
    "data/ir_cron_data.xml"
  ]
}
```

### Representative source files

- `addons/hr_calendar_google/__init__.py` (1 lines)
- `addons/hr_calendar_google/__manifest__.py` (13 lines)
- `addons/hr_calendar_google/data/ir_cron_data.xml` (16 lines)
- `addons/hr_calendar_google/i18n/ar.po` (70 lines)
- `addons/hr_calendar_google/i18n/az.po` (69 lines)
- `addons/hr_calendar_google/i18n/bg.po` (69 lines)
- `addons/hr_calendar_google/i18n/bs.po` (70 lines)
- `addons/hr_calendar_google/i18n/ca.po` (69 lines)
- `addons/hr_calendar_google/i18n/cs.po` (69 lines)
- `addons/hr_calendar_google/i18n/da.po` (69 lines)
- `addons/hr_calendar_google/i18n/de.po` (73 lines)
- `addons/hr_calendar_google/i18n/el.po` (69 lines)
- `addons/hr_calendar_google/i18n/es.po` (70 lines)
- `addons/hr_calendar_google/i18n/es_419.po` (73 lines)
- `addons/hr_calendar_google/i18n/et.po` (69 lines)
- `addons/hr_calendar_google/i18n/fa.po` (69 lines)
- `addons/hr_calendar_google/i18n/fi.po` (70 lines)
- `addons/hr_calendar_google/i18n/fr.po` (73 lines)
- `addons/hr_calendar_google/i18n/he.po` (70 lines)
- `addons/hr_calendar_google/i18n/hi.po` (69 lines)
- `addons/hr_calendar_google/i18n/hr.po` (70 lines)
- `addons/hr_calendar_google/i18n/hr_calendar_google.pot` (66 lines)
- `addons/hr_calendar_google/i18n/hu.po` (69 lines)
- `addons/hr_calendar_google/i18n/id.po` (69 lines)
- `addons/hr_calendar_google/i18n/it.po` (73 lines)
- `addons/hr_calendar_google/i18n/ja.po` (73 lines)
- `addons/hr_calendar_google/i18n/kab.po` (69 lines)
- `addons/hr_calendar_google/i18n/ko.po` (69 lines)
- `addons/hr_calendar_google/i18n/ku.po` (69 lines)
- `addons/hr_calendar_google/i18n/lo.po` (69 lines)
- `addons/hr_calendar_google/i18n/lt.po` (71 lines)
- `addons/hr_calendar_google/i18n/lv.po` (70 lines)
- `addons/hr_calendar_google/i18n/mn.po` (69 lines)
- `addons/hr_calendar_google/i18n/my.po` (69 lines)
- `addons/hr_calendar_google/i18n/nb.po` (69 lines)
- `addons/hr_calendar_google/i18n/nl.po` (73 lines)
- `addons/hr_calendar_google/i18n/pl.po` (70 lines)
- `addons/hr_calendar_google/i18n/pt.po` (69 lines)
- `addons/hr_calendar_google/i18n/pt_BR.po` (75 lines)
- `addons/hr_calendar_google/i18n/ro.po` (70 lines)
- `addons/hr_calendar_google/i18n/ru.po` (70 lines)
- `addons/hr_calendar_google/i18n/sk.po` (69 lines)
- `addons/hr_calendar_google/i18n/sl.po` (70 lines)
- `addons/hr_calendar_google/i18n/sr@latin.po` (70 lines)
- `addons/hr_calendar_google/i18n/sv.po` (70 lines)
- `addons/hr_calendar_google/i18n/th.po` (70 lines)
- `addons/hr_calendar_google/i18n/tr.po` (69 lines)
- `addons/hr_calendar_google/i18n/uk.po` (70 lines)
- `addons/hr_calendar_google/i18n/uz.po` (69 lines)
- `addons/hr_calendar_google/i18n/vi.po` (69 lines)
- `addons/hr_calendar_google/i18n/zh_CN.po` (73 lines)
- `addons/hr_calendar_google/i18n/zh_TW.po` (69 lines)
- `addons/hr_calendar_google/models/__init__.py` (2 lines)
- `addons/hr_calendar_google/models/google_sync.py` (68 lines)
- `addons/hr_calendar_google/models/res_users.py` (56 lines)
- `addons/hr_calendar_google/tests/__init__.py` (1 lines)
- `addons/hr_calendar_google/tests/test_work_location_sync.py` (113 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
