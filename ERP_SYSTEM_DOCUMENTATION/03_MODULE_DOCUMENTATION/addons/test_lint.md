# Module: test_lint

- **Module ID:** MOD-661
- **Path:** `odoo/addons/test_lint`
- **Manifest:** `odoo/addons/test_lint/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test Odoo code with various linters.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 27 | Test files found by path/name convention. |
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

- `odoo/addons/test_lint/__init__.py` (1 lines)
- `odoo/addons/test_lint/__manifest__.py` (9 lines)
- `odoo/addons/test_lint/tests/__init__.py` (21 lines)
- `odoo/addons/test_lint/tests/_odoo_checker_gettext.py` (116 lines)
- `odoo/addons/test_lint/tests/_odoo_checker_sql_injection.py` (392 lines)
- `odoo/addons/test_lint/tests/_odoo_checker_unlink_override.py` (42 lines)
- `odoo/addons/test_lint/tests/_pylint_path_setup.py` (71 lines)
- `odoo/addons/test_lint/tests/common.py` (60 lines)
- `odoo/addons/test_lint/tests/eslintrc` (76 lines)
- `odoo/addons/test_lint/tests/test_checkers.py` (498 lines)
- `odoo/addons/test_lint/tests/test_docstring.py` (358 lines)
- `odoo/addons/test_lint/tests/test_dunderinit.py` (21 lines)
- `odoo/addons/test_lint/tests/test_eslint.py` (51 lines)
- `odoo/addons/test_lint/tests/test_i18n.py` (128 lines)
- `odoo/addons/test_lint/tests/test_icons.py` (74 lines)
- `odoo/addons/test_lint/tests/test_index.py` (342 lines)
- `odoo/addons/test_lint/tests/test_jstranslate.py` (147 lines)
- `odoo/addons/test_lint/tests/test_l10n.py` (51 lines)
- `odoo/addons/test_lint/tests/test_manifests.py` (283 lines)
- `odoo/addons/test_lint/tests/test_markers.py` (41 lines)
- `odoo/addons/test_lint/tests/test_model_attributes.py` (45 lines)
- `odoo/addons/test_lint/tests/test_override_signatures.py` (226 lines)
- `odoo/addons/test_lint/tests/test_override_translated_fields.py` (128 lines)
- `odoo/addons/test_lint/tests/test_pofile.py` (25 lines)
- `odoo/addons/test_lint/tests/test_pylint.py` (111 lines)
- `odoo/addons/test_lint/tests/test_python_lint.py` (136 lines)
- `odoo/addons/test_lint/tests/test_routes.py` (50 lines)
- `odoo/addons/test_lint/tests/test_security_files.py` (33 lines)
- `odoo/addons/test_lint/tests/test_sql_injection.py` (522 lines)
- `odoo/addons/test_lint/tests/test_test_holes.py` (79 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
