# Module: test_web

- **Module ID:** MOD-666
- **Path:** `odoo/addons/test_web`
- **Manifest:** `odoo/addons/test_web/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Tests for the search panel python methods

Declared dependencies: `web`, `test_base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 20 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web",
    "test_base"
  ],
  "data": [
    "ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "test_web/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `odoo/addons/test_web/__init__.py` (1 lines)
- `odoo/addons/test_web/__manifest__.py` (20 lines)
- `odoo/addons/test_web/ir.access.csv` (8 lines)
- `odoo/addons/test_web/models/__init__.py` (4 lines)
- `odoo/addons/test_web/models/models.py` (50 lines)
- `odoo/addons/test_web/models/test_orm.py` (72 lines)
- `odoo/addons/test_web/models/test_read_group.py` (7 lines)
- `odoo/addons/test_web/models/test_web.py` (33 lines)
- `odoo/addons/test_web/static/tests/tours/translate.tours.js` (68 lines)
- `odoo/addons/test_web/static/tests/tours/x2many.js` (564 lines)
- `odoo/addons/test_web/tests/__init__.py` (16 lines)
- `odoo/addons/test_web/tests/test_fields.py` (41 lines)
- `odoo/addons/test_web/tests/test_onchange.py` (1,499 lines)
- `odoo/addons/test_web/tests/test_properties.py` (1,382 lines)
- `odoo/addons/test_web/tests/test_read_group_formatted.py` (2,299 lines)
- `odoo/addons/test_web/tests/test_read_grouping_sets.py` (441 lines)
- `odoo/addons/test_web/tests/test_read_progress_bar.py` (202 lines)
- `odoo/addons/test_web/tests/test_search_panel_select_multi_range.py` (741 lines)
- `odoo/addons/test_web/tests/test_search_panel_select_range.py` (1,067 lines)
- `odoo/addons/test_web/tests/test_translate.py` (68 lines)
- `odoo/addons/test_web/tests/test_views.py` (168 lines)
- `odoo/addons/test_web/tests/test_web_fill_temporal.py` (996 lines)
- `odoo/addons/test_web/tests/test_web_group_expand.py` (496 lines)
- `odoo/addons/test_web/tests/test_web_read.py` (889 lines)
- `odoo/addons/test_web/tests/test_web_read_group.py` (1,317 lines)
- `odoo/addons/test_web/tests/test_web_save.py` (98 lines)
- `odoo/addons/test_web/tests/test_x2many.py` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
