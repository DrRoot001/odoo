# Module: l10n_lk

- **Module ID:** MOD-262
- **Path:** `addons/l10n_lk`
- **Manifest:** `addons/l10n_lk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Provides accounting localizations for Sri Lanka.


Sri Lankan Accounting module
============================
- Chart of Accounts
- Fiscal Position
- Taxes & Tax Groups

Forms
=====
- VAT001
- WHT001

Tax Invoice
===========
- Custom tax invoice sequence format: YYMMM_QQQQ_XXXXX
- Tax Invoice / Supply Date / Mode of Payment in PDF report
- VAT registration tracking for companies and partners
    

Declared dependencies: `account`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/form_vat001.xml",
    "data/form_wht001.xml",
    "views/report_invoice.xml",
    "views/res_partner_views.xml",
    "views/res_company_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_lk/__init__.py` (2 lines)
- `addons/l10n_lk/__manifest__.py` (45 lines)
- `addons/l10n_lk/data/account.account.tag.csv` (4 lines)
- `addons/l10n_lk/data/form_vat001.xml` (1,206 lines)
- `addons/l10n_lk/data/form_wht001.xml` (556 lines)
- `addons/l10n_lk/data/template/account.account-lk.csv` (146 lines)
- `addons/l10n_lk/data/template/account.depreciation.model-lk.csv` (10 lines)
- `addons/l10n_lk/data/template/account.fiscal.position-lk.csv` (3 lines)
- `addons/l10n_lk/data/template/account.tax-lk.csv` (237 lines)
- `addons/l10n_lk/data/template/account.tax.group-lk.csv` (6 lines)
- `addons/l10n_lk/demo/demo_company.xml` (35 lines)
- `addons/l10n_lk/models/__init__.py` (7 lines)
- `addons/l10n_lk/models/account_move.py` (275 lines)
- `addons/l10n_lk/models/account_resequence.py` (76 lines)
- `addons/l10n_lk/models/res_company.py` (15 lines)
- `addons/l10n_lk/models/res_partner.py` (26 lines)
- `addons/l10n_lk/models/template_lk.py` (76 lines)
- `addons/l10n_lk/tests/__init__.py` (3 lines)
- `addons/l10n_lk/tests/test_lk_tax_invoice_sequence.py` (799 lines)
- `addons/l10n_lk/views/report_invoice.xml` (71 lines)
- `addons/l10n_lk/views/res_company_views.xml` (13 lines)
- `addons/l10n_lk/views/res_partner_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
