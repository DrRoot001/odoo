# Module: test_base_automation

- **Module ID:** MOD-569
- **Path:** `addons/test_base_automation`
- **Manifest:** `addons/test_base_automation/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Base Automation Tests: Ensure Flow Robustness

This module contains tests related to base automation. Those are
present in a separate module as it contains models used only to perform
tests independently to functional aspects of other models.

Declared dependencies: `base_automation`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_automation"
  ],
  "data": [
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "test_base_automation/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_base_automation/__init__.py` (4 lines)
- `addons/test_base_automation/__manifest__.py` (22 lines)
- `addons/test_base_automation/models/__init__.py` (4 lines)
- `addons/test_base_automation/models/test_base_automation.py` (208 lines)
- `addons/test_base_automation/security/ir.access.csv` (14 lines)
- `addons/test_base_automation/static/tests/tour/base_automation_tour.js` (668 lines)
- `addons/test_base_automation/tests/__init__.py` (6 lines)
- `addons/test_base_automation/tests/test_flow.py` (1,949 lines)
- `addons/test_base_automation/tests/test_server_actions.py` (80 lines)
- `addons/test_base_automation/tests/test_tour.py` (304 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
