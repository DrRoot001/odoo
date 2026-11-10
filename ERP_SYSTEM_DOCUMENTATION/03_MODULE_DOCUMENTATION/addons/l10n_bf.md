# Module: l10n_bf

- **Module ID:** MOD-132
- **Path:** `addons/l10n_bf`
- **Manifest:** `addons/l10n_bf/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements the tax for Burkina Faso.
=================================================================

The Chart of Accounts is from SYSCOHADA.

    

Declared dependencies: `l10n_syscohada`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "l10n_syscohada",
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

- `addons/l10n_bf/__init__.py` (1 lines)
- `addons/l10n_bf/__manifest__.py` (25 lines)
- `addons/l10n_bf/data/account_tax_report_data.xml` (477 lines)
- `addons/l10n_bf/data/template/account.fiscal.position-bf.csv` (3 lines)
- `addons/l10n_bf/data/template/account.fiscal.position-bf_syscebnl.csv` (3 lines)
- `addons/l10n_bf/data/template/account.tax-bf.csv` (39 lines)
- `addons/l10n_bf/data/template/account.tax-bf_syscebnl.csv` (39 lines)
- `addons/l10n_bf/data/template/account.tax.group-bf.csv` (4 lines)
- `addons/l10n_bf/data/template/account.tax.group-bf_syscebnl.csv` (4 lines)
- `addons/l10n_bf/demo/demo_company.xml` (35 lines)
- `addons/l10n_bf/i18n/fr.po` (63 lines)
- `addons/l10n_bf/i18n/l10n_bf.pot` (59 lines)
- `addons/l10n_bf/models/__init__.py` (2 lines)
- `addons/l10n_bf/models/template_bf.py` (30 lines)
- `addons/l10n_bf/models/template_bf_syscebnl.py` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
