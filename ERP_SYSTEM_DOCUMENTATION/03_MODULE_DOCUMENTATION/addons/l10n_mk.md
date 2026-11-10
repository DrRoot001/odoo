# Module: l10n_mk

- **Module ID:** MOD-268
- **Path:** `addons/l10n_mk`
- **Manifest:** `addons/l10n_mk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    Chart Of Account and Taxes for North Macedonia.
    

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

- `addons/l10n_mk/__init__.py` (1 lines)
- `addons/l10n_mk/__manifest__.py` (21 lines)
- `addons/l10n_mk/data/tax_report.xml` (343 lines)
- `addons/l10n_mk/data/template/account.account-mk.csv` (433 lines)
- `addons/l10n_mk/data/template/account.fiscal.position-mk.csv` (14 lines)
- `addons/l10n_mk/data/template/account.tax-mk.csv` (37 lines)
- `addons/l10n_mk/data/template/account.tax.group-mk.csv` (5 lines)
- `addons/l10n_mk/demo/demo_company.xml` (35 lines)
- `addons/l10n_mk/i18n/l10n_mk.pot` (43 lines)
- `addons/l10n_mk/i18n/mk.po` (46 lines)
- `addons/l10n_mk/models/__init__.py` (1 lines)
- `addons/l10n_mk/models/template_mk.py` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
