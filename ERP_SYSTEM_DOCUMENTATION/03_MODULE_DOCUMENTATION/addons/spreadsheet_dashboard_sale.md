# Module: spreadsheet_dashboard_sale

- **Module ID:** MOD-554
- **Path:** `addons/spreadsheet_dashboard_sale`
- **Manifest:** `addons/spreadsheet_dashboard_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['sale']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `sale`.

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
    "sale"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_sale/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_sale/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_sale/data/dashboards.xml` (26 lines)
- `addons/spreadsheet_dashboard_sale/data/files/product_dashboard.json` (843 lines)
- `addons/spreadsheet_dashboard_sale/data/files/product_sample_dashboard.json` (2,822 lines)
- `addons/spreadsheet_dashboard_sale/data/files/sales_dashboard.json` (2,038 lines)
- `addons/spreadsheet_dashboard_sale/data/files/sales_sample_dashboard.json` (1,742 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ar.po` (374 lines)
- `addons/spreadsheet_dashboard_sale/i18n/az.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/bg.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/bs.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ca.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/cs.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/da.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/de.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/el.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/es.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/es_419.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/es_CL.po` (305 lines)
- `addons/spreadsheet_dashboard_sale/i18n/et.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/fa.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/fi.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/fr.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/he.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/hi.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/hr.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/hu.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/id.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/it.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ja.po` (374 lines)
- `addons/spreadsheet_dashboard_sale/i18n/kab.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ko.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ku.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/lo.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/lt.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/lv.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/mn.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/my.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/nb.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/nl.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/pl.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/pt.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/pt_BR.po` (375 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ro.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/ru.po` (376 lines)
- `addons/spreadsheet_dashboard_sale/i18n/sk.po` (371 lines)
- `addons/spreadsheet_dashboard_sale/i18n/sl.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/spreadsheet_dashboard_sale.pot` (368 lines)
- `addons/spreadsheet_dashboard_sale/i18n/sr@latin.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/sv.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/th.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/tr.po` (376 lines)
- `addons/spreadsheet_dashboard_sale/i18n/uk.po` (372 lines)
- `addons/spreadsheet_dashboard_sale/i18n/uz.po` (418 lines)
- `addons/spreadsheet_dashboard_sale/i18n/vi.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/zh_CN.po` (373 lines)
- `addons/spreadsheet_dashboard_sale/i18n/zh_TW.po` (376 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
