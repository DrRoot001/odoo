# Module: l10n_kr

- **Module ID:** MOD-254
- **Path:** `addons/l10n_kr`
- **Manifest:** `addons/l10n_kr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Accounting Module for the Republic of Korea
===========================================
This provides a base chart of accounts and taxes template for use in Odoo.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
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
    "data/account.account.tag.csv",
    "data/res_country_data.xml",
    "data/general_tax_report.xml",
    "data/simplified_tax_report.xml",
    "views/res_partner_views.xml",
    "views/account_move_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_kr/__init__.py` (2 lines)
- `addons/l10n_kr/__manifest__.py` (26 lines)
- `addons/l10n_kr/data/account.account.tag.csv` (32 lines)
- `addons/l10n_kr/data/general_tax_report.xml` (2,196 lines)
- `addons/l10n_kr/data/res_country_data.xml` (32 lines)
- `addons/l10n_kr/data/simplified_tax_report.xml` (1,895 lines)
- `addons/l10n_kr/data/template/account.account-kr.csv` (253 lines)
- `addons/l10n_kr/data/template/account.depreciation.model-kr.csv` (5 lines)
- `addons/l10n_kr/data/template/account.fiscal.position-kr.csv` (5 lines)
- `addons/l10n_kr/data/template/account.tax-kr.csv` (90 lines)
- `addons/l10n_kr/data/template/account.tax.group-kr.csv` (7 lines)
- `addons/l10n_kr/demo/demo_company.xml` (35 lines)
- `addons/l10n_kr/i18n/ko.po` (178 lines)
- `addons/l10n_kr/i18n/l10n_kr.pot` (174 lines)
- `addons/l10n_kr/models/__init__.py` (4 lines)
- `addons/l10n_kr/models/account_move.py` (42 lines)
- `addons/l10n_kr/models/res_partner.py` (26 lines)
- `addons/l10n_kr/models/template_kr.py` (80 lines)
- `addons/l10n_kr/tests/__init__.py` (2 lines)
- `addons/l10n_kr/tests/test_account_move.py` (46 lines)
- `addons/l10n_kr/views/account_move_views.xml` (18 lines)
- `addons/l10n_kr/views/res_partner_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
