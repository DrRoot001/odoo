# Module: l10n_th

- **Module ID:** MOD-324
- **Path:** `addons/l10n_th`
- **Manifest:** `addons/l10n_th/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart of Accounts for Thailand.
===============================

Thai accounting chart and localization.
    

Declared dependencies: `account_qr_code_emv`, `account`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 25 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_qr_code_emv",
    "account",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/res_country_data.xml",
    "data/account_tax_tags_data.xml",
    "data/report_paperformat_data.xml",
    "views/account_move_views.xml",
    "views/account_payment_views.xml",
    "views/account_tax_views.xml",
    "views/report_invoice.xml",
    "views/res_partner_view.xml",
    "views/res_company_view.xml",
    "views/res_config_settings_views.xml",
    "wizards/account_payment_register_views.xml",
    "report/report_tawi.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_th/__init__.py` (9 lines)
- `addons/l10n_th/__manifest__.py` (43 lines)
- `addons/l10n_th/controllers/__init__.py` (1 lines)
- `addons/l10n_th/controllers/download_tawi_reports.py` (25 lines)
- `addons/l10n_th/data/account_tax_report_data.xml` (233 lines)
- `addons/l10n_th/data/account_tax_tags_data.xml` (30 lines)
- `addons/l10n_th/data/report_paperformat_data.xml` (15 lines)
- `addons/l10n_th/data/res_country_data.xml` (34 lines)
- `addons/l10n_th/data/template/account.account-th.csv` (146 lines)
- `addons/l10n_th/data/template/account.asset-th.csv` (13 lines)
- `addons/l10n_th/data/template/account.fiscal.position-th.csv` (6 lines)
- `addons/l10n_th/data/template/account.tax-th.csv` (195 lines)
- `addons/l10n_th/data/template/account.tax.group-th.csv` (10 lines)
- `addons/l10n_th/demo/demo_company.xml` (36 lines)
- `addons/l10n_th/i18n/l10n_th.pot` (927 lines)
- `addons/l10n_th/i18n/th.po` (990 lines)
- `addons/l10n_th/models/__init__.py` (10 lines)
- `addons/l10n_th/models/account_move.py` (349 lines)
- `addons/l10n_th/models/account_partial_reconcile.py` (10 lines)
- `addons/l10n_th/models/account_payment.py` (100 lines)
- `addons/l10n_th/models/account_tax.py` (47 lines)
- `addons/l10n_th/models/l10n_th_tax_invoice.py` (109 lines)
- `addons/l10n_th/models/res_bank.py` (71 lines)
- `addons/l10n_th/models/res_company.py` (16 lines)
- `addons/l10n_th/models/res_partner.py` (66 lines)
- `addons/l10n_th/models/template_th.py` (63 lines)
- `addons/l10n_th/report/__init__.py` (1 lines)
- `addons/l10n_th/report/report_tawi.py` (17 lines)
- `addons/l10n_th/report/report_tawi.xml` (401 lines)
- `addons/l10n_th/security/ir.access.csv` (4 lines)
- `addons/l10n_th/tests/__init__.py` (6 lines)
- `addons/l10n_th/tests/test_credit_debit_note_pdf_report.py` (206 lines)
- `addons/l10n_th/tests/test_fiscal_position.py` (51 lines)
- `addons/l10n_th/tests/test_l10n_th_emv_qr.py` (78 lines)
- `addons/l10n_th/tests/test_l10n_th_tax_invoice.py` (595 lines)
- `addons/l10n_th/tests/test_res_partner.py` (32 lines)
- `addons/l10n_th/tests/test_wth_payment.py` (59 lines)
- `addons/l10n_th/views/account_move_views.xml` (30 lines)
- `addons/l10n_th/views/account_payment_views.xml` (29 lines)
- `addons/l10n_th/views/account_tax_views.xml` (28 lines)
- `addons/l10n_th/views/report_invoice.xml` (235 lines)
- `addons/l10n_th/views/res_company_view.xml` (13 lines)
- `addons/l10n_th/views/res_config_settings_views.xml` (22 lines)
- `addons/l10n_th/views/res_partner_view.xml` (17 lines)
- `addons/l10n_th/wizards/__init__.py` (3 lines)
- `addons/l10n_th/wizards/account_payment_register.py` (55 lines)
- `addons/l10n_th/wizards/account_payment_register_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
