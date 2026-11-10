# Module: test_spreadsheet

- **Module ID:** MOD-583
- **Path:** `addons/test_spreadsheet`
- **Manifest:** `addons/test_spreadsheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Spreadsheet Test, mainly to test the mixin behavior

This module contains tests related to spreadsheet.
    The modules exposes some mixin that are only implemented in other functional modules.
    When trying to test a global behavior of the mixin, it makes no sense to test it in
    each module implementing the mixin but rather test a dummy implementation of the later,
    hence the need for this test module.
    

Declared dependencies: `spreadsheet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "spreadsheet"
  ],
  "data": [
    "security/spreadsheet_test_security.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_spreadsheet/__init__.py` (1 lines)
- `addons/test_spreadsheet/__manifest__.py` (17 lines)
- `addons/test_spreadsheet/models/__init__.py` (1 lines)
- `addons/test_spreadsheet/models/spreadsheet_mixin_test.py` (9 lines)
- `addons/test_spreadsheet/security/ir.access.csv` (3 lines)
- `addons/test_spreadsheet/security/spreadsheet_test_security.xml` (9 lines)
- `addons/test_spreadsheet/tests/__init__.py` (1 lines)
- `addons/test_spreadsheet/tests/test_spreadsheet.py` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
