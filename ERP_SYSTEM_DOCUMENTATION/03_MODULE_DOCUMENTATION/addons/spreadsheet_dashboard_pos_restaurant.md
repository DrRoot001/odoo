# Module: spreadsheet_dashboard_pos_restaurant

- **Module ID:** MOD-553
- **Path:** `addons/spreadsheet_dashboard_pos_restaurant`
- **Manifest:** `addons/spreadsheet_dashboard_pos_restaurant/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['pos_hr', 'pos_restaurant']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `pos_hr`, `pos_restaurant`.

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
    "pos_hr",
    "pos_restaurant"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_pos_restaurant/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/data/files/pos_restaurant_dashboard.json` (1,597 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/data/files/pos_restaurant_sample_dashboard.json` (1,385 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ar.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/az.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/bg.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/bs.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ca.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/cs.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/da.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/de.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/el.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/es.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/es_419.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/et.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/fa.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/fi.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/fr.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/he.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/hi.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/hr.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/hu.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/id.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/it.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ja.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/kab.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ko.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ku.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/lo.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/lt.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/lv.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/mn.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/my.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/nb.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/nl.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/pl.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/pt.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/pt_BR.po` (228 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ro.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/ru.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/sk.po` (223 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/sl.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/spreadsheet_dashboard_pos_restaurant.pot` (220 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/sr@latin.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/sv.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/th.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/tr.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/uk.po` (224 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/uz.po` (247 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/vi.po` (225 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/zh_CN.po` (226 lines)
- `addons/spreadsheet_dashboard_pos_restaurant/i18n/zh_TW.po` (228 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
