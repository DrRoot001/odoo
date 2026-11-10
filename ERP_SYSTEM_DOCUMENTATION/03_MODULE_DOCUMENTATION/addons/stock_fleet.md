# Module: stock_fleet

- **Module ID:** MOD-563
- **Path:** `addons/stock_fleet`
- **Manifest:** `addons/stock_fleet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Stock Transport Management

Allows organizing deliveries by dock, assigning drivers and vehicles, and printing the associated consignment notes.

Declared dependencies: `stock`, `fleet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
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
    "fleet"
  ],
  "data": [
    "views/fleet_vehicle_model.xml",
    "views/stock_picking_batch.xml",
    "views/stock_picking_type.xml",
    "views/stock_picking_view.xml",
    "report/report_picking_batch.xml",
    "report/report_picking_cmr.xml",
    "report/stock_fleet_reports.xml",
    "views/stock_location.xml"
  ],
  "demo": [
    "data/stock_fleet_demo.xml"
  ],
  "assets": {
    "web.report_assets_common": [
      "stock_fleet/static/src/scss/report_picking_cmr.scss"
    ]
  }
}
```

### Representative source files

- `addons/stock_fleet/__init__.py` (15 lines)
- `addons/stock_fleet/__manifest__.py` (29 lines)
- `addons/stock_fleet/data/stock_fleet_demo.xml` (55 lines)
- `addons/stock_fleet/i18n/ar.po` (664 lines)
- `addons/stock_fleet/i18n/az.po` (673 lines)
- `addons/stock_fleet/i18n/bg.po` (681 lines)
- `addons/stock_fleet/i18n/bs.po` (678 lines)
- `addons/stock_fleet/i18n/ca.po` (660 lines)
- `addons/stock_fleet/i18n/cs.po` (661 lines)
- `addons/stock_fleet/i18n/da.po` (683 lines)
- `addons/stock_fleet/i18n/de.po` (671 lines)
- `addons/stock_fleet/i18n/el.po` (660 lines)
- `addons/stock_fleet/i18n/es.po` (662 lines)
- `addons/stock_fleet/i18n/es_419.po` (669 lines)
- `addons/stock_fleet/i18n/et.po` (660 lines)
- `addons/stock_fleet/i18n/fa.po` (684 lines)
- `addons/stock_fleet/i18n/fi.po` (664 lines)
- `addons/stock_fleet/i18n/fr.po` (667 lines)
- `addons/stock_fleet/i18n/he.po` (686 lines)
- `addons/stock_fleet/i18n/hi.po` (682 lines)
- `addons/stock_fleet/i18n/hr.po` (717 lines)
- `addons/stock_fleet/i18n/hu.po` (660 lines)
- `addons/stock_fleet/i18n/id.po` (666 lines)
- `addons/stock_fleet/i18n/it.po` (670 lines)
- `addons/stock_fleet/i18n/ja.po` (667 lines)
- `addons/stock_fleet/i18n/kab.po` (665 lines)
- `addons/stock_fleet/i18n/ko.po` (660 lines)
- `addons/stock_fleet/i18n/ku.po` (662 lines)
- `addons/stock_fleet/i18n/lo.po` (672 lines)
- `addons/stock_fleet/i18n/lt.po` (683 lines)
- `addons/stock_fleet/i18n/lv.po` (677 lines)
- `addons/stock_fleet/i18n/mn.po` (677 lines)
- `addons/stock_fleet/i18n/my.po` (669 lines)
- `addons/stock_fleet/i18n/nb.po` (660 lines)
- `addons/stock_fleet/i18n/nl.po` (672 lines)
- `addons/stock_fleet/i18n/pl.po` (663 lines)
- `addons/stock_fleet/i18n/pt.po` (665 lines)
- `addons/stock_fleet/i18n/pt_BR.po` (675 lines)
- `addons/stock_fleet/i18n/ro.po` (718 lines)
- `addons/stock_fleet/i18n/ru.po` (664 lines)
- `addons/stock_fleet/i18n/sk.po` (680 lines)
- `addons/stock_fleet/i18n/sl.po` (661 lines)
- `addons/stock_fleet/i18n/sr@latin.po` (667 lines)
- `addons/stock_fleet/i18n/stock_fleet.pot` (643 lines)
- `addons/stock_fleet/i18n/sv.po` (660 lines)
- `addons/stock_fleet/i18n/th.po` (661 lines)
- `addons/stock_fleet/i18n/tr.po` (664 lines)
- `addons/stock_fleet/i18n/uk.po` (687 lines)
- `addons/stock_fleet/i18n/uz.po` (723 lines)
- `addons/stock_fleet/i18n/vi.po` (662 lines)
- `addons/stock_fleet/i18n/zh_CN.po` (668 lines)
- `addons/stock_fleet/i18n/zh_TW.po` (659 lines)
- `addons/stock_fleet/models/__init__.py` (4 lines)
- `addons/stock_fleet/models/fleet_vehicle_model.py` (31 lines)
- `addons/stock_fleet/models/stock_picking.py` (72 lines)
- `addons/stock_fleet/models/stock_picking_batch.py` (113 lines)
- `addons/stock_fleet/models/stock_warehouse.py` (23 lines)
- `addons/stock_fleet/report/__init__.py` (1 lines)
- `addons/stock_fleet/report/report_picking_batch.xml` (34 lines)
- `addons/stock_fleet/report/report_picking_cmr.py` (173 lines)
- `addons/stock_fleet/report/report_picking_cmr.xml` (637 lines)
- `addons/stock_fleet/report/stock_fleet_reports.xml` (39 lines)
- `addons/stock_fleet/static/src/scss/report_picking_cmr.scss` (18 lines)
- `addons/stock_fleet/views/fleet_vehicle_model.xml` (39 lines)
- `addons/stock_fleet/views/stock_location.xml` (14 lines)
- `addons/stock_fleet/views/stock_picking_batch.xml` (164 lines)
- `addons/stock_fleet/views/stock_picking_type.xml` (64 lines)
- `addons/stock_fleet/views/stock_picking_view.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
