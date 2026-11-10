# Module: l10n_tw_edi_ecpay

- **Module ID:** MOD-328
- **Path:** `addons/l10n_tw_edi_ecpay`
- **Manifest:** `addons/l10n_tw_edi_ecpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

E-invoicing using ECpay


Taiwan - E-invoicing
=====================
This module allows the user to send their invoices to the Ecpay system.


Declared dependencies: `l10n_tw`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_tw"
  ],
  "data": [
    "views/res_config_setting_view.xml",
    "views/account_tax.xml",
    "views/account_move_view.xml",
    "views/account_move_reversal_view.xml",
    "views/l10n_tw_edi_invoice_cancel_view.xml",
    "views/l10n_tw_edi_invoice_print_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_tw_edi_ecpay/__init__.py` (9 lines)
- `addons/l10n_tw_edi_ecpay/__manifest__.py` (26 lines)
- `addons/l10n_tw_edi_ecpay/controllers/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay/controllers/main.py` (19 lines)
- `addons/l10n_tw_edi_ecpay/data/neutralize.sql` (2 lines)
- `addons/l10n_tw_edi_ecpay/i18n/l10n_tw_edi_ecpay.pot` (982 lines)
- `addons/l10n_tw_edi_ecpay/i18n/zh_TW.po` (1,014 lines)
- `addons/l10n_tw_edi_ecpay/models/__init__.py` (9 lines)
- `addons/l10n_tw_edi_ecpay/models/account_move.py` (858 lines)
- `addons/l10n_tw_edi_ecpay/models/account_move_line.py` (7 lines)
- `addons/l10n_tw_edi_ecpay/models/account_move_send.py` (144 lines)
- `addons/l10n_tw_edi_ecpay/models/account_tax.py` (60 lines)
- `addons/l10n_tw_edi_ecpay/models/res_company.py` (17 lines)
- `addons/l10n_tw_edi_ecpay/models/res_config_settings.py` (12 lines)
- `addons/l10n_tw_edi_ecpay/models/res_partner.py` (18 lines)
- `addons/l10n_tw_edi_ecpay/security/ir.access.csv` (5 lines)
- `addons/l10n_tw_edi_ecpay/tests/__init__.py` (3 lines)
- `addons/l10n_tw_edi_ecpay/tests/test_edi.py` (790 lines)
- `addons/l10n_tw_edi_ecpay/utils.py` (106 lines)
- `addons/l10n_tw_edi_ecpay/views/account_move_reversal_view.xml` (19 lines)
- `addons/l10n_tw_edi_ecpay/views/account_move_view.xml` (53 lines)
- `addons/l10n_tw_edi_ecpay/views/account_tax.xml` (18 lines)
- `addons/l10n_tw_edi_ecpay/views/l10n_tw_edi_invoice_cancel_view.xml` (19 lines)
- `addons/l10n_tw_edi_ecpay/views/l10n_tw_edi_invoice_print_view.xml` (20 lines)
- `addons/l10n_tw_edi_ecpay/views/res_config_setting_view.xml` (36 lines)
- `addons/l10n_tw_edi_ecpay/wizard/__init__.py` (5 lines)
- `addons/l10n_tw_edi_ecpay/wizard/account_move_reversal.py` (44 lines)
- `addons/l10n_tw_edi_ecpay/wizard/l10n_tw_edi_invoice_cancel.py` (29 lines)
- `addons/l10n_tw_edi_ecpay/wizard/l10n_tw_edi_invoice_print.py` (56 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
