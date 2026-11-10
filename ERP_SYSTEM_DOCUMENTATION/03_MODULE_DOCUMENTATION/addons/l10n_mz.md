# Module: l10n_mz

- **Module ID:** MOD-282
- **Path:** `addons/l10n_mz`
- **Manifest:** `addons/l10n_mz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Mozambican Accounting localization
    

Declared dependencies: `base`, `account`.

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
    "base",
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

- `addons/l10n_mz/__init__.py` (2 lines)
- `addons/l10n_mz/__manifest__.py` (24 lines)
- `addons/l10n_mz/data/tax_report.xml` (308 lines)
- `addons/l10n_mz/data/template/account.account-mz.csv` (412 lines)
- `addons/l10n_mz/data/template/account.fiscal.position-mz.csv` (3 lines)
- `addons/l10n_mz/data/template/account.tax-mz.csv` (45 lines)
- `addons/l10n_mz/data/template/account.tax.group-mz.csv` (4 lines)
- `addons/l10n_mz/demo/demo_company.xml` (35 lines)
- `addons/l10n_mz/i18n/l10n_mz.pot` (247 lines)
- `addons/l10n_mz/i18n/pt.po` (251 lines)
- `addons/l10n_mz/models/__init__.py` (2 lines)
- `addons/l10n_mz/models/template_mz.py` (35 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
