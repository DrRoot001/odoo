# Module: l10n_la

- **Module ID:** MOD-258
- **Path:** `addons/l10n_la`
- **Manifest:** `addons/l10n_la/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Chart of accounts, VAT taxes and monthly VAT return for Laos


Chart of Accounts for Laos.
===========================

Chart of accounts for non-public-interest entities, as set by the Ministry of Finance
Decision No. 0369 of 4 February 2020.
    

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

- `addons/l10n_la/__init__.py` (2 lines)
- `addons/l10n_la/__manifest__.py` (28 lines)
- `addons/l10n_la/data/account_tax_report_data.xml` (498 lines)
- `addons/l10n_la/data/template/account.account-la.csv` (544 lines)
- `addons/l10n_la/data/template/account.depreciation.model-la.csv` (7 lines)
- `addons/l10n_la/data/template/account.fiscal.position-la.csv` (4 lines)
- `addons/l10n_la/data/template/account.tax-la.csv` (75 lines)
- `addons/l10n_la/data/template/account.tax.group-la.csv` (6 lines)
- `addons/l10n_la/demo/demo_company.xml` (29 lines)
- `addons/l10n_la/i18n/l10n_la.pot` (167 lines)
- `addons/l10n_la/i18n/lo.po` (167 lines)
- `addons/l10n_la/models/__init__.py` (2 lines)
- `addons/l10n_la/models/template_la.py` (93 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
