# Module: test_install_auto

- **Module ID:** MOD-651
- **Path:** `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto`
- **Manifest:** `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `True`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `test_install_base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "test_install_base"
  ],
  "data": [
    "data/ir_cron.xml"
  ]
}
```

### Representative source files

- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/__init__.py` (1 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/__manifest__.py` (13 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/data/ir_cron.xml` (15 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/models/__init__.py` (1 lines)
- `odoo/addons/test_base/tests/test_modules/test_install_addons/test_install_auto/models/res_currency.py` (11 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
