# Module: l10n_lv

- **Module ID:** MOD-265
- **Path:** `addons/l10n_lv`
- **Manifest:** `addons/l10n_lv/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart of Accounts (COA) Template for Latvia's Accounting.
This module also includes:
* Tax groups,
* Most common Latvian Taxes,
* Fiscal positions,
* Latvian bank list.

author is Allegro IT (visit for more information https://www.allegro.lv)
co-author is Chick.Farm (visit for more information https://www.myacc.cloud)
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

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
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_lv/Readme.txt` (29 lines)
- `addons/l10n_lv/__init__.py` (4 lines)
- `addons/l10n_lv/__manifest__.py` (32 lines)
- `addons/l10n_lv/data/account.account.tag.csv` (33 lines)
- `addons/l10n_lv/data/account_tax_report_data.xml` (740 lines)
- `addons/l10n_lv/data/template/account.account-lv.csv` (245 lines)
- `addons/l10n_lv/data/template/account.fiscal.position-lv.csv` (5 lines)
- `addons/l10n_lv/data/template/account.tax-lv.csv` (143 lines)
- `addons/l10n_lv/data/template/account.tax.group-lv.csv` (6 lines)
- `addons/l10n_lv/demo/demo_company.xml` (42 lines)
- `addons/l10n_lv/i18n/l10n_lv.pot` (211 lines)
- `addons/l10n_lv/i18n/lv.po` (217 lines)
- `addons/l10n_lv/models/__init__.py` (2 lines)
- `addons/l10n_lv/models/template_lv.py` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
