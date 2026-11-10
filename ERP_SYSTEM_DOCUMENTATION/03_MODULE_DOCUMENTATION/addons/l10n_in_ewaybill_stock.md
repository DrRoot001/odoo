# Module: l10n_in_ewaybill_stock

- **Module ID:** MOD-232
- **Path:** `addons/l10n_in_ewaybill_stock`
- **Manifest:** `addons/l10n_in_ewaybill_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Indian E-waybill for Stock
==========================

This module enables users to create E-waybill from Inventory App without generating an invoice
    

Declared dependencies: `l10n_in_stock`, `l10n_in_ewaybill`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in_stock",
    "l10n_in_ewaybill"
  ],
  "data": [
    "data/ewaybill_type_data.xml",
    "views/l10n_in_ewaybill_views.xml",
    "views/stock_picking_views.xml",
    "report/ewaybill_report_inherit.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_in_ewaybill_stock/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill_stock/__manifest__.py` (27 lines)
- `addons/l10n_in_ewaybill_stock/data/ewaybill_type_data.xml` (74 lines)
- `addons/l10n_in_ewaybill_stock/i18n/hi.po` (240 lines)
- `addons/l10n_in_ewaybill_stock/i18n/l10n_in_ewaybill_stock.pot` (235 lines)
- `addons/l10n_in_ewaybill_stock/models/__init__.py` (5 lines)
- `addons/l10n_in_ewaybill_stock/models/l10n_in_ewaybill.py` (292 lines)
- `addons/l10n_in_ewaybill_stock/models/stock_move.py` (53 lines)
- `addons/l10n_in_ewaybill_stock/models/stock_picking.py` (65 lines)
- `addons/l10n_in_ewaybill_stock/report/ewaybill_report_inherit.xml` (16 lines)
- `addons/l10n_in_ewaybill_stock/security/ir.access.csv` (4 lines)
- `addons/l10n_in_ewaybill_stock/tests/__init__.py` (1 lines)
- `addons/l10n_in_ewaybill_stock/tests/test_ewaybill_stock.py` (240 lines)
- `addons/l10n_in_ewaybill_stock/views/l10n_in_ewaybill_views.xml` (73 lines)
- `addons/l10n_in_ewaybill_stock/views/stock_picking_views.xml` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
