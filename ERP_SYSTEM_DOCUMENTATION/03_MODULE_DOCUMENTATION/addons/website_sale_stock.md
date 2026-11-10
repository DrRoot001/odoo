# Module: website_sale_stock

- **Module ID:** MOD-642
- **Path:** `addons/website_sale_stock`
- **Manifest:** `addons/website_sale_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage product inventory & availability


Manage the inventory of your products and display their availability status in your eCommerce store.
In case of stockout, you can decide to block further sales or to keep selling.
A default behavior can be selected in the Website settings.
Then it can be made specific at the product level.
    

Declared dependencies: `website_sale`, `sale_stock`, `stock_delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 31 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 17 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 17 | Client behavior/assets. |
| Tests | 16 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale",
    "sale_stock",
    "stock_delivery"
  ],
  "data": [
    "views/checkout_templates.xml",
    "views/delivery_form.xml",
    "views/res_config_settings_views.xml",
    "views/sale_order_views.xml",
    "views/stock_picking_views.xml",
    "wizard/choose_delivery_carrier_views.xml"
  ],
  "demo": [
    "data/website_sale_stock_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale_stock/static/src/interactions/**/*",
      "website_sale_stock/static/src/js/combo_configurator_dialog/*",
      "website_sale_stock/static/src/js/models/*",
      "website_sale_stock/static/src/js/product_card/*",
      "website_sale_stock/static/src/js/location_selector/**/*"
    ],
    "web.assets_backend": [
      "website_sale_stock/static/src/js/location_selector/**/*",
      "website_sale_stock/static/src/js/pickup_location_many2one/**/*"
    ],
    "web.assets_tests": [
      "website_sale_stock/static/tests/tours/*",
      "website_sale_stock/static/src/js/tours/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_stock/__init__.py` (3 lines)
- `addons/website_sale_stock/__manifest__.py` (44 lines)
- `addons/website_sale_stock/controllers/__init__.py` (3 lines)
- `addons/website_sale_stock/controllers/location_selector.py` (43 lines)
- `addons/website_sale_stock/data/website_sale_stock_demo.xml` (19 lines)
- `addons/website_sale_stock/i18n/af.po` (345 lines)
- `addons/website_sale_stock/i18n/ar.po` (352 lines)
- `addons/website_sale_stock/i18n/az.po` (362 lines)
- `addons/website_sale_stock/i18n/bg.po` (373 lines)
- `addons/website_sale_stock/i18n/bs.po` (376 lines)
- `addons/website_sale_stock/i18n/ca.po` (379 lines)
- `addons/website_sale_stock/i18n/cs.po` (382 lines)
- `addons/website_sale_stock/i18n/da.po` (367 lines)
- `addons/website_sale_stock/i18n/de.po` (362 lines)
- `addons/website_sale_stock/i18n/el.po` (360 lines)
- `addons/website_sale_stock/i18n/es.po` (388 lines)
- `addons/website_sale_stock/i18n/es_419.po` (359 lines)
- `addons/website_sale_stock/i18n/et.po` (381 lines)
- `addons/website_sale_stock/i18n/fa.po` (376 lines)
- `addons/website_sale_stock/i18n/fi.po` (379 lines)
- `addons/website_sale_stock/i18n/fr.po` (355 lines)
- `addons/website_sale_stock/i18n/gu.po` (344 lines)
- `addons/website_sale_stock/i18n/he.po` (380 lines)
- `addons/website_sale_stock/i18n/hi.po` (369 lines)
- `addons/website_sale_stock/i18n/hr.po` (371 lines)
- `addons/website_sale_stock/i18n/hu.po` (366 lines)
- `addons/website_sale_stock/i18n/id.po` (379 lines)
- `addons/website_sale_stock/i18n/is.po` (341 lines)
- `addons/website_sale_stock/i18n/it.po` (353 lines)
- `addons/website_sale_stock/i18n/ja.po` (350 lines)
- `addons/website_sale_stock/i18n/kab.po` (352 lines)
- `addons/website_sale_stock/i18n/km.po` (345 lines)
- `addons/website_sale_stock/i18n/ko.po` (378 lines)
- `addons/website_sale_stock/i18n/ku.po` (343 lines)
- `addons/website_sale_stock/i18n/lo.po` (349 lines)
- `addons/website_sale_stock/i18n/lt.po` (366 lines)
- `addons/website_sale_stock/i18n/lv.po` (366 lines)
- `addons/website_sale_stock/i18n/mn.po` (364 lines)
- `addons/website_sale_stock/i18n/my.po` (353 lines)
- `addons/website_sale_stock/i18n/nb.po` (363 lines)
- `addons/website_sale_stock/i18n/nl.po` (352 lines)
- `addons/website_sale_stock/i18n/pl.po` (368 lines)
- `addons/website_sale_stock/i18n/pt.po` (380 lines)
- `addons/website_sale_stock/i18n/pt_BR.po` (359 lines)
- `addons/website_sale_stock/i18n/ro.po` (382 lines)
- `addons/website_sale_stock/i18n/ru.po` (376 lines)
- `addons/website_sale_stock/i18n/sk.po` (375 lines)
- `addons/website_sale_stock/i18n/sl.po` (371 lines)
- `addons/website_sale_stock/i18n/sr@latin.po` (365 lines)
- `addons/website_sale_stock/i18n/sv.po` (378 lines)
- `addons/website_sale_stock/i18n/th.po` (372 lines)
- `addons/website_sale_stock/i18n/tr.po` (383 lines)
- `addons/website_sale_stock/i18n/uk.po` (374 lines)
- `addons/website_sale_stock/i18n/uz.po` (358 lines)
- `addons/website_sale_stock/i18n/vi.po` (380 lines)
- `addons/website_sale_stock/i18n/website_sale_stock.pot` (333 lines)
- `addons/website_sale_stock/i18n/zh_CN.po` (376 lines)
- `addons/website_sale_stock/i18n/zh_TW.po` (376 lines)
- `addons/website_sale_stock/models/__init__.py` (12 lines)
- `addons/website_sale_stock/models/delivery_carrier.py` (59 lines)
- `addons/website_sale_stock/models/product_product.py` (17 lines)
- `addons/website_sale_stock/models/product_template.py` (12 lines)
- `addons/website_sale_stock/models/res_config_settings.py` (14 lines)
- `addons/website_sale_stock/models/res_partner.py` (82 lines)
- `addons/website_sale_stock/models/sale_order.py` (88 lines)
- `addons/website_sale_stock/models/stock_picking.py` (71 lines)
- `addons/website_sale_stock/models/website.py` (22 lines)
- `addons/website_sale_stock/static/description/icon.png` (24 lines)
- `addons/website_sale_stock/static/description/icon.svg` (1 lines)
- `addons/website_sale_stock/static/description/icon_hi.png` (115 lines)
- `addons/website_sale_stock/static/src/interactions/checkout.js` (212 lines)
- `addons/website_sale_stock/static/src/js/combo_configurator_dialog/combo_configurator_dialog.js` (36 lines)
- `addons/website_sale_stock/static/src/js/combo_configurator_dialog/combo_configurator_dialog.xml` (27 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location/location.js` (35 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location/location.xml` (46 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_list/location_list.js` (46 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_list/location_list.xml` (27 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_schedule/location_schedule.js` (25 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_schedule/location_schedule.xml` (28 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_selector_dialog/location_selector_dialog.js` (187 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_selector_dialog/location_selector_dialog.scss` (83 lines)
- `addons/website_sale_stock/static/src/js/location_selector/location_selector_dialog/location_selector_dialog.xml` (129 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map/map-pin-indicator.xml` (20 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map/map.js` (145 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map/map.scss` (21 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map/map.xml` (10 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map_container/map_container.js` (89 lines)
- `addons/website_sale_stock/static/src/js/location_selector/map_container/map_container.xml` (86 lines)
- `addons/website_sale_stock/static/src/js/models/product_product.js` (23 lines)
- `addons/website_sale_stock/static/src/js/pickup_location_many2one/pickup_location_many2one.js` (119 lines)
- `addons/website_sale_stock/static/src/js/pickup_location_many2one/pickup_location_many2one.xml` (18 lines)
- `addons/website_sale_stock/static/src/js/product_card/product_card.js` (14 lines)
- `addons/website_sale_stock/static/src/js/product_card/product_card.xml` (61 lines)
- `addons/website_sale_stock/static/src/js/tours/combo_configurator_tour_utils.js` (26 lines)
- `addons/website_sale_stock/static/src/js/tours/website_sale_stock_reorder_from_portal.js` (26 lines)
- `addons/website_sale_stock/static/tests/tours/website_sale_stock_combo_configurator.js` (65 lines)
- `addons/website_sale_stock/static/tests/tours/website_sale_stock_message_after_close_configurator_modal.js` (40 lines)
- `addons/website_sale_stock/static/tests/tours/website_sale_stock_multilang.js` (48 lines)
- `addons/website_sale_stock/static/tests/tours/website_sale_stock_stock_notification.js` (29 lines)
- `addons/website_sale_stock/tests/__init__.py` (18 lines)
- `addons/website_sale_stock/tests/common.py` (47 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_abandoned_cart_email.py` (69 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_checkout.py` (47 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_configurators.py` (40 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_gmc.py` (54 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_location_selector.py` (63 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_multilang.py` (38 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_product_combo.py` (87 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_product_product.py` (35 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_product_template.py` (140 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_product_warehouse.py` (146 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_reorder_from_portal.py` (47 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_sale_order_line.py` (92 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_stock_message.py` (62 lines)
- `addons/website_sale_stock/tests/test_website_sale_stock_stock_notification.py` (103 lines)
- `addons/website_sale_stock/views/checkout_templates.xml` (28 lines)
- `addons/website_sale_stock/views/delivery_form.xml` (61 lines)
- `addons/website_sale_stock/views/res_config_settings_views.xml` (22 lines)
- `addons/website_sale_stock/views/sale_order_views.xml` (43 lines)
- `addons/website_sale_stock/views/stock_picking_views.xml` (41 lines)
- `addons/website_sale_stock/wizard/__init__.py` (1 lines)
- `addons/website_sale_stock/wizard/choose_delivery_carrier.py` (47 lines)
- `addons/website_sale_stock/wizard/choose_delivery_carrier_views.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
