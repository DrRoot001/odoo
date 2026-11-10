# Module: api_doc

- **Module ID:** MOD-018
- **Path:** `addons/api_doc`
- **Manifest:** `addons/api_doc/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Odoo Dynamic API Documentation
==============================

This module provides a dynamic documentation page for developpers at the
/doc URL. The documentation is generated using the database to list the
models and their fields and methods. It also provides a playground to run
the methods over HTTP, with examples in various programming languages.


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 21 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "security/res_groups.xml",
    "views/docclient.xml"
  ],
  "assets": {
    "api_doc.assets": [
      [
        "include",
        "web.icons_fonts"
      ],
      [
        "include",
        "web._assets_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap"
      ],
      [
        "include",
        "web._assets_core"
      ],
      "web/static/src/core/code_editor/**",
      "api_doc/static/src/**/*.xml",
      "api_doc/static/src/**/*.js",
      "api_doc/static/src/doc_client.css",
      [
        "remove",
        "api_doc/static/src/api_action.js"
      ]
    ],
    "web.assets_unit_tests": [
      "api_doc/static/src/**/*.xml",
      "api_doc/static/src/**/*.js",
      "api_doc/static/src/doc_client.css",
      [
        "remove",
        "api_doc/static/src/api_action.js"
      ],
      [
        "remove",
        "api_doc/static/src/main.js"
      ],
      "api_doc/static/tests/**/*.test.js",
      "api_doc/static/tests/doc_test_helpers.js"
    ],
    "web.assets_backend": [
      "api_doc/static/src/api_action.js"
    ]
  }
}
```

### Representative source files

- `addons/api_doc/__init__.py` (2 lines)
- `addons/api_doc/__manifest__.py` (53 lines)
- `addons/api_doc/controllers/__init__.py` (1 lines)
- `addons/api_doc/controllers/api_doc.py` (676 lines)
- `addons/api_doc/i18n/api_doc.pot` (236 lines)
- `addons/api_doc/i18n/ar.po` (243 lines)
- `addons/api_doc/i18n/az.po` (240 lines)
- `addons/api_doc/i18n/bg.po` (240 lines)
- `addons/api_doc/i18n/bs.po` (242 lines)
- `addons/api_doc/i18n/ca.po` (241 lines)
- `addons/api_doc/i18n/cs.po` (240 lines)
- `addons/api_doc/i18n/da.po` (240 lines)
- `addons/api_doc/i18n/de.po` (240 lines)
- `addons/api_doc/i18n/el.po` (240 lines)
- `addons/api_doc/i18n/es.po` (241 lines)
- `addons/api_doc/i18n/es_419.po` (241 lines)
- `addons/api_doc/i18n/et.po` (240 lines)
- `addons/api_doc/i18n/fa.po` (240 lines)
- `addons/api_doc/i18n/fi.po` (241 lines)
- `addons/api_doc/i18n/fr.po` (242 lines)
- `addons/api_doc/i18n/he.po` (241 lines)
- `addons/api_doc/i18n/hi.po` (240 lines)
- `addons/api_doc/i18n/hr.po` (241 lines)
- `addons/api_doc/i18n/hu.po` (240 lines)
- `addons/api_doc/i18n/id.po` (240 lines)
- `addons/api_doc/i18n/it.po` (240 lines)
- `addons/api_doc/i18n/ja.po` (241 lines)
- `addons/api_doc/i18n/kab.po` (241 lines)
- `addons/api_doc/i18n/ko.po` (240 lines)
- `addons/api_doc/i18n/ku.po` (240 lines)
- `addons/api_doc/i18n/lt.po` (242 lines)
- `addons/api_doc/i18n/lv.po` (242 lines)
- `addons/api_doc/i18n/mn.po` (240 lines)
- `addons/api_doc/i18n/my.po` (241 lines)
- `addons/api_doc/i18n/nb.po` (240 lines)
- `addons/api_doc/i18n/nl.po` (242 lines)
- `addons/api_doc/i18n/pl.po` (242 lines)
- `addons/api_doc/i18n/pt.po` (240 lines)
- `addons/api_doc/i18n/pt_BR.po` (241 lines)
- `addons/api_doc/i18n/ro.po` (241 lines)
- `addons/api_doc/i18n/ru.po` (242 lines)
- `addons/api_doc/i18n/sk.po` (241 lines)
- `addons/api_doc/i18n/sl.po` (241 lines)
- `addons/api_doc/i18n/sr@latin.po` (241 lines)
- `addons/api_doc/i18n/sv.po` (241 lines)
- `addons/api_doc/i18n/th.po` (240 lines)
- `addons/api_doc/i18n/tr.po` (242 lines)
- `addons/api_doc/i18n/uk.po` (241 lines)
- `addons/api_doc/i18n/vi.po` (241 lines)
- `addons/api_doc/i18n/zh_CN.po` (241 lines)
- `addons/api_doc/i18n/zh_TW.po` (240 lines)
- `addons/api_doc/models/__init__.py` (1 lines)
- `addons/api_doc/models/ir_attachment.py` (23 lines)
- `addons/api_doc/security/res_groups.xml` (10 lines)
- `addons/api_doc/static/src/api_action.js` (12 lines)
- `addons/api_doc/static/src/components/doc_copyable_pre.js` (32 lines)
- `addons/api_doc/static/src/components/doc_error_dialog.js` (53 lines)
- `addons/api_doc/static/src/components/doc_loading_indicator.js` (18 lines)
- `addons/api_doc/static/src/components/doc_method.js` (83 lines)
- `addons/api_doc/static/src/components/doc_method.xml` (58 lines)
- `addons/api_doc/static/src/components/doc_modal_api_key.js` (36 lines)
- `addons/api_doc/static/src/components/doc_modal_api_key.xml` (27 lines)
- `addons/api_doc/static/src/components/doc_modal_search.js` (91 lines)
- `addons/api_doc/static/src/components/doc_modal_search.xml` (57 lines)
- `addons/api_doc/static/src/components/doc_model.js` (302 lines)
- `addons/api_doc/static/src/components/doc_model.xml` (92 lines)
- `addons/api_doc/static/src/components/doc_request.js` (90 lines)
- `addons/api_doc/static/src/components/doc_request.xml` (100 lines)
- `addons/api_doc/static/src/components/doc_sidebar.js` (98 lines)
- `addons/api_doc/static/src/components/doc_sidebar.xml` (42 lines)
- `addons/api_doc/static/src/components/doc_table.js` (175 lines)
- `addons/api_doc/static/src/components/doc_table.xml` (104 lines)
- `addons/api_doc/static/src/doc_client.css` (665 lines)
- `addons/api_doc/static/src/doc_client.js` (126 lines)
- `addons/api_doc/static/src/doc_client.xml` (68 lines)
- `addons/api_doc/static/src/doc_model_store.js` (208 lines)
- `addons/api_doc/static/src/main.js` (3 lines)
- `addons/api_doc/static/src/start_doc_client.js` (13 lines)
- `addons/api_doc/static/src/utils/doc_code_gen.js` (95 lines)
- `addons/api_doc/static/src/utils/doc_model_search.js` (84 lines)
- `addons/api_doc/static/src/utils/doc_model_utils.js` (148 lines)
- `addons/api_doc/static/src/utils/doc_ui_store.js` (31 lines)
- `addons/api_doc/static/tests/api_doc.test.js` (456 lines)
- `addons/api_doc/static/tests/doc_test_helpers.js` (91 lines)
- `addons/api_doc/tests/__init__.py` (2 lines)
- `addons/api_doc/tests/dummy_methods.py` (196 lines)
- `addons/api_doc/tests/test_api_doc_tour.py` (25 lines)
- `addons/api_doc/tests/test_doc.py` (312 lines)
- `addons/api_doc/views/docclient.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
