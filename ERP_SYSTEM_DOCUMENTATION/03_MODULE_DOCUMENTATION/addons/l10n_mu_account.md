# Module: l10n_mu_account

- **Module ID:** MOD-276
- **Path:** `addons/l10n_mu_account`
- **Manifest:** `addons/l10n_mu_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for the Republic of Mauritius in Odoo.
==============================================================================================
    - Chart of accounts
    - Taxes
    - Fiscal positions
    - Default settings
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/tax_report-mu.xml",
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_mu_account/__init__.py` (2 lines)
- `addons/l10n_mu_account/__manifest__.py` (27 lines)
- `addons/l10n_mu_account/data/tax_report-mu.xml` (484 lines)
- `addons/l10n_mu_account/data/template/account.account-mu.csv` (43 lines)
- `addons/l10n_mu_account/data/template/account.fiscal.position-mu.csv` (3 lines)
- `addons/l10n_mu_account/data/template/account.tax-mu.csv` (49 lines)
- `addons/l10n_mu_account/data/template/account.tax.group-mu.csv` (3 lines)
- `addons/l10n_mu_account/demo/demo_company.xml` (42 lines)
- `addons/l10n_mu_account/i18n/fr.po` (428 lines)
- `addons/l10n_mu_account/i18n/l10n_mu_account.pot` (421 lines)
- `addons/l10n_mu_account/models/__init__.py` (4 lines)
- `addons/l10n_mu_account/models/account_move.py` (12 lines)
- `addons/l10n_mu_account/models/base_document_layout.py` (19 lines)
- `addons/l10n_mu_account/models/template_mu.py` (47 lines)
- `addons/l10n_mu_account/views/report_invoice.xml` (51 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
