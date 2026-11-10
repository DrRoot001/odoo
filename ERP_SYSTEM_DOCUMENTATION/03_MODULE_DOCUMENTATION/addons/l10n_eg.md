# Module: l10n_eg

- **Module ID:** MOD-171
- **Path:** `addons/l10n_eg`
- **Manifest:** `addons/l10n_eg/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Egypt Accounting Module
==============================================================================
Egypt Accounting Basic Charts and Localization.

Activates:

- Chart of Accounts
- Taxes
- VAT Return
- Withholding Tax Report
- Schedule Tax Report
- Other Taxes Report
- Fiscal Positions
    

Declared dependencies: `account`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
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
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "views/account_tax.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_partner.xml"
  ]
}
```

### Representative source files

- `addons/l10n_eg/__init__.py` (1 lines)
- `addons/l10n_eg/__manifest__.py` (38 lines)
- `addons/l10n_eg/data/account_tax_report_data.xml` (400 lines)
- `addons/l10n_eg/data/template/account.account-eg.csv` (236 lines)
- `addons/l10n_eg/data/template/account.depreciation.model-eg.csv` (6 lines)
- `addons/l10n_eg/data/template/account.fiscal.position-eg.csv` (3 lines)
- `addons/l10n_eg/data/template/account.tax-eg.csv` (67 lines)
- `addons/l10n_eg/data/template/account.tax.group-eg.csv` (8 lines)
- `addons/l10n_eg/demo/demo_company.xml` (36 lines)
- `addons/l10n_eg/demo/demo_partner.xml` (17 lines)
- `addons/l10n_eg/i18n/ar.po` (780 lines)
- `addons/l10n_eg/i18n/l10n_eg.pot` (501 lines)
- `addons/l10n_eg/models/__init__.py` (3 lines)
- `addons/l10n_eg/models/account_tax.py` (67 lines)
- `addons/l10n_eg/models/template_eg.py` (114 lines)
- `addons/l10n_eg/static/description/icon.png` (31 lines)
- `addons/l10n_eg/views/account_tax.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
