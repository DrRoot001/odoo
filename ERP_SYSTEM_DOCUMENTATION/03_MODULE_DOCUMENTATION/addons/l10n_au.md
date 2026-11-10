# Module: l10n_au

- **Module ID:** MOD-126
- **Path:** `addons/l10n_au`
- **Manifest:** `addons/l10n_au/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Australian Accounting Module
============================

Australian accounting basic charts and localizations.

Also:
    - activates a number of regional currencies.
    - sets up Australian taxes.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/account_tax_template_data.xml",
    "data/bas_a.xml",
    "data/bas_c.xml",
    "data/bas_d.xml",
    "data/bas_f.xml",
    "data/bas_g.xml",
    "data/bas_u.xml",
    "data/bas_v.xml",
    "data/bas_w.xml",
    "data/bas_x.xml",
    "data/bas_y.xml",
    "data/res_currency_data.xml",
    "data/account.account.tag.csv",
    "views/menuitems.xml",
    "views/report_invoice.xml",
    "views/res_company_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_au/__init__.py` (3 lines)
- `addons/l10n_au/__manifest__.py` (45 lines)
- `addons/l10n_au/data/account.account.tag.csv` (2 lines)
- `addons/l10n_au/data/account_tax_template_data.xml` (13 lines)
- `addons/l10n_au/data/bas_a.xml` (661 lines)
- `addons/l10n_au/data/bas_c.xml` (804 lines)
- `addons/l10n_au/data/bas_d.xml` (403 lines)
- `addons/l10n_au/data/bas_f.xml` (487 lines)
- `addons/l10n_au/data/bas_g.xml` (804 lines)
- `addons/l10n_au/data/bas_u.xml` (673 lines)
- `addons/l10n_au/data/bas_v.xml` (816 lines)
- `addons/l10n_au/data/bas_w.xml` (427 lines)
- `addons/l10n_au/data/bas_x.xml` (511 lines)
- `addons/l10n_au/data/bas_y.xml` (828 lines)
- `addons/l10n_au/data/res_currency_data.xml` (26 lines)
- `addons/l10n_au/data/template/account.account-au.csv` (125 lines)
- `addons/l10n_au/data/template/account.depreciation.model-au.csv` (7 lines)
- `addons/l10n_au/data/template/account.fiscal.position-au.csv` (5 lines)
- `addons/l10n_au/data/template/account.tax-au.csv` (131 lines)
- `addons/l10n_au/data/template/account.tax.group-au.csv` (5 lines)
- `addons/l10n_au/demo/demo_company.xml` (36 lines)
- `addons/l10n_au/models/__init__.py` (6 lines)
- `addons/l10n_au/models/account_move.py` (31 lines)
- `addons/l10n_au/models/res_company.py` (8 lines)
- `addons/l10n_au/models/res_partner_bank.py` (16 lines)
- `addons/l10n_au/models/template_au.py` (57 lines)
- `addons/l10n_au/views/menuitems.xml` (4 lines)
- `addons/l10n_au/views/report_invoice.xml` (83 lines)
- `addons/l10n_au/views/res_company_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
