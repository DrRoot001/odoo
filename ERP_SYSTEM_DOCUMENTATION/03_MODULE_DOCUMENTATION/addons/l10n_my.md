# Module: l10n_my

- **Module ID:** MOD-278
- **Path:** `addons/l10n_my`
- **Manifest:** `addons/l10n_my/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Malaysia in Odoo.
==============================================================================
    

Declared dependencies: `account`, `account_tax_python`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
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
    "account",
    "account_tax_python"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/account.account.tag.csv",
    "views/product_template_view.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_my/__init__.py` (2 lines)
- `addons/l10n_my/__manifest__.py` (29 lines)
- `addons/l10n_my/data/account.account.tag.csv` (8 lines)
- `addons/l10n_my/data/account_tax_report_data.xml` (640 lines)
- `addons/l10n_my/data/template/account.account-my.csv` (240 lines)
- `addons/l10n_my/data/template/account.depreciation.model-my.csv` (7 lines)
- `addons/l10n_my/data/template/account.fiscal.position-my.csv` (6 lines)
- `addons/l10n_my/data/template/account.tax-my.csv` (141 lines)
- `addons/l10n_my/data/template/account.tax.group-my.csv` (11 lines)
- `addons/l10n_my/demo/demo_company.xml` (37 lines)
- `addons/l10n_my/i18n/l10n_my.pot` (133 lines)
- `addons/l10n_my/i18n/ms.po` (137 lines)
- `addons/l10n_my/migrations/1.1/end-migrate_update_taxes.py` (9 lines)
- `addons/l10n_my/models/__init__.py` (4 lines)
- `addons/l10n_my/models/product_template.py` (10 lines)
- `addons/l10n_my/models/res_partner.py` (11 lines)
- `addons/l10n_my/models/template_my.py` (82 lines)
- `addons/l10n_my/tests/__init__.py` (1 lines)
- `addons/l10n_my/tests/test_res_partner.py` (45 lines)
- `addons/l10n_my/views/product_template_view.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
