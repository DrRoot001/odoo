# Module: sale_product_matrix

- **Module ID:** MOD-523
- **Path:** `addons/sale_product_matrix`
- **Manifest:** `addons/sale_product_matrix/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Add variants to Sales Order through a grid entry.


This module allows to fill Sales Order rapidly
by choosing product variants quantity through a Grid Entry.
    

Declared dependencies: `sale`, `product_matrix`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "product_matrix"
  ],
  "data": [
    "views/product_template_views.xml",
    "views/sale_order_views.xml",
    "report/sale_report_templates.xml"
  ],
  "demo": [
    "data/product_matrix_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_product_matrix/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_product_matrix/__init__.py` (3 lines)
- `addons/sale_product_matrix/__manifest__.py` (21 lines)
- `addons/sale_product_matrix/data/product_matrix_demo.xml` (6 lines)
- `addons/sale_product_matrix/i18n/ar.po` (136 lines)
- `addons/sale_product_matrix/i18n/az.po` (128 lines)
- `addons/sale_product_matrix/i18n/bg.po` (128 lines)
- `addons/sale_product_matrix/i18n/bs.po` (130 lines)
- `addons/sale_product_matrix/i18n/ca.po` (134 lines)
- `addons/sale_product_matrix/i18n/cs.po` (135 lines)
- `addons/sale_product_matrix/i18n/da.po` (137 lines)
- `addons/sale_product_matrix/i18n/de.po` (146 lines)
- `addons/sale_product_matrix/i18n/el.po` (129 lines)
- `addons/sale_product_matrix/i18n/es.po` (142 lines)
- `addons/sale_product_matrix/i18n/es_419.po` (135 lines)
- `addons/sale_product_matrix/i18n/et.po` (132 lines)
- `addons/sale_product_matrix/i18n/fa.po` (128 lines)
- `addons/sale_product_matrix/i18n/fi.po` (139 lines)
- `addons/sale_product_matrix/i18n/fr.po` (139 lines)
- `addons/sale_product_matrix/i18n/he.po` (134 lines)
- `addons/sale_product_matrix/i18n/hi.po` (128 lines)
- `addons/sale_product_matrix/i18n/hr.po` (134 lines)
- `addons/sale_product_matrix/i18n/hu.po` (139 lines)
- `addons/sale_product_matrix/i18n/id.po` (135 lines)
- `addons/sale_product_matrix/i18n/it.po` (143 lines)
- `addons/sale_product_matrix/i18n/ja.po` (133 lines)
- `addons/sale_product_matrix/i18n/kab.po` (129 lines)
- `addons/sale_product_matrix/i18n/ko.po` (133 lines)
- `addons/sale_product_matrix/i18n/ku.po` (128 lines)
- `addons/sale_product_matrix/i18n/lo.po` (128 lines)
- `addons/sale_product_matrix/i18n/lt.po` (136 lines)
- `addons/sale_product_matrix/i18n/lv.po` (129 lines)
- `addons/sale_product_matrix/i18n/mn.po` (134 lines)
- `addons/sale_product_matrix/i18n/my.po` (128 lines)
- `addons/sale_product_matrix/i18n/nb.po` (134 lines)
- `addons/sale_product_matrix/i18n/nl.po` (139 lines)
- `addons/sale_product_matrix/i18n/pl.po` (141 lines)
- `addons/sale_product_matrix/i18n/pt.po` (139 lines)
- `addons/sale_product_matrix/i18n/pt_BR.po` (148 lines)
- `addons/sale_product_matrix/i18n/ro.po` (139 lines)
- `addons/sale_product_matrix/i18n/ru.po` (137 lines)
- `addons/sale_product_matrix/i18n/sale_product_matrix.pot` (124 lines)
- `addons/sale_product_matrix/i18n/sk.po` (128 lines)
- `addons/sale_product_matrix/i18n/sl.po` (130 lines)
- `addons/sale_product_matrix/i18n/sr@latin.po` (129 lines)
- `addons/sale_product_matrix/i18n/sv.po` (135 lines)
- `addons/sale_product_matrix/i18n/th.po` (133 lines)
- `addons/sale_product_matrix/i18n/tr.po` (139 lines)
- `addons/sale_product_matrix/i18n/uk.po` (136 lines)
- `addons/sale_product_matrix/i18n/uz.po` (151 lines)
- `addons/sale_product_matrix/i18n/vi.po` (138 lines)
- `addons/sale_product_matrix/i18n/zh_CN.po` (140 lines)
- `addons/sale_product_matrix/i18n/zh_TW.po` (135 lines)
- `addons/sale_product_matrix/models/__init__.py` (3 lines)
- `addons/sale_product_matrix/models/product_template.py` (23 lines)
- `addons/sale_product_matrix/models/sale_order.py` (191 lines)
- `addons/sale_product_matrix/models/sale_order_line.py` (11 lines)
- `addons/sale_product_matrix/report/sale_report_templates.xml` (8 lines)
- `addons/sale_product_matrix/static/src/js/sale_product_mixin.js` (46 lines)
- `addons/sale_product_matrix/views/product_template_views.xml` (28 lines)
- `addons/sale_product_matrix/views/sale_order_views.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
