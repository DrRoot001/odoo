# Module: l10n_zm_account

- **Module ID:** MOD-347
- **Path:** `addons/l10n_zm_account`
- **Manifest:** `addons/l10n_zm_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the basic Zambian localization necessary to run Odoo in ZM:
================================================================================
    - Chart of Accounts
    - Taxes
    - Fiscal Positions
    - Default Settings
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "data/account_tax_report_data.xml",
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_zm_account/__init__.py` (3 lines)
- `addons/l10n_zm_account/__manifest__.py` (29 lines)
- `addons/l10n_zm_account/data/account_tax_report_data.xml` (530 lines)
- `addons/l10n_zm_account/data/template/account.account-zm.csv` (130 lines)
- `addons/l10n_zm_account/data/template/account.fiscal.position-zm.csv` (3 lines)
- `addons/l10n_zm_account/data/template/account.tax-zm.csv` (77 lines)
- `addons/l10n_zm_account/data/template/account.tax.group-zm.csv` (4 lines)
- `addons/l10n_zm_account/demo/demo_company.xml` (36 lines)
- `addons/l10n_zm_account/models/__init__.py` (4 lines)
- `addons/l10n_zm_account/models/account_move.py` (11 lines)
- `addons/l10n_zm_account/models/template_zm.py` (39 lines)
- `addons/l10n_zm_account/views/report_invoice.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
