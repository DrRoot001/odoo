# Module: l10n_lt

- **Module ID:** MOD-263
- **Path:** `addons/l10n_lt`
- **Manifest:** `addons/l10n_lt/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart of Accounts (COA) Template for Lithuania's Accounting.

This module also includes:

* List of available banks in Lithuania.
* Tax groups.
* Most common Lithuanian Taxes.
* Fiscal positions.
* Account Tags.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
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
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account_account_tag_data.xml",
    "data/tax_report_data.xml",
    "views/account_tax.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_lt/__init__.py` (2 lines)
- `addons/l10n_lt/__manifest__.py` (34 lines)
- `addons/l10n_lt/data/account_account_tag_data.xml` (438 lines)
- `addons/l10n_lt/data/tax_report_data.xml` (388 lines)
- `addons/l10n_lt/data/template/account.account-lt.csv` (190 lines)
- `addons/l10n_lt/data/template/account.fiscal.position-lt.csv` (5 lines)
- `addons/l10n_lt/data/template/account.tax-lt.csv` (261 lines)
- `addons/l10n_lt/data/template/account.tax.group-lt.csv` (6 lines)
- `addons/l10n_lt/demo/demo_company.xml` (43 lines)
- `addons/l10n_lt/i18n/l10n_lt.pot` (515 lines)
- `addons/l10n_lt/i18n/lt.po` (525 lines)
- `addons/l10n_lt/models/__init__.py` (4 lines)
- `addons/l10n_lt/models/account_journal.py` (19 lines)
- `addons/l10n_lt/models/account_tax.py` (7 lines)
- `addons/l10n_lt/models/template_lt.py` (56 lines)
- `addons/l10n_lt/views/account_tax.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
