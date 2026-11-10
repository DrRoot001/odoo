# Module: spreadsheet_dashboard_pos_hr

- **Module ID:** MOD-552
- **Path:** `addons/spreadsheet_dashboard_pos_hr`
- **Manifest:** `addons/spreadsheet_dashboard_pos_hr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['pos_hr']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `pos_hr`.

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
    "pos_hr"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_pos_hr/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_pos_hr/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_pos_hr/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_pos_hr/data/files/pos_dashboard.json` (1,281 lines)
- `addons/spreadsheet_dashboard_pos_hr/data/files/pos_sample_dashboard.json` (1,176 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ar.po` (174 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/az.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/bg.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/bs.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ca.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/cs.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/da.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/de.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/el.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/es.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/es_419.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/et.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/fa.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/fi.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/fr.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/he.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/hi.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/hr.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/hu.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/id.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/it.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ja.po` (174 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/kab.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ko.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ku.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/lo.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/lt.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/lv.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/mn.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/my.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/nb.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/nl.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/pl.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/pt.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/pt_BR.po` (175 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ro.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/ru.po` (175 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/sk.po` (171 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/sl.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/spreadsheet_dashboard_pos_hr.pot` (168 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/sr@latin.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/sv.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/th.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/tr.po` (173 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/uk.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/uz.po` (197 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/vi.po` (172 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/zh_CN.po` (174 lines)
- `addons/spreadsheet_dashboard_pos_hr/i18n/zh_TW.po` (175 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
