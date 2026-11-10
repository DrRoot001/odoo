# Module: account_fleet

- **Module ID:** MOD-007
- **Path:** `addons/account_fleet`
- **Manifest:** `addons/account_fleet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage accounting with fleets

No manifest description declared.

Declared dependencies: `fleet`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "fleet",
    "account"
  ],
  "data": [
    "data/fleet_service_type_data.xml",
    "views/account_move_views.xml",
    "views/fleet_vehicle_views.xml",
    "views/fleet_vehicle_log_services_views.xml",
    "views/account_account_views.xml",
    "views/report_invoice.xml"
  ]
}
```

### Representative source files

- `addons/account_fleet/__init__.py` (5 lines)
- `addons/account_fleet/__manifest__.py` (18 lines)
- `addons/account_fleet/data/fleet_service_type_data.xml` (7 lines)
- `addons/account_fleet/i18n/account_fleet.pot` (209 lines)
- `addons/account_fleet/i18n/ar.po` (231 lines)
- `addons/account_fleet/i18n/az.po` (217 lines)
- `addons/account_fleet/i18n/bg.po` (217 lines)
- `addons/account_fleet/i18n/bs.po` (219 lines)
- `addons/account_fleet/i18n/ca.po` (225 lines)
- `addons/account_fleet/i18n/cs.po` (228 lines)
- `addons/account_fleet/i18n/da.po` (233 lines)
- `addons/account_fleet/i18n/de.po` (234 lines)
- `addons/account_fleet/i18n/el.po` (218 lines)
- `addons/account_fleet/i18n/es.po` (232 lines)
- `addons/account_fleet/i18n/es_419.po` (233 lines)
- `addons/account_fleet/i18n/et.po` (222 lines)
- `addons/account_fleet/i18n/fa.po` (217 lines)
- `addons/account_fleet/i18n/fi.po` (232 lines)
- `addons/account_fleet/i18n/fr.po` (234 lines)
- `addons/account_fleet/i18n/he.po` (218 lines)
- `addons/account_fleet/i18n/hi.po` (222 lines)
- `addons/account_fleet/i18n/hr.po` (218 lines)
- `addons/account_fleet/i18n/hu.po` (218 lines)
- `addons/account_fleet/i18n/id.po` (234 lines)
- `addons/account_fleet/i18n/it.po` (233 lines)
- `addons/account_fleet/i18n/ja.po` (233 lines)
- `addons/account_fleet/i18n/kab.po` (218 lines)
- `addons/account_fleet/i18n/ko.po` (227 lines)
- `addons/account_fleet/i18n/ku.po` (219 lines)
- `addons/account_fleet/i18n/lo.po` (229 lines)
- `addons/account_fleet/i18n/lt.po` (219 lines)
- `addons/account_fleet/i18n/lv.po` (219 lines)
- `addons/account_fleet/i18n/mn.po` (217 lines)
- `addons/account_fleet/i18n/my.po` (219 lines)
- `addons/account_fleet/i18n/nb.po` (217 lines)
- `addons/account_fleet/i18n/nl.po` (234 lines)
- `addons/account_fleet/i18n/pl.po` (226 lines)
- `addons/account_fleet/i18n/pt.po` (225 lines)
- `addons/account_fleet/i18n/pt_BR.po` (231 lines)
- `addons/account_fleet/i18n/ro.po` (225 lines)
- `addons/account_fleet/i18n/ru.po` (228 lines)
- `addons/account_fleet/i18n/sk.po` (218 lines)
- `addons/account_fleet/i18n/sl.po` (226 lines)
- `addons/account_fleet/i18n/sr@latin.po` (218 lines)
- `addons/account_fleet/i18n/sv.po` (233 lines)
- `addons/account_fleet/i18n/th.po` (226 lines)
- `addons/account_fleet/i18n/tr.po` (233 lines)
- `addons/account_fleet/i18n/uk.po` (234 lines)
- `addons/account_fleet/i18n/uz.po` (253 lines)
- `addons/account_fleet/i18n/vi.po` (227 lines)
- `addons/account_fleet/i18n/zh_CN.po` (225 lines)
- `addons/account_fleet/i18n/zh_TW.po` (225 lines)
- `addons/account_fleet/models/__init__.py` (7 lines)
- `addons/account_fleet/models/account_account.py` (17 lines)
- `addons/account_fleet/models/account_move.py` (98 lines)
- `addons/account_fleet/models/account_tax.py` (35 lines)
- `addons/account_fleet/models/fleet_vehicle.py` (44 lines)
- `addons/account_fleet/models/fleet_vehicle_log_services.py` (79 lines)
- `addons/account_fleet/tests/__init__.py` (5 lines)
- `addons/account_fleet/tests/test_account_fleet.py` (49 lines)
- `addons/account_fleet/tests/test_account_fleet_tax_report.py` (114 lines)
- `addons/account_fleet/tests/test_fleet_vehicle_log_services.py` (180 lines)
- `addons/account_fleet/views/account_account_views.xml` (13 lines)
- `addons/account_fleet/views/account_move_views.xml` (55 lines)
- `addons/account_fleet/views/fleet_vehicle_log_services_views.xml` (46 lines)
- `addons/account_fleet/views/fleet_vehicle_views.xml` (20 lines)
- `addons/account_fleet/views/report_invoice.xml` (15 lines)
- `addons/account_fleet/wizard/__init__.py` (3 lines)
- `addons/account_fleet/wizard/account_automatic_entry_wizard.py` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
