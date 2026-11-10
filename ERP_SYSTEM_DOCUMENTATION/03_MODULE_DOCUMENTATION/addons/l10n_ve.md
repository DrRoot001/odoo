# Module: l10n_ve

- **Module ID:** MOD-340
- **Path:** `addons/l10n_ve`
- **Manifest:** `addons/l10n_ve/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart of Account for Venezuela.
===============================

Venezuela doesn't have any chart of account by law, but the default
proposed in Odoo should comply with some Accepted best practices in Venezuela,
this plan comply with this practices.

This module has been tested as base for more of 1000 companies, because
it is based in a mixtures of most common software in the Venezuelan
market what will allow for sure to accountants feel them first steps with
Odoo more comfortable.

This module doesn't pretend be the total localization for Venezuela,
but it will help you to start really quickly with Odoo in this country.

This module give you.
---------------------

- Basic taxes for Venezuela.
- Have basic data to run tests with community localization.
- Start a company from 0 if your needs are basic from an accounting PoV.

We recomend use of account_anglo_saxon if you want valued your
stocks as Venezuela does with out invoices.

If you install this module, and select Custom chart a basic chart will be proposed,
but you will need set manually account defaults for taxes.


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
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
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ve/__init__.py` (2 lines)
- `addons/l10n_ve/__manifest__.py` (46 lines)
- `addons/l10n_ve/data/template/account.account-ve.csv` (267 lines)
- `addons/l10n_ve/data/template/account.tax-ve.csv` (33 lines)
- `addons/l10n_ve/data/template/account.tax.group-ve.csv` (5 lines)
- `addons/l10n_ve/demo/demo_company.xml` (36 lines)
- `addons/l10n_ve/i18n/es_419.po` (107 lines)
- `addons/l10n_ve/i18n/l10n_ve.pot` (69 lines)
- `addons/l10n_ve/models/__init__.py` (2 lines)
- `addons/l10n_ve/models/template_ve.py` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
