# Module: l10n_ge

- **Module ID:** MOD-202
- **Path:** `addons/l10n_ge`
- **Manifest:** `addons/l10n_ge/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Georgian accounting localization package


This module provides the basic accounting configuration required to use Odoo Accounting in Georgia, including:
==================================================================================================================
* Georgian chart of accounts
* Tax groups and taxes
* Fiscal Positions
* Georgian VAT report

The module is designed to provide a standard accounting setup for companies operating in Georgia and can be extended further based on specific business or legal requirements.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/res_partner_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ge/__init__.py` (1 lines)
- `addons/l10n_ge/__manifest__.py` (28 lines)
- `addons/l10n_ge/data/account_tax_report_data.xml` (693 lines)
- `addons/l10n_ge/data/template/account.account-ge.csv` (307 lines)
- `addons/l10n_ge/data/template/account.fiscal.position-ge.csv` (5 lines)
- `addons/l10n_ge/data/template/account.tax-ge.csv` (151 lines)
- `addons/l10n_ge/data/template/account.tax.group-ge.csv` (6 lines)
- `addons/l10n_ge/demo/demo_company.xml` (35 lines)
- `addons/l10n_ge/demo/res_partner_demo.xml` (25 lines)
- `addons/l10n_ge/i18n/ka.po` (82 lines)
- `addons/l10n_ge/i18n/l10n_ge.pot` (76 lines)
- `addons/l10n_ge/models/__init__.py` (1 lines)
- `addons/l10n_ge/models/template_ge.py` (67 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
