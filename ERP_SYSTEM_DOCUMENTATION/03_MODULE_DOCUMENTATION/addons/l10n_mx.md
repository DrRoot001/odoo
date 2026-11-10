# Module: l10n_mx

- **Module ID:** MOD-277
- **Path:** `addons/l10n_mx`
- **Manifest:** `addons/l10n_mx/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Minimal accounting configuration for Mexico.
============================================

This Chart of account is a minimal proposal to be able to use OoB the
accounting feature of Odoo.

This doesn't pretend be all the localization for MX it is just the minimal
data required to start from 0 in mexican localization.

This modules and its content is updated frequently by openerp-mexico team.

With this module you will have:

 - Minimal chart of account tested in production environments.
 - Minimal chart of taxes, to comply with SAT_ requirements.

.. _SAT: http://www.sat.gob.mx/
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
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
    "data/account.account.tag.csv",
    "data/account_report_diot.xml",
    "views/account_views.xml",
    "views/account_tax_view.xml",
    "views/res_config_settings_views.xml",
    "data/l10n_mx_uom.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_mx/__init__.py` (8 lines)
- `addons/l10n_mx/__manifest__.py` (46 lines)
- `addons/l10n_mx/data/account.account.tag.csv` (3 lines)
- `addons/l10n_mx/data/account_report_diot.xml` (372 lines)
- `addons/l10n_mx/data/l10n_mx_uom.xml` (18 lines)
- `addons/l10n_mx/data/template/account.account-mx.csv` (325 lines)
- `addons/l10n_mx/data/template/account.asset-mx.csv` (10 lines)
- `addons/l10n_mx/data/template/account.depreciation.model-mx.csv` (6 lines)
- `addons/l10n_mx/data/template/account.fiscal.position-mx.csv` (6 lines)
- `addons/l10n_mx/data/template/account.tax-mx.csv` (139 lines)
- `addons/l10n_mx/data/template/account.tax.group-mx.csv` (15 lines)
- `addons/l10n_mx/demo/demo_company.xml` (46 lines)
- `addons/l10n_mx/i18n/es_419.po` (289 lines)
- `addons/l10n_mx/i18n/l10n_mx.pot` (204 lines)
- `addons/l10n_mx/migrations/2.1/post-migrate.py` (15 lines)
- `addons/l10n_mx/migrations/2.2/end-migrate.py` (7 lines)
- `addons/l10n_mx/migrations/2.4/post-migrate.py` (19 lines)
- `addons/l10n_mx/models/__init__.py` (7 lines)
- `addons/l10n_mx/models/account_account.py` (24 lines)
- `addons/l10n_mx/models/account_move_line.py` (18 lines)
- `addons/l10n_mx/models/account_tax.py` (34 lines)
- `addons/l10n_mx/models/res_company.py` (16 lines)
- `addons/l10n_mx/models/res_config_settings.py` (15 lines)
- `addons/l10n_mx/models/template_mx.py` (106 lines)
- `addons/l10n_mx/tests/__init__.py` (3 lines)
- `addons/l10n_mx/tests/common.py` (41 lines)
- `addons/l10n_mx/tests/test_account_account.py` (42 lines)
- `addons/l10n_mx/tests/test_account_move.py` (58 lines)
- `addons/l10n_mx/views/account_tax_view.xml` (13 lines)
- `addons/l10n_mx/views/account_views.xml` (13 lines)
- `addons/l10n_mx/views/res_config_settings_views.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
