# Module: l10n_qa

- **Module ID:** MOD-302
- **Path:** `addons/l10n_qa`
- **Manifest:** `addons/l10n_qa/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Qatar in Odoo.
==============================================================================
Qatar accounting basic charts and localization.
Activates:
- Chart of accounts
    

Declared dependencies: `account`, `l10n_gcc_invoice`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_gcc_invoice"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_qa/__init__.py` (1 lines)
- `addons/l10n_qa/__manifest__.py` (22 lines)
- `addons/l10n_qa/data/template/account.account-qa.csv` (166 lines)
- `addons/l10n_qa/demo/demo_company.xml` (36 lines)
- `addons/l10n_qa/i18n/ar.po` (182 lines)
- `addons/l10n_qa/i18n/l10n_qa.pot` (156 lines)
- `addons/l10n_qa/models/__init__.py` (1 lines)
- `addons/l10n_qa/models/template_qa.py` (47 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
