# Module: sale_purchase

- **Module ID:** MOD-528
- **Path:** `addons/sale_purchase`
- **Manifest:** `addons/sale_purchase/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Sale based on service outsourcing.


Allows the outsourcing of services. This module allows one to sell services provided
by external providers and will automatically generate purchase orders directed to the service seller.
    

Declared dependencies: `sale`, `purchase`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "purchase"
  ],
  "data": [
    "data/mail_templates.xml",
    "views/product_views.xml",
    "views/sale_order_views.xml",
    "views/purchase_order_views.xml"
  ]
}
```

### Representative source files

- `addons/sale_purchase/__init__.py` (3 lines)
- `addons/sale_purchase/__manifest__.py` (24 lines)
- `addons/sale_purchase/data/mail_templates.xml` (68 lines)
- `addons/sale_purchase/i18n/ar.po` (256 lines)
- `addons/sale_purchase/i18n/az.po` (251 lines)
- `addons/sale_purchase/i18n/bg.po` (245 lines)
- `addons/sale_purchase/i18n/bs.po` (251 lines)
- `addons/sale_purchase/i18n/ca.po` (264 lines)
- `addons/sale_purchase/i18n/cs.po` (259 lines)
- `addons/sale_purchase/i18n/da.po` (258 lines)
- `addons/sale_purchase/i18n/de.po` (272 lines)
- `addons/sale_purchase/i18n/el.po` (261 lines)
- `addons/sale_purchase/i18n/es.po` (270 lines)
- `addons/sale_purchase/i18n/es_419.po` (262 lines)
- `addons/sale_purchase/i18n/et.po` (265 lines)
- `addons/sale_purchase/i18n/fa.po` (260 lines)
- `addons/sale_purchase/i18n/fi.po` (273 lines)
- `addons/sale_purchase/i18n/fr.po` (267 lines)
- `addons/sale_purchase/i18n/gu.po` (245 lines)
- `addons/sale_purchase/i18n/he.po` (258 lines)
- `addons/sale_purchase/i18n/hi.po` (245 lines)
- `addons/sale_purchase/i18n/hr.po` (255 lines)
- `addons/sale_purchase/i18n/hu.po` (256 lines)
- `addons/sale_purchase/i18n/id.po` (258 lines)
- `addons/sale_purchase/i18n/is.po` (242 lines)
- `addons/sale_purchase/i18n/it.po` (267 lines)
- `addons/sale_purchase/i18n/ja.po` (261 lines)
- `addons/sale_purchase/i18n/kab.po` (246 lines)
- `addons/sale_purchase/i18n/ko.po` (256 lines)
- `addons/sale_purchase/i18n/ku.po` (245 lines)
- `addons/sale_purchase/i18n/lo.po` (245 lines)
- `addons/sale_purchase/i18n/lt.po` (259 lines)
- `addons/sale_purchase/i18n/lv.po` (246 lines)
- `addons/sale_purchase/i18n/mn.po` (259 lines)
- `addons/sale_purchase/i18n/my.po` (246 lines)
- `addons/sale_purchase/i18n/nb.po` (258 lines)
- `addons/sale_purchase/i18n/nl.po` (263 lines)
- `addons/sale_purchase/i18n/pl.po` (267 lines)
- `addons/sale_purchase/i18n/pt.po` (262 lines)
- `addons/sale_purchase/i18n/pt_BR.po` (270 lines)
- `addons/sale_purchase/i18n/ro.po` (260 lines)
- `addons/sale_purchase/i18n/ru.po` (262 lines)
- `addons/sale_purchase/i18n/sale_purchase.pot` (240 lines)
- `addons/sale_purchase/i18n/sk.po` (260 lines)
- `addons/sale_purchase/i18n/sl.po` (253 lines)
- `addons/sale_purchase/i18n/sr@latin.po` (252 lines)
- `addons/sale_purchase/i18n/sv.po` (255 lines)
- `addons/sale_purchase/i18n/th.po` (251 lines)
- `addons/sale_purchase/i18n/tr.po` (271 lines)
- `addons/sale_purchase/i18n/uk.po` (259 lines)
- `addons/sale_purchase/i18n/uz.po` (294 lines)
- `addons/sale_purchase/i18n/vi.po` (259 lines)
- `addons/sale_purchase/i18n/zh_CN.po` (259 lines)
- `addons/sale_purchase/i18n/zh_TW.po` (252 lines)
- `addons/sale_purchase/models/__init__.py` (7 lines)
- `addons/sale_purchase/models/product_template.py` (57 lines)
- `addons/sale_purchase/models/purchase_order.py` (93 lines)
- `addons/sale_purchase/models/sale_order.py` (80 lines)
- `addons/sale_purchase/models/sale_order_line.py` (298 lines)
- `addons/sale_purchase/tests/__init__.py` (6 lines)
- `addons/sale_purchase/tests/common.py` (69 lines)
- `addons/sale_purchase/tests/test_access_rights.py` (85 lines)
- `addons/sale_purchase/tests/test_sale_purchase.py` (527 lines)
- `addons/sale_purchase/views/product_views.xml` (15 lines)
- `addons/sale_purchase/views/purchase_order_views.xml` (18 lines)
- `addons/sale_purchase/views/sale_order_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
