# Module: test_website

- **Module ID:** MOD-586
- **Path:** `addons/test_website`
- **Manifest:** `addons/test_website/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Website Test, mainly for module install/uninstall tests

This module contains tests related to website. Those are
present in a separate module as we are testing module install/uninstall/upgrade
and we don't want to reload the website module every time, including it's possible
dependencies. Neither we want to add in website module some routes, views and
models which only purpose is to run tests.

Declared dependencies: `web_unsplash`, `website`, `theme_default`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 35 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 19 | Client behavior/assets. |
| Tests | 28 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 37 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web_unsplash",
    "website",
    "theme_default"
  ],
  "data": [
    "security/test_website_security.xml",
    "views/templates.xml",
    "views/test_model_multi_website_views.xml",
    "views/test_model_views.xml",
    "data/test_website_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/test_website_demo.xml"
  ],
  "assets": {
    "test_website.test_bundle": [
      "http://test.external.link/javascript1.js",
      [
        "include",
        "web.icons_fonts"
      ],
      "http://test.external.link/style1.css",
      "/web/static/src/module_loader.js",
      "http://test.external.link/javascript2.js",
      "http://test.external.link/style2.css"
    ],
    "web.assets_frontend": [
      "test_website/static/src/interactions/**/*"
    ],
    "website.website_builder_assets": [
      "test_website/static/src/website_builder/**/*"
    ],
    "web.assets_tests": [
      "test_website/static/tests/tours/*"
    ],
    "web.assets_unit_tests": [
      "test_website/static/tests/builder/*"
    ]
  }
}
```

### Representative source files

- `addons/test_website/__init__.py` (5 lines)
- `addons/test_website/__manifest__.py` (53 lines)
- `addons/test_website/controllers/__init__.py` (4 lines)
- `addons/test_website/controllers/main.py` (190 lines)
- `addons/test_website/data/test_website_data.xml` (168 lines)
- `addons/test_website/data/test_website_demo.xml` (9 lines)
- `addons/test_website/models/__init__.py` (2 lines)
- `addons/test_website/models/model.py` (111 lines)
- `addons/test_website/models/website.py` (18 lines)
- `addons/test_website/security/ir.access.csv` (13 lines)
- `addons/test_website/security/test_website_security.xml` (18 lines)
- `addons/test_website/static/src/interactions/test_error.js` (13 lines)
- `addons/test_website/static/src/website_builder/builder.scss` (5 lines)
- `addons/test_website/static/tests/builder/drag_and_drop.test.js` (24 lines)
- `addons/test_website/static/tests/tours/custom_snippets.js` (109 lines)
- `addons/test_website/static/tests/tours/error_views.js` (235 lines)
- `addons/test_website/static/tests/tours/form.js` (58 lines)
- `addons/test_website/static/tests/tours/image_link.js` (107 lines)
- `addons/test_website/static/tests/tours/image_upload_progress.js` (276 lines)
- `addons/test_website/static/tests/tours/json_auth.js` (24 lines)
- `addons/test_website/static/tests/tours/page_manager.js` (101 lines)
- `addons/test_website/static/tests/tours/replace_media.js` (181 lines)
- `addons/test_website/static/tests/tours/reset_views.js` (113 lines)
- `addons/test_website/static/tests/tours/restricted_editor.js` (170 lines)
- `addons/test_website/static/tests/tours/snippet_background_video.js` (69 lines)
- `addons/test_website/static/tests/tours/systray.js` (274 lines)
- `addons/test_website/static/tests/tours/translation.js` (471 lines)
- `addons/test_website/static/tests/tours/website_controller_page.js` (85 lines)
- `addons/test_website/static/tests/tours/website_field_sanitize.js` (58 lines)
- `addons/test_website/static/tests/tours/website_page_properties.js` (348 lines)
- `addons/test_website/static/tests/tours/website_settings.js` (38 lines)
- `addons/test_website/tests/__init__.py` (30 lines)
- `addons/test_website/tests/asset_tag.xml` (35 lines)
- `addons/test_website/tests/template_qweb_test.xml` (32 lines)
- `addons/test_website/tests/test_controller_args.py` (53 lines)
- `addons/test_website/tests/test_custom_snippet.py` (13 lines)
- `addons/test_website/tests/test_error.py` (10 lines)
- `addons/test_website/tests/test_form.py` (15 lines)
- `addons/test_website/tests/test_fuzzy.py` (200 lines)
- `addons/test_website/tests/test_image_upload_progress.py` (63 lines)
- `addons/test_website/tests/test_is_multilang.py` (103 lines)
- `addons/test_website/tests/test_media.py` (22 lines)
- `addons/test_website/tests/test_menu.py` (43 lines)
- `addons/test_website/tests/test_multi_company.py` (16 lines)
- `addons/test_website/tests/test_page.py` (59 lines)
- `addons/test_website/tests/test_page_manager.py` (29 lines)
- `addons/test_website/tests/test_performance.py` (13 lines)
- `addons/test_website/tests/test_qweb.py` (91 lines)
- `addons/test_website/tests/test_redirect.py` (454 lines)
- `addons/test_website/tests/test_reset_views.py` (116 lines)
- `addons/test_website/tests/test_restricted_editor.py` (53 lines)
- `addons/test_website/tests/test_session.py` (89 lines)
- `addons/test_website/tests/test_settings.py` (13 lines)
- `addons/test_website/tests/test_snippet_background_video.py` (10 lines)
- `addons/test_website/tests/test_systray.py` (84 lines)
- `addons/test_website/tests/test_theme_ir_asset.py` (77 lines)
- `addons/test_website/tests/test_translation.py` (141 lines)
- `addons/test_website/tests/test_views_during_module_operation.py` (223 lines)
- `addons/test_website/tests/test_website_controller_page.py` (191 lines)
- `addons/test_website/tests/test_website_field_sanitize.py` (32 lines)
- `addons/test_website/tests/test_website_page_properties.py` (28 lines)
- `addons/test_website/views/templates.xml` (103 lines)
- `addons/test_website/views/test_model_multi_website_views.xml` (73 lines)
- `addons/test_website/views/test_model_views.xml` (80 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
