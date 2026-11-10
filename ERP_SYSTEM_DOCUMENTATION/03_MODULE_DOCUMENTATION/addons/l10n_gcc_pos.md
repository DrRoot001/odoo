# Module: l10n_gcc_pos

- **Module ID:** MOD-201
- **Path:** `addons/l10n_gcc_pos`
- **Manifest:** `addons/l10n_gcc_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Adds Arabic as a secondary language on your receipt
    

Declared dependencies: `point_of_sale`, `l10n_gcc_invoice`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "l10n_gcc_invoice"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_gcc_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_gcc_pos/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_gcc_pos/__init__.py` (2 lines)
- `addons/l10n_gcc_pos/__manifest__.py` (24 lines)
- `addons/l10n_gcc_pos/models/__init__.py` (2 lines)
- `addons/l10n_gcc_pos/models/pos_config.py` (7 lines)
- `addons/l10n_gcc_pos/models/res_config_settings.py` (7 lines)
- `addons/l10n_gcc_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_gcc_pos/receipt/pos_order_receipt.py` (17 lines)
- `addons/l10n_gcc_pos/receipt/pos_order_receipt.xml` (98 lines)
- `addons/l10n_gcc_pos/static/src/app/models/pos_order.js` (25 lines)
- `addons/l10n_gcc_pos/static/src/app/utils/printer/generate_printer_data.js` (15 lines)
- `addons/l10n_gcc_pos/static/tests/pos/tours/gcc_receipt_header_tour.js` (57 lines)
- `addons/l10n_gcc_pos/tests/__init__.py` (4 lines)
- `addons/l10n_gcc_pos/tests/test_gcc_pos.py` (60 lines)
- `addons/l10n_gcc_pos/tests/test_order_receipt.py` (35 lines)
- `addons/l10n_gcc_pos/views/res_config_settings_views.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
