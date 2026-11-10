# Module: test_assetsbundle

- **Module ID:** MOD-649
- **Path:** `odoo/addons/test_assetsbundle`
- **Manifest:** `odoo/addons/test_assetsbundle/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to verify the Assets Bundle mechanism.

Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "data/ir_asset.xml",
    "views/views.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "test_assetsbundle/static/tests/test_css_error.js"
    ],
    "test_assetsbundle.bundle2": [
      "test_assetsbundle/static/src/css/test_cssfile1.css"
    ],
    "test_assetsbundle.bundle3": [
      "test_assetsbundle/static/src/scss/test_file1.scss"
    ],
    "test_assetsbundle.bundle4": [
      "test_assetsbundle/static/src/js/test_jsfile1.js",
      "test_assetsbundle/static/src/js/test_jsfile2.js",
      "http://test.external.link/javascript1.js",
      "test_assetsbundle/static/src/css/test_cssfile1.css",
      "http://test.external.link/style1.css",
      "test_assetsbundle/static/src/css/test_cssfile2.css",
      "test_assetsbundle/static/src/js/test_jsfile3.js",
      "http://test.external.link/javascript2.js",
      "http://test.external.link/style2.css"
    ],
    "test_assetsbundle.manifest1": [
      "test_assetsbundle/static/src/*/**"
    ],
    "test_assetsbundle.manifest2": [
      "test_assetsbundle/static/src/js/test_jsfile1.js",
      "test_assetsbundle/static/src/*/**"
    ],
    "test_assetsbundle.manifest3": [
      "test_assetsbundle/static/src/js/test_jsfile3.js",
      "test_assetsbundle/static/src/*/**"
    ],
    "test_assetsbundle.manifest4": [
      "test_assetsbundle/static/src/js/test_jsfile3.js"
    ],
    "test_assetsbundle.manifest5": [
      "test_assetsbundle/static/src/js/test_jsfile1.js",
      "test_assetsbundle/static/src/js/test_jsfile2.js",
      "test_assetsbundle/static/src/js/test_jsfile3.js",
      "test_assetsbundle/static/src/js/test_jsfile4.js"
    ],
    "test_assetsbundle.manifest6": [
      [
        "include",
        "test_assetsbundle.manifest4"
      ]
    ],
    "test_assetsbundle.manifest_multi_module1": [],
    "test_assetsbundle.broken_css": [
      "test_assetsbundle/static/invalid_src/css/invalid_css.css"
    ],
    "test_assetsbundle.lazy_test_component": [
      "test_assetsbundle/static/tests/lazy_test_component/**/*"
    ],
    "test_assetsbundle.broken_xml": [
      "test_assetsbundle/static/invalid_src/xml/invalid_xml.xml"
    ],
    "test_assetsbundle.multiple_broken_xml": [
      "test_assetsbundle/static/invalid_src/xml/invalid_xml.xml",
      "test_assetsbundle/static/invalid_src/xml/second_invalid_xml.xml"
    ],
    "test_assetsbundle.multiple_same_name": [
      "test_assetsbundle/static/invalid_src/xml/multiple_same_name.xml"
    ],
    "test_assetsbundle.wo_name": [
      "test_assetsbundle/static/invalid_src/xml/template_wo_name.xml"
    ],
    "test_assetsbundle.file_not_found": [
      "test_assetsbundle/static/invalid_src/xml/file_not_found.xml"
    ],
    "web.assets_unit_tests": [
      "test_assetsbundle/static/tests/lazy_component.test.js"
    ]
  }
}
```

### Representative source files

- `odoo/addons/test_assetsbundle/__init__.py` (2 lines)
- `odoo/addons/test_assetsbundle/__manifest__.py` (88 lines)
- `odoo/addons/test_assetsbundle/controllers/__init__.py` (4 lines)
- `odoo/addons/test_assetsbundle/controllers/main.py` (11 lines)
- `odoo/addons/test_assetsbundle/data/ir_asset.xml` (9 lines)
- `odoo/addons/test_assetsbundle/models/__init__.py` (1 lines)
- `odoo/addons/test_assetsbundle/models/ir_qweb.py` (16 lines)
- `odoo/addons/test_assetsbundle/static/accessible.xml` (1 lines)
- `odoo/addons/test_assetsbundle/static/invalid_src/css/invalid_css.css` (8 lines)
- `odoo/addons/test_assetsbundle/static/invalid_src/xml/invalid_xml.xml` (6 lines)
- `odoo/addons/test_assetsbundle/static/invalid_src/xml/multiple_same_name.xml` (9 lines)
- `odoo/addons/test_assetsbundle/static/invalid_src/xml/second_invalid_xml.xml` (7 lines)
- `odoo/addons/test_assetsbundle/static/invalid_src/xml/template_wo_name.xml` (6 lines)
- `odoo/addons/test_assetsbundle/static/src/css/test_cssfile1.css` (11 lines)
- `odoo/addons/test_assetsbundle/static/src/css/test_cssfile2.css` (3 lines)
- `odoo/addons/test_assetsbundle/static/src/css/test_cssfile3.css` (3 lines)
- `odoo/addons/test_assetsbundle/static/src/css/test_error.scss` (3 lines)
- `odoo/addons/test_assetsbundle/static/src/js/test_jsfile1.js` (2 lines)
- `odoo/addons/test_assetsbundle/static/src/js/test_jsfile2.js` (2 lines)
- `odoo/addons/test_assetsbundle/static/src/js/test_jsfile3.js` (2 lines)
- `odoo/addons/test_assetsbundle/static/src/js/test_jsfile4.js` (2 lines)
- `odoo/addons/test_assetsbundle/static/src/scss/test_file1.scss` (3 lines)
- `odoo/addons/test_assetsbundle/static/src/scss/test_prefix.scss` (90 lines)
- `odoo/addons/test_assetsbundle/static/tests/lazy_component.test.js` (25 lines)
- `odoo/addons/test_assetsbundle/static/tests/lazy_test_component/lazy_test_component.js` (16 lines)
- `odoo/addons/test_assetsbundle/static/tests/lazy_test_component/lazy_test_component.scss` (3 lines)
- `odoo/addons/test_assetsbundle/static/tests/lazy_test_component/lazy_test_component.xml` (8 lines)
- `odoo/addons/test_assetsbundle/static/tests/test_css_error.js` (25 lines)
- `odoo/addons/test_assetsbundle/tests/__init__.py` (6 lines)
- `odoo/addons/test_assetsbundle/tests/test_assetsbundle.py` (2,093 lines)
- `odoo/addons/test_assetsbundle/tests/test_js_transpiler.py` (499 lines)
- `odoo/addons/test_assetsbundle/tests/test_js_transpiler_regex.py` (83 lines)
- `odoo/addons/test_assetsbundle/views/views.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
