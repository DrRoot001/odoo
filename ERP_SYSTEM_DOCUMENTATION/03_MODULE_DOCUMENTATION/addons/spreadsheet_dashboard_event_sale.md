# Module: spreadsheet_dashboard_event_sale

- **Module ID:** MOD-548
- **Path:** `addons/spreadsheet_dashboard_event_sale`
- **Manifest:** `addons/spreadsheet_dashboard_event_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['event_sale']`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet

Spreadsheet

Declared dependencies: `spreadsheet_dashboard`, `event_sale`.

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
    "event_sale"
  ],
  "data": [
    "data/dashboards.xml"
  ]
}
```

### Representative source files

- `addons/spreadsheet_dashboard_event_sale/__init__.py` (1 lines)
- `addons/spreadsheet_dashboard_event_sale/__manifest__.py` (14 lines)
- `addons/spreadsheet_dashboard_event_sale/data/dashboards.xml` (15 lines)
- `addons/spreadsheet_dashboard_event_sale/data/files/events_dashboard.json` (1,108 lines)
- `addons/spreadsheet_dashboard_event_sale/data/files/events_sample_dashboard.json` (794 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ar.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/az.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/bg.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/bs.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ca.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/cs.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/da.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/de.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/el.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/es.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/es_419.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/et.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/fa.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/fi.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/fr.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/he.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/hi.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/hr.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/hu.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/id.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/it.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ja.po` (151 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/kab.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ko.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ku.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/lo.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/lt.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/lv.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/mn.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/my.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/nb.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/nl.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/pl.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/pt.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/pt_BR.po` (150 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ro.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/ru.po` (151 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/sk.po` (147 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/sl.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/spreadsheet_dashboard_event_sale.pot` (144 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/sr@latin.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/sv.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/th.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/tr.po` (150 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/uk.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/uz.po` (172 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/vi.po` (148 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/zh_CN.po` (149 lines)
- `addons/spreadsheet_dashboard_event_sale/i18n/zh_TW.po` (152 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
