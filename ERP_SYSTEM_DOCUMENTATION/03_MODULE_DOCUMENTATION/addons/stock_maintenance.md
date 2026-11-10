# Module: stock_maintenance

- **Module ID:** MOD-565
- **Path:** `addons/stock_maintenance`
- **Manifest:** `addons/stock_maintenance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

See lots used in maintenance


Stock in Maintenance
====================
Open the record of the serial number from an equipment form


Declared dependencies: `stock`, `maintenance`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock",
    "maintenance"
  ],
  "data": [
    "views/maintenance_views.xml",
    "views/stock_location.xml"
  ]
}
```

### Representative source files

- `addons/stock_maintenance/__init__.py` (3 lines)
- `addons/stock_maintenance/__manifest__.py` (20 lines)
- `addons/stock_maintenance/i18n/ar.po` (99 lines)
- `addons/stock_maintenance/i18n/az.po` (94 lines)
- `addons/stock_maintenance/i18n/bg.po` (94 lines)
- `addons/stock_maintenance/i18n/bs.po` (95 lines)
- `addons/stock_maintenance/i18n/ca.po` (98 lines)
- `addons/stock_maintenance/i18n/cs.po` (94 lines)
- `addons/stock_maintenance/i18n/da.po` (95 lines)
- `addons/stock_maintenance/i18n/de.po` (101 lines)
- `addons/stock_maintenance/i18n/el.po` (95 lines)
- `addons/stock_maintenance/i18n/es.po` (102 lines)
- `addons/stock_maintenance/i18n/es_419.po` (98 lines)
- `addons/stock_maintenance/i18n/et.po` (97 lines)
- `addons/stock_maintenance/i18n/fa.po` (94 lines)
- `addons/stock_maintenance/i18n/fi.po` (98 lines)
- `addons/stock_maintenance/i18n/fr.po` (98 lines)
- `addons/stock_maintenance/i18n/he.po` (95 lines)
- `addons/stock_maintenance/i18n/hi.po` (94 lines)
- `addons/stock_maintenance/i18n/hr.po` (95 lines)
- `addons/stock_maintenance/i18n/hu.po` (94 lines)
- `addons/stock_maintenance/i18n/id.po` (98 lines)
- `addons/stock_maintenance/i18n/it.po` (97 lines)
- `addons/stock_maintenance/i18n/ja.po` (97 lines)
- `addons/stock_maintenance/i18n/kab.po` (94 lines)
- `addons/stock_maintenance/i18n/ko.po` (98 lines)
- `addons/stock_maintenance/i18n/ku.po` (94 lines)
- `addons/stock_maintenance/i18n/lo.po` (93 lines)
- `addons/stock_maintenance/i18n/lt.po` (96 lines)
- `addons/stock_maintenance/i18n/lv.po` (94 lines)
- `addons/stock_maintenance/i18n/mn.po` (94 lines)
- `addons/stock_maintenance/i18n/my.po` (95 lines)
- `addons/stock_maintenance/i18n/nb.po` (94 lines)
- `addons/stock_maintenance/i18n/nl.po` (99 lines)
- `addons/stock_maintenance/i18n/pl.po` (99 lines)
- `addons/stock_maintenance/i18n/pt.po` (95 lines)
- `addons/stock_maintenance/i18n/pt_BR.po` (102 lines)
- `addons/stock_maintenance/i18n/ro.po` (95 lines)
- `addons/stock_maintenance/i18n/ru.po` (99 lines)
- `addons/stock_maintenance/i18n/sk.po` (93 lines)
- `addons/stock_maintenance/i18n/sl.po` (95 lines)
- `addons/stock_maintenance/i18n/sr@latin.po` (95 lines)
- `addons/stock_maintenance/i18n/stock_maintenance.pot` (90 lines)
- `addons/stock_maintenance/i18n/sv.po` (98 lines)
- `addons/stock_maintenance/i18n/th.po` (98 lines)
- `addons/stock_maintenance/i18n/tr.po` (99 lines)
- `addons/stock_maintenance/i18n/uk.po` (95 lines)
- `addons/stock_maintenance/i18n/uz.po` (110 lines)
- `addons/stock_maintenance/i18n/vi.po` (95 lines)
- `addons/stock_maintenance/i18n/zh_CN.po` (102 lines)
- `addons/stock_maintenance/i18n/zh_TW.po` (101 lines)
- `addons/stock_maintenance/models/__init__.py` (4 lines)
- `addons/stock_maintenance/models/maintenance.py` (44 lines)
- `addons/stock_maintenance/models/stock_location.py` (18 lines)
- `addons/stock_maintenance/views/maintenance_views.xml` (22 lines)
- `addons/stock_maintenance/views/stock_location.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
