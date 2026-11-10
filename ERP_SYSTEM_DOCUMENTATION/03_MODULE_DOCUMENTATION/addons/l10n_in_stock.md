# Module: l10n_in_stock

- **Module ID:** MOD-238
- **Path:** `addons/l10n_in_stock`
- **Manifest:** `addons/l10n_in_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

GST Stock Report

Declared dependencies: `l10n_in`, `stock`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in",
    "stock",
    "stock_account"
  ],
  "data": [
    "views/report_stockpicking_operations.xml"
  ],
  "demo": [
    "data/product_demo.xml",
    "data/warehouse_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_in_stock/__init__.py` (4 lines)
- `addons/l10n_in_stock/__manifest__.py` (22 lines)
- `addons/l10n_in_stock/data/product_demo.xml` (7 lines)
- `addons/l10n_in_stock/data/warehouse_demo.xml` (8 lines)
- `addons/l10n_in_stock/i18n/hi.po` (57 lines)
- `addons/l10n_in_stock/i18n/l10n_in_stock.pot` (53 lines)
- `addons/l10n_in_stock/models/__init__.py` (5 lines)
- `addons/l10n_in_stock/models/stock_move.py` (23 lines)
- `addons/l10n_in_stock/models/stock_picking.py` (33 lines)
- `addons/l10n_in_stock/views/report_stockpicking_operations.xml` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
