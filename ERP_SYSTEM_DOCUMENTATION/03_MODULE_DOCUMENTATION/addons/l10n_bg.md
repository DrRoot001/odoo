# Module: l10n_bg

- **Module ID:** MOD-133
- **Path:** `addons/l10n_bg`
- **Manifest:** `addons/l10n_bg/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart accounting and taxes for Bulgaria
    

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
    "data/tax_report.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_bg/__init__.py` (2 lines)
- `addons/l10n_bg/__manifest__.py` (23 lines)
- `addons/l10n_bg/data/tax_report.xml` (471 lines)
- `addons/l10n_bg/data/template/account.account-bg.csv` (333 lines)
- `addons/l10n_bg/data/template/account.fiscal.position-bg.csv` (5 lines)
- `addons/l10n_bg/data/template/account.tax-bg.csv` (113 lines)
- `addons/l10n_bg/data/template/account.tax.group-bg.csv` (4 lines)
- `addons/l10n_bg/demo/demo_company.xml` (43 lines)
- `addons/l10n_bg/i18n/bg.po` (47 lines)
- `addons/l10n_bg/i18n/l10n_bg.pot` (43 lines)
- `addons/l10n_bg/models/__init__.py` (2 lines)
- `addons/l10n_bg/models/template_bg.py` (35 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
