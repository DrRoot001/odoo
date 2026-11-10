# Module: test_html_field_history

- **Module ID:** MOD-573
- **Path:** `addons/test_html_field_history`
- **Manifest:** `addons/test_html_field_history/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `html_editor`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "html_editor"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_html_field_history/__init__.py` (4 lines)
- `addons/test_html_field_history/__manifest__.py` (12 lines)
- `addons/test_html_field_history/models/__init__.py` (4 lines)
- `addons/test_html_field_history/models/model_html_field_history_test.py` (19 lines)
- `addons/test_html_field_history/security/ir.access.csv` (2 lines)
- `addons/test_html_field_history/tests/__init__.py` (4 lines)
- `addons/test_html_field_history/tests/test_model.py` (138 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
