# Module: test_l10n

- **Module ID:** MOD-660
- **Path:** `odoo/addons/test_l10n`
- **Manifest:** `odoo/addons/test_l10n/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test all localizations.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ]
}
```

### Representative source files

- `odoo/addons/test_l10n/__init__.py` (0 lines)
- `odoo/addons/test_l10n/__manifest__.py` (9 lines)
- `odoo/addons/test_l10n/tests/__init__.py` (2 lines)
- `odoo/addons/test_l10n/tests/install_all_l10n.py` (17 lines)
- `odoo/addons/test_l10n/tests/test_country.py` (48 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
