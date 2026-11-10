# Module: website_sale

- **Module ID:** MOD-634
- **Path:** `addons/website_sale`
- **Manifest:** `addons/website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Sell your products online

No manifest description declared.

Declared dependencies: `website`, `sale`, `website_payment`, `website_mail`, `portal_rating`, `digest`, `delivery`, `html_builder`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 123 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 42 | Files under `models/` or `models.py`. |
| Controller-path Python files | 17 | Files under `controllers/` or `controllers.py`. |
| XML files | 108 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 165 | Client behavior/assets. |
| Tests | 58 | Test files found by path/name convention. |
| Security artifacts | 3 | Access CSV and/or security XML. |
| Route declarations | 62 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "sale",
    "website_payment",
    "website_mail",
    "portal_rating",
    "digest",
    "delivery",
    "html_builder"
  ],
  "data": [
    "security/ir_access.xml",
    "security/res_groups.xml",
    "data/mail_template_data.xml",
    "data/data.xml",
    "data/digest_data.xml",
    "data/donation_data.xml",
    "data/ir_actions_server_data.xml",
    "data/ir_cron_data.xml",
    "data/product_attribute_data.xml",
    "data/product_ribbon_data.xml",
    "data/tour.xml",
    "data/website_checkout_step_data.xml",
    "data/website_snippet_filter_data.xml",
    "report/sale_report_views.xml",
    "templates/comparison_templates.xml",
    "templates/product_tile_templates.xml",
    "templates/gmc_templates.xml",
    "templates/product_page_templates.xml",
    "templates/sale_portal_templates.xml",
    "templates/shop_page_templates.xml",
    "templates/shop_empty_screens/shop_page_empty_screen.xml",
    "templates/shop_empty_screens/svg_templates.xml",
    "templates/website_templates.xml",
    "templates/wishlist_templates.xml",
    "templates/checkout/checkout_templates.xml",
    "templates/checkout/address_templates.xml",
    "templates/checkout/cart_templates.xml",
    "templates/checkout/confirmation_templates.xml",
    "templates/checkout/extra_info_templates.xml",
    "templates/checkout/payment_templates.xml",
    "views/account_move_views.xml",
    "views/delivery_carrier_views.xml",
    "views/digest_views.xml",
    "views/product_attribute_category_views.xml",
    "views/product_attribute_views.xml",
    "views/product_document_views.xml",
    "views/product_feed_views.xml",
    "views/product_image_views.xml",
    "views/product_pricelist_views.xml",
    "views/product_product_add.xml",
    "views/product_public_category_views.xml",
    "views/product_ribbon_views.xml",
    "views/product_views.xml",
    "views/res_config_settings_views.xml",
    "views/sale_order_views.xml",
    "views/website_sale_menus.xml",
    "views/website_sale_visitor_views.xml",
    "views/website_views.xml",
    "templates/snippets/snippets.xml",
    "templates/snippets/product_snippet_template_data.xml",
    "templates/snippets/s_add_to_cart.xml",
    "templates/snippets/s_donation.xml",
    "templates/snippets/s_dynamic_snippet_products.xml",
    "templates/snippets/s_dynamic_snippet_categories.xml",
    "templates/snippets/s_dynamic_snippet_products_preview_data.xml",
    "templates/snippets/s_dynamic_snippet_category_preview_data.xml",
    "templates/snippets/snippet_category_template_data.xml",
    "templates/generate_primary_template.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/demo.xml",
    "data/product_attribute_category_data.xml",
    "data/product_attribute_category_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale/static/src/interactions/**/*",
      "website_sale/static/src/snippets/**/*.js",
      "website_sale/static/src/js/tours/tour_utils.js",
      "website_sale/static/src/scss/product_tile.scss",
      "website_sale/static/src/scss/website_sale.scss",
      "website_sale/static/src/scss/website_sale_frontend.scss",
      "website_sale/static/src/scss/shop_page_empty_screen.scss",
      "website_sale/static/src/scss/website_sale_comparison.scss",
      "website_sale/static/src/scss/website_sale_comparison.options.scss",
      "website_sale/static/src/scss/website_sale_delivery.scss",
      "website_sale/static/src/scss/website_sale_wishlist.scss",
      "website_sale/static/src/scss/website_sale_wishlist.options.scss",
      "website_sale/static/src/snippets/s_dynamic_snippet_categories/000.scss",
      "website_sale/static/src/snippets/s_dynamic_snippet_categories/000.xml",
      "website_sale/static/src/snippets/s_dynamic_snippet_products/000.xml",
      "website/static/lib/multirange/multirange_custom.scss",
      "sale/static/src/scss/sale_portal.scss",
      "website_sale/static/src/scss/product_configurator.scss",
      "website_sale/static/src/js/cart_service.js",
      "website_sale/static/src/xml/website_sale.xml",
      "website_sale/static/src/js/website_sale_utils.js",
      "website_sale/static/src/js/wishlist_utils.js",
      "website_sale/static/src/js/comparison_utils.js",
      "website/static/lib/multirange/multirange_custom.js",
      "website/static/src/interactions/multirange_input.js",
      "website_sale/static/src/xml/website_sale_image_viewer.xml",
      "website_sale/static/src/xml/website_sale_product_availability.xml",
      "website_sale/static/src/js/components/alert_banner/*",
      "website_sale/static/src/js/components/website_sale_image_viewer.js",
      "website_sale/static/src/js/cart_notification/item_added_notification/item_added_notification.js",
      "website_sale/static/src/js/cart_notification/item_added_notification/item_added_notification.xml",
      "website_sale/static/src/js/cart_notification/cart_notification_container/cart_notification_container.js",
      "website_sale/static/src/js/cart_notification/cart_notification_container/cart_notification_container.xml",
      "website_sale/static/src/js/cart_notification/warning_notification/warning_notification.js",
      "website_sale/static/src/js/cart_notification/warning_notification/warning_notification.xml",
      "sale/static/src/js/badge_extra_price/*",
      "sale/static/src/js/combo_configurator_dialog/*",
      "sale/static/src/js/models/*",
      "sale/static/src/js/product/*",
      "sale/static/src/js/product_card/*",
      "sale/static/src/js/product_configurator_dialog/*",
      "sale/static/src/js/product_list/*",
      "sale/static/src/js/product_template_attribute_line/*",
      "sale/static/src/js/quantity_buttons/*",
      "sale/static/src/js/sale_utils.js",
      "website_sale/static/src/js/combo_configurator_dialog/*",
      "website_sale/static/src/js/product/*",
      "website_sale/static/src/js/product_configurator_dialog/*",
      "website_sale/static/src/js/product_list/*",
      "website_sale/static/src/js/product_template_attribute_line/*",
      "website_sale/static/src/js/quantity_buttons/*",
      "website_sale/static/src/js/product_row/*",
      "website_sale/static/src/js/product_comparison_bottom_bar/*"
    ],
    "web._assets_primary_variables": [
      "website_sale/static/src/scss/primary_variables.scss"
    ],
    "web.assets_backend": [
      "website_sale/static/src/js/client_actions/**/*",
      "website_sale/static/src/js/tours/tour_utils.js",
      "website_sale/static/src/js/website_sale_video_field_preview.js",
      "website_sale/static/src/scss/website_sale_backend.scss",
      "website_sale/static/src/js/tours/website_sale_shop.js",
      "website_sale/static/src/js/product_image/**/*",
      "website_sale/static/src/xml/website_sale.xml",
      "website_sale/static/src/scss/kanban_record.scss",
      "website_sale/static/src/js/dashboard/dashboard.js",
      "website_sale/static/src/views/**/*"
    ],
    "website.website_builder_assets": [
      "website_sale/static/src/website_builder/**/*",
      "website_sale/static/src/js/website_sale_utils.js",
      [
        "remove",
        "website_sale/static/src/**/*.edit.*"
      ]
    ],
    "website.assets_wysiwyg": [
      "website_sale/static/src/scss/website_sale.editor.scss",
      "website_sale/static/src/js/website_sale_form_editor.js"
    ],
    "website.assets_editor": [
      "website_sale/static/src/js/systray_items/*.js",
      "website_sale/static/src/xml/website_sale_editor_previews.xml"
    ],
    "website.assets_inside_builder_iframe": [
      "web/static/lib/bootstrap/scss/_variables.scss",
      "website_sale/static/src/website_builder/**/*.edit.*"
    ],
    "website.assets_inside_builder_iframe_tests": [
      "website_sale/static/src/website_builder/**/*.edit.xml"
    ],
    "web.assets_tests": [
      "website_sale/static/tests/tours/**/*",
      "website_sale/static/src/js/tours/product_configurator_tour_utils.js",
      "website_sale/static/src/js/tours/wishlist_tour_utils.js"
    ],
    "web.assets_unit_tests": [
      "website_sale/static/tests/interactions/**/*",
      "website_sale/static/tests/builder/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_sale/static/src/interactions/**/*",
      "website_sale/static/src/js/product_row/*",
      "website_sale/static/src/js/product_comparison_bottom_bar/*",
      "website_sale/static/src/snippets/s_dynamic_snippet_products/dynamic_snippet_products.js",
      "website_sale/static/src/snippets/s_dynamic_snippet_products/000.xml",
      "website_sale/static/src/js/comparison_utils.js",
      "website_sale/static/src/js/wishlist_utils.js",
      "website_sale/static/src/js/website_sale_utils.js",
      "website_sale/static/src/js/components/alert_banner/*",
      "website_sale/static/src/js/components/website_sale_image_viewer.js"
    ],
    "html_builder.iframe_add_dialog": [
      "website_sale/static/src/snippets/**/*.preview.scss"
    ]
  }
}
```

### Representative source files

- `addons/website_sale/README.md` (153 lines)
- `addons/website_sale/__init__.py` (51 lines)
- `addons/website_sale/__manifest__.py` (216 lines)
- `addons/website_sale/const.py` (413 lines)
- `addons/website_sale/controllers/__init__.py` (20 lines)
- `addons/website_sale/controllers/cart.py` (627 lines)
- `addons/website_sale/controllers/combo_configurator.py` (48 lines)
- `addons/website_sale/controllers/comparison.py` (48 lines)
- `addons/website_sale/controllers/delivery.py` (304 lines)
- `addons/website_sale/controllers/donation.py` (31 lines)
- `addons/website_sale/controllers/main.py` (2,173 lines)
- `addons/website_sale/controllers/payment.py` (97 lines)
- `addons/website_sale/controllers/portal.py` (19 lines)
- `addons/website_sale/controllers/product_configurator.py` (263 lines)
- `addons/website_sale/controllers/product_feed.py` (68 lines)
- `addons/website_sale/controllers/reorder.py` (82 lines)
- `addons/website_sale/controllers/sale.py` (40 lines)
- `addons/website_sale/controllers/thread.py` (11 lines)
- `addons/website_sale/controllers/variant.py` (134 lines)
- `addons/website_sale/controllers/website.py` (104 lines)
- `addons/website_sale/controllers/wishlist.py` (120 lines)
- `addons/website_sale/data/data.xml` (76 lines)
- `addons/website_sale/data/demo.xml` (1,294 lines)
- `addons/website_sale/data/digest_data.xml` (8 lines)
- `addons/website_sale/data/donation_data.xml` (21 lines)
- `addons/website_sale/data/ir_actions_server_data.xml` (17 lines)
- `addons/website_sale/data/ir_cron_data.xml` (41 lines)
- `addons/website_sale/data/mail_template_data.xml` (416 lines)
- `addons/website_sale/data/product_attribute_category_data.xml` (7 lines)
- `addons/website_sale/data/product_attribute_category_demo.xml` (82 lines)
- `addons/website_sale/data/product_attribute_data.xml` (23 lines)
- `addons/website_sale/data/product_ribbon_data.xml` (36 lines)
- `addons/website_sale/data/tour.xml` (8 lines)
- `addons/website_sale/data/website_checkout_step_data.xml` (49 lines)
- `addons/website_sale/data/website_snippet_filter_data.xml` (134 lines)
- `addons/website_sale/i18n/af.po` (8,279 lines)
- `addons/website_sale/i18n/ar.po` (9,338 lines)
- `addons/website_sale/i18n/az.po` (8,464 lines)
- `addons/website_sale/i18n/bg.po` (8,412 lines)
- `addons/website_sale/i18n/bs.po` (8,312 lines)
- `addons/website_sale/i18n/ca.po` (8,641 lines)
- `addons/website_sale/i18n/cs.po` (8,480 lines)
- `addons/website_sale/i18n/da.po` (8,498 lines)
- `addons/website_sale/i18n/de.po` (10,964 lines)
- `addons/website_sale/i18n/el.po` (8,361 lines)
- `addons/website_sale/i18n/es.po` (10,669 lines)
- `addons/website_sale/i18n/es_419.po` (10,863 lines)
- `addons/website_sale/i18n/es_CL.po` (367 lines)
- `addons/website_sale/i18n/et.po` (8,470 lines)
- `addons/website_sale/i18n/eu.po` (8,278 lines)
- `addons/website_sale/i18n/fa.po` (8,410 lines)
- `addons/website_sale/i18n/fi.po` (10,425 lines)
- `addons/website_sale/i18n/fr.po` (9,681 lines)
- `addons/website_sale/i18n/gl.po` (8,277 lines)
- `addons/website_sale/i18n/gu.po` (8,284 lines)
- `addons/website_sale/i18n/he.po` (8,378 lines)
- `addons/website_sale/i18n/hi.po` (8,325 lines)
- `addons/website_sale/i18n/hr.po` (8,489 lines)
- `addons/website_sale/i18n/hu.po` (8,368 lines)
- `addons/website_sale/i18n/id.po` (10,745 lines)
- `addons/website_sale/i18n/is.po` (8,281 lines)
- `addons/website_sale/i18n/it.po` (10,776 lines)
- `addons/website_sale/i18n/ja.po` (9,858 lines)
- `addons/website_sale/i18n/ka.po` (8,277 lines)
- `addons/website_sale/i18n/kab.po` (8,298 lines)
- `addons/website_sale/i18n/km.po` (8,280 lines)
- `addons/website_sale/i18n/ko.po` (9,425 lines)
- `addons/website_sale/i18n/ku.po` (8,314 lines)
- `addons/website_sale/i18n/lo.po` (9,779 lines)
- `addons/website_sale/i18n/lt.po` (8,376 lines)
- `addons/website_sale/i18n/lv.po` (8,316 lines)
- `addons/website_sale/i18n/mk.po` (8,286 lines)
- `addons/website_sale/i18n/mn.po` (9,926 lines)
- `addons/website_sale/i18n/my.po` (8,327 lines)
- `addons/website_sale/i18n/nb.po` (8,358 lines)
- `addons/website_sale/i18n/nl.po` (10,753 lines)
- `addons/website_sale/i18n/pl.po` (9,533 lines)
- `addons/website_sale/i18n/pt.po` (9,523 lines)
- `addons/website_sale/i18n/pt_BR.po` (10,911 lines)
- `addons/website_sale/i18n/ro.po` (8,610 lines)
- `addons/website_sale/i18n/ru.po` (10,199 lines)
- `addons/website_sale/i18n/sk.po` (8,334 lines)
- `addons/website_sale/i18n/sl.po` (8,380 lines)
- `addons/website_sale/i18n/sr@latin.po` (9,405 lines)
- `addons/website_sale/i18n/sv.po` (8,490 lines)
- `addons/website_sale/i18n/th.po` (10,355 lines)
- `addons/website_sale/i18n/tr.po` (9,352 lines)
- `addons/website_sale/i18n/uk.po` (8,397 lines)
- `addons/website_sale/i18n/uz.po` (9,456 lines)
- `addons/website_sale/i18n/vi.po` (8,718 lines)
- `addons/website_sale/i18n/website_sale.pot` (8,014 lines)
- `addons/website_sale/i18n/zh_CN.po` (10,695 lines)
- `addons/website_sale/i18n/zh_TW.po` (8,601 lines)
- `addons/website_sale/models/__init__.py` (47 lines)
- `addons/website_sale/models/account_move.py` (20 lines)
- `addons/website_sale/models/crm_team.py` (58 lines)
- `addons/website_sale/models/delivery_carrier.py` (78 lines)
- `addons/website_sale/models/digest.py` (30 lines)
- `addons/website_sale/models/ir_http.py` (35 lines)
- `addons/website_sale/models/ir_module_module.py` (62 lines)
- `addons/website_sale/models/payment_transaction.py` (55 lines)
- `addons/website_sale/models/product_attribute.py` (42 lines)
- `addons/website_sale/models/product_attribute_category.py` (19 lines)
- `addons/website_sale/models/product_combo.py` (25 lines)
- `addons/website_sale/models/product_document.py` (20 lines)
- `addons/website_sale/models/product_feed.py` (410 lines)
- `addons/website_sale/models/product_image.py` (95 lines)
- `addons/website_sale/models/product_pricelist.py` (129 lines)
- `addons/website_sale/models/product_pricelist_item.py` (21 lines)
- `addons/website_sale/models/product_product.py` (591 lines)
- `addons/website_sale/models/product_public_category.py` (245 lines)
- `addons/website_sale/models/product_ribbon.py` (140 lines)
- `addons/website_sale/models/product_stock_notification.py` (19 lines)
- `addons/website_sale/models/product_tag.py` (8 lines)
- `addons/website_sale/models/product_template.py` (2,065 lines)
- `addons/website_sale/models/product_template_attribute_line.py` (59 lines)
- `addons/website_sale/models/product_template_attribute_value.py` (50 lines)
- `addons/website_sale/models/product_wishlist.py` (96 lines)
- `addons/website_sale/models/res_company.py` (28 lines)
- `addons/website_sale/models/res_config_settings.py` (183 lines)
- `addons/website_sale/models/res_groups.py` (14 lines)
- `addons/website_sale/models/res_partner.py` (98 lines)
- `addons/website_sale/models/res_users.py` (13 lines)
- `addons/website_sale/models/sale_order.py` (1,569 lines)
- `addons/website_sale/models/sale_order_line.py` (265 lines)
- `addons/website_sale/models/theme_utils.py` (28 lines)
- `addons/website_sale/models/website.py` (1,294 lines)
- `addons/website_sale/models/website_checkout_alert_mixin.py` (59 lines)
- `addons/website_sale/models/website_checkout_step.py` (178 lines)
- `addons/website_sale/models/website_menu.py` (15 lines)
- `addons/website_sale/models/website_sale_extra_field.py` (20 lines)
- `addons/website_sale/models/website_snippet_filter.py` (391 lines)
- `addons/website_sale/models/website_track.py` (11 lines)
- `addons/website_sale/models/website_visitor.py` (34 lines)
- `addons/website_sale/models/withdrawal_request.py` (146 lines)
- `addons/website_sale/report/__init__.py` (1 lines)
- `addons/website_sale/report/sale_report.py` (33 lines)
- `addons/website_sale/report/sale_report_views.xml` (130 lines)
- `addons/website_sale/security/ir.access.csv` (39 lines)
- `addons/website_sale/security/ir_access.xml` (17 lines)
- `addons/website_sale/security/res_groups.xml` (34 lines)
- `addons/website_sale/static/description/icon.png` (24 lines)
- `addons/website_sale/static/description/icon.svg` (1 lines)
- `addons/website_sale/static/description/icon_hi.png` (65 lines)
- `addons/website_sale/static/shapes/s_donation_gift.svg` (87 lines)
- `addons/website_sale/static/src/img/categories/bins.jpg` (342 lines)
- `addons/website_sale/static/src/img/categories/boxes.jpg` (240 lines)
- `addons/website_sale/static/src/img/categories/cabinets.jpg` (128 lines)
- `addons/website_sale/static/src/img/categories/desk_components.jpg` (272 lines)
- `addons/website_sale/static/src/img/categories/desks.jpg` (193 lines)
- `addons/website_sale/static/src/img/categories/drawers.jpg` (199 lines)
- `addons/website_sale/static/src/img/categories/furnitures.jpg` (172 lines)
- `addons/website_sale/static/src/img/categories/lamps.jpg` (237 lines)
- `addons/website_sale/static/src/img/categories/placeholder_thumbnail.png` (23 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_1.png` (83 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_2.png` (35 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_3.png` (7 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_4.png` (92 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_5.png` (6 lines)
- `addons/website_sale/static/src/img/categories/shape_mixed_6.png` (87 lines)

Additional files not expanded here: 407. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
