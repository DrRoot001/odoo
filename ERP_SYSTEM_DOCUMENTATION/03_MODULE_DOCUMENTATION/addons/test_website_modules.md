# Module: test_website_modules

- **Module ID:** MOD-587
- **Path:** `addons/test_website_modules`
- **Manifest:** `addons/test_website_modules/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

This module contains tests related to website modules.
It allows to test website business code when another website module is
installed.

Declared dependencies: `theme_default`, `website`, `website_blog`, `website_event_sale`, `website_slides`, `website_livechat`, `website_crm_iap_reveal`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "theme_default",
    "website",
    "website_blog",
    "website_event_sale",
    "website_slides",
    "website_livechat",
    "website_crm_iap_reveal",
    "website_sale"
  ],
  "assets": {
    "web.assets_tests": [
      "test_website_modules/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_website_modules/__init__.py` (2 lines)
- `addons/test_website_modules/__manifest__.py` (27 lines)
- `addons/test_website_modules/static/tests/tours/configurator_flow.js` (110 lines)
- `addons/test_website_modules/tests/__init__.py` (7 lines)
- `addons/test_website_modules/tests/test_configurator.py` (12 lines)
- `addons/test_website_modules/tests/test_controllers.py` (152 lines)
- `addons/test_website_modules/tests/test_models.py` (21 lines)
- `addons/test_website_modules/tests/test_performance.py` (391 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
