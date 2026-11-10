# Module: spreadsheet_dashboard_hr_timesheet

- **Module ID:** MOD-550
- **Path:** `addons/spreadsheet_dashboard_hr_timesheet`
- **Manifest:** `addons/spreadsheet_dashboard_hr_timesheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['hr_timesheet']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `hr_timesheet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet_dashboard",
    "hr_timesheet"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_hr_timesheet/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/data/dashboards.xml` (14 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/data/files/tasks_dashboard.json` (1,305 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/data/files/tasks_sample_dashboard.json` (925 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ar.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/az.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/bg.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/bs.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ca.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/cs.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/da.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/de.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/el.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/es.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/es_419.po` (200 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/et.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/fa.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/fi.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/fr.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/he.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/hi.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/hr.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/hu.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/id.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/it.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ja.po` (200 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/kab.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ko.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ku.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/lo.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/lt.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/lv.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/mn.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/my.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/nb.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/nl.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/pl.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/pt.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/pt_BR.po` (200 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ro.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/ru.po` (200 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/sk.po` (197 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/sl.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/spreadsheet_dashboard_hr_timesheet.pot` (194 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/sr@latin.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/sv.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/th.po` (199 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/tr.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/uk.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/uz.po` (229 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/vi.po` (198 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/zh_CN.po` (200 lines)
- `addons/spreadsheet_dashboard_hr_timesheet/i18n/zh_TW.po` (201 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
