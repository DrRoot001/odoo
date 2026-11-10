# Module: l10n_ke

- **Module ID:** MOD-250
- **Path:** `addons/l10n_ke`
- **Manifest:** `addons/l10n_ke/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This provides a base chart of accounts and taxes template for use in Odoo.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/account_tax_views.xml",
    "views/l10n_ke_item_code_views.xml",
    "data/l10n_ke.item.code.csv",
    "data/account_tax_report_data.xml",
    "data/account_wh_tax_report_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ke/__init__.py` (2 lines)
- `addons/l10n_ke/__manifest__.py` (29 lines)
- `addons/l10n_ke/data/account_tax_report_data.xml` (378 lines)
- `addons/l10n_ke/data/account_wh_tax_report_data.xml` (78 lines)
- `addons/l10n_ke/data/l10n_ke.item.code.csv` (344 lines)
- `addons/l10n_ke/data/template/account.account-ke.csv` (129 lines)
- `addons/l10n_ke/data/template/account.fiscal.position-ke.csv` (3 lines)
- `addons/l10n_ke/data/template/account.tax-ke.csv` (117 lines)
- `addons/l10n_ke/data/template/account.tax.group-ke.csv` (6 lines)
- `addons/l10n_ke/demo/demo_company.xml` (35 lines)
- `addons/l10n_ke/i18n/l10n_ke.pot` (354 lines)
- `addons/l10n_ke/i18n/sw.po` (358 lines)
- `addons/l10n_ke/models/__init__.py` (6 lines)
- `addons/l10n_ke/models/account_move.py` (14 lines)
- `addons/l10n_ke/models/account_tax.py` (19 lines)
- `addons/l10n_ke/models/l10n_ke_item_code.py` (25 lines)
- `addons/l10n_ke/models/res_company.py` (18 lines)
- `addons/l10n_ke/models/template_ke.py` (49 lines)
- `addons/l10n_ke/security/ir.access.csv` (3 lines)
- `addons/l10n_ke/views/account_move_views.xml` (16 lines)
- `addons/l10n_ke/views/account_tax_views.xml` (27 lines)
- `addons/l10n_ke/views/l10n_ke_item_code_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
