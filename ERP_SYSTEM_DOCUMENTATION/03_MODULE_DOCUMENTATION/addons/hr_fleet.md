# Module: hr_fleet

- **Module ID:** MOD-087
- **Path:** `addons/hr_fleet`
- **Manifest:** `addons/hr_fleet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Get history of driven cars by employees

No manifest description declared.

Declared dependencies: `hr`, `fleet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "fleet"
  ],
  "data": [
    "views/hr_employee_views.xml",
    "views/fleet_vehicle_views.xml",
    "views/fleet_vehicle_cost_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_fleet_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_fleet/static/src/views/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_fleet/__init__.py` (3 lines)
- `addons/hr_fleet/__manifest__.py` (24 lines)
- `addons/hr_fleet/data/hr_fleet_demo.xml` (53 lines)
- `addons/hr_fleet/i18n/ar.po` (252 lines)
- `addons/hr_fleet/i18n/az.po` (243 lines)
- `addons/hr_fleet/i18n/bg.po` (243 lines)
- `addons/hr_fleet/i18n/bs.po` (245 lines)
- `addons/hr_fleet/i18n/ca.po` (246 lines)
- `addons/hr_fleet/i18n/cs.po` (250 lines)
- `addons/hr_fleet/i18n/da.po` (250 lines)
- `addons/hr_fleet/i18n/de.po` (261 lines)
- `addons/hr_fleet/i18n/el.po` (244 lines)
- `addons/hr_fleet/i18n/es.po` (253 lines)
- `addons/hr_fleet/i18n/es_419.po` (255 lines)
- `addons/hr_fleet/i18n/et.po` (243 lines)
- `addons/hr_fleet/i18n/fa.po` (243 lines)
- `addons/hr_fleet/i18n/fi.po` (248 lines)
- `addons/hr_fleet/i18n/fr.po` (261 lines)
- `addons/hr_fleet/i18n/he.po` (251 lines)
- `addons/hr_fleet/i18n/hi.po` (243 lines)
- `addons/hr_fleet/i18n/hr.po` (253 lines)
- `addons/hr_fleet/i18n/hr_fleet.pot` (240 lines)
- `addons/hr_fleet/i18n/hu.po` (250 lines)
- `addons/hr_fleet/i18n/id.po` (248 lines)
- `addons/hr_fleet/i18n/it.po` (259 lines)
- `addons/hr_fleet/i18n/ja.po` (250 lines)
- `addons/hr_fleet/i18n/kab.po` (244 lines)
- `addons/hr_fleet/i18n/ko.po` (247 lines)
- `addons/hr_fleet/i18n/ku.po` (243 lines)
- `addons/hr_fleet/i18n/lo.po` (248 lines)
- `addons/hr_fleet/i18n/lt.po` (253 lines)
- `addons/hr_fleet/i18n/lv.po` (244 lines)
- `addons/hr_fleet/i18n/mn.po` (249 lines)
- `addons/hr_fleet/i18n/my.po` (243 lines)
- `addons/hr_fleet/i18n/nb.po` (247 lines)
- `addons/hr_fleet/i18n/nl.po` (257 lines)
- `addons/hr_fleet/i18n/pl.po` (256 lines)
- `addons/hr_fleet/i18n/pt.po` (254 lines)
- `addons/hr_fleet/i18n/pt_BR.po` (257 lines)
- `addons/hr_fleet/i18n/ro.po` (251 lines)
- `addons/hr_fleet/i18n/ru.po` (249 lines)
- `addons/hr_fleet/i18n/sk.po` (243 lines)
- `addons/hr_fleet/i18n/sl.po` (247 lines)
- `addons/hr_fleet/i18n/sr@latin.po` (244 lines)
- `addons/hr_fleet/i18n/sv.po` (249 lines)
- `addons/hr_fleet/i18n/th.po` (247 lines)
- `addons/hr_fleet/i18n/tr.po` (258 lines)
- `addons/hr_fleet/i18n/uk.po` (252 lines)
- `addons/hr_fleet/i18n/uz.po` (277 lines)
- `addons/hr_fleet/i18n/vi.po` (249 lines)
- `addons/hr_fleet/i18n/zh_CN.po` (254 lines)
- `addons/hr_fleet/i18n/zh_TW.po` (253 lines)
- `addons/hr_fleet/models/__init__.py` (10 lines)
- `addons/hr_fleet/models/fleet_vehicle.py` (147 lines)
- `addons/hr_fleet/models/fleet_vehicle_assignation_log.py` (106 lines)
- `addons/hr_fleet/models/fleet_vehicle_log_contract.py` (23 lines)
- `addons/hr_fleet/models/fleet_vehicle_log_services.py` (25 lines)
- `addons/hr_fleet/models/fleet_vehicle_odometer.py` (13 lines)
- `addons/hr_fleet/models/hr_employee.py` (106 lines)
- `addons/hr_fleet/models/hr_employee_departure.py` (53 lines)
- `addons/hr_fleet/models/ir_attachment.py` (14 lines)
- `addons/hr_fleet/security/ir.access.csv` (2 lines)
- `addons/hr_fleet/static/src/views/hr_fleet_kanban/hr_fleet_kanban_controller.js` (40 lines)
- `addons/hr_fleet/static/src/views/hr_fleet_kanban/hr_fleet_kanban_controller.xml` (11 lines)
- `addons/hr_fleet/static/src/views/hr_fleet_kanban/hr_fleet_kanban_view.js` (10 lines)
- `addons/hr_fleet/tests/__init__.py` (4 lines)
- `addons/hr_fleet/tests/test_hr_fleet_driver.py` (237 lines)
- `addons/hr_fleet/views/fleet_vehicle_cost_views.xml` (82 lines)
- `addons/hr_fleet/views/fleet_vehicle_views.xml` (120 lines)
- `addons/hr_fleet/views/hr_employee_views.xml` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
