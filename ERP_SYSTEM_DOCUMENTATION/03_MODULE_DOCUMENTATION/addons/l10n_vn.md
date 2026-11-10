# Module: l10n_vn

- **Module ID:** MOD-341
- **Path:** `addons/l10n_vn`
- **Manifest:** `addons/l10n_vn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the accounting chart, bank information for Vietnam in Odoo.
========================================================================================

- This module applies to companies based in Vietnamese Accounting Standard (VAS)
  with Chart of account under Circular No. 200/2014/TT-BTC
- Add Vietnamese bank information (like name, bic ..) as announced and yearly updated by State Bank
  of Viet Nam (https://sbv.gov.vn/webcenter/portal/en/home/sbv/paytreasury/bankidno).
- Add VietQR feature for invoice

**Credits:**
    - General Solutions.
    - Trobz
    - Jean Nguyen - The Bean Family (https://github.com/anhjean/vietqr) for VietQR.



Declared dependencies: `account_qr_code_emv`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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
    "data/account_tax_report_data.xml",
    "views/account_move_views.xml",
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_vn/__init__.py` (2 lines)
- `addons/l10n_vn/__manifest__.py` (41 lines)
- `addons/l10n_vn/data/account_tax_report_data.xml` (693 lines)
- `addons/l10n_vn/data/template/account.account-vn.csv` (302 lines)
- `addons/l10n_vn/data/template/account.tax-vn.csv` (101 lines)
- `addons/l10n_vn/data/template/account.tax.group-vn.csv` (8 lines)
- `addons/l10n_vn/demo/demo_company.xml` (36 lines)
- `addons/l10n_vn/i18n/l10n_vn.pot` (197 lines)
- `addons/l10n_vn/i18n/vi.po` (209 lines)
- `addons/l10n_vn/migrations/14.0.2.0.1/post-migration.py` (22 lines)
- `addons/l10n_vn/migrations/17.0.2.0.2/post-migration.py` (27 lines)
- `addons/l10n_vn/migrations/2.0.3/end-migrate_update_taxes.py` (13 lines)
- `addons/l10n_vn/models/__init__.py` (4 lines)
- `addons/l10n_vn/models/account_move.py` (12 lines)
- `addons/l10n_vn/models/res_bank.py` (100 lines)
- `addons/l10n_vn/models/template_vn.py` (65 lines)
- `addons/l10n_vn/tests/__init__.py` (2 lines)
- `addons/l10n_vn/tests/test_l10n_vn_account_codes.py` (30 lines)
- `addons/l10n_vn/tests/test_l10n_vn_emv_qr.py` (132 lines)
- `addons/l10n_vn/views/account_move_views.xml` (23 lines)
- `addons/l10n_vn/views/res_bank_views.xml` (17 lines)
- `addons/l10n_vn/views/res_config_settings_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
