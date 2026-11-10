# Module: l10n_sa_edi_pos

- **Module ID:** MOD-312
- **Path:** `addons/l10n_sa_edi_pos`
- **Manifest:** `addons/l10n_sa_edi_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

ZATCA E-Invoicing, support for PoS


E-invoice implementation for Saudi Arabia; Integration with ZATCA (POS)
    

Declared dependencies: `l10n_sa_pos`, `l10n_sa_edi`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_sa_pos",
    "l10n_sa_edi"
  ],
  "data": [
    "receipt/pos_receipt_common.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_sa_edi_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_sa_edi_pos/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_sa_edi_pos/__init__.py` (2 lines)
- `addons/l10n_sa_edi_pos/__manifest__.py` (30 lines)
- `addons/l10n_sa_edi_pos/i18n/ar.po` (165 lines)
- `addons/l10n_sa_edi_pos/i18n/l10n_sa_edi_pos.pot` (159 lines)
- `addons/l10n_sa_edi_pos/models/__init__.py` (4 lines)
- `addons/l10n_sa_edi_pos/models/account_edi_xml_ubl_21_zatca.py` (14 lines)
- `addons/l10n_sa_edi_pos/models/account_move.py` (49 lines)
- `addons/l10n_sa_edi_pos/models/l10n_sa_edi_document.py` (12 lines)
- `addons/l10n_sa_edi_pos/models/pos_order.py` (45 lines)
- `addons/l10n_sa_edi_pos/models/res_company.py` (14 lines)
- `addons/l10n_sa_edi_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_sa_edi_pos/receipt/pos_order_receipt.py` (17 lines)
- `addons/l10n_sa_edi_pos/receipt/pos_order_receipt.xml` (13 lines)
- `addons/l10n_sa_edi_pos/receipt/pos_receipt_common.xml` (23 lines)
- `addons/l10n_sa_edi_pos/static/src/app/utils/order_payment_validation.js` (73 lines)
- `addons/l10n_sa_edi_pos/static/src/overrides/components/invoice_button/invoice_button.js` (22 lines)
- `addons/l10n_sa_edi_pos/static/src/overrides/models/pos_order.js` (69 lines)
- `addons/l10n_sa_edi_pos/static/src/overrides/models/pos_store.js` (14 lines)
- `addons/l10n_sa_edi_pos/static/src/overrides/utils/printer/generate_printer_data.js` (14 lines)
- `addons/l10n_sa_edi_pos/static/tests/tours/generic_tour.js` (28 lines)
- `addons/l10n_sa_edi_pos/static/tests/tours/test_zatca_pos_invoice.js` (46 lines)
- `addons/l10n_sa_edi_pos/tests/__init__.py` (4 lines)
- `addons/l10n_sa_edi_pos/tests/test_order_receipt.py` (35 lines)
- `addons/l10n_sa_edi_pos/tests/test_sa_edi_pos.py` (238 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
