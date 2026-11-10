# Module: sale_margin

- **Module ID:** MOD-519
- **Path:** `addons/sale_margin`
- **Manifest:** `addons/sale_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module adds the 'Margin' on sales order.
=============================================

This gives the profitability by calculating the difference between the Unit
Price and Cost Price.
    

Declared dependencies: `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_management"
  ],
  "data": [
    "views/sale_order_views.xml",
    "views/sale_order_template_views.xml",
    "report/sale_report_views.xml"
  ],
  "demo": [
    "data/sale_margin_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_margin/static/src/js/labeled_field_short_labels.js"
    ]
  }
}
```

### Representative source files

- `addons/sale_margin/__init__.py` (3 lines)
- `addons/sale_margin/__manifest__.py` (28 lines)
- `addons/sale_margin/data/sale_margin_demo.xml` (36 lines)
- `addons/sale_margin/i18n/af.po` (200 lines)
- `addons/sale_margin/i18n/am.po` (200 lines)
- `addons/sale_margin/i18n/ar.po` (222 lines)
- `addons/sale_margin/i18n/az.po` (220 lines)
- `addons/sale_margin/i18n/bg.po` (222 lines)
- `addons/sale_margin/i18n/bs.po` (220 lines)
- `addons/sale_margin/i18n/ca.po` (221 lines)
- `addons/sale_margin/i18n/cs.po` (223 lines)
- `addons/sale_margin/i18n/da.po` (222 lines)
- `addons/sale_margin/i18n/de.po` (233 lines)
- `addons/sale_margin/i18n/el.po` (221 lines)
- `addons/sale_margin/i18n/es.po` (229 lines)
- `addons/sale_margin/i18n/es_419.po` (236 lines)
- `addons/sale_margin/i18n/es_CL.po` (36 lines)
- `addons/sale_margin/i18n/et.po` (224 lines)
- `addons/sale_margin/i18n/eu.po` (202 lines)
- `addons/sale_margin/i18n/fa.po` (223 lines)
- `addons/sale_margin/i18n/fi.po` (231 lines)
- `addons/sale_margin/i18n/fo.po` (202 lines)
- `addons/sale_margin/i18n/fr.po` (226 lines)
- `addons/sale_margin/i18n/fr_BE.po` (24 lines)
- `addons/sale_margin/i18n/fr_CA.po` (24 lines)
- `addons/sale_margin/i18n/gl.po` (202 lines)
- `addons/sale_margin/i18n/gu.po` (203 lines)
- `addons/sale_margin/i18n/he.po` (223 lines)
- `addons/sale_margin/i18n/hi.po` (217 lines)
- `addons/sale_margin/i18n/hr.po` (222 lines)
- `addons/sale_margin/i18n/hu.po` (222 lines)
- `addons/sale_margin/i18n/id.po` (223 lines)
- `addons/sale_margin/i18n/is.po` (200 lines)
- `addons/sale_margin/i18n/it.po` (231 lines)
- `addons/sale_margin/i18n/ja.po` (229 lines)
- `addons/sale_margin/i18n/ka.po` (202 lines)
- `addons/sale_margin/i18n/kab.po` (218 lines)
- `addons/sale_margin/i18n/km.po` (203 lines)
- `addons/sale_margin/i18n/ko.po` (222 lines)
- `addons/sale_margin/i18n/ku.po` (217 lines)
- `addons/sale_margin/i18n/lo.po` (218 lines)
- `addons/sale_margin/i18n/lt.po` (225 lines)
- `addons/sale_margin/i18n/lv.po` (221 lines)
- `addons/sale_margin/i18n/mk.po` (203 lines)
- `addons/sale_margin/i18n/mn.po` (222 lines)
- `addons/sale_margin/i18n/my.po` (218 lines)
- `addons/sale_margin/i18n/nb.po` (221 lines)
- `addons/sale_margin/i18n/nl.po` (231 lines)
- `addons/sale_margin/i18n/pl.po` (225 lines)
- `addons/sale_margin/i18n/pt.po` (223 lines)
- `addons/sale_margin/i18n/pt_BR.po` (241 lines)
- `addons/sale_margin/i18n/ro.po` (224 lines)
- `addons/sale_margin/i18n/ru.po` (221 lines)
- `addons/sale_margin/i18n/sale_margin.pot` (214 lines)
- `addons/sale_margin/i18n/sk.po` (222 lines)
- `addons/sale_margin/i18n/sl.po` (223 lines)
- `addons/sale_margin/i18n/sr@latin.po` (221 lines)
- `addons/sale_margin/i18n/sv.po` (223 lines)
- `addons/sale_margin/i18n/ta.po` (202 lines)
- `addons/sale_margin/i18n/th.po` (223 lines)
- `addons/sale_margin/i18n/tr.po` (223 lines)
- `addons/sale_margin/i18n/uk.po` (223 lines)
- `addons/sale_margin/i18n/uz.po` (232 lines)
- `addons/sale_margin/i18n/vi.po` (222 lines)
- `addons/sale_margin/i18n/zh_CN.po` (228 lines)
- `addons/sale_margin/i18n/zh_TW.po` (222 lines)
- `addons/sale_margin/models/__init__.py` (3 lines)
- `addons/sale_margin/models/sale_order.py` (49 lines)
- `addons/sale_margin/models/sale_order_line.py` (163 lines)
- `addons/sale_margin/models/sale_order_template_line.py` (20 lines)
- `addons/sale_margin/report/__init__.py` (3 lines)
- `addons/sale_margin/report/sale_report.py` (21 lines)
- `addons/sale_margin/report/sale_report_views.xml` (110 lines)
- `addons/sale_margin/static/src/js/labeled_field_short_labels.js` (13 lines)
- `addons/sale_margin/tests/__init__.py` (3 lines)
- `addons/sale_margin/tests/test_sale_margin.py` (339 lines)
- `addons/sale_margin/views/sale_order_template_views.xml` (24 lines)
- `addons/sale_margin/views/sale_order_views.xml` (60 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
