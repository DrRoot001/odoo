# Module: test_import_export

- **Module ID:** MOD-574
- **Path:** `addons/test_import_export`
- **Manifest:** `addons/test_import_export/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Base Import & Export Tests: Ensure Flow Robustness

This module contains tests related to base import and export.

Declared dependencies: `web`, `base_import`, `website`, `test_base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web",
    "base_import",
    "website",
    "test_base"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/test_import_export/__init__.py` (1 lines)
- `addons/test_import_export/__manifest__.py` (14 lines)
- `addons/test_import_export/data/contacts.json` (1 lines)
- `addons/test_import_export/data/contacts_big.json` (1 lines)
- `addons/test_import_export/data/generated_0.xls` (16 lines)
- `addons/test_import_export/data/generated_0.xlsx` (34 lines)
- `addons/test_import_export/data/generated_1.xls` (16 lines)
- `addons/test_import_export/data/generated_1.xlsx` (33 lines)
- `addons/test_import_export/data/test_import.ods` (45 lines)
- `addons/test_import_export/data/test_import.xls` (33 lines)
- `addons/test_import_export/data/test_import.xlsx` (47 lines)
- `addons/test_import_export/models/__init__.py` (3 lines)
- `addons/test_import_export/models/models_export.py` (42 lines)
- `addons/test_import_export/models/models_export_impex.py` (353 lines)
- `addons/test_import_export/models/models_import.py` (169 lines)
- `addons/test_import_export/security/ir.access.csv` (57 lines)
- `addons/test_import_export/tests/__init__.py` (8 lines)
- `addons/test_import_export/tests/test_export.py` (788 lines)
- `addons/test_import_export/tests/test_export_impex.py` (705 lines)
- `addons/test_import_export/tests/test_import.py` (1,670 lines)
- `addons/test_import_export/tests/test_import_csv_magic.py` (155 lines)
- `addons/test_import_export/tests/test_import_files.py` (55 lines)
- `addons/test_import_export/tests/test_load.py` (1,828 lines)
- `addons/test_import_export/tests/test_properties.py` (590 lines)
- `addons/test_import_export/tests/test_security.py` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
