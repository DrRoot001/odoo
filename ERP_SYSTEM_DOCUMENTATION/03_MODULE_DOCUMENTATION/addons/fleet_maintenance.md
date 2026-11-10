# Module: fleet_maintenance

- **Module ID:** MOD-073
- **Path:** `addons/fleet_maintenance`
- **Manifest:** `addons/fleet_maintenance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrates Fleet and Maintenance

Bridge between Fleet and Maintenance.

Declared dependencies: `fleet`, `maintenance`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "fleet",
    "maintenance"
  ],
  "data": [
    "security/fleet_maintenance_security.xml",
    "views/maintenance_equipment_views.xml",
    "views/fleet_vehicle_views.xml"
  ]
}
```

### Representative source files

- `addons/fleet_maintenance/__init__.py` (3 lines)
- `addons/fleet_maintenance/__manifest__.py` (18 lines)
- `addons/fleet_maintenance/i18n/ar.po` (82 lines)
- `addons/fleet_maintenance/i18n/az.po` (81 lines)
- `addons/fleet_maintenance/i18n/bg.po` (81 lines)
- `addons/fleet_maintenance/i18n/bs.po` (82 lines)
- `addons/fleet_maintenance/i18n/ca.po` (81 lines)
- `addons/fleet_maintenance/i18n/cs.po` (81 lines)
- `addons/fleet_maintenance/i18n/da.po` (81 lines)
- `addons/fleet_maintenance/i18n/de.po` (82 lines)
- `addons/fleet_maintenance/i18n/el.po` (81 lines)
- `addons/fleet_maintenance/i18n/es.po` (82 lines)
- `addons/fleet_maintenance/i18n/es_419.po` (82 lines)
- `addons/fleet_maintenance/i18n/et.po` (81 lines)
- `addons/fleet_maintenance/i18n/fa.po` (81 lines)
- `addons/fleet_maintenance/i18n/fi.po` (82 lines)
- `addons/fleet_maintenance/i18n/fleet_maintenance.pot` (78 lines)
- `addons/fleet_maintenance/i18n/fr.po` (83 lines)
- `addons/fleet_maintenance/i18n/he.po` (82 lines)
- `addons/fleet_maintenance/i18n/hi.po` (81 lines)
- `addons/fleet_maintenance/i18n/hr.po` (82 lines)
- `addons/fleet_maintenance/i18n/hu.po` (81 lines)
- `addons/fleet_maintenance/i18n/id.po` (81 lines)
- `addons/fleet_maintenance/i18n/it.po` (82 lines)
- `addons/fleet_maintenance/i18n/ja.po` (82 lines)
- `addons/fleet_maintenance/i18n/kab.po` (81 lines)
- `addons/fleet_maintenance/i18n/ko.po` (81 lines)
- `addons/fleet_maintenance/i18n/ku.po` (81 lines)
- `addons/fleet_maintenance/i18n/lo.po` (81 lines)
- `addons/fleet_maintenance/i18n/lt.po` (83 lines)
- `addons/fleet_maintenance/i18n/lv.po` (82 lines)
- `addons/fleet_maintenance/i18n/mn.po` (81 lines)
- `addons/fleet_maintenance/i18n/my.po` (82 lines)
- `addons/fleet_maintenance/i18n/nb.po` (81 lines)
- `addons/fleet_maintenance/i18n/nl.po` (82 lines)
- `addons/fleet_maintenance/i18n/pl.po` (82 lines)
- `addons/fleet_maintenance/i18n/pt.po` (81 lines)
- `addons/fleet_maintenance/i18n/pt_BR.po` (82 lines)
- `addons/fleet_maintenance/i18n/ro.po` (82 lines)
- `addons/fleet_maintenance/i18n/ru.po` (82 lines)
- `addons/fleet_maintenance/i18n/sk.po` (81 lines)
- `addons/fleet_maintenance/i18n/sl.po` (82 lines)
- `addons/fleet_maintenance/i18n/sr@latin.po` (82 lines)
- `addons/fleet_maintenance/i18n/sv.po` (82 lines)
- `addons/fleet_maintenance/i18n/th.po` (82 lines)
- `addons/fleet_maintenance/i18n/tr.po` (81 lines)
- `addons/fleet_maintenance/i18n/uk.po` (82 lines)
- `addons/fleet_maintenance/i18n/uz.po` (81 lines)
- `addons/fleet_maintenance/i18n/vi.po` (81 lines)
- `addons/fleet_maintenance/i18n/zh_CN.po` (83 lines)
- `addons/fleet_maintenance/i18n/zh_TW.po` (81 lines)
- `addons/fleet_maintenance/models/__init__.py` (4 lines)
- `addons/fleet_maintenance/models/fleet_vehicle.py` (20 lines)
- `addons/fleet_maintenance/models/maintenance_equipment.py` (48 lines)
- `addons/fleet_maintenance/security/fleet_maintenance_security.xml` (7 lines)
- `addons/fleet_maintenance/views/fleet_vehicle_views.xml` (21 lines)
- `addons/fleet_maintenance/views/maintenance_equipment_views.xml` (65 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
