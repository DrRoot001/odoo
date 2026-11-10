# Module: l10n_hu

- **Module ID:** MOD-219
- **Path:** `addons/l10n_hu`
- **Manifest:** `addons/l10n_hu/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Accounting chart and localization for Hungary
    

Declared dependencies: `account`.

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

- `addons/l10n_hu/__init__.py` (2 lines)
- `addons/l10n_hu/__manifest__.py` (24 lines)
- `addons/l10n_hu/data/account_tax_report_data.xml` (462 lines)
- `addons/l10n_hu/data/template/account.account-hu.csv` (391 lines)
- `addons/l10n_hu/data/template/account.fiscal.position-hu.csv` (6 lines)
- `addons/l10n_hu/data/template/account.tax-hu.csv` (221 lines)
- `addons/l10n_hu/data/template/account.tax.group-hu.csv` (6 lines)
- `addons/l10n_hu/demo/demo_company.xml` (43 lines)
- `addons/l10n_hu/i18n/hu.po` (72 lines)
- `addons/l10n_hu/i18n/l10n_hu.pot` (68 lines)
- `addons/l10n_hu/migrations/3.1/end-migrate_update_taxes.py` (10 lines)
- `addons/l10n_hu/models/__init__.py` (4 lines)
- `addons/l10n_hu/models/account_move.py` (22 lines)
- `addons/l10n_hu/models/res_partner.py` (15 lines)
- `addons/l10n_hu/models/template_hu.py` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
