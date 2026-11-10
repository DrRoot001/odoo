# Module: website_event_sale

- **Module ID:** MOD-613
- **Path:** `addons/website_event_sale`
- **Manifest:** `addons/website_event_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Sell event tickets online


Sell event tickets through eCommerce app.
    

Declared dependencies: `website_event`, `event_sale`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event",
    "event_sale",
    "website_sale"
  ],
  "data": [
    "data/event_data.xml",
    "report/event_sale_report_views.xml",
    "views/event_event_views.xml",
    "views/website_event_templates.xml",
    "views/website_sale_templates.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "website_event_sale/static/tests/**/*"
    ],
    "web.assets_frontend": [
      "website_event_sale/static/src/scss/*.scss"
    ]
  }
}
```

### Representative source files

- `addons/website_event_sale/__init__.py` (6 lines)
- `addons/website_event_sale/__manifest__.py` (29 lines)
- `addons/website_event_sale/controllers/__init__.py` (4 lines)
- `addons/website_event_sale/controllers/main.py` (106 lines)
- `addons/website_event_sale/controllers/sale.py` (32 lines)
- `addons/website_event_sale/data/event_data.xml` (10 lines)
- `addons/website_event_sale/i18n/af.po` (222 lines)
- `addons/website_event_sale/i18n/ar.po` (234 lines)
- `addons/website_event_sale/i18n/az.po` (234 lines)
- `addons/website_event_sale/i18n/bg.po` (244 lines)
- `addons/website_event_sale/i18n/bs.po` (235 lines)
- `addons/website_event_sale/i18n/ca.po` (250 lines)
- `addons/website_event_sale/i18n/cs.po` (238 lines)
- `addons/website_event_sale/i18n/da.po` (242 lines)
- `addons/website_event_sale/i18n/de.po` (239 lines)
- `addons/website_event_sale/i18n/el.po` (230 lines)
- `addons/website_event_sale/i18n/es.po` (240 lines)
- `addons/website_event_sale/i18n/es_419.po` (231 lines)
- `addons/website_event_sale/i18n/es_CL.po` (24 lines)
- `addons/website_event_sale/i18n/et.po` (241 lines)
- `addons/website_event_sale/i18n/eu.po` (219 lines)
- `addons/website_event_sale/i18n/fa.po` (246 lines)
- `addons/website_event_sale/i18n/fi.po` (239 lines)
- `addons/website_event_sale/i18n/fo.po` (219 lines)
- `addons/website_event_sale/i18n/fr.po` (237 lines)
- `addons/website_event_sale/i18n/fr_CA.po` (24 lines)
- `addons/website_event_sale/i18n/gl.po` (219 lines)
- `addons/website_event_sale/i18n/gu.po` (221 lines)
- `addons/website_event_sale/i18n/he.po` (238 lines)
- `addons/website_event_sale/i18n/hi.po` (235 lines)
- `addons/website_event_sale/i18n/hr.po` (235 lines)
- `addons/website_event_sale/i18n/hu.po` (234 lines)
- `addons/website_event_sale/i18n/id.po` (239 lines)
- `addons/website_event_sale/i18n/is.po` (217 lines)
- `addons/website_event_sale/i18n/it.po` (234 lines)
- `addons/website_event_sale/i18n/ja.po` (233 lines)
- `addons/website_event_sale/i18n/ka.po` (223 lines)
- `addons/website_event_sale/i18n/kab.po` (230 lines)
- `addons/website_event_sale/i18n/km.po` (222 lines)
- `addons/website_event_sale/i18n/ko.po` (236 lines)
- `addons/website_event_sale/i18n/ku.po` (227 lines)
- `addons/website_event_sale/i18n/lo.po` (230 lines)
- `addons/website_event_sale/i18n/lt.po` (244 lines)
- `addons/website_event_sale/i18n/lv.po` (232 lines)
- `addons/website_event_sale/i18n/mk.po` (221 lines)
- `addons/website_event_sale/i18n/mn.po` (240 lines)
- `addons/website_event_sale/i18n/my.po` (232 lines)
- `addons/website_event_sale/i18n/nb.po` (230 lines)
- `addons/website_event_sale/i18n/nl.po` (235 lines)
- `addons/website_event_sale/i18n/pl.po` (240 lines)
- `addons/website_event_sale/i18n/pt.po` (245 lines)
- `addons/website_event_sale/i18n/pt_BR.po` (240 lines)
- `addons/website_event_sale/i18n/ro.po` (241 lines)
- `addons/website_event_sale/i18n/ru.po` (235 lines)
- `addons/website_event_sale/i18n/sk.po` (234 lines)
- `addons/website_event_sale/i18n/sl.po` (233 lines)
- `addons/website_event_sale/i18n/sr@latin.po` (237 lines)
- `addons/website_event_sale/i18n/sv.po` (239 lines)
- `addons/website_event_sale/i18n/th.po` (235 lines)
- `addons/website_event_sale/i18n/tr.po` (240 lines)
- `addons/website_event_sale/i18n/uk.po` (243 lines)
- `addons/website_event_sale/i18n/uz.po` (260 lines)
- `addons/website_event_sale/i18n/vi.po` (239 lines)
- `addons/website_event_sale/i18n/website_event_sale.pot` (217 lines)
- `addons/website_event_sale/i18n/zh_CN.po` (235 lines)
- `addons/website_event_sale/i18n/zh_TW.po` (231 lines)
- `addons/website_event_sale/models/__init__.py` (6 lines)
- `addons/website_event_sale/models/event_event.py` (23 lines)
- `addons/website_event_sale/models/event_ticket.py` (23 lines)
- `addons/website_event_sale/models/product.py` (40 lines)
- `addons/website_event_sale/models/product_pricelist.py` (22 lines)
- `addons/website_event_sale/models/sale_order.py` (171 lines)
- `addons/website_event_sale/models/sale_order_line.py` (32 lines)
- `addons/website_event_sale/report/__init__.py` (1 lines)
- `addons/website_event_sale/report/event_sale_report.py` (15 lines)
- `addons/website_event_sale/report/event_sale_report_views.xml` (14 lines)
- `addons/website_event_sale/static/description/icon.png` (26 lines)
- `addons/website_event_sale/static/description/icon.svg` (1 lines)
- `addons/website_event_sale/static/description/icon_hi.png` (136 lines)
- `addons/website_event_sale/static/img/event_ticket_placeholder_thumbnail.png` (33 lines)
- `addons/website_event_sale/static/src/scss/website_event_sale_templates.scss` (18 lines)
- `addons/website_event_sale/static/tests/tours/helpers/WebsiteEventSaleTourMethods.js` (62 lines)
- `addons/website_event_sale/static/tests/tours/website_event_sale.js` (121 lines)
- `addons/website_event_sale/static/tests/tours/website_event_sale_last_ticket.js` (61 lines)
- `addons/website_event_sale/static/tests/tours/website_event_sale_pricelists.js` (72 lines)
- `addons/website_event_sale/tests/__init__.py` (8 lines)
- `addons/website_event_sale/tests/common.py` (100 lines)
- `addons/website_event_sale/tests/test_event_checkout.py` (68 lines)
- `addons/website_event_sale/tests/test_frontend_buy_tickets.py` (259 lines)
- `addons/website_event_sale/tests/test_website_event_sale.py` (217 lines)
- `addons/website_event_sale/tests/test_website_event_sale_cart.py` (83 lines)
- `addons/website_event_sale/tests/test_website_event_sale_pricelist.py` (61 lines)
- `addons/website_event_sale/views/event_event_views.xml` (13 lines)
- `addons/website_event_sale/views/website_event_templates.xml` (102 lines)
- `addons/website_event_sale/views/website_sale_templates.xml` (105 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
