# Module: l10n_tw

- **Module ID:** MOD-327
- **Path:** `addons/l10n_tw`
- **Manifest:** `addons/l10n_tw/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Taiwan in Odoo.
==============================================================================
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/res_currency_data.xml",
    "data/res_country_data.xml",
    "data/res.city.csv",
    "data/tax_report_401.xml",
    "data/tax_report_403.xml",
    "data/tax_report_404.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_tw/__init__.py` (2 lines)
- `addons/l10n_tw/__manifest__.py` (27 lines)
- `addons/l10n_tw/data/res.city.csv` (372 lines)
- `addons/l10n_tw/data/res_country_data.xml` (6 lines)
- `addons/l10n_tw/data/res_currency_data.xml` (9 lines)
- `addons/l10n_tw/data/tax_report_401.xml` (739 lines)
- `addons/l10n_tw/data/tax_report_403.xml` (1,146 lines)
- `addons/l10n_tw/data/tax_report_404.xml` (307 lines)
- `addons/l10n_tw/data/template/account.account-tw.csv` (136 lines)
- `addons/l10n_tw/data/template/account.fiscal.position-tw.csv` (9 lines)
- `addons/l10n_tw/data/template/account.tax-tw.csv` (291 lines)
- `addons/l10n_tw/data/template/account.tax.group-tw.csv` (20 lines)
- `addons/l10n_tw/demo/demo_company.xml` (36 lines)
- `addons/l10n_tw/i18n/l10n_tw.pot` (1,890 lines)
- `addons/l10n_tw/i18n/zh_TW.po` (1,894 lines)
- `addons/l10n_tw/models/__init__.py` (2 lines)
- `addons/l10n_tw/models/template_tw.py` (68 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
