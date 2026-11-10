# Module: l10n_jo_edi_pos

- **Module ID:** MOD-247
- **Path:** `addons/l10n_jo_edi_pos`
- **Manifest:** `addons/l10n_jo_edi_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Jordan Accounting EDI for POS
=============================
Provides electronic invoicing for Jordan in the POS.


Declared dependencies: `l10n_jo_edi`, `pos_edi_ubl`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_jo_edi",
    "pos_edi_ubl"
  ],
  "data": [
    "receipt/pos_order_receipt.xml",
    "views/pos_order_views.xml",
    "views/pos_payment_method_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_jo_edi_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_jo_edi_pos/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_jo_edi_pos/__init__.py` (2 lines)
- `addons/l10n_jo_edi_pos/__manifest__.py` (27 lines)
- `addons/l10n_jo_edi_pos/demo/demo_company.xml` (9 lines)
- `addons/l10n_jo_edi_pos/i18n/ar.po` (374 lines)
- `addons/l10n_jo_edi_pos/i18n/l10n_jo_edi_pos.pot` (366 lines)
- `addons/l10n_jo_edi_pos/models/__init__.py` (6 lines)
- `addons/l10n_jo_edi_pos/models/account_move.py` (11 lines)
- `addons/l10n_jo_edi_pos/models/pos_edi_ubl_21_jo.py` (419 lines)
- `addons/l10n_jo_edi_pos/models/pos_order.py` (224 lines)
- `addons/l10n_jo_edi_pos/models/pos_payment_method.py` (18 lines)
- `addons/l10n_jo_edi_pos/models/res_company.py` (15 lines)
- `addons/l10n_jo_edi_pos/models/res_config_settings.py` (8 lines)
- `addons/l10n_jo_edi_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_jo_edi_pos/receipt/pos_order_receipt.py` (14 lines)
- `addons/l10n_jo_edi_pos/receipt/pos_order_receipt.xml` (25 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/app/utils/generate_printer_data.js` (16 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/models/feedback_screen.js` (29 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/models/invoice_button.js` (22 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/models/pos_order.js` (9 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/screens/ticket_screen.js` (34 lines)
- `addons/l10n_jo_edi_pos/static/src/overrides/screens/ticket_screen.xml` (11 lines)
- `addons/l10n_jo_edi_pos/static/tests/tours/l10n_jo_edi_pos_tour.js` (32 lines)
- `addons/l10n_jo_edi_pos/tests/__init__.py` (3 lines)
- `addons/l10n_jo_edi_pos/tests/jo_edi_pos_common.py` (63 lines)
- `addons/l10n_jo_edi_pos/tests/test_jo_edi_pos_precision.py` (143 lines)
- `addons/l10n_jo_edi_pos/tests/test_jo_edi_pos_types.py` (513 lines)
- `addons/l10n_jo_edi_pos/tests/test_l10n_jo_edi_pos_tour.py` (25 lines)
- `addons/l10n_jo_edi_pos/views/pos_order_views.xml` (57 lines)
- `addons/l10n_jo_edi_pos/views/pos_payment_method_views.xml` (13 lines)
- `addons/l10n_jo_edi_pos/views/res_config_settings_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
