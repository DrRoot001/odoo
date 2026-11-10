# Module: spreadsheet_dashboard_hr_expense

- **Module ID:** MOD-549
- **Path:** `addons/spreadsheet_dashboard_hr_expense`
- **Manifest:** `addons/spreadsheet_dashboard_hr_expense/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['sale_expense']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `sale_expense`.

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
    "sale_expense"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_hr_expense/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_hr_expense/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_hr_expense/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_hr_expense/data/files/expense_dashboard.json` (1,063 lines)
- `addons/spreadsheet_dashboard_hr_expense/data/files/expense_sample_dashboard.json` (807 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ar.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/az.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/bg.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/bs.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ca.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/cs.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/da.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/de.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/el.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/es.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/es_419.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/et.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/fa.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/fi.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/fr.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/he.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/hi.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/hr.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/hu.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/id.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/it.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ja.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/kab.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ko.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ku.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/lo.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/lt.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/lv.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/mn.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/my.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/nb.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/nl.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/pl.po` (149 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/pt.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/pt_BR.po` (150 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ro.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/ru.po` (150 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/sk.po` (146 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/sl.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/spreadsheet_dashboard_hr_expense.pot` (143 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/sr@latin.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/sv.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/th.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/tr.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/uk.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/uz.po` (170 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/vi.po` (147 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/zh_CN.po` (148 lines)
- `addons/spreadsheet_dashboard_hr_expense/i18n/zh_TW.po` (150 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
