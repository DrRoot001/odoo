# Module: l10n_in_purchase_stock

- **Module ID:** MOD-235
- **Path:** `addons/l10n_in_purchase_stock`
- **Manifest:** `addons/l10n_in_purchase_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Get warehouse address if the bill is created from Purchase Order


Get the warehouse address if the bill is created from the Purchase Order

So this module is to get the warehouse address if the bill is created from Purchase Order
    

Declared dependencies: `l10n_in_stock`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in_stock",
    "purchase_stock"
  ]
}
```

### Representative source files

- `addons/l10n_in_purchase_stock/__init__.py` (4 lines)
- `addons/l10n_in_purchase_stock/__manifest__.py` (24 lines)
- `addons/l10n_in_purchase_stock/i18n/hi.po` (69 lines)
- `addons/l10n_in_purchase_stock/i18n/l10n_in_purchase_stock.pot` (64 lines)
- `addons/l10n_in_purchase_stock/models/__init__.py` (5 lines)
- `addons/l10n_in_purchase_stock/models/account_move.py` (18 lines)
- `addons/l10n_in_purchase_stock/models/stock_move.py` (35 lines)
- `addons/l10n_in_purchase_stock/models/stock_picking.py` (19 lines)
- `addons/l10n_in_purchase_stock/tests/__init__.py` (1 lines)
- `addons/l10n_in_purchase_stock/tests/test_purchase_stock_fiscal_position.py` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
