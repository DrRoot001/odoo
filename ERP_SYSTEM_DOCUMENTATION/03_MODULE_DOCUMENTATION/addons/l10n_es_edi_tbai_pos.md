# Module: l10n_es_edi_tbai_pos

- **Module ID:** MOD-178
- **Path:** `addons/l10n_es_edi_tbai_pos`
- **Manifest:** `addons/l10n_es_edi_tbai_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `l10n_es_edi_tbai`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_es_edi_tbai",
    "point_of_sale"
  ],
  "data": [
    "views/pos_order_view.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_es_edi_tbai_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_es_edi_tbai_pos/__init__.py` (2 lines)
- `addons/l10n_es_edi_tbai_pos/__manifest__.py` (21 lines)
- `addons/l10n_es_edi_tbai_pos/i18n/es.po` (213 lines)
- `addons/l10n_es_edi_tbai_pos/i18n/l10n_es_edi_tbai_pos.pot` (184 lines)
- `addons/l10n_es_edi_tbai_pos/models/__init__.py` (3 lines)
- `addons/l10n_es_edi_tbai_pos/models/pos_config.py` (19 lines)
- `addons/l10n_es_edi_tbai_pos/models/pos_order.py` (231 lines)
- `addons/l10n_es_edi_tbai_pos/models/res_company.py` (13 lines)
- `addons/l10n_es_edi_tbai_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_es_edi_tbai_pos/receipt/pos_order_receipt.py` (15 lines)
- `addons/l10n_es_edi_tbai_pos/receipt/pos_order_receipt.xml` (13 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/components/popups/add_tbai_refund_reason_popup/add_tbai_refund_reason_popup.js` (26 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/components/popups/add_tbai_refund_reason_popup/add_tbai_refund_reason_popup.xml` (23 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/models/order.js` (8 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/screens/ticket_screen/ticket_screen.js` (33 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/utils/order_payment_validation.js` (19 lines)
- `addons/l10n_es_edi_tbai_pos/static/src/app/utils/printer/generate_printer_data.js` (18 lines)
- `addons/l10n_es_edi_tbai_pos/tests/__init__.py` (4 lines)
- `addons/l10n_es_edi_tbai_pos/tests/common.py` (25 lines)
- `addons/l10n_es_edi_tbai_pos/tests/test_es_tbai_pos.py` (18 lines)
- `addons/l10n_es_edi_tbai_pos/tests/test_order_receipt.py` (19 lines)
- `addons/l10n_es_edi_tbai_pos/tests/test_tbai_pos.py` (301 lines)
- `addons/l10n_es_edi_tbai_pos/views/pos_order_view.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
