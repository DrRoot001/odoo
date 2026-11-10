# Module: l10n_et

- **Module ID:** MOD-184
- **Path:** `addons/l10n_et`
- **Manifest:** `addons/l10n_et/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Base Module for Ethiopian Localization
======================================

This is the latest Ethiopian Odoo localization and consists of:
    - Chart of Accounts
    - VAT tax structure
    - Withholding tax structure
    - Regional State listings
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
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
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_et/__init__.py` (2 lines)
- `addons/l10n_et/__manifest__.py` (31 lines)
- `addons/l10n_et/data/account_tax_report_data.xml` (301 lines)
- `addons/l10n_et/data/template/account.account-et.csv` (101 lines)
- `addons/l10n_et/data/template/account.tax-et.csv` (53 lines)
- `addons/l10n_et/data/template/account.tax.group-et.csv` (6 lines)
- `addons/l10n_et/demo/demo_company.xml` (36 lines)
- `addons/l10n_et/i18n/am.po` (208 lines)
- `addons/l10n_et/i18n/l10n_et.pot` (205 lines)
- `addons/l10n_et/models/__init__.py` (2 lines)
- `addons/l10n_et/models/template_et.py` (35 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
