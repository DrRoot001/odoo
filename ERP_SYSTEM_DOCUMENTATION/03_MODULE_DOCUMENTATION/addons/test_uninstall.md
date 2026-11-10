# Module: test_uninstall

- **Module ID:** MOD-665
- **Path:** `odoo/addons/test_uninstall`
- **Manifest:** `odoo/addons/test_uninstall/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test the uninstall feature.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 3 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 1 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "ir.access.csv"
  ]
}
```

### Representative source files

- `odoo/addons/test_uninstall/__init__.py` (4 lines)
- `odoo/addons/test_uninstall/__manifest__.py` (11 lines)
- `odoo/addons/test_uninstall/ir.access.csv` (2 lines)
- `odoo/addons/test_uninstall/models.py` (43 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
