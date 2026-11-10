# Module: l10n_id

- **Module ID:** MOD-221
- **Path:** `addons/l10n_id`
- **Manifest:** `addons/l10n_id/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the latest Indonesian Odoo localisation necessary to run Odoo accounting for SMEs with:
=================================================================================================
    - generic Indonesian chart of accounts
    - tax structure

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/ir_cron.xml",
    "views/account_move_views.xml",
    "views/res_bank.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_id/__init__.py` (13 lines)
- `addons/l10n_id/__manifest__.py` (31 lines)
- `addons/l10n_id/controllers/__init__.py` (1 lines)
- `addons/l10n_id/controllers/portal.py` (13 lines)
- `addons/l10n_id/data/ir_cron.xml` (12 lines)
- `addons/l10n_id/data/template/account.account-id.csv` (201 lines)
- `addons/l10n_id/data/template/account.depreciation.model-id.csv` (7 lines)
- `addons/l10n_id/data/template/account.fiscal.position-id.csv` (4 lines)
- `addons/l10n_id/data/template/account.tax-id.csv` (76 lines)
- `addons/l10n_id/data/template/account.tax.group-id.csv` (8 lines)
- `addons/l10n_id/demo/demo_company.xml` (36 lines)
- `addons/l10n_id/i18n/id.po` (268 lines)
- `addons/l10n_id/i18n/l10n_id.pot` (250 lines)
- `addons/l10n_id/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_id/migrations/1.2/end-migrate_update_taxes.py` (40 lines)
- `addons/l10n_id/migrations/1.3/end-migrate_update_taxes.py` (136 lines)
- `addons/l10n_id/models/__init__.py` (6 lines)
- `addons/l10n_id/models/account_move.py` (153 lines)
- `addons/l10n_id/models/qris_transaction.py` (83 lines)
- `addons/l10n_id/models/res_bank.py` (151 lines)
- `addons/l10n_id/models/template_id.py` (95 lines)
- `addons/l10n_id/security/ir.access.csv` (2 lines)
- `addons/l10n_id/tests/__init__.py` (2 lines)
- `addons/l10n_id/tests/test_qris.py` (197 lines)
- `addons/l10n_id/tests/test_qris_transaction.py` (112 lines)
- `addons/l10n_id/views/account_move_views.xml` (15 lines)
- `addons/l10n_id/views/res_bank.xml` (16 lines)
- `addons/l10n_id/views/res_config_settings_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
