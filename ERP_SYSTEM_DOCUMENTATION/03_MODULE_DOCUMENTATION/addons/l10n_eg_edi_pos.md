# Module: l10n_eg_edi_pos

- **Module ID:** MOD-173
- **Path:** `addons/l10n_eg_edi_pos`
- **Manifest:** `addons/l10n_eg_edi_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Submit POS receipts to the Egyptian Tax Authority


Egypt E-Receipts (POS)
======================
Submits POS sales receipts to the Egyptian Tax Authority (ETA) eReceipt API
after order payment. Prints a compliant QR on the receipt when accepted, prints
RECEIPT WITHOUT FISCAL VALUE when not, and tracks ETA state per-order.


Declared dependencies: `point_of_sale`, `l10n_eg_edi_eta`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "l10n_eg_edi_eta"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/pos_order_views.xml",
    "views/pos_payment_method_views.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_eg_edi_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_eg_edi_pos/__init__.py` (2 lines)
- `addons/l10n_eg_edi_pos/__manifest__.py` (28 lines)
- `addons/l10n_eg_edi_pos/i18n/ar.po` (600 lines)
- `addons/l10n_eg_edi_pos/i18n/l10n_eg_edi_pos.pot` (542 lines)
- `addons/l10n_eg_edi_pos/models/__init__.py` (4 lines)
- `addons/l10n_eg_edi_pos/models/pos_config.py` (109 lines)
- `addons/l10n_eg_edi_pos/models/pos_order.py` (432 lines)
- `addons/l10n_eg_edi_pos/models/pos_payment_method.py` (22 lines)
- `addons/l10n_eg_edi_pos/models/res_config_settings.py` (11 lines)
- `addons/l10n_eg_edi_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_eg_edi_pos/receipt/pos_order_receipt.py` (11 lines)
- `addons/l10n_eg_edi_pos/receipt/pos_order_receipt.xml` (24 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/app/utils/generate_printer_data.js` (18 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/models/invoice_button.js` (22 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/screens/feedback_screen.js` (29 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/screens/ticket_screen.js` (29 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/screens/ticket_screen.xml` (10 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/services/pos_store.js` (17 lines)
- `addons/l10n_eg_edi_pos/static/src/overrides/utils/order_payment_validation.js` (38 lines)
- `addons/l10n_eg_edi_pos/tests/__init__.py` (7 lines)
- `addons/l10n_eg_edi_pos/tests/common.py` (289 lines)
- `addons/l10n_eg_edi_pos/tests/test_action_pos_order_paid.py` (70 lines)
- `addons/l10n_eg_edi_pos/tests/test_check_data.py` (96 lines)
- `addons/l10n_eg_edi_pos/tests/test_envelope.py` (55 lines)
- `addons/l10n_eg_edi_pos/tests/test_payload_builders.py` (162 lines)
- `addons/l10n_eg_edi_pos/tests/test_send_flow.py` (120 lines)
- `addons/l10n_eg_edi_pos/tests/test_token_cache.py` (67 lines)
- `addons/l10n_eg_edi_pos/views/pos_order_views.xml` (55 lines)
- `addons/l10n_eg_edi_pos/views/pos_payment_method_views.xml` (13 lines)
- `addons/l10n_eg_edi_pos/views/res_config_settings_views.xml` (53 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
