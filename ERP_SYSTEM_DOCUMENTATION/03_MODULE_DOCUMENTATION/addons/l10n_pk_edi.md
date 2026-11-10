# Module: l10n_pk_edi

- **Module ID:** MOD-296
- **Path:** `addons/l10n_pk_edi`
- **Manifest:** `addons/l10n_pk_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Electronic Invoicing for Pakistan FBR(v1.12)


Pakistan - E-invoicing
======================

To submit invoices through API to the Pakistan government:

- Step 1: Generate an API token from the Pakistan E-Invoice portal.
- Step 2: Switch to the company associated with that API token in Odoo.
- Step 3: Configure the token in Odoo, by going to Invoicing/Accounting → Configuration →
  Settings, then searching for “Pakistan Electronic Invoicing” and pasting the token.
- Step 4: Create a customer invoice and use Send & Print to submit it to the Pakistan
  E-Invoicing system.


Declared dependencies: `account_debit_note`, `iap`, `l10n_pk`, `stock_delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_debit_note",
    "iap",
    "l10n_pk",
    "stock_delivery"
  ],
  "data": [
    "security/ir.access.csv",
    "data/uom.uom.csv",
    "data/ir_config_data.xml",
    "data/l10n_pk_edi_sro_data.xml",
    "views/account_move_views.xml",
    "views/l10n_pk_edi_sro.xml",
    "views/l10n_pk_edi_menus.xml",
    "views/product_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/uom_uom_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pk_edi/__init__.py` (2 lines)
- `addons/l10n_pk_edi/__manifest__.py` (44 lines)
- `addons/l10n_pk_edi/data/ir_config_data.xml` (13 lines)
- `addons/l10n_pk_edi/data/l10n_pk_edi_data.py` (867 lines)
- `addons/l10n_pk_edi/data/l10n_pk_edi_sro_data.xml` (504 lines)
- `addons/l10n_pk_edi/data/neutralize.sql` (4 lines)
- `addons/l10n_pk_edi/data/uom.uom.csv` (29 lines)
- `addons/l10n_pk_edi/demo/demo_company.xml` (6 lines)
- `addons/l10n_pk_edi/models/__init__.py` (13 lines)
- `addons/l10n_pk_edi/models/account_move.py` (400 lines)
- `addons/l10n_pk_edi/models/account_move_line.py` (44 lines)
- `addons/l10n_pk_edi/models/account_move_send.py` (72 lines)
- `addons/l10n_pk_edi/models/account_tax.py` (13 lines)
- `addons/l10n_pk_edi/models/iap_account.py` (131 lines)
- `addons/l10n_pk_edi/models/l10n_pk_edi_sro.py` (31 lines)
- `addons/l10n_pk_edi/models/l10n_pk_edi_sro_item.py` (16 lines)
- `addons/l10n_pk_edi/models/product_product.py` (45 lines)
- `addons/l10n_pk_edi/models/product_template.py` (16 lines)
- `addons/l10n_pk_edi/models/res_company.py` (218 lines)
- `addons/l10n_pk_edi/models/res_config_settings.py` (34 lines)
- `addons/l10n_pk_edi/models/res_partner.py` (94 lines)
- `addons/l10n_pk_edi/models/uom_uom.py` (81 lines)
- `addons/l10n_pk_edi/security/ir.access.csv` (5 lines)
- `addons/l10n_pk_edi/static/src/img/img_fbr_einvoice.png` (208 lines)
- `addons/l10n_pk_edi/tests/__init__.py` (1 lines)
- `addons/l10n_pk_edi/tests/test_l10n_pk_edi_payload.py` (333 lines)
- `addons/l10n_pk_edi/views/account_move_views.xml` (22 lines)
- `addons/l10n_pk_edi/views/l10n_pk_edi_menus.xml` (16 lines)
- `addons/l10n_pk_edi/views/l10n_pk_edi_sro.xml` (53 lines)
- `addons/l10n_pk_edi/views/product_views.xml` (17 lines)
- `addons/l10n_pk_edi/views/report_invoice.xml` (34 lines)
- `addons/l10n_pk_edi/views/res_config_settings_views.xml` (42 lines)
- `addons/l10n_pk_edi/views/res_partner_views.xml` (35 lines)
- `addons/l10n_pk_edi/views/uom_uom_views.xml` (23 lines)
- `addons/l10n_pk_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_pk_edi/wizard/account_debit_note.py` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
