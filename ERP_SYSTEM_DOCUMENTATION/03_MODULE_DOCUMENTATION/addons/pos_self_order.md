# Module: pos_self_order

- **Module ID:** MOD-455
- **Path:** `addons/pos_self_order`
- **Manifest:** `addons/pos_self_order/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['pos_restaurant']`
- **License:** `LGPL-3`

## Purpose and dependencies

Addon for the POS App that allows customers to view the menu on their smartphone.

No manifest description declared.

Declared dependencies: `pos_restaurant`, `http_routing`, `link_tracker`, `google_address_autocomplete`, `base_geolocalize`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 51 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 23 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 59 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 146 | Client behavior/assets. |
| Tests | 20 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 18 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_restaurant",
    "http_routing",
    "link_tracker",
    "google_address_autocomplete",
    "base_geolocalize"
  ],
  "data": [
    "data/mail_template_data.xml",
    "data/preset_data.xml",
    "views/pos_self_order.index.xml",
    "views/qr_code.xml",
    "views/pos_category_views.xml",
    "views/pos_config_view.xml",
    "views/custom_link_views.xml",
    "views/pos_restaurant_views.xml",
    "views/product_views.xml",
    "views/pos_preset_view.xml",
    "data/init_access.xml",
    "views/res_config_settings_views.xml",
    "views/point_of_sale_dashboard.xml",
    "receipt/pos_order_receipt.xml",
    "receipt/pos_order_change_receipt.xml",
    "receipt/dynamic_qr_receipt.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/kiosk_demo_data.xml"
  ],
  "assets": {
    "web.assets_unit_tests_setup": [
      [
        "include",
        "pos_self_order.assets"
      ],
      [
        "remove",
        "pos_self_order/static/src/app/root.js"
      ],
      [
        "remove",
        "pos_self_order/static/src/backend/pos_open_ui_button/pos_open_ui_button.js"
      ],
      [
        "remove",
        "pos_self_order/static/src/**/*.scss"
      ],
      "web/static/src/core/debug/**/*",
      "web/static/src/core/browser/router.js"
    ],
    "web.assets_unit_tests": [
      "pos_self_order/static/tests/unit/**/*"
    ],
    "point_of_sale._assets_pos": [
      "pos_self_order/static/src/app/models/utils/snooze_tracker.js",
      "pos_self_order/static/src/backend/qr_order_button/*",
      "pos_self_order/static/src/overrides/**/*"
    ],
    "web.assets_backend": [
      "pos_self_order/static/src/upgrade_selection_field.js",
      "pos_self_order/static/src/backend/qr_order_button/*",
      "pos_self_order/static/src/backend/pos_open_ui_button/pos_open_ui_button.js"
    ],
    "pos_self_order.assets": [
      "pos_self_order/static/src/app/primary_variables.scss",
      "pos_self_order/static/src/app/bootstrap_overridden.scss",
      [
        "include",
        "point_of_sale.base_app"
      ],
      "google_address_autocomplete/static/src/google_places_session.js",
      "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.js",
      "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.xml",
      "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.scss",
      "web/static/src/core/autocomplete/*",
      "web/static/src/views/fields/char/*",
      "web/static/src/views/fields/translation/*",
      "web/static/src/views/fields/dynamic_placeholder_hook.js",
      "web/static/src/views/fields/dynamic_placeholder_popover.*",
      "web/static/src/views/fields/formatters.js",
      "web/static/src/views/fields/standard_field_props.js",
      "web/static/src/views/fields/input_field_hook.js",
      "web/static/src/core/model_field_selector/model_field_selector_popover.js",
      "web/static/src/core/model_field_selector/model_field_selector_popover.xml",
      "web/static/src/core/model_field_selector/model_field_selector_popover.scss",
      "web/static/src/core/currency.js",
      "barcodes/static/src/barcode_plugin.js",
      "point_of_sale/static/src/utils.js",
      "point_of_sale/static/src/app/utils/convert_python_template.js",
      "point_of_sale/static/src/lazy_getter.js",
      "point_of_sale/static/src/app/utils/init_lna.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/src/libs/bootstrap.js",
      "html_editor/static/src/scss/base_style.scss",
      "html_editor/static/src/scss/html_editor.common.scss",
      "point_of_sale/static/src/app/utils/make_awaitable_dialog.js",
      "point_of_sale/static/src/app/components/numpad/*",
      "point_of_sale/static/src/app/components/loader/*",
      "point_of_sale/static/src/app/components/loader/critical_pos_error/*",
      "point_of_sale/static/src/app/components/product_card/*",
      "point_of_sale/static/src/app/components/order_display/*",
      "point_of_sale/static/src/app/components/orderline/*",
      "point_of_sale/static/src/app/components/centered_icon/*",
      "point_of_sale/static/src/app/components/validation_animation/*",
      "point_of_sale/static/src/app/components/epos_templates.xml",
      "point_of_sale/static/src/css/pos_receipts.css",
      "pos_self_order/static/src/overrides/utils/printer/generate_printer_data.js",
      "point_of_sale/static/src/app/utils/printer/*",
      "point_of_sale/static/src/app/utils/html-to-image.js",
      "point_of_sale/static/src/app/utils/use_timed_press.js",
      "point_of_sale/static/src/app/components/popups/select_default_printer_popup/select_default_printer_popup.js",
      "point_of_sale/static/src/app/plugins/pos_number_buffer_plugin.js",
      "mail/static/src/core/common/sound_effects_plugin.js",
      "point_of_sale/static/src/app/plugins/pos_ticket_printer_plugin.js",
      "point_of_sale/static/src/app/components/popups/retry_print_popup/**",
      "point_of_sale/static/src/app/components/popups/text_input_popup/**",
      "pos_self_order/static/src/app/**/*",
      "web/static/src/core/utils/render.js",
      "account/static/src/helpers/*.js",
      "web/static/src/model/**/*",
      "web/static/src/search/**/*",
      "web/static/src/views/fields/parsers.js",
      "point_of_sale/static/src/app/models/data_service_options.js",
      "point_of_sale/static/src/app/models/utils/indexed_db.js",
      "point_of_sale/static/src/app/models/related_models/**/*",
      "point_of_sale/static/src/app/plugins/pos_data_plugin.js",
      "point_of_sale/static/src/app/models/**/*",
      "pos_restaurant/static/src/app/models/restaurant_table.js",
      "point_of_sale/static/src/app/utils/numbers.js",
      "point_of_sale/static/src/app/utils/pretty_console_log.js",
      "point_of_sale/static/src/app/utils/devices_identifier_sequence.js",
      "point_of_sale/static/src/app/hooks/hooks.js",
      "point_of_sale/static/src/app/utils/debug-formatter.js",
      [
        "include",
        "point_of_sale.payment_terminals"
      ]
    ],
    "pos_self_order.assets_tests": [
      [
        "include",
        "point_of_sale.base_tests"
      ],
      "pos_self_order/static/tests/tours/**/*",
      "point_of_sale/static/tests/generic_helpers/numpad_util.js",
      "point_of_sale/static/tests/generic_helpers/dialog_util.js",
      "point_of_sale/static/tests/generic_helpers/notification_util.js",
      "point_of_sale/static/tests/generic_helpers/utils.js",
      "point_of_sale/static/tests/pos/tours/utils/chrome_util.js"
    ],
    "web.assets_tests": [
      "pos_self_order/static/tests/pos/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order/__init__.py` (3 lines)
- `addons/pos_self_order/__manifest__.py` (157 lines)
- `addons/pos_self_order/controllers/__init__.py` (5 lines)
- `addons/pos_self_order/controllers/orders.py` (459 lines)
- `addons/pos_self_order/controllers/self_entry.py` (83 lines)
- `addons/pos_self_order/controllers/webmanifest.py` (38 lines)
- `addons/pos_self_order/data/init_access.xml` (6 lines)
- `addons/pos_self_order/data/kiosk_demo_data.xml` (6 lines)
- `addons/pos_self_order/data/mail_template_data.xml` (78 lines)
- `addons/pos_self_order/data/preset_data.xml` (27 lines)
- `addons/pos_self_order/i18n/ar.po` (2,287 lines)
- `addons/pos_self_order/i18n/az.po` (2,258 lines)
- `addons/pos_self_order/i18n/bg.po` (2,258 lines)
- `addons/pos_self_order/i18n/bs.po` (2,258 lines)
- `addons/pos_self_order/i18n/ca.po` (2,445 lines)
- `addons/pos_self_order/i18n/cs.po` (2,262 lines)
- `addons/pos_self_order/i18n/da.po` (2,285 lines)
- `addons/pos_self_order/i18n/de.po` (2,492 lines)
- `addons/pos_self_order/i18n/el.po` (2,259 lines)
- `addons/pos_self_order/i18n/es.po` (2,479 lines)
- `addons/pos_self_order/i18n/es_419.po` (2,465 lines)
- `addons/pos_self_order/i18n/et.po` (2,260 lines)
- `addons/pos_self_order/i18n/fa.po` (2,258 lines)
- `addons/pos_self_order/i18n/fi.po` (2,289 lines)
- `addons/pos_self_order/i18n/fr.po` (2,327 lines)
- `addons/pos_self_order/i18n/he.po` (2,259 lines)
- `addons/pos_self_order/i18n/hi.po` (2,257 lines)
- `addons/pos_self_order/i18n/hr.po` (2,259 lines)
- `addons/pos_self_order/i18n/hu.po` (2,259 lines)
- `addons/pos_self_order/i18n/id.po` (2,471 lines)
- `addons/pos_self_order/i18n/it.po` (2,315 lines)
- `addons/pos_self_order/i18n/ja.po` (2,300 lines)
- `addons/pos_self_order/i18n/kab.po` (2,257 lines)
- `addons/pos_self_order/i18n/ko.po` (2,283 lines)
- `addons/pos_self_order/i18n/ku.po` (2,257 lines)
- `addons/pos_self_order/i18n/lo.po` (2,436 lines)
- `addons/pos_self_order/i18n/lt.po` (2,261 lines)
- `addons/pos_self_order/i18n/lv.po` (2,257 lines)
- `addons/pos_self_order/i18n/mn.po` (2,258 lines)
- `addons/pos_self_order/i18n/my.po` (2,258 lines)
- `addons/pos_self_order/i18n/nb.po` (2,259 lines)
- `addons/pos_self_order/i18n/nl.po` (2,487 lines)
- `addons/pos_self_order/i18n/pl.po` (2,484 lines)
- `addons/pos_self_order/i18n/pos_self_order.pot` (2,221 lines)
- `addons/pos_self_order/i18n/pt.po` (2,439 lines)
- `addons/pos_self_order/i18n/pt_BR.po` (2,478 lines)
- `addons/pos_self_order/i18n/ro.po` (2,286 lines)
- `addons/pos_self_order/i18n/ru.po` (2,360 lines)
- `addons/pos_self_order/i18n/sk.po` (2,256 lines)
- `addons/pos_self_order/i18n/sl.po` (2,260 lines)
- `addons/pos_self_order/i18n/sr@latin.po` (2,259 lines)
- `addons/pos_self_order/i18n/sv.po` (2,283 lines)
- `addons/pos_self_order/i18n/th.po` (2,276 lines)
- `addons/pos_self_order/i18n/tr.po` (2,299 lines)
- `addons/pos_self_order/i18n/uk.po` (2,288 lines)
- `addons/pos_self_order/i18n/uz.po` (2,512 lines)
- `addons/pos_self_order/i18n/vi.po` (2,281 lines)
- `addons/pos_self_order/i18n/zh_CN.po` (2,435 lines)
- `addons/pos_self_order/i18n/zh_TW.po` (2,277 lines)
- `addons/pos_self_order/models/__init__.py` (24 lines)
- `addons/pos_self_order/models/ir_http.py` (48 lines)
- `addons/pos_self_order/models/ir_ui_view.py` (23 lines)
- `addons/pos_self_order/models/mail_template.py` (16 lines)
- `addons/pos_self_order/models/pos_category.py` (13 lines)
- `addons/pos_self_order/models/pos_config.py` (554 lines)
- `addons/pos_self_order/models/pos_load_mixin.py` (70 lines)
- `addons/pos_self_order/models/pos_order.py` (623 lines)
- `addons/pos_self_order/models/pos_order_line.py` (27 lines)
- `addons/pos_self_order/models/pos_payment_method.py` (21 lines)
- `addons/pos_self_order/models/pos_prep_line.py` (9 lines)
- `addons/pos_self_order/models/pos_prep_order.py` (9 lines)
- `addons/pos_self_order/models/pos_preset.py` (187 lines)
- `addons/pos_self_order/models/pos_restaurant.py` (47 lines)
- `addons/pos_self_order/models/pos_self_order_custom_link.py` (53 lines)
- `addons/pos_self_order/models/pos_session.py` (52 lines)
- `addons/pos_self_order/models/pos_snooze.py` (18 lines)
- `addons/pos_self_order/models/product_product.py` (33 lines)
- `addons/pos_self_order/models/product_tag.py` (15 lines)
- `addons/pos_self_order/models/product_template.py` (104 lines)
- `addons/pos_self_order/models/res_config_settings.py` (226 lines)
- `addons/pos_self_order/models/res_country.py` (11 lines)
- `addons/pos_self_order/models/res_partner.py` (17 lines)
- `addons/pos_self_order/receipt/__init__.py` (1 lines)
- `addons/pos_self_order/receipt/dynamic_qr_receipt.xml` (44 lines)
- `addons/pos_self_order/receipt/pos_order_change_receipt.xml` (11 lines)
- `addons/pos_self_order/receipt/pos_order_receipt.py` (36 lines)
- `addons/pos_self_order/receipt/pos_order_receipt.xml` (22 lines)
- `addons/pos_self_order/security/ir.access.csv` (3 lines)
- `addons/pos_self_order/static/img/delivery.jpg` (301 lines)
- `addons/pos_self_order/static/img/dine_in.jpg` (367 lines)
- `addons/pos_self_order/static/img/eatin.svg` (1 lines)
- `addons/pos_self_order/static/img/kiosk_background.jpg` (321 lines)
- `addons/pos_self_order/static/img/landing_01.jpg` (486 lines)
- `addons/pos_self_order/static/img/landing_02.jpg` (800 lines)
- `addons/pos_self_order/static/img/landing_03.jpg` (760 lines)
- `addons/pos_self_order/static/img/takeAway.svg` (1 lines)
- `addons/pos_self_order/static/img/take_out.jpg` (467 lines)
- `addons/pos_self_order/static/src/app/bootstrap_overridden.scss` (31 lines)
- `addons/pos_self_order/static/src/app/components/attribute_selection/attribute_selection.js` (119 lines)
- `addons/pos_self_order/static/src/app/components/attribute_selection/attribute_selection.scss` (10 lines)
- `addons/pos_self_order/static/src/app/components/attribute_selection/attribute_selection.xml` (40 lines)
- `addons/pos_self_order/static/src/app/components/attribute_selection/attribute_selection_helper.js` (74 lines)
- `addons/pos_self_order/static/src/app/components/cancel_popup/cancel_popup.js` (20 lines)
- `addons/pos_self_order/static/src/app/components/cancel_popup/cancel_popup.xml` (25 lines)
- `addons/pos_self_order/static/src/app/components/category_list_popup/category_list_popup.js` (23 lines)
- `addons/pos_self_order/static/src/app/components/category_list_popup/category_list_popup.xml` (32 lines)
- `addons/pos_self_order/static/src/app/components/choose_combo_popup/choose_combo_popup.js` (69 lines)
- `addons/pos_self_order/static/src/app/components/choose_combo_popup/choose_combo_popup.xml` (102 lines)
- `addons/pos_self_order/static/src/app/components/combo_stepper/combo_stepper.js` (40 lines)
- `addons/pos_self_order/static/src/app/components/combo_stepper/combo_stepper.scss` (43 lines)
- `addons/pos_self_order/static/src/app/components/combo_stepper/combo_stepper.xml` (15 lines)
- `addons/pos_self_order/static/src/app/components/info_popup/info_popup.js` (10 lines)
- `addons/pos_self_order/static/src/app/components/info_popup/info_popup.xml` (30 lines)
- `addons/pos_self_order/static/src/app/components/language_popup/language_popup.js` (42 lines)
- `addons/pos_self_order/static/src/app/components/language_popup/language_popup.scss` (16 lines)
- `addons/pos_self_order/static/src/app/components/language_popup/language_popup.xml` (26 lines)
- `addons/pos_self_order/static/src/app/components/language_selector/language_selector.js` (26 lines)
- `addons/pos_self_order/static/src/app/components/language_selector/language_selector.scss` (3 lines)
- `addons/pos_self_order/static/src/app/components/language_selector/language_selector.xml` (10 lines)
- `addons/pos_self_order/static/src/app/components/loading_overlay/loading_overlay.js` (17 lines)
- `addons/pos_self_order/static/src/app/components/loading_overlay/loading_overlay.xml` (8 lines)
- `addons/pos_self_order/static/src/app/components/missing_required_details/missing_required_details.scss` (12 lines)
- `addons/pos_self_order/static/src/app/components/missing_required_details/missing_required_details.xml` (12 lines)
- `addons/pos_self_order/static/src/app/components/network_connectionLost_popup/network_connectionLost_popup.js` (83 lines)
- `addons/pos_self_order/static/src/app/components/network_connectionLost_popup/network_connectionLost_popup.xml` (47 lines)
- `addons/pos_self_order/static/src/app/components/number_popup/number_popup.js` (61 lines)
- `addons/pos_self_order/static/src/app/components/number_popup/number_popup.scss` (19 lines)
- `addons/pos_self_order/static/src/app/components/number_popup/number_popup.xml` (29 lines)
- `addons/pos_self_order/static/src/app/components/order_widget/order_widget.js` (8 lines)
- `addons/pos_self_order/static/src/app/components/order_widget/order_widget.xml` (18 lines)
- `addons/pos_self_order/static/src/app/components/pills_selection_popup/pills_selection_popup.js` (99 lines)
- `addons/pos_self_order/static/src/app/components/pills_selection_popup/pills_selection_popup.scss` (62 lines)
- `addons/pos_self_order/static/src/app/components/pills_selection_popup/pills_selection_popup.xml` (64 lines)
- `addons/pos_self_order/static/src/app/components/preset_info_popup/preset_info_popup.js` (401 lines)
- `addons/pos_self_order/static/src/app/components/preset_info_popup/preset_info_popup.scss` (37 lines)
- `addons/pos_self_order/static/src/app/components/preset_info_popup/preset_info_popup.xml` (104 lines)
- `addons/pos_self_order/static/src/app/components/printing_failure_popup/printing_failure_popup.js` (22 lines)
- `addons/pos_self_order/static/src/app/components/printing_failure_popup/printing_failure_popup.xml` (24 lines)
- `addons/pos_self_order/static/src/app/components/product_card/product_card.js` (98 lines)
- `addons/pos_self_order/static/src/app/components/product_card/product_card.scss` (23 lines)
- `addons/pos_self_order/static/src/app/components/product_card/product_card.xml` (35 lines)
- `addons/pos_self_order/static/src/app/components/product_info_popup/product_info_popup.js` (21 lines)
- `addons/pos_self_order/static/src/app/components/product_info_popup/product_info_popup.xml` (45 lines)
- `addons/pos_self_order/static/src/app/components/product_interface/product_interface.js` (26 lines)
- `addons/pos_self_order/static/src/app/components/product_interface/product_interface.scss` (29 lines)
- `addons/pos_self_order/static/src/app/components/product_interface/product_interface.xml` (45 lines)
- `addons/pos_self_order/static/src/app/components/quantity_widget/quantity_widget.xml` (18 lines)
- `addons/pos_self_order/static/src/app/components/slots_popup/slots_popup.xml` (36 lines)
- `addons/pos_self_order/static/src/app/components/timeout_popup/timeout_popup.js` (25 lines)
- `addons/pos_self_order/static/src/app/components/timeout_popup/timeout_popup.xml` (28 lines)
- `addons/pos_self_order/static/src/app/components/unavailable_product_dialog/unavailable_product_dialog.js` (17 lines)
- `addons/pos_self_order/static/src/app/components/unavailable_product_dialog/unavailable_product_dialog.xml` (24 lines)
- `addons/pos_self_order/static/src/app/data_service_options.js` (25 lines)
- `addons/pos_self_order/static/src/app/kiosk_style.js` (121 lines)
- `addons/pos_self_order/static/src/app/models/pos_config.js` (15 lines)
- `addons/pos_self_order/static/src/app/models/pos_order.js` (81 lines)
- `addons/pos_self_order/static/src/app/models/pos_order_line.js` (63 lines)
- `addons/pos_self_order/static/src/app/models/pos_preset.js` (35 lines)
- `addons/pos_self_order/static/src/app/models/product_template.js` (38 lines)
- `addons/pos_self_order/static/src/app/models/restaurant_floor.js` (12 lines)

Additional files not expanded here: 177. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
