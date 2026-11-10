# Module: l10n_rs

- **Module ID:** MOD-307
- **Path:** `addons/l10n_rs`
- **Manifest:** `addons/l10n_rs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module of the Serbian localization. It manages chart of accounts and taxes.
This module is based on the official document "Pravilnik o kontnom okviru i sadržini računa u kontnom okviru za privredna društva, zadruge i preduzetnike ("Sl. glasnik RS", br. 89/2020)"
Source: https://www.paragraf.rs/propisi/pravilnik-o-kontnom-okviru-sadrzini-racuna-za-privredna-drustva-zadruge.html
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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
    "data/account_tax_report_data.xml",
    "data/menuitem_data.xml",
    "views/account_move.xml",
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_rs/__init__.py` (4 lines)
- `addons/l10n_rs/__manifest__.py` (28 lines)
- `addons/l10n_rs/data/account_tax_report_data.xml` (268 lines)
- `addons/l10n_rs/data/menuitem_data.xml` (10 lines)
- `addons/l10n_rs/data/template/account.account-rs.csv` (421 lines)
- `addons/l10n_rs/data/template/account.fiscal.position-rs.csv` (4 lines)
- `addons/l10n_rs/data/template/account.tax-rs.csv` (53 lines)
- `addons/l10n_rs/data/template/account.tax.group-rs.csv` (5 lines)
- `addons/l10n_rs/demo/demo_company.xml` (42 lines)
- `addons/l10n_rs/i18n/l10n_rs.pot` (68 lines)
- `addons/l10n_rs/i18n/sr@latin.po` (78 lines)
- `addons/l10n_rs/models/__init__.py` (3 lines)
- `addons/l10n_rs/models/account_move.py` (10 lines)
- `addons/l10n_rs/models/template_rs.py` (35 lines)
- `addons/l10n_rs/views/account_move.xml` (15 lines)
- `addons/l10n_rs/views/report_invoice.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
