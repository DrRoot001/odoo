# Module: l10n_ug

- **Module ID:** MOD-334
- **Path:** `addons/l10n_ug`
- **Manifest:** `addons/l10n_ug/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the basic Ugandian localisation necessary to run Odoo in UG:
================================================================================
    - Chart of accounts
    - Taxes
    - Fiscal positions
    - Default settings
    - Tax report
    

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

- `addons/l10n_ug/__init__.py` (3 lines)
- `addons/l10n_ug/__manifest__.py` (27 lines)
- `addons/l10n_ug/data/account_tax_report_data.xml` (637 lines)
- `addons/l10n_ug/data/template/account.account-ug.csv` (125 lines)
- `addons/l10n_ug/data/template/account.fiscal.position-ug.csv` (3 lines)
- `addons/l10n_ug/data/template/account.tax-ug.csv` (81 lines)
- `addons/l10n_ug/data/template/account.tax.group-ug.csv` (2 lines)
- `addons/l10n_ug/demo/demo_company.xml` (36 lines)
- `addons/l10n_ug/i18n/l10n_ug.pot` (293 lines)
- `addons/l10n_ug/i18n/sw.po` (296 lines)
- `addons/l10n_ug/models/__init__.py` (3 lines)
- `addons/l10n_ug/models/template_ug.py` (48 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
