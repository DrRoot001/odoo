# Module: l10n_mr

- **Module ID:** MOD-273
- **Path:** `addons/l10n_mr`
- **Manifest:** `addons/l10n_mr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Mauritania basic package that contains the chart of accounts, the taxes, tax reports, etc.
    

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

- `addons/l10n_mr/__init__.py` (1 lines)
- `addons/l10n_mr/__manifest__.py` (22 lines)
- `addons/l10n_mr/data/account_tax_report_data.xml` (342 lines)
- `addons/l10n_mr/data/template/account.account-mr.csv` (614 lines)
- `addons/l10n_mr/data/template/account.depreciation.model-mr.csv` (5 lines)
- `addons/l10n_mr/data/template/account.fiscal.position-mr.csv` (3 lines)
- `addons/l10n_mr/data/template/account.tax-mr.csv` (61 lines)
- `addons/l10n_mr/data/template/account.tax.group-mr.csv` (5 lines)
- `addons/l10n_mr/demo/demo_company.xml` (42 lines)
- `addons/l10n_mr/i18n/fr.po` (192 lines)
- `addons/l10n_mr/i18n/l10n_mr.pot` (153 lines)
- `addons/l10n_mr/models/__init__.py` (1 lines)
- `addons/l10n_mr/models/template_mr.py` (51 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
