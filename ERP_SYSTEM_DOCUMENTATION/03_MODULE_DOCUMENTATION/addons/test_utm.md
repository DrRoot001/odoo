# Module: test_utm

- **Module ID:** MOD-585
- **Path:** `addons/test_utm`
- **Manifest:** `addons/test_utm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

UTM Tests: tests specific to the UTM module

This module contains tests related to UTMs. Those are
present in a separate module as it contains models used only to perform
tests independently to functional aspects of other models. 

Declared dependencies: `utm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "utm"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_utm/__init__.py` (3 lines)
- `addons/test_utm/__manifest__.py` (19 lines)
- `addons/test_utm/models/__init__.py` (4 lines)
- `addons/test_utm/models/test_utm_mailing.py` (10 lines)
- `addons/test_utm/models/test_utm_sale_order.py` (11 lines)
- `addons/test_utm/security/ir.access.csv` (3 lines)
- `addons/test_utm/tests/__init__.py` (3 lines)
- `addons/test_utm/tests/test_utm_mixin.py` (95 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
