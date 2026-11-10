# Module: l10n_pk

- **Module ID:** MOD-295
- **Path:** `addons/l10n_pk`
- **Manifest:** `addons/l10n_pk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Pakistan Accounting Module
=======================================================
Pakistan accounting basic charts and localization.

Activates:

- Chart of Accounts
- Taxes
- Tax Report
- Withholding Tax Report
    

Declared dependencies: `account`, `account_tax_python`, `l10n_account_withholding_tax`, `product`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_tax_python",
    "l10n_account_withholding_tax",
    "product"
  ],
  "data": [
    "data/ir_actions_server_data.xml",
    "data/ir_config_data.xml",
    "data/res_country_data.xml",
    "views/account_tax_views.xml"
  ],
  "demo": [
    "demo/res_partner_demo.xml",
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pk/__init__.py` (2 lines)
- `addons/l10n_pk/__manifest__.py` (39 lines)
- `addons/l10n_pk/data/ir_actions_server_data.xml` (10 lines)
- `addons/l10n_pk/data/ir_config_data.xml` (7 lines)
- `addons/l10n_pk/data/res_country_data.xml` (8 lines)
- `addons/l10n_pk/data/template/account.account-pk.csv` (200 lines)
- `addons/l10n_pk/data/template/account.depreciation.model-pk.csv` (6 lines)
- `addons/l10n_pk/data/template/account.tax-pk.csv` (53 lines)
- `addons/l10n_pk/data/template/account.tax.group-pk.csv` (5 lines)
- `addons/l10n_pk/demo/__init__.py` (1 lines)
- `addons/l10n_pk/demo/account_demo.py` (274 lines)
- `addons/l10n_pk/demo/demo_company.xml` (37 lines)
- `addons/l10n_pk/demo/res_partner_demo.xml` (40 lines)
- `addons/l10n_pk/migrations/1.1/end-migrate_update_taxes.py` (7 lines)
- `addons/l10n_pk/models/__init__.py` (5 lines)
- `addons/l10n_pk/models/account_journal.py` (26 lines)
- `addons/l10n_pk/models/account_tax.py` (21 lines)
- `addons/l10n_pk/models/res_company.py` (41 lines)
- `addons/l10n_pk/models/res_config_settings.py` (16 lines)
- `addons/l10n_pk/models/template_pk.py` (69 lines)
- `addons/l10n_pk/tests/__init__.py` (1 lines)
- `addons/l10n_pk/tests/test_l10n_pk_identifiers.py` (43 lines)
- `addons/l10n_pk/views/account_tax_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
