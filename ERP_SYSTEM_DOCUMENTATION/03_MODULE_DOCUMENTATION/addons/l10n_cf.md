# Module: l10n_cf

- **Module ID:** MOD-144
- **Path:** `addons/l10n_cf`
- **Manifest:** `addons/l10n_cf/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements the tax for Central African Republic.
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

- `addons/l10n_cf/__init__.py` (1 lines)
- `addons/l10n_cf/__manifest__.py` (25 lines)
- `addons/l10n_cf/data/account_tax_report_data.xml` (229 lines)
- `addons/l10n_cf/data/template/account.fiscal.position-cf.csv` (3 lines)
- `addons/l10n_cf/data/template/account.fiscal.position-cf_syscebnl.csv` (3 lines)
- `addons/l10n_cf/data/template/account.tax-cf.csv` (33 lines)
- `addons/l10n_cf/data/template/account.tax-cf_syscebnl.csv` (33 lines)
- `addons/l10n_cf/data/template/account.tax.group-cf.csv` (4 lines)
- `addons/l10n_cf/data/template/account.tax.group-cf_syscebnl.csv` (4 lines)
- `addons/l10n_cf/demo/demo_company.xml` (35 lines)
- `addons/l10n_cf/i18n/fr.po` (63 lines)
- `addons/l10n_cf/i18n/l10n_cf.pot` (59 lines)
- `addons/l10n_cf/models/__init__.py` (2 lines)
- `addons/l10n_cf/models/template_cf.py` (31 lines)
- `addons/l10n_cf/models/template_cf_syscebnl.py` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
