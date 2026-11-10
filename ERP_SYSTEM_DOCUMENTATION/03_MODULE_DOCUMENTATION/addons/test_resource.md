# Module: test_resource

- **Module ID:** MOD-580
- **Path:** `addons/test_resource`
- **Manifest:** `addons/test_resource/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `resource`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "resource"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_resource/__init__.py` (4 lines)
- `addons/test_resource/__manifest__.py` (13 lines)
- `addons/test_resource/models/__init__.py` (4 lines)
- `addons/test_resource/models/test_resource.py` (45 lines)
- `addons/test_resource/security/ir.access.csv` (4 lines)
- `addons/test_resource/tests/__init__.py` (12 lines)
- `addons/test_resource/tests/common.py` (163 lines)
- `addons/test_resource/tests/test_2_weeks_calendar.py` (258 lines)
- `addons/test_resource/tests/test_calendar.py` (369 lines)
- `addons/test_resource/tests/test_extract_comodel_domain.py` (166 lines)
- `addons/test_resource/tests/test_mixin.py` (479 lines)
- `addons/test_resource/tests/test_performance.py` (51 lines)
- `addons/test_resource/tests/test_resource.py` (96 lines)
- `addons/test_resource/tests/test_resource_errors.py` (31 lines)
- `addons/test_resource/tests/test_timezones.py` (199 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
