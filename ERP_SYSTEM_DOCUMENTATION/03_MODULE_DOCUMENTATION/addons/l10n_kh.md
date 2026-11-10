# Module: l10n_kh

- **Module ID:** MOD-252
- **Path:** `addons/l10n_kh`
- **Manifest:** `addons/l10n_kh/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    Chart Of Account and Taxes for Cambodia.
    

Declared dependencies: `account_qr_code_emv`, `l10n_account_withholding_tax`.

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
    "account_qr_code_emv",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/form_t7001.xml",
    "data/form_wt003.xml",
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_kh/__init__.py` (2 lines)
- `addons/l10n_kh/__manifest__.py` (26 lines)
- `addons/l10n_kh/data/form_t7001.xml` (649 lines)
- `addons/l10n_kh/data/form_wt003.xml` (256 lines)
- `addons/l10n_kh/data/template/account.account-kh.csv` (192 lines)
- `addons/l10n_kh/data/template/account.fiscal.position-kh.csv` (4 lines)
- `addons/l10n_kh/data/template/account.tax-kh.csv` (198 lines)
- `addons/l10n_kh/data/template/account.tax.group-kh.csv` (14 lines)
- `addons/l10n_kh/demo/demo_company.xml` (31 lines)
- `addons/l10n_kh/i18n/km.po` (541 lines)
- `addons/l10n_kh/i18n/l10n_kh.pot` (537 lines)
- `addons/l10n_kh/models/__init__.py` (4 lines)
- `addons/l10n_kh/models/res_bank.py` (95 lines)
- `addons/l10n_kh/models/template_kh.py` (53 lines)
- `addons/l10n_kh/views/res_bank_views.xml` (13 lines)
- `addons/l10n_kh/views/res_config_settings_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
