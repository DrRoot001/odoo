# Module: product_matrix

- **Module ID:** MOD-474
- **Path:** `addons/product_matrix`
- **Manifest:** `addons/product_matrix/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Technical module: Matrix Implementation


Please refer to Sale Matrix or Purchase Matrix for the use of this module.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/res_groups.xml",
    "views/matrix_templates.xml"
  ],
  "demo": [
    "data/product_matrix_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "product_matrix/static/src/js/matrix_configurator_hook.js",
      "product_matrix/static/src/js/product_matrix_dialog.js",
      "product_matrix/static/src/scss/product_matrix.scss",
      "product_matrix/static/src/xml/**/*"
    ]
  }
}
```

### Representative source files

- `addons/product_matrix/__init__.py` (3 lines)
- `addons/product_matrix/__manifest__.py` (23 lines)
- `addons/product_matrix/data/product_matrix_demo.xml` (46 lines)
- `addons/product_matrix/data/res_groups.xml` (8 lines)
- `addons/product_matrix/i18n/ar.po` (128 lines)
- `addons/product_matrix/i18n/az.po` (120 lines)
- `addons/product_matrix/i18n/bg.po` (120 lines)
- `addons/product_matrix/i18n/bs.po` (122 lines)
- `addons/product_matrix/i18n/ca.po` (123 lines)
- `addons/product_matrix/i18n/cs.po` (126 lines)
- `addons/product_matrix/i18n/da.po` (125 lines)
- `addons/product_matrix/i18n/de.po` (133 lines)
- `addons/product_matrix/i18n/el.po` (121 lines)
- `addons/product_matrix/i18n/es.po` (131 lines)
- `addons/product_matrix/i18n/es_419.po` (124 lines)
- `addons/product_matrix/i18n/et.po` (125 lines)
- `addons/product_matrix/i18n/fa.po` (120 lines)
- `addons/product_matrix/i18n/fi.po` (125 lines)
- `addons/product_matrix/i18n/fr.po` (131 lines)
- `addons/product_matrix/i18n/he.po` (126 lines)
- `addons/product_matrix/i18n/hi.po` (120 lines)
- `addons/product_matrix/i18n/hr.po` (128 lines)
- `addons/product_matrix/i18n/hu.po` (126 lines)
- `addons/product_matrix/i18n/id.po` (125 lines)
- `addons/product_matrix/i18n/it.po` (133 lines)
- `addons/product_matrix/i18n/ja.po` (125 lines)
- `addons/product_matrix/i18n/kab.po` (121 lines)
- `addons/product_matrix/i18n/ko.po` (123 lines)
- `addons/product_matrix/i18n/ku.po` (120 lines)
- `addons/product_matrix/i18n/lo.po` (120 lines)
- `addons/product_matrix/i18n/lt.po` (128 lines)
- `addons/product_matrix/i18n/lv.po` (121 lines)
- `addons/product_matrix/i18n/mn.po` (126 lines)
- `addons/product_matrix/i18n/my.po` (120 lines)
- `addons/product_matrix/i18n/nb.po` (125 lines)
- `addons/product_matrix/i18n/nl.po` (129 lines)
- `addons/product_matrix/i18n/pl.po` (136 lines)
- `addons/product_matrix/i18n/product_matrix.pot` (117 lines)
- `addons/product_matrix/i18n/pt.po` (133 lines)
- `addons/product_matrix/i18n/pt_BR.po` (133 lines)
- `addons/product_matrix/i18n/ro.po` (127 lines)
- `addons/product_matrix/i18n/ru.po` (128 lines)
- `addons/product_matrix/i18n/sk.po` (120 lines)
- `addons/product_matrix/i18n/sl.po` (122 lines)
- `addons/product_matrix/i18n/sr@latin.po` (122 lines)
- `addons/product_matrix/i18n/sv.po` (126 lines)
- `addons/product_matrix/i18n/th.po` (122 lines)
- `addons/product_matrix/i18n/tr.po` (137 lines)
- `addons/product_matrix/i18n/uk.po` (126 lines)
- `addons/product_matrix/i18n/uz.po` (146 lines)
- `addons/product_matrix/i18n/vi.po` (128 lines)
- `addons/product_matrix/i18n/zh_CN.po` (128 lines)
- `addons/product_matrix/i18n/zh_TW.po` (124 lines)
- `addons/product_matrix/models/__init__.py` (1 lines)
- `addons/product_matrix/models/product_template.py` (90 lines)
- `addons/product_matrix/static/img/matrix_mycompany_tshirt.jpeg` (672 lines)
- `addons/product_matrix/static/src/js/matrix_configurator_hook.js` (59 lines)
- `addons/product_matrix/static/src/js/product_matrix_dialog.js` (103 lines)
- `addons/product_matrix/static/src/scss/product_matrix.scss` (35 lines)
- `addons/product_matrix/static/src/xml/product_matrix.xml` (69 lines)
- `addons/product_matrix/static/src/xml/product_matrix_dialog.xml` (16 lines)
- `addons/product_matrix/tests/__init__.py` (3 lines)
- `addons/product_matrix/tests/common.py` (48 lines)
- `addons/product_matrix/views/matrix_templates.xml` (51 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
