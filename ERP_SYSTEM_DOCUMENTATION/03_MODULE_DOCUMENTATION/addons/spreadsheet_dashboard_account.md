# Module: spreadsheet_dashboard_account

- **Module ID:** MOD-547
- **Path:** `addons/spreadsheet_dashboard_account`
- **Manifest:** `addons/spreadsheet_dashboard_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['spreadsheet_account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `spreadsheet_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet_dashboard",
    "spreadsheet_account"
  ],
  "data": [
    "data/dashboards.xml"
  ],
  "assets": {
    "spreadsheet.o_spreadsheet": [
      "spreadsheet_dashboard_account/static/src/bundle/**/*.js"
    ],
    "web.assets_unit_tests": [
      "spreadsheet_dashboard_account/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/spreadsheet_dashboard_account/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_account/__manifest__.py` (22 lines)
- `addons/spreadsheet_dashboard_account/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_account/data/files/invoicing_dashboard.json` (1,434 lines)
- `addons/spreadsheet_dashboard_account/data/files/invoicing_sample_dashboard.json` (1,123 lines)
- `addons/spreadsheet_dashboard_account/i18n/ar.po` (256 lines)
- `addons/spreadsheet_dashboard_account/i18n/az.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/bg.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/bs.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/ca.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/cs.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/da.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/de.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/el.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/es.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/es_419.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/et.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/fa.po` (261 lines)
- `addons/spreadsheet_dashboard_account/i18n/fi.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/fr.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/he.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/hi.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/hr.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/hu.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/id.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/it.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/ja.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/kab.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/ko.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/ku.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/lo.po` (253 lines)
- `addons/spreadsheet_dashboard_account/i18n/lt.po` (256 lines)
- `addons/spreadsheet_dashboard_account/i18n/lv.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/mn.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/my.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/nb.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/nl.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/pl.po` (256 lines)
- `addons/spreadsheet_dashboard_account/i18n/pt.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/pt_BR.po` (256 lines)
- `addons/spreadsheet_dashboard_account/i18n/ro.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/ru.po` (257 lines)
- `addons/spreadsheet_dashboard_account/i18n/sk.po` (253 lines)
- `addons/spreadsheet_dashboard_account/i18n/sl.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/spreadsheet_dashboard_account.pot` (250 lines)
- `addons/spreadsheet_dashboard_account/i18n/sr@latin.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/sv.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/th.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/tr.po` (257 lines)
- `addons/spreadsheet_dashboard_account/i18n/uk.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/uz.po` (293 lines)
- `addons/spreadsheet_dashboard_account/i18n/vi.po` (254 lines)
- `addons/spreadsheet_dashboard_account/i18n/zh_CN.po` (255 lines)
- `addons/spreadsheet_dashboard_account/i18n/zh_TW.po` (258 lines)
- `addons/spreadsheet_dashboard_account/static/src/bundle/account_dashboard_loader.js` (15 lines)
- `addons/spreadsheet_dashboard_account/static/tests/fiscal_year_filter_dashboard.test.js` (91 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
