# Module: lunch

- **Module ID:** MOD-350
- **Path:** `addons/lunch`
- **Manifest:** `addons/lunch/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Handle lunch orders of your employees


The base module to manage lunch.
================================

Many companies order sandwiches, pizzas and other, from usual vendors, for their employees to offer them more facilities.

However lunches management within the company requires proper administration especially when the number of employees or vendors is important.

The “Lunch Order” module has been developed to make this management easier but also to offer employees more tools and usability.

In addition to a full meal and vendor management, this module offers the possibility to display warning and provides quick order selection based on employee’s preferences.

If you want to save your employees' time and avoid them to always have coins in their pockets, this module is essential.
    

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 25 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 18 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "security/lunch_security.xml",
    "report/lunch_cashmove_report_views.xml",
    "views/lunch_templates.xml",
    "views/lunch_alert_views.xml",
    "views/lunch_cashmove_views.xml",
    "views/lunch_location_views.xml",
    "views/lunch_orders_views.xml",
    "views/lunch_product_views.xml",
    "views/lunch_supplier_views.xml",
    "views/res_config_settings.xml",
    "views/lunch_views.xml",
    "data/mail_template_data.xml",
    "data/lunch_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/lunch_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "lunch/static/src/components/*",
      "lunch/static/src/mixins/*.js",
      "lunch/static/src/views/*",
      "lunch/static/src/scss/lunch_kanban.scss"
    ],
    "web.assets_tests": [
      "lunch/static/tests/tours/*.js"
    ],
    "web.assets_unit_tests": [
      "lunch/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/lunch/__init__.py` (6 lines)
- `addons/lunch/__manifest__.py` (55 lines)
- `addons/lunch/controllers/__init__.py` (4 lines)
- `addons/lunch/controllers/main.py` (162 lines)
- `addons/lunch/data/lunch_data.xml` (67 lines)
- `addons/lunch/data/lunch_demo.xml` (490 lines)
- `addons/lunch/data/mail_template_data.xml` (77 lines)
- `addons/lunch/i18n/af.po` (2,294 lines)
- `addons/lunch/i18n/am.po` (2,290 lines)
- `addons/lunch/i18n/ar.po` (2,352 lines)
- `addons/lunch/i18n/az.po` (2,313 lines)
- `addons/lunch/i18n/bg.po` (2,324 lines)
- `addons/lunch/i18n/bs.po` (2,305 lines)
- `addons/lunch/i18n/ca.po` (2,380 lines)
- `addons/lunch/i18n/cs.po` (2,342 lines)
- `addons/lunch/i18n/da.po` (2,348 lines)
- `addons/lunch/i18n/de.po` (2,566 lines)
- `addons/lunch/i18n/el.po` (2,316 lines)
- `addons/lunch/i18n/es.po` (2,543 lines)
- `addons/lunch/i18n/es_419.po` (2,554 lines)
- `addons/lunch/i18n/es_CL.po` (198 lines)
- `addons/lunch/i18n/et.po` (2,368 lines)
- `addons/lunch/i18n/eu.po` (2,293 lines)
- `addons/lunch/i18n/fa.po` (2,331 lines)
- `addons/lunch/i18n/fi.po` (2,570 lines)
- `addons/lunch/i18n/fo.po` (2,293 lines)
- `addons/lunch/i18n/fr.po` (2,544 lines)
- `addons/lunch/i18n/fr_BE.po` (191 lines)
- `addons/lunch/i18n/fr_CA.po` (153 lines)
- `addons/lunch/i18n/gl.po` (2,293 lines)
- `addons/lunch/i18n/gu.po` (2,302 lines)
- `addons/lunch/i18n/he.po` (2,349 lines)
- `addons/lunch/i18n/hi.po` (2,301 lines)
- `addons/lunch/i18n/hr.po` (2,330 lines)
- `addons/lunch/i18n/hu.po` (2,337 lines)
- `addons/lunch/i18n/id.po` (2,525 lines)
- `addons/lunch/i18n/is.po` (2,294 lines)
- `addons/lunch/i18n/it.po` (2,561 lines)
- `addons/lunch/i18n/ja.po` (2,524 lines)
- `addons/lunch/i18n/ka.po` (2,293 lines)
- `addons/lunch/i18n/kab.po` (2,302 lines)
- `addons/lunch/i18n/km.po` (2,300 lines)
- `addons/lunch/i18n/ko.po` (2,513 lines)
- `addons/lunch/i18n/ku.po` (2,300 lines)
- `addons/lunch/i18n/lb.po` (2,295 lines)
- `addons/lunch/i18n/lo.po` (2,529 lines)
- `addons/lunch/i18n/lt.po` (2,338 lines)
- `addons/lunch/i18n/lunch.pot` (2,258 lines)
- `addons/lunch/i18n/lv.po` (2,317 lines)
- `addons/lunch/i18n/mk.po` (2,293 lines)
- `addons/lunch/i18n/mn.po` (2,338 lines)
- `addons/lunch/i18n/my.po` (2,302 lines)
- `addons/lunch/i18n/nb.po` (2,321 lines)
- `addons/lunch/i18n/nl.po` (2,560 lines)
- `addons/lunch/i18n/pl.po` (2,561 lines)
- `addons/lunch/i18n/pt.po` (2,367 lines)
- `addons/lunch/i18n/pt_BR.po` (2,540 lines)
- `addons/lunch/i18n/ro.po` (2,356 lines)
- `addons/lunch/i18n/ru.po` (2,543 lines)
- `addons/lunch/i18n/sk.po` (2,333 lines)
- `addons/lunch/i18n/sl.po` (2,365 lines)
- `addons/lunch/i18n/sq.po` (2,301 lines)
- `addons/lunch/i18n/sr@latin.po` (2,313 lines)
- `addons/lunch/i18n/sv.po` (2,372 lines)
- `addons/lunch/i18n/ta.po` (2,294 lines)
- `addons/lunch/i18n/th.po` (2,503 lines)
- `addons/lunch/i18n/tr.po` (2,385 lines)
- `addons/lunch/i18n/uk.po` (2,361 lines)
- `addons/lunch/i18n/uz.po` (2,696 lines)
- `addons/lunch/i18n/vi.po` (2,530 lines)
- `addons/lunch/i18n/zh_CN.po` (2,517 lines)
- `addons/lunch/i18n/zh_TW.po` (2,345 lines)
- `addons/lunch/models/__init__.py` (15 lines)
- `addons/lunch/models/lunch_alert.py` (190 lines)
- `addons/lunch/models/lunch_cashmove.py` (31 lines)
- `addons/lunch/models/lunch_location.py` (13 lines)
- `addons/lunch/models/lunch_order.py` (320 lines)
- `addons/lunch/models/lunch_product.py` (120 lines)
- `addons/lunch/models/lunch_product_category.py` (43 lines)
- `addons/lunch/models/lunch_supplier.py` (365 lines)
- `addons/lunch/models/lunch_topping.py` (26 lines)
- `addons/lunch/models/res_company.py` (13 lines)
- `addons/lunch/models/res_config_settings.py` (12 lines)
- `addons/lunch/models/res_groups.py` (13 lines)
- `addons/lunch/models/res_users.py` (10 lines)
- `addons/lunch/report/__init__.py` (4 lines)
- `addons/lunch/report/lunch_cashmove_report.py` (51 lines)
- `addons/lunch/report/lunch_cashmove_report_views.xml` (142 lines)
- `addons/lunch/security/ir.access.csv` (25 lines)
- `addons/lunch/security/lunch_security.xml` (26 lines)
- `addons/lunch/static/description/icon.png` (38 lines)
- `addons/lunch/static/description/icon.svg` (1 lines)
- `addons/lunch/static/description/icon_hi.png` (124 lines)
- `addons/lunch/static/img/4formaggio.png` (74 lines)
- `addons/lunch/static/img/Coke.png` (61 lines)
- `addons/lunch/static/img/bacon_burger.png` (94 lines)
- `addons/lunch/static/img/brie.png` (58 lines)
- `addons/lunch/static/img/burger.png` (24 lines)
- `addons/lunch/static/img/cheeseburger.png` (69 lines)
- `addons/lunch/static/img/chicken_curry.png` (72 lines)
- `addons/lunch/static/img/chirashi.png` (59 lines)
- `addons/lunch/static/img/club.png` (60 lines)
- `addons/lunch/static/img/coke_zero.png` (77 lines)
- `addons/lunch/static/img/drink.png` (14 lines)
- `addons/lunch/static/img/fanta.png` (57 lines)
- `addons/lunch/static/img/fuze_black.png` (48 lines)
- `addons/lunch/static/img/fuze_green.png` (36 lines)
- `addons/lunch/static/img/gouda.png` (73 lines)
- `addons/lunch/static/img/italiana.png` (78 lines)
- `addons/lunch/static/img/lipton.png` (72 lines)
- `addons/lunch/static/img/lunch.png` (17 lines)
- `addons/lunch/static/img/maki.png` (77 lines)
- `addons/lunch/static/img/mozza.png` (52 lines)
- `addons/lunch/static/img/napoli.png` (88 lines)
- `addons/lunch/static/img/pasta_bolognese.png` (68 lines)
- `addons/lunch/static/img/pizza.jpeg` (45 lines)
- `addons/lunch/static/img/pizza.png` (31 lines)
- `addons/lunch/static/img/pizza_funghi.png` (73 lines)
- `addons/lunch/static/img/pizza_margherita.png` (81 lines)
- `addons/lunch/static/img/pizza_veggie.png` (57 lines)
- `addons/lunch/static/img/salmon_sushi.png` (62 lines)
- `addons/lunch/static/img/temaki.png` (73 lines)
- `addons/lunch/static/img/tuna_sandwich.png` (56 lines)
- `addons/lunch/static/src/components/lunch_dashboard.js` (219 lines)
- `addons/lunch/static/src/components/lunch_dashboard.scss` (32 lines)
- `addons/lunch/static/src/components/lunch_dashboard.xml` (287 lines)
- `addons/lunch/static/src/components/lunch_is_favorite_field.js` (14 lines)
- `addons/lunch/static/src/mixins/lunch_renderer_mixin.js` (45 lines)
- `addons/lunch/static/src/scss/lunch_kanban.scss` (13 lines)
- `addons/lunch/static/src/views/kanban.js` (53 lines)
- `addons/lunch/static/src/views/kanban.xml` (17 lines)
- `addons/lunch/static/src/views/list.js` (49 lines)
- `addons/lunch/static/src/views/list.xml` (15 lines)
- `addons/lunch/static/src/views/no_content_helper.xml` (18 lines)
- `addons/lunch/static/src/views/search_model.js` (74 lines)
- `addons/lunch/static/src/views/search_panel.js` (11 lines)
- `addons/lunch/static/tests/lunch_is_favorite_field.test.js` (77 lines)
- `addons/lunch/static/tests/lunch_kanban.test.js` (368 lines)
- `addons/lunch/static/tests/tours/order_lunch.js` (47 lines)
- `addons/lunch/tests/__init__.py` (8 lines)
- `addons/lunch/tests/common.py` (115 lines)
- `addons/lunch/tests/test_alert.py` (61 lines)
- `addons/lunch/tests/test_order.py` (104 lines)
- `addons/lunch/tests/test_supplier.py` (275 lines)
- `addons/lunch/tests/test_ui.py` (51 lines)
- `addons/lunch/views/lunch_alert_views.xml` (106 lines)
- `addons/lunch/views/lunch_cashmove_views.xml` (93 lines)
- `addons/lunch/views/lunch_location_views.xml` (72 lines)
- `addons/lunch/views/lunch_orders_views.xml` (277 lines)
- `addons/lunch/views/lunch_product_views.xml` (310 lines)
- `addons/lunch/views/lunch_supplier_views.xml` (153 lines)
- `addons/lunch/views/lunch_templates.xml` (6 lines)
- `addons/lunch/views/lunch_views.xml` (25 lines)
- `addons/lunch/views/res_config_settings.xml` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
