# Module: l10n_co_pos

- **Module ID:** MOD-153
- **Path:** `addons/l10n_co_pos`
- **Manifest:** `addons/l10n_co_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Colombian - Point of Sale

Declared dependencies: `l10n_co`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_co",
    "point_of_sale"
  ],
  "data": [
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_co_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_co_pos/__init__.py` (2 lines)
- `addons/l10n_co_pos/__manifest__.py` (22 lines)
- `addons/l10n_co_pos/i18n/es_419.po` (49 lines)
- `addons/l10n_co_pos/i18n/l10n_co_pos.pot` (44 lines)
- `addons/l10n_co_pos/models/__init__.py` (1 lines)
- `addons/l10n_co_pos/models/pos_order.py` (11 lines)
- `addons/l10n_co_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_co_pos/receipt/pos_order_receipt.py` (12 lines)
- `addons/l10n_co_pos/receipt/pos_order_receipt.xml` (12 lines)
- `addons/l10n_co_pos/static/src/app/models/pos_order.js` (13 lines)
- `addons/l10n_co_pos/static/src/app/services/pos.js` (8 lines)
- `addons/l10n_co_pos/static/src/app/utils/printer/generate_printer_data.js` (13 lines)
- `addons/l10n_co_pos/tests/__init__.py` (1 lines)
- `addons/l10n_co_pos/tests/test_co_pos.py` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
