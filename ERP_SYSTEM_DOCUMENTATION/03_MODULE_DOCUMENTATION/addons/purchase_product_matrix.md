# Module: purchase_product_matrix

- **Module ID:** MOD-499
- **Path:** `addons/purchase_product_matrix`
- **Manifest:** `addons/purchase_product_matrix/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Add variants to your purchase orders through an Order Grid Entry.


This module allows to fill Purchase Orders rapidly
by choosing product variants quantity through a Grid Entry.
    

Declared dependencies: `purchase`, `product_matrix`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase",
    "product_matrix"
  ],
  "data": [
    "views/purchase_views.xml",
    "report/purchase_quotation_templates.xml",
    "report/purchase_order_templates.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "purchase_product_matrix/static/src/**/*"
    ],
    "web.assets_tests": [
      "purchase_product_matrix/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/purchase_product_matrix/__init__.py` (3 lines)
- `addons/purchase_product_matrix/__manifest__.py` (26 lines)
- `addons/purchase_product_matrix/i18n/ar.po` (147 lines)
- `addons/purchase_product_matrix/i18n/az.po` (137 lines)
- `addons/purchase_product_matrix/i18n/bg.po` (140 lines)
- `addons/purchase_product_matrix/i18n/bs.po` (149 lines)
- `addons/purchase_product_matrix/i18n/ca.po` (146 lines)
- `addons/purchase_product_matrix/i18n/cs.po` (148 lines)
- `addons/purchase_product_matrix/i18n/da.po` (149 lines)
- `addons/purchase_product_matrix/i18n/de.po` (157 lines)
- `addons/purchase_product_matrix/i18n/el.po` (138 lines)
- `addons/purchase_product_matrix/i18n/es.po` (154 lines)
- `addons/purchase_product_matrix/i18n/es_419.po` (146 lines)
- `addons/purchase_product_matrix/i18n/et.po` (146 lines)
- `addons/purchase_product_matrix/i18n/fa.po` (137 lines)
- `addons/purchase_product_matrix/i18n/fi.po` (144 lines)
- `addons/purchase_product_matrix/i18n/fr.po` (150 lines)
- `addons/purchase_product_matrix/i18n/he.po` (152 lines)
- `addons/purchase_product_matrix/i18n/hi.po` (138 lines)
- `addons/purchase_product_matrix/i18n/hr.po` (145 lines)
- `addons/purchase_product_matrix/i18n/hu.po` (148 lines)
- `addons/purchase_product_matrix/i18n/id.po` (146 lines)
- `addons/purchase_product_matrix/i18n/it.po` (154 lines)
- `addons/purchase_product_matrix/i18n/ja.po` (144 lines)
- `addons/purchase_product_matrix/i18n/kab.po` (146 lines)
- `addons/purchase_product_matrix/i18n/ko.po` (145 lines)
- `addons/purchase_product_matrix/i18n/ku.po` (140 lines)
- `addons/purchase_product_matrix/i18n/lo.po` (156 lines)
- `addons/purchase_product_matrix/i18n/lt.po` (148 lines)
- `addons/purchase_product_matrix/i18n/lv.po` (147 lines)
- `addons/purchase_product_matrix/i18n/mn.po` (145 lines)
- `addons/purchase_product_matrix/i18n/my.po` (138 lines)
- `addons/purchase_product_matrix/i18n/nb.po` (141 lines)
- `addons/purchase_product_matrix/i18n/nl.po` (150 lines)
- `addons/purchase_product_matrix/i18n/pl.po` (151 lines)
- `addons/purchase_product_matrix/i18n/pt.po` (153 lines)
- `addons/purchase_product_matrix/i18n/pt_BR.po` (161 lines)
- `addons/purchase_product_matrix/i18n/purchase_product_matrix.pot` (133 lines)
- `addons/purchase_product_matrix/i18n/ro.po` (150 lines)
- `addons/purchase_product_matrix/i18n/ru.po` (149 lines)
- `addons/purchase_product_matrix/i18n/sk.po` (158 lines)
- `addons/purchase_product_matrix/i18n/sl.po` (142 lines)
- `addons/purchase_product_matrix/i18n/sr@latin.po` (138 lines)
- `addons/purchase_product_matrix/i18n/sv.po` (146 lines)
- `addons/purchase_product_matrix/i18n/th.po` (144 lines)
- `addons/purchase_product_matrix/i18n/tr.po` (151 lines)
- `addons/purchase_product_matrix/i18n/uk.po` (151 lines)
- `addons/purchase_product_matrix/i18n/uz.po` (169 lines)
- `addons/purchase_product_matrix/i18n/vi.po` (149 lines)
- `addons/purchase_product_matrix/i18n/zh_CN.po` (149 lines)
- `addons/purchase_product_matrix/i18n/zh_TW.po` (146 lines)
- `addons/purchase_product_matrix/models/__init__.py` (3 lines)
- `addons/purchase_product_matrix/models/purchase.py` (162 lines)
- `addons/purchase_product_matrix/report/purchase_order_templates.xml` (8 lines)
- `addons/purchase_product_matrix/report/purchase_quotation_templates.xml` (8 lines)
- `addons/purchase_product_matrix/static/src/js/purchase_product_field.js` (67 lines)
- `addons/purchase_product_matrix/static/src/js/purchase_product_field.xml` (20 lines)
- `addons/purchase_product_matrix/static/tests/tours/purchase_product_matrix_tour.js` (111 lines)
- `addons/purchase_product_matrix/tests/__init__.py` (4 lines)
- `addons/purchase_product_matrix/tests/test_purchase_matrix.py` (69 lines)
- `addons/purchase_product_matrix/views/purchase_views.xml` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
