# Module: l10n_hk

- **Module ID:** MOD-214
- **Path:** `addons/l10n_hk`
- **Manifest:** `addons/l10n_hk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

 This is the base module to manage chart of accounting and localization for Hong Kong 

Declared dependencies: `account_qr_code_emv`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_qr_code_emv",
    "account"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/account_chart_template_data.xml",
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_hk/__init__.py` (2 lines)
- `addons/l10n_hk/__manifest__.py` (25 lines)
- `addons/l10n_hk/data/account.account.tag.csv` (4 lines)
- `addons/l10n_hk/data/account_chart_template_data.xml` (8 lines)
- `addons/l10n_hk/data/template/account.account-hk.csv` (218 lines)
- `addons/l10n_hk/data/template/account.depreciation.model-hk.csv` (8 lines)
- `addons/l10n_hk/demo/demo_company.xml` (37 lines)
- `addons/l10n_hk/i18n/l10n_hk.pot` (157 lines)
- `addons/l10n_hk/i18n/zh_TW.po` (168 lines)
- `addons/l10n_hk/models/__init__.py` (3 lines)
- `addons/l10n_hk/models/res_bank.py` (80 lines)
- `addons/l10n_hk/models/template_hk.py` (79 lines)
- `addons/l10n_hk/tests/__init__.py` (1 lines)
- `addons/l10n_hk/tests/test_l10n_hk_emv_qr.py` (121 lines)
- `addons/l10n_hk/views/res_bank_views.xml` (17 lines)
- `addons/l10n_hk/views/res_config_settings_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
