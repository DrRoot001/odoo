# Module: l10n_ae

- **Module ID:** MOD-117
- **Path:** `addons/l10n_ae`
- **Manifest:** `addons/l10n_ae/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


United Arab Emirates Accounting Module
=======================================================
United Arab Emirates accounting basic charts and localization.

Activates:

- Chart of Accounts
- Taxes
- Tax Report
- Fiscal Positions
    

Declared dependencies: `account`, `l10n_gcc_invoice`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_gcc_invoice"
  ],
  "data": [
    "data/l10n_ae_data.xml",
    "data/account_tax_report_data.xml",
    "views/report_invoice_templates.xml",
    "views/account_move.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ae/__init__.py` (3 lines)
- `addons/l10n_ae/__manifest__.py` (36 lines)
- `addons/l10n_ae/data/account_tax_report_data.xml` (403 lines)
- `addons/l10n_ae/data/l10n_ae_data.xml` (10 lines)
- `addons/l10n_ae/data/template/account.account-ae.csv` (240 lines)
- `addons/l10n_ae/data/template/account.depreciation.model-ae.csv` (6 lines)
- `addons/l10n_ae/data/template/account.fiscal.position-ae.csv` (10 lines)
- `addons/l10n_ae/data/template/account.tax-ae.csv` (75 lines)
- `addons/l10n_ae/data/template/account.tax.group-ae.csv` (6 lines)
- `addons/l10n_ae/demo/demo_company.xml` (37 lines)
- `addons/l10n_ae/i18n/ar.po` (243 lines)
- `addons/l10n_ae/i18n/l10n_ae.pot` (239 lines)
- `addons/l10n_ae/models/__init__.py` (2 lines)
- `addons/l10n_ae/models/account_move.py` (28 lines)
- `addons/l10n_ae/models/template_ae.py` (102 lines)
- `addons/l10n_ae/views/account_move.xml` (15 lines)
- `addons/l10n_ae/views/report_invoice_templates.xml` (87 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
