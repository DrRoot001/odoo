# Module: l10n_nz

- **Module ID:** MOD-287
- **Path:** `addons/l10n_nz`
- **Manifest:** `addons/l10n_nz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


New Zealand Accounting Module
=============================

New Zealand accounting basic charts and localizations.

Also:
    - activates a number of regional currencies.
    - sets up New Zealand taxes.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/res_currency_data.xml",
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_nz/__init__.py` (2 lines)
- `addons/l10n_nz/__manifest__.py` (33 lines)
- `addons/l10n_nz/data/account_tax_report_data.xml` (142 lines)
- `addons/l10n_nz/data/res_currency_data.xml` (26 lines)
- `addons/l10n_nz/data/template/account.account-nz.csv` (102 lines)
- `addons/l10n_nz/data/template/account.fiscal.position-nz.csv` (3 lines)
- `addons/l10n_nz/data/template/account.tax-nz.csv` (25 lines)
- `addons/l10n_nz/data/template/account.tax.group-nz.csv` (4 lines)
- `addons/l10n_nz/demo/demo_company.xml` (37 lines)
- `addons/l10n_nz/migrations/1.2/post-migrate.py` (10 lines)
- `addons/l10n_nz/migrations/1.2/pre-migrate.py` (10 lines)
- `addons/l10n_nz/models/__init__.py` (4 lines)
- `addons/l10n_nz/models/account_move.py` (13 lines)
- `addons/l10n_nz/models/template_nz.py` (40 lines)
- `addons/l10n_nz/views/report_invoice.xml` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
