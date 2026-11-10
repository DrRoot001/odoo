# Module: website_sale_loyalty

- **Module ID:** MOD-637
- **Path:** `addons/website_sale_loyalty`
- **Manifest:** `addons/website_sale_loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['website_sale', 'sale_loyalty']`
- **License:** `LGPL-3`

## Purpose and dependencies

Use coupon, promotion, gift cards and loyalty programs in your eCommerce store


Create coupons, promotion codes, gift cards and loyalty programs to boost your sales (free products,
discounts, etc.). Shoppers can use them in the eCommerce checkout.

Coupon & promotion programs can be edited in the Catalog menu of the Website app.
    

Declared dependencies: `website_sale`, `website_links`, `sale_loyalty`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 27 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 5 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 12 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 8 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale",
    "website_links",
    "sale_loyalty"
  ],
  "data": [
    "views/loyalty_card_views.xml",
    "views/loyalty_program_views.xml",
    "views/website_sale_templates.xml",
    "views/website_sale_loyalty_menus.xml",
    "wizard/coupon_share_views.xml",
    "wizard/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/product_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale_loyalty/static/src/js/**/*",
      "website_sale_loyalty/static/src/interactions/**/*"
    ],
    "web.assets_tests": [
      "website_sale_loyalty/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_loyalty/__init__.py` (3 lines)
- `addons/website_sale_loyalty/__manifest__.py` (34 lines)
- `addons/website_sale_loyalty/controllers/__init__.py` (3 lines)
- `addons/website_sale_loyalty/controllers/cart.py` (54 lines)
- `addons/website_sale_loyalty/controllers/delivery.py` (46 lines)
- `addons/website_sale_loyalty/controllers/main.py` (126 lines)
- `addons/website_sale_loyalty/controllers/portal.py` (26 lines)
- `addons/website_sale_loyalty/data/product_demo.xml` (23 lines)
- `addons/website_sale_loyalty/i18n/ar.po` (389 lines)
- `addons/website_sale_loyalty/i18n/az.po` (371 lines)
- `addons/website_sale_loyalty/i18n/bg.po` (371 lines)
- `addons/website_sale_loyalty/i18n/bs.po` (373 lines)
- `addons/website_sale_loyalty/i18n/ca.po` (389 lines)
- `addons/website_sale_loyalty/i18n/cs.po` (375 lines)
- `addons/website_sale_loyalty/i18n/da.po` (392 lines)
- `addons/website_sale_loyalty/i18n/de.po` (406 lines)
- `addons/website_sale_loyalty/i18n/el.po` (375 lines)
- `addons/website_sale_loyalty/i18n/es.po` (395 lines)
- `addons/website_sale_loyalty/i18n/es_419.po` (403 lines)
- `addons/website_sale_loyalty/i18n/et.po` (372 lines)
- `addons/website_sale_loyalty/i18n/fa.po` (371 lines)
- `addons/website_sale_loyalty/i18n/fi.po` (389 lines)
- `addons/website_sale_loyalty/i18n/fr.po` (394 lines)
- `addons/website_sale_loyalty/i18n/he.po` (372 lines)
- `addons/website_sale_loyalty/i18n/hi.po` (371 lines)
- `addons/website_sale_loyalty/i18n/hr.po` (372 lines)
- `addons/website_sale_loyalty/i18n/hu.po` (376 lines)
- `addons/website_sale_loyalty/i18n/id.po` (390 lines)
- `addons/website_sale_loyalty/i18n/it.po` (399 lines)
- `addons/website_sale_loyalty/i18n/ja.po` (391 lines)
- `addons/website_sale_loyalty/i18n/kab.po` (372 lines)
- `addons/website_sale_loyalty/i18n/ko.po` (388 lines)
- `addons/website_sale_loyalty/i18n/ku.po` (371 lines)
- `addons/website_sale_loyalty/i18n/lo.po` (383 lines)
- `addons/website_sale_loyalty/i18n/lt.po` (373 lines)
- `addons/website_sale_loyalty/i18n/lv.po` (372 lines)
- `addons/website_sale_loyalty/i18n/mn.po` (371 lines)
- `addons/website_sale_loyalty/i18n/my.po` (372 lines)
- `addons/website_sale_loyalty/i18n/nb.po` (375 lines)
- `addons/website_sale_loyalty/i18n/nl.po` (396 lines)
- `addons/website_sale_loyalty/i18n/pl.po` (385 lines)
- `addons/website_sale_loyalty/i18n/pt.po` (391 lines)
- `addons/website_sale_loyalty/i18n/pt_BR.po` (407 lines)
- `addons/website_sale_loyalty/i18n/ro.po` (378 lines)
- `addons/website_sale_loyalty/i18n/ru.po` (395 lines)
- `addons/website_sale_loyalty/i18n/sk.po` (371 lines)
- `addons/website_sale_loyalty/i18n/sl.po` (376 lines)
- `addons/website_sale_loyalty/i18n/sr@latin.po` (372 lines)
- `addons/website_sale_loyalty/i18n/sv.po` (381 lines)
- `addons/website_sale_loyalty/i18n/th.po` (377 lines)
- `addons/website_sale_loyalty/i18n/tr.po` (390 lines)
- `addons/website_sale_loyalty/i18n/uk.po` (372 lines)
- `addons/website_sale_loyalty/i18n/uz.po` (450 lines)
- `addons/website_sale_loyalty/i18n/vi.po` (386 lines)
- `addons/website_sale_loyalty/i18n/website_sale_loyalty.pot` (366 lines)
- `addons/website_sale_loyalty/i18n/zh_CN.po` (392 lines)
- `addons/website_sale_loyalty/i18n/zh_TW.po` (390 lines)
- `addons/website_sale_loyalty/models/__init__.py` (10 lines)
- `addons/website_sale_loyalty/models/loyalty_card.py` (11 lines)
- `addons/website_sale_loyalty/models/loyalty_program.py` (24 lines)
- `addons/website_sale_loyalty/models/loyalty_rule.py` (42 lines)
- `addons/website_sale_loyalty/models/product_product.py` (49 lines)
- `addons/website_sale_loyalty/models/sale_order.py` (443 lines)
- `addons/website_sale_loyalty/models/sale_order_line.py` (42 lines)
- `addons/website_sale_loyalty/security/ir.access.csv` (2 lines)
- `addons/website_sale_loyalty/static/description/icon.png` (39 lines)
- `addons/website_sale_loyalty/static/description/icon.svg` (1 lines)
- `addons/website_sale_loyalty/static/description/icon_hi.png` (97 lines)
- `addons/website_sale_loyalty/static/src/interactions/checkout.js` (33 lines)
- `addons/website_sale_loyalty/static/src/interactions/coupon_toaster.js` (34 lines)
- `addons/website_sale_loyalty/static/src/js/cart_notification/item_added_notification/item_added_notification.js` (18 lines)
- `addons/website_sale_loyalty/static/src/js/cart_notification/item_added_notification/item_added_notification.xml` (22 lines)
- `addons/website_sale_loyalty/static/src/js/portal_loyalty_card.xml` (56 lines)
- `addons/website_sale_loyalty/static/src/js/promotion_progress_bar/promotion_progress_bar.js` (16 lines)
- `addons/website_sale_loyalty/static/src/js/promotion_progress_bar/promotion_progress_bar.xml` (26 lines)
- `addons/website_sale_loyalty/static/tests/tours/delivery_with_gift_card.js` (18 lines)
- `addons/website_sale_loyalty/static/tests/tours/ewallet.js` (48 lines)
- `addons/website_sale_loyalty/static/tests/tours/gift_card.js` (29 lines)
- `addons/website_sale_loyalty/static/tests/tours/promotions.js` (104 lines)
- `addons/website_sale_loyalty/static/tests/tours/shipping_discount.js` (41 lines)
- `addons/website_sale_loyalty/static/tests/tours/test_apply_discount_code.js` (35 lines)
- `addons/website_sale_loyalty/static/tests/tours/test_website_sale_free_shipping_discount_line.js` (41 lines)
- `addons/website_sale_loyalty/static/tests/tours/tour_utils.js` (28 lines)
- `addons/website_sale_loyalty/tests/__init__.py` (14 lines)
- `addons/website_sale_loyalty/tests/test_apply_pending_coupon.py` (149 lines)
- `addons/website_sale_loyalty/tests/test_concurrent_promo_code.py` (138 lines)
- `addons/website_sale_loyalty/tests/test_ewallet.py` (84 lines)
- `addons/website_sale_loyalty/tests/test_free_product_reward.py` (168 lines)
- `addons/website_sale_loyalty/tests/test_sale_coupon_multiwebsite.py` (237 lines)
- `addons/website_sale_loyalty/tests/test_shop_loyalty_payment.py` (105 lines)
- `addons/website_sale_loyalty/tests/test_shop_multi_reward.py` (188 lines)
- `addons/website_sale_loyalty/tests/test_shop_sale_coupon.py` (612 lines)
- `addons/website_sale_loyalty/tests/test_website_sale_auto_invoice.py` (49 lines)
- `addons/website_sale_loyalty/tests/test_website_sale_loyalty_delivery.py` (284 lines)
- `addons/website_sale_loyalty/views/loyalty_card_views.xml` (13 lines)
- `addons/website_sale_loyalty/views/loyalty_program_views.xml` (50 lines)
- `addons/website_sale_loyalty/views/website_sale_loyalty_menus.xml` (17 lines)
- `addons/website_sale_loyalty/views/website_sale_templates.xml` (258 lines)
- `addons/website_sale_loyalty/wizard/__init__.py` (3 lines)
- `addons/website_sale_loyalty/wizard/coupon_share.py` (122 lines)
- `addons/website_sale_loyalty/wizard/coupon_share_views.xml` (32 lines)
- `addons/website_sale_loyalty/wizard/res_config_settings_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
