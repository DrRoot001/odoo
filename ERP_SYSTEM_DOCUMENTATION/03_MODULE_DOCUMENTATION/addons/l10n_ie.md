# Module: l10n_ie

- **Module ID:** MOD-225
- **Path:** `addons/l10n_ie`
- **Manifest:** `addons/l10n_ie/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Republic of Ireland in Odoo.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
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
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/tax_report-ie.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ie/__init__.py` (2 lines)
- `addons/l10n_ie/__manifest__.py` (25 lines)
- `addons/l10n_ie/data/account.account.tag.csv` (82 lines)
- `addons/l10n_ie/data/tax_report-ie.xml` (127 lines)
- `addons/l10n_ie/data/template/account.account-ie.csv` (146 lines)
- `addons/l10n_ie/data/template/account.fiscal.position-ie.csv` (5 lines)
- `addons/l10n_ie/data/template/account.tax-ie.csv` (191 lines)
- `addons/l10n_ie/data/template/account.tax.group-ie.csv` (6 lines)
- `addons/l10n_ie/demo/demo_company.xml` (43 lines)
- `addons/l10n_ie/migrations/2.1/end-migrate.py` (7 lines)
- `addons/l10n_ie/models/__init__.py` (4 lines)
- `addons/l10n_ie/models/account_chart_template.py` (12 lines)
- `addons/l10n_ie/models/account_journal.py` (20 lines)
- `addons/l10n_ie/models/template_ie.py` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
