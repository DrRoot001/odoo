# Module: l10n_tw_edi_ecpay_website_sale

- **Module ID:** MOD-331
- **Path:** `addons/l10n_tw_edi_ecpay_website_sale`
- **Manifest:** `addons/l10n_tw_edi_ecpay_website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

ECpay E-invoice bridge module for Ecommerce


        This bridge module allows the user to input Ecpay information in ecommerce for sending their invoices to the Ecpay system
    

Declared dependencies: `website_sale`, `l10n_tw_edi_ecpay_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale",
    "l10n_tw_edi_ecpay_sale"
  ],
  "data": [
    "data/data.xml",
    "views/templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_tw_edi_ecpay_website_sale/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_tw_edi_ecpay_website_sale/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_tw_edi_ecpay_website_sale/__init__.py` (10 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/__manifest__.py` (30 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/controllers/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/controllers/main.py` (237 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/data/data.xml` (13 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/i18n/l10n_tw_edi_ecpay_website_sale.pot` (250 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/i18n/zh_TW.po` (255 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/models/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/models/res_partner.py` (14 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/models/website.py` (17 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/models/website_checkout_step.py` (20 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/static/src/js/address.js` (26 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/static/src/js/edi_invoicing_info.js` (250 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/static/src/js/invoicing_info.js` (19 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/static/tests/tours/test_checkout.js` (363 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/tests/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/tests/test_l10n_tw_edi_website_sale.py` (112 lines)
- `addons/l10n_tw_edi_ecpay_website_sale/views/templates.xml` (135 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
