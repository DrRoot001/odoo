# Module: l10n_pk_edi_pos

- **Module ID:** MOD-297
- **Path:** `addons/l10n_pk_edi_pos`
- **Manifest:** `addons/l10n_pk_edi_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module brings the technical requirement for the Pakistan regulation.
Install this if you are using the Point of Sale app in Pakistan.
    

Declared dependencies: `l10n_pk`, `pos_discount`, `iap`, `stock_delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_pk",
    "pos_discount",
    "iap",
    "stock_delivery"
  ],
  "data": [
    "data/l10n_pk_edi_pos_data.xml",
    "receipt/pos_order_receipt.xml",
    "data/product_data.xml",
    "views/product_views.xml",
    "views/pos_order_views.xml",
    "views/pos_payment_method_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_pk_edi_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_pk_edi_pos/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_pk_edi_pos/__init__.py` (2 lines)
- `addons/l10n_pk_edi_pos/__manifest__.py` (35 lines)
- `addons/l10n_pk_edi_pos/data/l10n_pk_edi_pos_data.xml` (7 lines)
- `addons/l10n_pk_edi_pos/data/product_data.xml` (15 lines)
- `addons/l10n_pk_edi_pos/models/__init__.py` (6 lines)
- `addons/l10n_pk_edi_pos/models/account_move.py` (25 lines)
- `addons/l10n_pk_edi_pos/models/pos_config.py` (62 lines)
- `addons/l10n_pk_edi_pos/models/pos_order.py` (368 lines)
- `addons/l10n_pk_edi_pos/models/pos_payment_method.py` (16 lines)
- `addons/l10n_pk_edi_pos/models/product_template.py` (10 lines)
- `addons/l10n_pk_edi_pos/models/res_config_settings.py` (13 lines)
- `addons/l10n_pk_edi_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_pk_edi_pos/receipt/pos_order_receipt.py` (14 lines)
- `addons/l10n_pk_edi_pos/receipt/pos_order_receipt.xml` (24 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/app/utils/generate_printer_data.js` (13 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/models/invoice_button.js` (22 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/models/pos_order.js` (76 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/models/pos_order_line.js` (13 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/screens/control_buttons.xml` (10 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/screens/order_details_dialog.js` (29 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/screens/ticket_screen.js` (12 lines)
- `addons/l10n_pk_edi_pos/static/src/overrides/screens/ticket_screen.xml` (10 lines)
- `addons/l10n_pk_edi_pos/static/tests/tours/l10n_pk_edi_pos_discount_tour.js` (17 lines)
- `addons/l10n_pk_edi_pos/static/tests/tours/l10n_pk_edi_pos_service_fee_tour.js` (39 lines)
- `addons/l10n_pk_edi_pos/tests/__init__.py` (1 lines)
- `addons/l10n_pk_edi_pos/tests/test_l10n_pk_edi_pos.py` (421 lines)
- `addons/l10n_pk_edi_pos/views/pos_order_views.xml` (57 lines)
- `addons/l10n_pk_edi_pos/views/pos_payment_method_views.xml` (13 lines)
- `addons/l10n_pk_edi_pos/views/product_views.xml` (13 lines)
- `addons/l10n_pk_edi_pos/views/report_invoice.xml` (13 lines)
- `addons/l10n_pk_edi_pos/views/res_config_settings_views.xml` (54 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
