# Module: l10n_uz

- **Module ID:** MOD-339
- **Path:** `addons/l10n_uz`
- **Manifest:** `addons/l10n_uz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Uzbekistan Accounting: Chart of Account.
========================================

Uzbekistan accounting chart and localization.
  

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
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
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_uz/__init__.py` (1 lines)
- `addons/l10n_uz/__manifest__.py` (24 lines)
- `addons/l10n_uz/data/account.account.tag.csv` (92 lines)
- `addons/l10n_uz/data/template/account.account-uz.csv` (275 lines)
- `addons/l10n_uz/data/template/account.tax-uz.csv` (17 lines)
- `addons/l10n_uz/data/template/account.tax.group-uz.csv` (4 lines)
- `addons/l10n_uz/demo/demo_company.xml` (39 lines)
- `addons/l10n_uz/i18n/l10n_uz.pot` (63 lines)
- `addons/l10n_uz/i18n/ru.po` (67 lines)
- `addons/l10n_uz/i18n/uz.po` (66 lines)
- `addons/l10n_uz/models/__init__.py` (2 lines)
- `addons/l10n_uz/models/res_partner.py` (13 lines)
- `addons/l10n_uz/models/template_uz.py` (35 lines)
- `addons/l10n_uz/views/report_invoice.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
