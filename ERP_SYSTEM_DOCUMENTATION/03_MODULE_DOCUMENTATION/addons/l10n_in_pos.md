# Module: l10n_in_pos

- **Module ID:** MOD-234
- **Path:** `addons/l10n_in_pos`
- **Manifest:** `addons/l10n_in_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

GST Point of Sale

Declared dependencies: `l10n_in`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 27 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 13 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 14 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in",
    "point_of_sale"
  ],
  "data": [
    "views/pos_order_line_views.xml",
    "views/pos_payment_method_views.xml",
    "views/report_invoice.xml",
    "views/product_view.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "data/pos_bill_data.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "demo": [
    "data/product_demo.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_in/static/src/helpers/hsn_summary.js",
      "l10n_in_pos/static/src/app/**/*"
    ],
    "web.assets_tests": [
      "l10n_in_pos/static/tests/tours/**/*"
    ],
    "point_of_sale.customer_display_assets": [
      "l10n_in_pos/static/src/customer_display/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_in_pos/__init__.py` (5 lines)
- `addons/l10n_in_pos/__manifest__.py` (39 lines)
- `addons/l10n_in_pos/data/pos_bill_data.xml` (8 lines)
- `addons/l10n_in_pos/data/product_demo.xml` (40 lines)
- `addons/l10n_in_pos/i18n/hi.po` (374 lines)
- `addons/l10n_in_pos/i18n/l10n_in_pos.pot` (370 lines)
- `addons/l10n_in_pos/models/__init__.py` (16 lines)
- `addons/l10n_in_pos/models/account_move.py` (14 lines)
- `addons/l10n_in_pos/models/account_move_line.py` (41 lines)
- `addons/l10n_in_pos/models/account_tax.py` (11 lines)
- `addons/l10n_in_pos/models/pos_bill.py` (15 lines)
- `addons/l10n_in_pos/models/pos_config.py` (8 lines)
- `addons/l10n_in_pos/models/pos_order.py` (38 lines)
- `addons/l10n_in_pos/models/pos_order_line.py` (34 lines)
- `addons/l10n_in_pos/models/pos_payment_method.py` (46 lines)
- `addons/l10n_in_pos/models/pos_session.py` (61 lines)
- `addons/l10n_in_pos/models/product.py` (70 lines)
- `addons/l10n_in_pos/models/product_template.py` (14 lines)
- `addons/l10n_in_pos/models/res_company.py` (14 lines)
- `addons/l10n_in_pos/models/res_partner_bank.py` (20 lines)
- `addons/l10n_in_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_in_pos/receipt/pos_order_receipt.py` (30 lines)
- `addons/l10n_in_pos/receipt/pos_order_receipt.xml` (54 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/cash_move_popup/cash_move_popup.js` (15 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/closing_popup/closing_popup.js` (34 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/company_state_dialog/company_state_dialog.js` (23 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/company_state_dialog/company_state_dialog.xml` (23 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/hsn_code_dialog/hsn_code_dialog.js` (27 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/hsn_code_dialog/hsn_code_dialog.xml` (25 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/product_info_popup/product_info_popup.js` (13 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/qr_code_popup/qr_code_popup.js` (6 lines)
- `addons/l10n_in_pos/static/src/app/components/popups/qr_code_popup/qr_code_popup.xml` (15 lines)
- `addons/l10n_in_pos/static/src/app/models/invoice_button.js` (15 lines)
- `addons/l10n_in_pos/static/src/app/models/payment_screen.js` (20 lines)
- `addons/l10n_in_pos/static/src/app/models/pos_order.js` (43 lines)
- `addons/l10n_in_pos/static/src/app/models/pos_order_line.js` (15 lines)
- `addons/l10n_in_pos/static/src/app/models/pos_payment.js` (18 lines)
- `addons/l10n_in_pos/static/src/app/utils/printer/generate_printer_data.js` (18 lines)
- `addons/l10n_in_pos/static/src/customer_display/customer_display.xml` (15 lines)
- `addons/l10n_in_pos/static/tests/tours/product_screen_tour.js` (19 lines)
- `addons/l10n_in_pos/static/tests/tours/test_hsn_summary.js` (60 lines)
- `addons/l10n_in_pos/tests/__init__.py` (10 lines)
- `addons/l10n_in_pos/tests/common.py` (94 lines)
- `addons/l10n_in_pos/tests/test_gstr_section.py` (39 lines)
- `addons/l10n_in_pos/tests/test_hsn_summary.py` (33 lines)
- `addons/l10n_in_pos/tests/test_in_pos.py` (74 lines)
- `addons/l10n_in_pos/tests/test_order_receipt.py` (30 lines)
- `addons/l10n_in_pos/tests/test_pos_flow.py` (72 lines)
- `addons/l10n_in_pos/tests/test_product_screen.py` (27 lines)
- `addons/l10n_in_pos/tests/test_standard_flows.py` (21 lines)
- `addons/l10n_in_pos/views/pos_order_line_views.xml` (13 lines)
- `addons/l10n_in_pos/views/pos_payment_method_views.xml` (14 lines)
- `addons/l10n_in_pos/views/product_view.xml` (41 lines)
- `addons/l10n_in_pos/views/report_invoice.xml` (8 lines)
- `addons/l10n_in_pos/views/res_config_settings_views.xml` (15 lines)
- `addons/l10n_in_pos/views/res_partner_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
