# Module: l10n_uk

- **Module ID:** MOD-335
- **Path:** `addons/l10n_uk`
- **Manifest:** `addons/l10n_uk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the latest UK Odoo localisation necessary to run Odoo accounting for UK SME's with:
=================================================================================================
    - a CT600-ready chart of accounts
    - VAT100-ready tax structure
    - InfoLogic UK counties listing
    - a few other adaptations

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/country_group.xml",
    "data/l10n_uk_chart_data.xml",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/l10n_uk_demo.xml",
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_uk/__init__.py` (2 lines)
- `addons/l10n_uk/__manifest__.py` (31 lines)
- `addons/l10n_uk/data/account_tax_report_data.xml` (134 lines)
- `addons/l10n_uk/data/country_group.xml` (8 lines)
- `addons/l10n_uk/data/l10n_uk_chart_data.xml` (6 lines)
- `addons/l10n_uk/data/template/account.account-uk.csv` (120 lines)
- `addons/l10n_uk/data/template/account.depreciation.model-uk.csv` (6 lines)
- `addons/l10n_uk/data/template/account.fiscal.position-uk.csv` (4 lines)
- `addons/l10n_uk/data/template/account.tax-uk.csv` (77 lines)
- `addons/l10n_uk/data/template/account.tax.group-uk.csv` (5 lines)
- `addons/l10n_uk/demo/demo_company.xml` (43 lines)
- `addons/l10n_uk/demo/l10n_uk_demo.xml` (27 lines)
- `addons/l10n_uk/migrations/1.1/end-migrate.py` (7 lines)
- `addons/l10n_uk/models/__init__.py` (3 lines)
- `addons/l10n_uk/models/template_uk.py` (72 lines)
- `addons/l10n_uk/models/template_xi.py` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
