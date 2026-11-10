# Module: l10n_tw_edi_ecpay_pos

- **Module ID:** MOD-329
- **Path:** `addons/l10n_tw_edi_ecpay_pos`
- **Manifest:** `addons/l10n_tw_edi_ecpay_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

ECpay E-invoice bridge module for POS


        This bridge module allows the user to input Ecpay information in pos for sending their invoices to the Ecpay system
    

Declared dependencies: `point_of_sale`, `l10n_tw_edi_ecpay`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "l10n_tw_edi_ecpay"
  ],
  "data": [
    "data/res_partner_data.xml",
    "views/pos_order_view.xml",
    "receipt/ecpay_certificate_receipt.xml",
    "receipt/ecpay_transaction_receipt.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_tw_edi_ecpay_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_tw_edi_ecpay_pos/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "l10n_tw_edi_ecpay_pos/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_tw_edi_ecpay_pos/__init__.py` (4 lines)
- `addons/l10n_tw_edi_ecpay_pos/__manifest__.py` (35 lines)
- `addons/l10n_tw_edi_ecpay_pos/data/res_partner_data.xml` (13 lines)
- `addons/l10n_tw_edi_ecpay_pos/i18n/l10n_tw_edi_ecpay_pos.pot` (559 lines)
- `addons/l10n_tw_edi_ecpay_pos/i18n/zh_TW.po` (535 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/__init__.py` (7 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/account_tax.py` (14 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/ir_ui_view.py` (15 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/pos_config.py` (31 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/pos_order.py` (174 lines)
- `addons/l10n_tw_edi_ecpay_pos/models/pos_session.py` (31 lines)
- `addons/l10n_tw_edi_ecpay_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_tw_edi_ecpay_pos/receipt/ecpay_certificate_receipt.xml` (49 lines)
- `addons/l10n_tw_edi_ecpay_pos/receipt/ecpay_transaction_receipt.xml` (87 lines)
- `addons/l10n_tw_edi_ecpay_pos/receipt/pos_order_receipt.py` (85 lines)
- `addons/l10n_tw_edi_ecpay_pos/receipt/pos_order_receipt.xml` (23 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/components/popups/ecpay_info_popup.js` (228 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/components/popups/ecpay_info_popup.xml` (112 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/models/pos_order.js` (119 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/plugins/pos_ticket_printer_plugin.js` (32 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/screens/payment_screen/payment_screen.js` (32 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/screens/ticket_screen/invoice_button/invoice_button.js` (33 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/screens/ticket_screen/ticket_screen.js` (22 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/services/pos_store.js` (67 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/src/app/utils/printer/generate_printer_data.js` (70 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/tests/tours/ecpay_tour.js` (125 lines)
- `addons/l10n_tw_edi_ecpay_pos/static/tests/unit/ecpay_info_popup.test.js` (63 lines)
- `addons/l10n_tw_edi_ecpay_pos/tests/__init__.py` (4 lines)
- `addons/l10n_tw_edi_ecpay_pos/tests/test_edi_pos_order.py` (188 lines)
- `addons/l10n_tw_edi_ecpay_pos/tests/test_edi_pos_order_ui.py` (65 lines)
- `addons/l10n_tw_edi_ecpay_pos/views/pos_order_view.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
