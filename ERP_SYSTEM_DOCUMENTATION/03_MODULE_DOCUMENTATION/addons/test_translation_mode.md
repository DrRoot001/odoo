# Module: test_translation_mode

- **Module ID:** MOD-584
- **Path:** `addons/test_translation_mode`
- **Manifest:** `addons/test_translation_mode/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

In-context and interactive translation mode to streamline the module translation process using Weblate


The translation mode is available when several languages are installed. Select the language to translate,
enable the interactive translation mode from the command palette then browse the screens to translate.
By default, the translate feature redirects to the Odoo official translation project powered by Weblate.
In the settings, a custom Weblate project can be targeted.

WARNING:
This module adds invisible meta data to the translated strings, which might interfere with certain workflows.
Do not use it on production databases


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "data/config_parameter.xml",
    "views/translation_mode_settings.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "test_translation_mode/static/src/**/*"
    ],
    "web.assets_frontend": [
      "test_translation_mode/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "test_translation_mode/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/test_translation_mode/__init__.py` (10 lines)
- `addons/test_translation_mode/__manifest__.py` (35 lines)
- `addons/test_translation_mode/data/config_parameter.xml` (8 lines)
- `addons/test_translation_mode/models/__init__.py` (2 lines)
- `addons/test_translation_mode/models/ir_http.py` (31 lines)
- `addons/test_translation_mode/models/res_config_settings.py` (17 lines)
- `addons/test_translation_mode/static/src/@types/services.d.ts` (7 lines)
- `addons/test_translation_mode/static/src/siphash.js` (180 lines)
- `addons/test_translation_mode/static/src/translate_mode_debug_providers.js` (49 lines)
- `addons/test_translation_mode/static/src/translation.patch.js` (158 lines)
- `addons/test_translation_mode/static/src/translation_mode.css` (61 lines)
- `addons/test_translation_mode/static/src/translation_mode_service.js` (733 lines)
- `addons/test_translation_mode/static/src/translation_mode_side_panel.js` (234 lines)
- `addons/test_translation_mode/static/src/translation_mode_side_panel.xml` (138 lines)
- `addons/test_translation_mode/static/tests/translation.patch.test.js` (77 lines)
- `addons/test_translation_mode/static/tests/translation_mode_side_panel.test.js` (163 lines)
- `addons/test_translation_mode/tools/__init__.py` (1 lines)
- `addons/test_translation_mode/tools/translate.py` (84 lines)
- `addons/test_translation_mode/views/translation_mode_settings.xml` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
