# Module: l10n_sa

- **Module ID:** MOD-310
- **Path:** `addons/l10n_sa`
- **Manifest:** `addons/l10n_sa/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Saudi Arabia Accounting Module
===========================================================
Saudi Arabia Accounting Basic Charts and Localization

Activates:

- Chart of Accounts
- Taxes
- VAT Return
- Withholding Return
- Fiscal Positions


Declared dependencies: `l10n_gcc_invoice`, `account`, `account_debit_note`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_gcc_invoice",
    "account",
    "account_debit_note",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account_data.xml",
    "data/account_tax_report_data.xml",
    "data/account_tax_report_withholding_data.xml",
    "data/report_paperformat_data.xml",
    "views/account_move_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "wizard/account_debit_note.xml",
    "wizard/account_move_reversal_views.xml",
    "views/report_templates_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.report_assets_common": [
      "l10n_sa/static/src/scss/styles.scss"
    ]
  }
}
```

### Representative source files

- `addons/l10n_sa/__init__.py` (3 lines)
- `addons/l10n_sa/__manifest__.py` (51 lines)
- `addons/l10n_sa/data/account_data.xml` (8 lines)
- `addons/l10n_sa/data/account_tax_report_data.xml` (252 lines)
- `addons/l10n_sa/data/account_tax_report_withholding_data.xml` (455 lines)
- `addons/l10n_sa/data/report_paperformat_data.xml` (14 lines)
- `addons/l10n_sa/data/template/account.account-sa.csv` (245 lines)
- `addons/l10n_sa/data/template/account.depreciation.model-sa.csv` (6 lines)
- `addons/l10n_sa/data/template/account.fiscal.position-sa.csv` (3 lines)
- `addons/l10n_sa/data/template/account.tax-sa.csv` (171 lines)
- `addons/l10n_sa/data/template/account.tax.group-sa.csv` (6 lines)
- `addons/l10n_sa/demo/__init__.py` (1 lines)
- `addons/l10n_sa/demo/account_demo.py` (264 lines)
- `addons/l10n_sa/demo/demo_company.xml` (51 lines)
- `addons/l10n_sa/i18n/ar.po` (715 lines)
- `addons/l10n_sa/i18n/l10n_sa.pot` (694 lines)
- `addons/l10n_sa/migrations/2.2/end-migrate.py` (48 lines)
- `addons/l10n_sa/migrations/2.3/end-migrate.py` (36 lines)
- `addons/l10n_sa/migrations/2.3/post-migrate.py` (8 lines)
- `addons/l10n_sa/migrations/2.3/pre-migrate.py` (60 lines)
- `addons/l10n_sa/models/__init__.py` (6 lines)
- `addons/l10n_sa/models/account_move.py` (115 lines)
- `addons/l10n_sa/models/account_move_line.py` (11 lines)
- `addons/l10n_sa/models/ir_attachment.py` (27 lines)
- `addons/l10n_sa/models/res_partner.py` (100 lines)
- `addons/l10n_sa/models/template_sa.py` (90 lines)
- `addons/l10n_sa/models/zatca_mixin.py` (77 lines)
- `addons/l10n_sa/static/src/scss/styles.scss` (3 lines)
- `addons/l10n_sa/tests/__init__.py` (2 lines)
- `addons/l10n_sa/tests/test_account_move.py` (65 lines)
- `addons/l10n_sa/tests/test_sa_additional_identifiers.py` (76 lines)
- `addons/l10n_sa/tools/partner_identifiers.py` (88 lines)
- `addons/l10n_sa/views/account_move_views.xml` (29 lines)
- `addons/l10n_sa/views/report_invoice.xml` (314 lines)
- `addons/l10n_sa/views/report_templates_views.xml` (59 lines)
- `addons/l10n_sa/views/res_config_settings_views.xml` (12 lines)
- `addons/l10n_sa/wizard/__init__.py` (2 lines)
- `addons/l10n_sa/wizard/account_debit_note.py` (14 lines)
- `addons/l10n_sa/wizard/account_debit_note.xml` (18 lines)
- `addons/l10n_sa/wizard/account_move_reversal.py` (14 lines)
- `addons/l10n_sa/wizard/account_move_reversal_views.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
