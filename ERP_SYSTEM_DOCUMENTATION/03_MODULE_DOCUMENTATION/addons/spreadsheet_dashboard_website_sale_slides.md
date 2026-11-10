# Module: spreadsheet_dashboard_website_sale_slides

- **Module ID:** MOD-558
- **Path:** `addons/spreadsheet_dashboard_website_sale_slides`
- **Manifest:** `addons/spreadsheet_dashboard_website_sale_slides/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['website_sale_slides']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `website_sale_slides`.

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
    "website_sale_slides"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_website_sale_slides/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/data/files/elearning_dashboard.json` (612 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/data/files/elearning_sample_dashboard.json` (314 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ar.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/az.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/bg.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/bs.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ca.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/cs.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/da.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/de.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/el.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/es.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/es_419.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/et.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/fa.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/fi.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/fr.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/he.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/hi.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/hr.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/hu.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/id.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/it.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ja.po` (116 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/kab.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ko.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ku.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/lo.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/lt.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/lv.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/mn.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/my.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/nb.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/nl.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/pl.po` (116 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/pt.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/pt_BR.po` (116 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ro.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/ru.po` (117 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/sk.po` (113 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/sl.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/spreadsheet_dashboard_website_sale_slides.pot` (110 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/sr@latin.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/sv.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/th.po` (115 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/tr.po` (116 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/uk.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/uz.po` (134 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/vi.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/zh_CN.po` (114 lines)
- `addons/spreadsheet_dashboard_website_sale_slides/i18n/zh_TW.po` (118 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
