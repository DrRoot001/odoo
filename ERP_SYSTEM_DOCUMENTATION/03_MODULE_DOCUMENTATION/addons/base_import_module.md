# Module: base_import_module

- **Module ID:** MOD-038
- **Path:** `addons/base_import_module`
- **Manifest:** `addons/base_import_module/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Import a custom data module
===========================

This module allows authorized users to import a custom data module (.xml files and static assests)
for customization purpose.


Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "views/base_import_module_view.xml",
    "views/ir_module_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "base_import_module/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "base_import_module/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/base_import_module/__init__.py` (3 lines)
- `addons/base_import_module/__manifest__.py` (29 lines)
- `addons/base_import_module/controllers/__init__.py` (2 lines)
- `addons/base_import_module/controllers/main.py` (25 lines)
- `addons/base_import_module/i18n/af.po` (362 lines)
- `addons/base_import_module/i18n/am.po` (358 lines)
- `addons/base_import_module/i18n/ar.po` (385 lines)
- `addons/base_import_module/i18n/az.po` (361 lines)
- `addons/base_import_module/i18n/base_import_module.pot` (349 lines)
- `addons/base_import_module/i18n/bg.po` (370 lines)
- `addons/base_import_module/i18n/bs.po` (371 lines)
- `addons/base_import_module/i18n/ca.po` (374 lines)
- `addons/base_import_module/i18n/cs.po` (382 lines)
- `addons/base_import_module/i18n/da.po` (390 lines)
- `addons/base_import_module/i18n/de.po` (402 lines)
- `addons/base_import_module/i18n/el.po` (361 lines)
- `addons/base_import_module/i18n/es.po` (403 lines)
- `addons/base_import_module/i18n/es_419.po` (398 lines)
- `addons/base_import_module/i18n/es_CL.po` (63 lines)
- `addons/base_import_module/i18n/et.po` (369 lines)
- `addons/base_import_module/i18n/eu.po` (361 lines)
- `addons/base_import_module/i18n/fa.po` (378 lines)
- `addons/base_import_module/i18n/fi.po` (401 lines)
- `addons/base_import_module/i18n/fo.po` (361 lines)
- `addons/base_import_module/i18n/fr.po` (405 lines)
- `addons/base_import_module/i18n/fr_BE.po` (53 lines)
- `addons/base_import_module/i18n/fr_CA.po` (63 lines)
- `addons/base_import_module/i18n/gl.po` (361 lines)
- `addons/base_import_module/i18n/gu.po` (362 lines)
- `addons/base_import_module/i18n/he.po` (371 lines)
- `addons/base_import_module/i18n/hi.po` (365 lines)
- `addons/base_import_module/i18n/hr.po` (407 lines)
- `addons/base_import_module/i18n/hu.po` (371 lines)
- `addons/base_import_module/i18n/id.po` (386 lines)
- `addons/base_import_module/i18n/is.po` (358 lines)
- `addons/base_import_module/i18n/it.po` (401 lines)
- `addons/base_import_module/i18n/ja.po` (396 lines)
- `addons/base_import_module/i18n/ka.po` (361 lines)
- `addons/base_import_module/i18n/kab.po` (359 lines)
- `addons/base_import_module/i18n/kk.po` (360 lines)
- `addons/base_import_module/i18n/km.po` (361 lines)
- `addons/base_import_module/i18n/ko.po` (376 lines)
- `addons/base_import_module/i18n/ku.po` (355 lines)
- `addons/base_import_module/i18n/lo.po` (388 lines)
- `addons/base_import_module/i18n/lt.po` (385 lines)
- `addons/base_import_module/i18n/lv.po` (375 lines)
- `addons/base_import_module/i18n/mk.po` (361 lines)
- `addons/base_import_module/i18n/ml_IN.po` (361 lines)
- `addons/base_import_module/i18n/mn.po` (361 lines)
- `addons/base_import_module/i18n/my.po` (357 lines)
- `addons/base_import_module/i18n/nb.po` (366 lines)
- `addons/base_import_module/i18n/nl.po` (392 lines)
- `addons/base_import_module/i18n/pl.po` (399 lines)
- `addons/base_import_module/i18n/pt.po` (407 lines)
- `addons/base_import_module/i18n/pt_BR.po` (401 lines)
- `addons/base_import_module/i18n/ro.po` (383 lines)
- `addons/base_import_module/i18n/ru.po` (387 lines)
- `addons/base_import_module/i18n/sk.po` (372 lines)
- `addons/base_import_module/i18n/sl.po` (385 lines)
- `addons/base_import_module/i18n/sq.po` (361 lines)
- `addons/base_import_module/i18n/sr@latin.po` (374 lines)
- `addons/base_import_module/i18n/sv.po` (395 lines)
- `addons/base_import_module/i18n/ta.po` (362 lines)
- `addons/base_import_module/i18n/th.po` (374 lines)
- `addons/base_import_module/i18n/tr.po` (396 lines)
- `addons/base_import_module/i18n/uk.po` (383 lines)
- `addons/base_import_module/i18n/uz.po` (438 lines)
- `addons/base_import_module/i18n/vi.po` (384 lines)
- `addons/base_import_module/i18n/zh_CN.po` (375 lines)
- `addons/base_import_module/i18n/zh_TW.po` (373 lines)
- `addons/base_import_module/models/__init__.py` (6 lines)
- `addons/base_import_module/models/base_import_module.py` (40 lines)
- `addons/base_import_module/models/ir_http.py` (22 lines)
- `addons/base_import_module/models/ir_module.py` (755 lines)
- `addons/base_import_module/models/ir_ui_view.py` (29 lines)
- `addons/base_import_module/security/ir.access.csv` (2 lines)
- `addons/base_import_module/static/src/base_import_list_renderer.js` (28 lines)
- `addons/base_import_module/static/src/base_import_list_view.js` (11 lines)
- `addons/base_import_module/static/src/search_panel.scss` (3 lines)
- `addons/base_import_module/static/tests/apps_searchpanel.test.js` (112 lines)
- `addons/base_import_module/tests/__init__.py` (5 lines)
- `addons/base_import_module/tests/test_cloc.py` (439 lines)
- `addons/base_import_module/tests/test_import_module.py` (535 lines)
- `addons/base_import_module/views/base_import_module_view.xml` (47 lines)
- `addons/base_import_module/views/ir_module_views.xml` (88 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
