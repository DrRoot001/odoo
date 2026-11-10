# Module: l10n_bd

- **Module ID:** MOD-127
- **Path:** `addons/l10n_bd`
- **Manifest:** `addons/l10n_bd/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Bangladesh in Odoo
==============================================================================

Bangladesh accounting basic charts and localization.

Activates:

- Chart of accounts
- Taxes


Declared dependencies: `account`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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
    "account",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account.account.tag.csv",
    "views/menu_items.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_bd/__init__.py` (3 lines)
- `addons/l10n_bd/__manifest__.py` (33 lines)
- `addons/l10n_bd/data/account.account.tag.csv` (4 lines)
- `addons/l10n_bd/data/template/account.account-bd.csv` (165 lines)
- `addons/l10n_bd/data/template/account.depreciation.model-bd.csv` (5 lines)
- `addons/l10n_bd/data/template/account.tax-bd.csv` (33 lines)
- `addons/l10n_bd/data/template/account.tax.group-bd.csv` (4 lines)
- `addons/l10n_bd/demo/__init__.py` (2 lines)
- `addons/l10n_bd/demo/account_demo.py` (45 lines)
- `addons/l10n_bd/demo/demo_company.xml` (36 lines)
- `addons/l10n_bd/i18n/bn.po` (76 lines)
- `addons/l10n_bd/i18n/l10n_bd.pot` (71 lines)
- `addons/l10n_bd/models/__init__.py` (2 lines)
- `addons/l10n_bd/models/template_bd.py` (73 lines)
- `addons/l10n_bd/views/menu_items.xml` (4 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
