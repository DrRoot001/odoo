# Module: l10n_cd

- **Module ID:** MOD-143
- **Path:** `addons/l10n_cd`
- **Manifest:** `addons/l10n_cd/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements the tax for the Democratic Republic of the Congo.
===========================================================================

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

- `addons/l10n_cd/__init__.py` (1 lines)
- `addons/l10n_cd/__manifest__.py` (25 lines)
- `addons/l10n_cd/data/account_tax_report_data.xml` (627 lines)
- `addons/l10n_cd/data/template/account.fiscal.position-cd.csv` (3 lines)
- `addons/l10n_cd/data/template/account.fiscal.position-cd_syscebnl.csv` (3 lines)
- `addons/l10n_cd/data/template/account.tax-cd.csv` (57 lines)
- `addons/l10n_cd/data/template/account.tax-cd_syscebnl.csv` (57 lines)
- `addons/l10n_cd/data/template/account.tax.group-cd.csv` (3 lines)
- `addons/l10n_cd/data/template/account.tax.group-cd_syscebnl.csv` (3 lines)
- `addons/l10n_cd/demo/demo_company.xml` (35 lines)
- `addons/l10n_cd/i18n/fr.po` (63 lines)
- `addons/l10n_cd/i18n/l10n_cd.pot` (59 lines)
- `addons/l10n_cd/models/__init__.py` (2 lines)
- `addons/l10n_cd/models/template_cd.py` (36 lines)
- `addons/l10n_cd/models/template_cd_syscebnl.py` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
