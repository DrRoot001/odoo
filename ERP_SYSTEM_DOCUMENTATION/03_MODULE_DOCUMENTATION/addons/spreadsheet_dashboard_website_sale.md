# Module: spreadsheet_dashboard_website_sale

- **Module ID:** MOD-557
- **Path:** `addons/spreadsheet_dashboard_website_sale`
- **Manifest:** `addons/spreadsheet_dashboard_website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['website_sale']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `website_sale`.

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
    "website_sale"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_website_sale/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_website_sale/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_website_sale/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_website_sale/data/files/ecommerce_dashboard.json` (861 lines)
- `addons/spreadsheet_dashboard_website_sale/data/files/ecommerce_sample_dashboard.json` (616 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ar.po` (154 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/az.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/bg.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/bs.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ca.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/cs.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/da.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/de.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/el.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/es.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/es_419.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/et.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/fa.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/fi.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/fr.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/he.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/hi.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/hr.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/hu.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/id.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/it.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ja.po` (154 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/kab.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ko.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ku.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/lo.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/lt.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/lv.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/mn.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/my.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/nb.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/nl.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/pl.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/pt.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/pt_BR.po` (154 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ro.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/ru.po` (155 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/sk.po` (151 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/sl.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/spreadsheet_dashboard_website_sale.pot` (148 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/sr@latin.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/sv.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/th.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/tr.po` (155 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/uk.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/uz.po` (176 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/vi.po` (152 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/zh_CN.po` (153 lines)
- `addons/spreadsheet_dashboard_website_sale/i18n/zh_TW.po` (155 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
