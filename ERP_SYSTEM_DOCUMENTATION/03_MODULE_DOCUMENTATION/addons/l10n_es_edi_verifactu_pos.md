# Module: l10n_es_edi_verifactu_pos

- **Module ID:** MOD-180
- **Path:** `addons/l10n_es_edi_verifactu_pos`
- **Manifest:** `addons/l10n_es_edi_verifactu_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add Veri*Factu support to Point of Sale

No manifest description declared.

Declared dependencies: `l10n_es_edi_verifactu`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_es_edi_verifactu",
    "point_of_sale"
  ],
  "data": [
    "views/pos_order_views.xml",
    "receipt/pos_order_receipt.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_es_edi_verifactu_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_es_edi_verifactu_pos/__init__.py` (2 lines)
- `addons/l10n_es_edi_verifactu_pos/__manifest__.py` (24 lines)
- `addons/l10n_es_edi_verifactu_pos/i18n/es.po` (340 lines)
- `addons/l10n_es_edi_verifactu_pos/i18n/l10n_es_edi_verifactu_pos.pot` (286 lines)
- `addons/l10n_es_edi_verifactu_pos/models/__init__.py` (5 lines)
- `addons/l10n_es_edi_verifactu_pos/models/account_move.py` (17 lines)
- `addons/l10n_es_edi_verifactu_pos/models/pos_config.py` (23 lines)
- `addons/l10n_es_edi_verifactu_pos/models/pos_order.py` (282 lines)
- `addons/l10n_es_edi_verifactu_pos/models/res_company.py` (13 lines)
- `addons/l10n_es_edi_verifactu_pos/models/verifactu_document.py` (11 lines)
- `addons/l10n_es_edi_verifactu_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_es_edi_verifactu_pos/receipt/pos_order_receipt.py` (16 lines)
- `addons/l10n_es_edi_verifactu_pos/receipt/pos_order_receipt.xml` (17 lines)
- `addons/l10n_es_edi_verifactu_pos/security/ir.access.csv` (2 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/components/popups/add_verifactu_refund_reason_popup/add_verifactu_refund_reason_popup.js` (26 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/components/popups/add_verifactu_refund_reason_popup/add_verifactu_refund_reason_popup.xml` (24 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/models/order.js` (10 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/screens/ticket_screen/ticket_screen.js` (18 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/utils/order_payment_validation.js` (15 lines)
- `addons/l10n_es_edi_verifactu_pos/static/src/app/utils/printer/generate_printer_data.js` (20 lines)
- `addons/l10n_es_edi_verifactu_pos/tests/__init__.py` (2 lines)
- `addons/l10n_es_edi_verifactu_pos/tests/common.py` (24 lines)
- `addons/l10n_es_edi_verifactu_pos/tests/files/test_order_not_invoiced_order.json` (49 lines)
- `addons/l10n_es_edi_verifactu_pos/tests/files/test_order_not_invoiced_refund.json` (65 lines)
- `addons/l10n_es_edi_verifactu_pos/tests/test_pos_order.py` (327 lines)
- `addons/l10n_es_edi_verifactu_pos/views/pos_order_views.xml` (95 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
