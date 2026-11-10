# Module: l10n_il

- **Module ID:** MOD-226
- **Path:** `addons/l10n_il`
- **Manifest:** `addons/l10n_il/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the latest basic Israelian localisation necessary to run Odoo in Israel:
================================================================================

This module consists of:
 - Generic Israel Chart of Accounts
 - Taxes and tax report
 - Multiple Fiscal positions
 

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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
    "data/account_account_tag.xml",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_il/__init__.py` (2 lines)
- `addons/l10n_il/__manifest__.py` (31 lines)
- `addons/l10n_il/data/account_account_tag.xml` (28 lines)
- `addons/l10n_il/data/account_tax_report_data.xml` (197 lines)
- `addons/l10n_il/data/template/account.account-il.csv` (97 lines)
- `addons/l10n_il/data/template/account.fiscal.position-il.csv` (7 lines)
- `addons/l10n_il/data/template/account.tax-il.csv` (59 lines)
- `addons/l10n_il/data/template/account.tax.group-il.csv` (5 lines)
- `addons/l10n_il/demo/demo_company.xml` (36 lines)
- `addons/l10n_il/i18n/he.po` (65 lines)
- `addons/l10n_il/i18n/l10n_il.pot` (59 lines)
- `addons/l10n_il/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_il/models/__init__.py` (2 lines)
- `addons/l10n_il/models/template_il.py` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
