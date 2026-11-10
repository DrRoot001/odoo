# Module: test_website_slides_full

- **Module ID:** MOD-588
- **Path:** `addons/test_website_slides_full`
- **Manifest:** `addons/test_website_slides_full/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module will test the main certification flow of Odoo.
It will install the e-learning, survey and e-commerce apps and make a complete
certification flow including purchase, certification, failure and success.


Declared dependencies: `website_sale_slides`, `website_slides_forum`, `website_slides_survey`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale_slides",
    "website_slides_forum",
    "website_slides_survey"
  ],
  "data": [
    "data/res_groups_data.xml"
  ],
  "demo": [
    "data/product_demo.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "test_website_slides_full/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_website_slides_full/__init__.py` (2 lines)
- `addons/test_website_slides_full/__manifest__.py` (28 lines)
- `addons/test_website_slides_full/data/product_demo.xml` (29 lines)
- `addons/test_website_slides_full/data/res_groups_data.xml` (11 lines)
- `addons/test_website_slides_full/static/tests/tours/slides_certification_member.js` (162 lines)
- `addons/test_website_slides_full/tests/__init__.py` (4 lines)
- `addons/test_website_slides_full/tests/test_ui_wslides.py` (185 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
