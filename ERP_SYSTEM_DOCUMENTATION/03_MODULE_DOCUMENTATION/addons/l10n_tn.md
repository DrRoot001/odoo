# Module: l10n_tn

- **Module ID:** MOD-325
- **Path:** `addons/l10n_tn`
- **Manifest:** `addons/l10n_tn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the accounting chart for Tunisia in Odoo.
=======================================================================


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

- `addons/l10n_tn/__init__.py` (2 lines)
- `addons/l10n_tn/__manifest__.py` (23 lines)
- `addons/l10n_tn/data/tax_report.xml` (465 lines)
- `addons/l10n_tn/data/template/account.account-tn.csv` (451 lines)
- `addons/l10n_tn/data/template/account.fiscal.position-tn.csv` (4 lines)
- `addons/l10n_tn/data/template/account.tax-tn.csv` (117 lines)
- `addons/l10n_tn/data/template/account.tax.group-tn.csv` (10 lines)
- `addons/l10n_tn/demo/demo_company.xml` (34 lines)
- `addons/l10n_tn/i18n/ar.po` (59 lines)
- `addons/l10n_tn/i18n/fr.po` (58 lines)
- `addons/l10n_tn/i18n/l10n_tn.pot` (54 lines)
- `addons/l10n_tn/models/__init__.py` (2 lines)
- `addons/l10n_tn/models/template_tn.py` (47 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
