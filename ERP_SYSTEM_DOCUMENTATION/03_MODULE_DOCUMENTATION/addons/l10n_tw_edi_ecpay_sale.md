# Module: l10n_tw_edi_ecpay_sale

- **Module ID:** MOD-330
- **Path:** `addons/l10n_tw_edi_ecpay_sale`
- **Manifest:** `addons/l10n_tw_edi_ecpay_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

ECPay E-invoice bridge module for Sales


        This bridge module allows the user to input ECPay information in Sales for sending their invoices to the ECPay system
    

Declared dependencies: `sale`, `l10n_tw_edi_ecpay`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "l10n_tw_edi_ecpay"
  ],
  "data": [
    "views/sale_order_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_tw_edi_ecpay_sale/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_sale/__manifest__.py` (20 lines)
- `addons/l10n_tw_edi_ecpay_sale/i18n/l10n_tw_edi_ecpay_sale.pot` (129 lines)
- `addons/l10n_tw_edi_ecpay_sale/i18n/zh_TW.po` (144 lines)
- `addons/l10n_tw_edi_ecpay_sale/models/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_sale/models/sale_order.py` (96 lines)
- `addons/l10n_tw_edi_ecpay_sale/tests/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_sale/tests/test_edi_sale_order.py` (40 lines)
- `addons/l10n_tw_edi_ecpay_sale/views/sale_order_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
