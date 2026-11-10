# Module: website_sale_collect

- **Module ID:** MOD-635
- **Path:** `addons/website_sale_collect`
- **Manifest:** `addons/website_sale_collect/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows customers to check in-store stock, pay on site, and pick up their orders at the shop.


Declared dependencies: `base_geolocalize`, `payment_custom`, `website_sale_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 31 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 18 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 12 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_geolocalize",
    "payment_custom",
    "website_sale_stock"
  ],
  "data": [
    "data/payment_provider_data.xml",
    "data/payment_method_data.xml",
    "data/product_product_data.xml",
    "data/delivery_carrier_data.xml",
    "views/delivery_carrier_views.xml",
    "views/delivery_form_templates.xml",
    "views/payment_provider_views.xml",
    "views/res_config_settings_views.xml",
    "views/sale_order_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_warehouse_views.xml",
    "views/templates.xml"
  ],
  "demo": [
    "demo/stock_warehouse_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale_collect/static/src/**/*",
      [
        "remove",
        "website_sale_collect/static/src/js/pickup_location_many2one/**/*"
      ]
    ],
    "web.assets_backend": [
      "website_sale_collect/static/src/js/location_selector/**/*",
      "website_sale_collect/static/src/js/pickup_location_many2one/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_collect/__init__.py` (12 lines)
- `addons/website_sale_collect/__manifest__.py` (39 lines)
- `addons/website_sale_collect/const.py` (7 lines)
- `addons/website_sale_collect/controllers/__init__.py` (3 lines)
- `addons/website_sale_collect/controllers/delivery.py` (78 lines)
- `addons/website_sale_collect/controllers/main.py` (92 lines)
- `addons/website_sale_collect/controllers/payment.py` (34 lines)
- `addons/website_sale_collect/data/delivery_carrier_data.xml` (12 lines)
- `addons/website_sale_collect/data/payment_method_data.xml` (15 lines)
- `addons/website_sale_collect/data/payment_provider_data.xml` (23 lines)
- `addons/website_sale_collect/data/product_product_data.xml` (12 lines)
- `addons/website_sale_collect/demo/stock_warehouse_demo.xml` (21 lines)
- `addons/website_sale_collect/i18n/ar.po` (443 lines)
- `addons/website_sale_collect/i18n/az.po` (439 lines)
- `addons/website_sale_collect/i18n/bg.po` (458 lines)
- `addons/website_sale_collect/i18n/bs.po` (442 lines)
- `addons/website_sale_collect/i18n/ca.po` (443 lines)
- `addons/website_sale_collect/i18n/cs.po` (432 lines)
- `addons/website_sale_collect/i18n/da.po` (447 lines)
- `addons/website_sale_collect/i18n/de.po` (447 lines)
- `addons/website_sale_collect/i18n/el.po` (429 lines)
- `addons/website_sale_collect/i18n/es.po` (448 lines)
- `addons/website_sale_collect/i18n/es_419.po` (446 lines)
- `addons/website_sale_collect/i18n/et.po` (455 lines)
- `addons/website_sale_collect/i18n/fa.po` (455 lines)
- `addons/website_sale_collect/i18n/fi.po` (452 lines)
- `addons/website_sale_collect/i18n/fr.po` (441 lines)
- `addons/website_sale_collect/i18n/he.po` (445 lines)
- `addons/website_sale_collect/i18n/hi.po` (447 lines)
- `addons/website_sale_collect/i18n/hr.po` (449 lines)
- `addons/website_sale_collect/i18n/hu.po` (438 lines)
- `addons/website_sale_collect/i18n/id.po` (445 lines)
- `addons/website_sale_collect/i18n/it.po` (440 lines)
- `addons/website_sale_collect/i18n/ja.po` (432 lines)
- `addons/website_sale_collect/i18n/kab.po` (433 lines)
- `addons/website_sale_collect/i18n/ko.po` (448 lines)
- `addons/website_sale_collect/i18n/ku.po` (428 lines)
- `addons/website_sale_collect/i18n/lo.po` (439 lines)
- `addons/website_sale_collect/i18n/lt.po` (445 lines)
- `addons/website_sale_collect/i18n/lv.po` (443 lines)
- `addons/website_sale_collect/i18n/mn.po` (441 lines)
- `addons/website_sale_collect/i18n/my.po` (436 lines)
- `addons/website_sale_collect/i18n/nb.po` (428 lines)
- `addons/website_sale_collect/i18n/nl.po` (448 lines)
- `addons/website_sale_collect/i18n/pl.po` (441 lines)
- `addons/website_sale_collect/i18n/pt.po` (444 lines)
- `addons/website_sale_collect/i18n/pt_BR.po` (445 lines)
- `addons/website_sale_collect/i18n/ro.po` (452 lines)
- `addons/website_sale_collect/i18n/ru.po` (449 lines)
- `addons/website_sale_collect/i18n/sk.po` (447 lines)
- `addons/website_sale_collect/i18n/sl.po` (431 lines)
- `addons/website_sale_collect/i18n/sr@latin.po` (441 lines)
- `addons/website_sale_collect/i18n/sv.po` (435 lines)
- `addons/website_sale_collect/i18n/th.po` (433 lines)
- `addons/website_sale_collect/i18n/tr.po` (448 lines)
- `addons/website_sale_collect/i18n/uk.po` (446 lines)
- `addons/website_sale_collect/i18n/uz.po` (488 lines)
- `addons/website_sale_collect/i18n/vi.po` (444 lines)
- `addons/website_sale_collect/i18n/website_sale_collect.pot` (417 lines)
- `addons/website_sale_collect/i18n/zh_CN.po` (452 lines)
- `addons/website_sale_collect/i18n/zh_TW.po` (450 lines)
- `addons/website_sale_collect/models/__init__.py` (14 lines)
- `addons/website_sale_collect/models/delivery_carrier.py` (178 lines)
- `addons/website_sale_collect/models/payment_method.py` (11 lines)
- `addons/website_sale_collect/models/payment_provider.py` (89 lines)
- `addons/website_sale_collect/models/payment_transaction.py` (30 lines)
- `addons/website_sale_collect/models/product_template.py` (124 lines)
- `addons/website_sale_collect/models/res_config_settings.py` (26 lines)
- `addons/website_sale_collect/models/sale_order.py` (197 lines)
- `addons/website_sale_collect/models/sale_order_line.py` (17 lines)
- `addons/website_sale_collect/models/stock_warehouse.py` (143 lines)
- `addons/website_sale_collect/models/website.py` (73 lines)
- `addons/website_sale_collect/static/description/icon.png` (20 lines)
- `addons/website_sale_collect/static/description/icon.svg` (1 lines)
- `addons/website_sale_collect/static/img/pay_on_site.png` (10 lines)
- `addons/website_sale_collect/static/src/interactions/checkout.js` (159 lines)
- `addons/website_sale_collect/static/src/interactions/payment_form.js` (16 lines)
- `addons/website_sale_collect/static/src/interactions/product_page.js` (17 lines)
- `addons/website_sale_collect/static/src/js/click_and_collect_availability/click_and_collect_availability.js` (179 lines)
- `addons/website_sale_collect/static/src/js/click_and_collect_availability/click_and_collect_availability.xml` (119 lines)
- `addons/website_sale_collect/static/src/js/location_selector/location/location.xml` (30 lines)
- `addons/website_sale_collect/static/src/js/location_selector/location_selector_dialog/location_selector_dialog.js` (137 lines)
- `addons/website_sale_collect/static/src/js/location_selector/location_selector_dialog/location_selector_dialog.xml` (60 lines)
- `addons/website_sale_collect/static/src/js/location_selector/map_container/map_container.js` (24 lines)
- `addons/website_sale_collect/static/src/js/location_selector/map_container/map_container.xml` (36 lines)
- `addons/website_sale_collect/static/src/js/pickup_location_many2one/pickup_location_many2one.js` (14 lines)
- `addons/website_sale_collect/static/src/scss/click_and_collect_availability.scss` (26 lines)
- `addons/website_sale_collect/static/src/tests/tours/buy_with_click_and_collect.js` (68 lines)
- `addons/website_sale_collect/static/src/xml/product_availability.xml` (11 lines)
- `addons/website_sale_collect/tests/__init__.py` (14 lines)
- `addons/website_sale_collect/tests/common.py` (55 lines)
- `addons/website_sale_collect/tests/test_click_and_collect_express_checkout.py` (27 lines)
- `addons/website_sale_collect/tests/test_click_and_collect_flow.py` (65 lines)
- `addons/website_sale_collect/tests/test_delivery_carrier.py` (113 lines)
- `addons/website_sale_collect/tests/test_in_store_delivery.py` (78 lines)
- `addons/website_sale_collect/tests/test_payment_provider.py` (64 lines)
- `addons/website_sale_collect/tests/test_payment_transaction.py` (26 lines)
- `addons/website_sale_collect/tests/test_product_template.py` (49 lines)
- `addons/website_sale_collect/tests/test_sale_order.py` (319 lines)
- `addons/website_sale_collect/tests/test_stock_warehouse.py` (55 lines)
- `addons/website_sale_collect/tests/test_website.py` (48 lines)
- `addons/website_sale_collect/utils.py` (76 lines)
- `addons/website_sale_collect/views/delivery_carrier_views.xml` (67 lines)
- `addons/website_sale_collect/views/delivery_form_templates.xml` (152 lines)
- `addons/website_sale_collect/views/payment_provider_views.xml` (18 lines)
- `addons/website_sale_collect/views/res_config_settings_views.xml` (23 lines)
- `addons/website_sale_collect/views/sale_order_views.xml` (13 lines)
- `addons/website_sale_collect/views/stock_picking_views.xml` (13 lines)
- `addons/website_sale_collect/views/stock_warehouse_views.xml` (15 lines)
- `addons/website_sale_collect/views/templates.xml` (49 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
