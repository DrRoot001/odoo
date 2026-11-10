# Module: spreadsheet_dashboard_sale_timesheet

- **Module ID:** MOD-555
- **Path:** `addons/spreadsheet_dashboard_sale_timesheet`
- **Manifest:** `addons/spreadsheet_dashboard_sale_timesheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['sale_timesheet']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `sale_timesheet`.

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
    "sale_timesheet"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_sale_timesheet/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/data/files/timesheet_dashboard.json` (1,423 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/data/files/timesheet_sample_dashboard.json` (1,102 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ar.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/az.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/bg.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/bs.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ca.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/cs.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/da.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/de.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/el.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/es.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/es_419.po` (290 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/et.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/fa.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/fi.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/fr.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/he.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/hi.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/hr.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/hu.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/id.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/it.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ja.po` (290 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/kab.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ko.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ku.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/lo.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/lt.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/lv.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/mn.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/my.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/nb.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/nl.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/pl.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/pt.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/pt_BR.po` (291 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ro.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/ru.po` (290 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/sk.po` (287 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/sl.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/spreadsheet_dashboard_sale_timesheet.pot` (284 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/sr@latin.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/sv.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/th.po` (289 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/tr.po` (290 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/uk.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/uz.po` (320 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/vi.po` (288 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/zh_CN.po` (290 lines)
- `addons/spreadsheet_dashboard_sale_timesheet/i18n/zh_TW.po` (291 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
