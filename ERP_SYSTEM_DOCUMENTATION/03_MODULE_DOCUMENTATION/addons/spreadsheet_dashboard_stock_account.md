# Module: spreadsheet_dashboard_stock_account

- **Module ID:** MOD-556
- **Path:** `addons/spreadsheet_dashboard_stock_account`
- **Manifest:** `addons/spreadsheet_dashboard_stock_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['stock_account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `stock_account`.

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
    "stock_account"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_stock_account/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_stock_account/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_stock_account/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_stock_account/data/files/warehouse_metrics_dashboard.json` (1,300 lines)
- `addons/spreadsheet_dashboard_stock_account/data/files/warehouse_metrics_sample_dashboard.json` (1,006 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ar.po` (162 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/az.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/bg.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/bs.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ca.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/cs.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/da.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/de.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/el.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/es.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/es_419.po` (163 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/et.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/fa.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/fi.po` (163 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/fr.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/he.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/hi.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/hr.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/hu.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/id.po` (163 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/it.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ja.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/kab.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ko.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ku.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/lo.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/lt.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/lv.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/mn.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/my.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/nb.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/nl.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/pl.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/pt.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/pt_BR.po` (164 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ro.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/ru.po` (164 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/sk.po` (159 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/sl.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/spreadsheet_dashboard_stock_account.pot` (156 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/sr@latin.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/sv.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/th.po` (161 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/tr.po` (164 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/uk.po` (160 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/uz.po` (180 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/vi.po` (162 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/zh_CN.po` (162 lines)
- `addons/spreadsheet_dashboard_stock_account/i18n/zh_TW.po` (162 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
