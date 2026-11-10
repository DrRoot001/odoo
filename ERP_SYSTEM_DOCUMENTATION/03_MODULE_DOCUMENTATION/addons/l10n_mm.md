# Module: l10n_mm

- **Module ID:** MOD-270
- **Path:** `addons/l10n_mm`
- **Manifest:** `addons/l10n_mm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    Chart Of Account and Taxes for Myanmar.
    

Declared dependencies: `account_qr_code_emv`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
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
    "l10n_account_withholding_tax"
  ],
  "data": [
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_mm/__init__.py` (2 lines)
- `addons/l10n_mm/__manifest__.py` (24 lines)
- `addons/l10n_mm/data/template/account.account-mm.csv` (132 lines)
- `addons/l10n_mm/data/template/account.tax-mm.csv` (77 lines)
- `addons/l10n_mm/data/template/account.tax.group-mm.csv` (11 lines)
- `addons/l10n_mm/demo/demo_company.xml` (35 lines)
- `addons/l10n_mm/i18n/l10n_mm.pot` (161 lines)
- `addons/l10n_mm/i18n/my.po` (161 lines)
- `addons/l10n_mm/models/__init__.py` (3 lines)
- `addons/l10n_mm/models/res_bank.py` (106 lines)
- `addons/l10n_mm/models/template_mm.py` (58 lines)
- `addons/l10n_mm/tests/__init__.py` (2 lines)
- `addons/l10n_mm/tests/test_l10n_mm_emv_qr.py` (159 lines)
- `addons/l10n_mm/views/res_bank_views.xml` (15 lines)
- `addons/l10n_mm/views/res_config_settings_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
