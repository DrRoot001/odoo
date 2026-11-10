# Module: l10n_hr_kuna

- **Module ID:** MOD-218
- **Path:** `addons/l10n_hr_kuna`
- **Manifest:** `addons/l10n_hr_kuna/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Croatian localisation.
======================

Author: Goran Kliska, Slobodni programi d.o.o., Zagreb
        https://www.slobodni-programi.hr

Contributions:
  Tomislav Bošnjaković, Storm Computers: tipovi konta
  Ivan Vađić, Slobodni programi: tipovi konta

Description:

Croatian Chart of Accounts (RRIF ver.2012)

RRIF-ov računski plan za poduzetnike za 2012.
Vrste konta
Kontni plan prema RRIF-u, dorađen u smislu kraćenja naziva i dodavanja analitika
Porezne grupe prema poreznoj prijavi
Porezi PDV obrasca
Ostali porezi
Osnovne fiskalne pozicije

Izvori podataka:
 https://www.rrif.hr/dok/preuzimanje/rrif-rp2011.rar
 https://www.rrif.hr/dok/preuzimanje/rrif-rp2012.rar



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

- `addons/l10n_hr_kuna/__init__.py` (2 lines)
- `addons/l10n_hr_kuna/__manifest__.py` (47 lines)
- `addons/l10n_hr_kuna/data/account_tax_report_data.xml` (826 lines)
- `addons/l10n_hr_kuna/data/template/account.account-hr_kuna.csv` (1,675 lines)
- `addons/l10n_hr_kuna/data/template/account.fiscal.position-hr_kuna.csv` (8 lines)
- `addons/l10n_hr_kuna/data/template/account.tax-hr_kuna.csv` (141 lines)
- `addons/l10n_hr_kuna/data/template/account.tax.group-hr_kuna.csv` (6 lines)
- `addons/l10n_hr_kuna/demo/demo_company.xml` (36 lines)
- `addons/l10n_hr_kuna/i18n/hr.po` (437 lines)
- `addons/l10n_hr_kuna/i18n/l10n_hr_kuna.pot` (431 lines)
- `addons/l10n_hr_kuna/models/__init__.py` (2 lines)
- `addons/l10n_hr_kuna/models/template_hr_kuna.py` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
