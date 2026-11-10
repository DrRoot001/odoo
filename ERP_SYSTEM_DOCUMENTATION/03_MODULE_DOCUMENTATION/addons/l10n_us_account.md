# Module: l10n_us_account

- **Module ID:** MOD-337
- **Path:** `addons/l10n_us_account`
- **Manifest:** `addons/l10n_us_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    

Declared dependencies: `l10n_us`, `account`, `base_address_extended`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_us",
    "account",
    "base_address_extended"
  ],
  "data": [
    "views/l10n_us_account_menus.xml",
    "views/account_tax_views.xml",
    "views/res_partner_bank_views.xml",
    "views/res_config_settings_views.xml",
    "data/tax_report.xml",
    "data/uom_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_us_account/__init__.py` (6 lines)
- `addons/l10n_us_account/__manifest__.py` (26 lines)
- `addons/l10n_us_account/data/tax_report.xml` (21 lines)
- `addons/l10n_us_account/data/template/account.account-us.csv` (130 lines)
- `addons/l10n_us_account/data/template/account.depreciation.model-us.csv` (7 lines)
- `addons/l10n_us_account/data/template/account.fiscal.position-us.csv` (3 lines)
- `addons/l10n_us_account/data/template/account.tax-us.csv` (185 lines)
- `addons/l10n_us_account/data/template/account.tax.group-us.csv` (24 lines)
- `addons/l10n_us_account/data/uom_data.xml` (29 lines)
- `addons/l10n_us_account/demo/__init__.py` (2 lines)
- `addons/l10n_us_account/demo/account_demo.py` (157 lines)
- `addons/l10n_us_account/demo/demo_company.xml` (11 lines)
- `addons/l10n_us_account/i18n/es_419.po` (194 lines)
- `addons/l10n_us_account/i18n/l10n_us_account.pot` (187 lines)
- `addons/l10n_us_account/models/__init__.py` (5 lines)
- `addons/l10n_us_account/models/account_tax.py` (98 lines)
- `addons/l10n_us_account/models/res_config_settings.py` (7 lines)
- `addons/l10n_us_account/models/res_partner_bank.py` (16 lines)
- `addons/l10n_us_account/models/template_us.py` (140 lines)
- `addons/l10n_us_account/views/account_tax_views.xml` (53 lines)
- `addons/l10n_us_account/views/l10n_us_account_menus.xml` (14 lines)
- `addons/l10n_us_account/views/res_config_settings_views.xml` (21 lines)
- `addons/l10n_us_account/views/res_partner_bank_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
