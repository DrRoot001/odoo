# Module: l10n_mn

- **Module ID:** MOD-271
- **Path:** `addons/l10n_mn`
- **Manifest:** `addons/l10n_mn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the accounting chart for Mongolia.
===============================================================

    * the Mongolia Official Chart of Accounts,
    * the Tax Code Chart for Mongolia
    * the main taxes used in Mongolia

Financial requirement contributor: Baskhuu Lodoikhuu. BumanIT LLC


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "data/vat_report.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_mn/__init__.py` (2 lines)
- `addons/l10n_mn/__manifest__.py` (32 lines)
- `addons/l10n_mn/data/account.account.tag.csv` (37 lines)
- `addons/l10n_mn/data/template/account.account-mn.csv` (305 lines)
- `addons/l10n_mn/data/template/account.fiscal.position-mn.csv` (5 lines)
- `addons/l10n_mn/data/template/account.tax-mn.csv` (165 lines)
- `addons/l10n_mn/data/template/account.tax.group-mn.csv` (7 lines)
- `addons/l10n_mn/data/vat_report.xml` (678 lines)
- `addons/l10n_mn/demo/demo_company.xml` (36 lines)
- `addons/l10n_mn/i18n/l10n_mn.pot` (470 lines)
- `addons/l10n_mn/i18n/mn.po` (533 lines)
- `addons/l10n_mn/models/__init__.py` (2 lines)
- `addons/l10n_mn/models/template_mn.py` (37 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
