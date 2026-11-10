# Module: test_populate

- **Module ID:** MOD-579
- **Path:** `addons/test_populate`
- **Manifest:** `addons/test_populate/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Test module for Odoo's Populate

Standalone testing module for Odoo Populate module.

Declared dependencies: `populate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 35 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "populate"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_populate/__init__.py` (1 lines)
- `addons/test_populate/__manifest__.py` (13 lines)
- `addons/test_populate/models/__init__.py` (1 lines)
- `addons/test_populate/models/test_models.py` (187 lines)
- `addons/test_populate/populate/sample_blueprints.xml` (302 lines)
- `addons/test_populate/security/ir.access.csv` (12 lines)
- `addons/test_populate/tests/__init__.py` (5 lines)
- `addons/test_populate/tests/blueprint/__init__.py` (6 lines)
- `addons/test_populate/tests/blueprint/test_basic.py` (337 lines)
- `addons/test_populate/tests/blueprint/test_import.py` (413 lines)
- `addons/test_populate/tests/blueprint/test_inheritance.py` (471 lines)
- `addons/test_populate/tests/blueprint/test_xml_parsing.py` (98 lines)
- `addons/test_populate/tests/common.py` (15 lines)
- `addons/test_populate/tests/generators/__init__.py` (13 lines)
- `addons/test_populate/tests/generators/test_binary.py` (129 lines)
- `addons/test_populate/tests/generators/test_choice.py` (70 lines)
- `addons/test_populate/tests/generators/test_fake.py` (199 lines)
- `addons/test_populate/tests/generators/test_features.py` (405 lines)
- `addons/test_populate/tests/generators/test_misc.py` (309 lines)
- `addons/test_populate/tests/generators/test_properties.py` (452 lines)
- `addons/test_populate/tests/generators/test_reference.py` (282 lines)
- `addons/test_populate/tests/generators/test_relation.py` (627 lines)
- `addons/test_populate/tests/generators/test_scalar.py` (171 lines)
- `addons/test_populate/tests/generators/test_temporal.py` (47 lines)
- `addons/test_populate/tests/generators/test_textual.py` (44 lines)
- `addons/test_populate/tests/integration/__init__.py` (10 lines)
- `addons/test_populate/tests/integration/test_populate_fields.py` (367 lines)
- `addons/test_populate/tests/integration/test_populate_import.py` (27 lines)
- `addons/test_populate/tests/integration/test_populate_model_data.py` (123 lines)
- `addons/test_populate/tests/integration/test_populate_nonstandard.py` (62 lines)
- `addons/test_populate/tests/integration/test_populate_unique.py` (128 lines)
- `addons/test_populate/tests/integration/test_populate_values.py` (213 lines)
- `addons/test_populate/tests/integration/test_session_basic.py` (220 lines)
- `addons/test_populate/tests/integration/test_session_jobs.py` (1,496 lines)
- `addons/test_populate/tests/utils/__init__.py` (7 lines)
- `addons/test_populate/tests/utils/test_distributions.py` (274 lines)
- `addons/test_populate/tests/utils/test_expression.py` (63 lines)
- `addons/test_populate/tests/utils/test_orm.py` (103 lines)
- `addons/test_populate/tests/utils/test_seed.py` (32 lines)
- `addons/test_populate/tests/utils/test_xml.py` (302 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
