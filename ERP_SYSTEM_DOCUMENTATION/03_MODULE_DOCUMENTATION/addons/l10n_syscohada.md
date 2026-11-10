# Module: l10n_syscohada

- **Module ID:** MOD-320
- **Path:** `addons/l10n_syscohada`
- **Manifest:** `addons/l10n_syscohada/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements the accounting chart for OHADA area.
===========================================================

It allows any company or association to manage its financial accounting.

Countries that use OHADA are the following:
-------------------------------------------
    Benin, Burkina Faso, Cameroon, Central African Republic, Comoros, Congo,

    Ivory Coast, Gabon, Guinea, Guinea Bissau, Equatorial Guinea, Mali, Niger,

    Democratic Republic of the Congo, Senegal, Chad, Togo.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "account"
  ],
  "data": [
    "data/menuitem_data.xml"
  ]
}
```

### Representative source files

- `addons/l10n_syscohada/__init__.py` (2 lines)
- `addons/l10n_syscohada/__manifest__.py` (28 lines)
- `addons/l10n_syscohada/data/menuitem_data.xml` (4 lines)
- `addons/l10n_syscohada/data/template/account.account-syscebnl.csv` (454 lines)
- `addons/l10n_syscohada/data/template/account.account-syscohada.csv` (1,135 lines)
- `addons/l10n_syscohada/data/template/account.account.group-syscebnl.csv` (92 lines)
- `addons/l10n_syscohada/i18n/fr.po` (65 lines)
- `addons/l10n_syscohada/i18n/l10n_syscohada.pot` (59 lines)
- `addons/l10n_syscohada/models/__init__.py` (3 lines)
- `addons/l10n_syscohada/models/template_syscebnl.py` (35 lines)
- `addons/l10n_syscohada/models/template_syscohada.py` (32 lines)
- `addons/l10n_syscohada/static/description/icon.jpeg` (94 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
