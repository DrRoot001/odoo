# Module: point_of_sale

- **Module ID:** MOD-417
- **Path:** `addons/point_of_sale`
- **Manifest:** `addons/point_of_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Handle checkouts and payments for shops and restaurants.

No manifest description declared.

Declared dependencies: `resource`, `product`, `account`, `barcodes_gs1_nomenclature`, `html_editor`, `digest`, `phone_validation`, `google_address_autocomplete`, `base_report_wkhtmltox`, `iot_webserial`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 103 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 55 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 147 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 391 | Client behavior/assets. |
| Tests | 29 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 11 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "resource",
    "product",
    "account",
    "barcodes_gs1_nomenclature",
    "html_editor",
    "digest",
    "phone_validation",
    "google_address_autocomplete",
    "base_report_wkhtmltox",
    "iot_webserial"
  ],
  "data": [
    "security/point_of_sale_security.xml",
    "data/default_barcode_patterns.xml",
    "data/digest_data.xml",
    "data/pos_note_data.xml",
    "data/point_of_sale_tour.xml",
    "data/mail_template_data.xml",
    "data/ir_config_parameter_data.xml",
    "wizard/pos_details.xml",
    "wizard/pos_payment.xml",
    "wizard/pos_daily_sales_reports.xml",
    "wizard/pos_confirmation_wizard.xml",
    "wizard/pos_make_invoice.xml",
    "wizard/pos_price_inclusion_wizard.xml",
    "views/pos_assets_index.xml",
    "views/point_of_sale_report.xml",
    "views/point_of_sale_view.xml",
    "views/pos_note_view.xml",
    "views/pos_order_view.xml",
    "views/pos_category_view.xml",
    "views/product_combo_views.xml",
    "views/product_pricelist_view.xml",
    "views/product_view.xml",
    "views/account_journal_view.xml",
    "views/pos_payment_method_views.xml",
    "views/pos_payment_views.xml",
    "views/pos_config_view.xml",
    "views/pos_bill_view.xml",
    "views/pos_session_view.xml",
    "views/point_of_sale_sequence.xml",
    "data/point_of_sale_data.xml",
    "views/pos_order_report_view.xml",
    "views/digest_views.xml",
    "views/res_partner_view.xml",
    "views/report_userlabel.xml",
    "views/report_saledetails.xml",
    "views/pos_preset_view.xml",
    "views/point_of_sale_dashboard.xml",
    "views/report_invoice.xml",
    "views/pos_printer_view.xml",
    "views/pos_ticket_view.xml",
    "views/res_config_settings_views.xml",
    "views/customer_display_index.xml",
    "views/account_move_views.xml",
    "views/pos_session_sales_details.xml",
    "views/product_tag_views.xml",
    "receipt/pos_receipt_common.xml",
    "receipt/pos_order_receipt.xml",
    "receipt/pos_order_change_receipt.xml",
    "receipt/pos_order_change_receipt_zpl.xml",
    "receipt/pos_tip_receipt.xml",
    "receipt/pos_cash_move_receipt.xml",
    "receipt/pos_sale_details_receipt.xml",
    "data/ir_cron_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/demo_data.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "point_of_sale/static/src/scss/pos_dashboard.scss",
      "point_of_sale/static/src/backend/tours/point_of_sale.js",
      "point_of_sale/static/src/backend/pos_kanban_view/*",
      "point_of_sale/static/src/backend/lna_checklist/*",
      "point_of_sale/static/src/backend/pos_payment_provider_cards/*",
      "point_of_sale/static/src/app/hooks/hooks.js",
      "point_of_sale/static/src/backend/many2many_placeholder_list_view/*",
      "point_of_sale/static/src/backend/views/**/*",
      [
        "remove",
        "point_of_sale/static/src/backend/views/pivot/*"
      ],
      [
        "remove",
        "point_of_sale/static/src/backend/views/graph/*"
      ],
      "point_of_sale/static/src/backend/test_epos/*",
      "point_of_sale/static/src/app/utils/init_lna.js",
      "point_of_sale/static/src/backend/pos_open_ui_button/*"
    ],
    "web.assets_backend_lazy": [
      "point_of_sale/static/src/backend/views/pivot/*",
      "point_of_sale/static/src/backend/views/graph/*"
    ],
    "web.assets_web_dark": [
      "point_of_sale/static/src/scss/pos_dashboard.dark.scss",
      "point_of_sale/static/src/backend/pos_kanban_view/pos_kanban_view.dark.scss"
    ],
    "web.assets_tests": [
      "point_of_sale/static/tests/pos/tours/**/*",
      "point_of_sale/static/tests/generic_helpers/**/*",
      "point_of_sale/static/src/utils.js"
    ],
    "web.assets_unit_tests_setup": [
      [
        "include",
        "point_of_sale.assets_prod"
      ],
      [
        "remove",
        "point_of_sale/static/src/app/main.js"
      ],
      [
        "remove",
        "point_of_sale/static/src/**/*.css"
      ],
      "web/static/src/core/errors/error_handlers.js",
      "web/static/src/core/dialog/dialog.scss",
      "point_of_sale/static/src/backend/views/**/*",
      "point_of_sale/static/src/customer_display/**/*",
      [
        "remove",
        "point_of_sale/static/src/customer_display/root.js"
      ],
      [
        "remove",
        "point_of_sale/static/src/customer_display/styles.scss"
      ]
    ],
    "web.assets_unit_tests": [
      "point_of_sale/static/tests/unit/**/*"
    ],
    "point_of_sale.base_app": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      [
        "include",
        "web._assets_core"
      ],
      "point_of_sale/static/src/app/plugins/offline_plugin.js",
      [
        "remove",
        "web/static/src/core/debug/**/*"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/views/fields/formatters.js",
      "point_of_sale/static/src/utils.js",
      "bus/static/src/services/bus_plugin.js",
      "bus/static/src/services/worker_plugin.js",
      "bus/static/src/bus_parameters_plugin.js",
      "bus/static/src/multi_tab_plugin.js",
      "bus/static/src/multi_tab_shared_worker_plugin.js",
      "bus/static/src/multi_tab_fallback_plugin.js",
      "bus/static/src/workers/*"
    ],
    "point_of_sale.payment_terminals": [
      "point_of_sale/static/src/app/utils/payment/payment_interface.js"
    ],
    "point_of_sale._assets_pos": [
      "web/static/src/scss/functions.scss",
      "web/static/src/module_loader.js",
      "point_of_sale/static/lib/**/*",
      "web/static/lib/luxon/luxon.js",
      "web/static/src/libs/luxon.js",
      "web/static/lib/owl/owl.js",
      "web/static/src/owl2/owl3_compatibility_layer.js",
      "web/static/src/owl2/utils.js",
      "web/static/lib/owl/odoo_module.js",
      "web/static/lib/zxing-library/zxing-library.js",
      [
        "include",
        "point_of_sale.base_app"
      ],
      "web/static/src/core/colorlist/colorlist.scss",
      "web/static/src/webclient/webclient_layout.scss",
      "web/static/src/webclient/icons.scss",
      "point_of_sale/static/src/scss/pos_variables_extra.scss",
      "web/static/src/scss/bootstrap_overridden.scss",
      "web/static/fonts/fonts.scss",
      "web/static/src/scss/ui.scss",
      [
        "remove",
        "web/static/src/core/errors/error_handlers.js"
      ],
      [
        "remove",
        "/web/static/src/core/dialog/dialog.scss"
      ],
      "web/static/src/core/currency.js",
      "barcodes/static/src/barcode_plugin.js",
      "barcodes/static/src/js/barcode_parser.js",
      "barcodes_gs1_nomenclature/static/src/js/barcode_parser.js",
      "barcodes_gs1_nomenclature/static/src/js/barcode_plugin.js",
      "barcodes_gs1_nomenclature/static/src/js/epc_model.js",
      "barcodes_gs1_nomenclature/static/src/js/epc_utils.js",
      "web/static/src/webclient/actions/reports/utils.js",
      "point_of_sale/static/src/**/*",
      [
        "remove",
        "point_of_sale/static/src/backend/**/*"
      ],
      [
        "remove",
        "point_of_sale/static/src/customer_display/**/*"
      ],
      [
        "include",
        "point_of_sale.payment_terminals"
      ],
      [
        "remove",
        "point_of_sale/static/src/app/main.js"
      ],
      [
        "include",
        "point_of_sale.base_tests"
      ],
      "account/static/src/helpers/*.js",
      "account/static/src/services/account_move_service.js",
      "mail/static/src/core/common/sound_effects_plugin.js",
      "web/static/src/core/browser/router.js",
      "web/static/src/core/debug/**/*",
      "web/static/src/model/**/*",
      "web/static/src/views/**/*",
      "web/static/src/search/**/*",
      "web/static/src/webclient/actions/**/*",
      [
        "remove",
        "web/static/src/webclient/actions/reports/report_layouts.scss"
      ],
      [
        "remove",
        "web/static/src/webclient/actions/**/*css"
      ],
      "google_address_autocomplete/static/src/**/*",
      "point_of_sale/static/src/backend/pos_res_partner_view/*",
      "iot_webserial/static/src/web_serial_*.js"
    ],
    "point_of_sale.base_tests": [
      [
        "include",
        "web_tour.assets"
      ]
    ],
    "point_of_sale.assets_prod": [
      [
        "include",
        "point_of_sale._assets_pos"
      ],
      "point_of_sale/static/src/app/main.js"
    ],
    "point_of_sale.assets_prod_dark": [
      [
        "include",
        "point_of_sale.assets_prod"
      ]
    ],
    "point_of_sale.customer_display_assets": [
      [
        "include",
        "point_of_sale.base_app"
      ],
      "point_of_sale/static/src/app/components/odoo_logo/*",
      "point_of_sale/static/src/app/utils/use_timed_press.js",
      "point_of_sale/static/src/utils.js",
      "point_of_sale/static/src/scss/pos_variables_extra.scss",
      "point_of_sale/static/src/customer_display/**/*",
      "point_of_sale/static/src/app/hooks/time_hook.js",
      "point_of_sale/static/src/app/pos_app.scss",
      "point_of_sale/static/src/app/screens/login_screen/login_screen.scss",
      "point_of_sale/static/src/app/components/price_formatter/**/*",
      "point_of_sale/static/src/app/components/validation_animation/**/*",
      "point_of_sale/static/src/app/components/feedback_payment_summary/**/*",
      "point_of_sale/static/src/app/utils/pretty_console_log.js"
    ],
    "point_of_sale.customer_display_assets_dark": [
      [
        "include",
        "point_of_sale.customer_display_assets"
      ]
    ],
    "point_of_sale.customer_display_assets_test": [
      [
        "include",
        "point_of_sale.base_tests"
      ],
      "point_of_sale/static/tests/pos/tours/utils/common.js",
      "point_of_sale/static/tests/generic_helpers/utils.js"
    ],
    "point_of_sale.assets_debug": [
      [
        "include",
        "point_of_sale.base_tests"
      ],
      "point_of_sale/static/tests/generic_helpers/**/*",
      "point_of_sale/static/tests/pos/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/point_of_sale/README.md` (109 lines)
- `addons/point_of_sale/__init__.py` (8 lines)
- `addons/point_of_sale/__manifest__.py` (291 lines)
- `addons/point_of_sale/controllers/__init__.py` (5 lines)
- `addons/point_of_sale/controllers/binary.py` (13 lines)
- `addons/point_of_sale/controllers/customer_display.py` (39 lines)
- `addons/point_of_sale/controllers/main.py` (339 lines)
- `addons/point_of_sale/data/default_barcode_patterns.xml` (38 lines)
- `addons/point_of_sale/data/demo_data.xml` (8 lines)
- `addons/point_of_sale/data/digest_data.xml` (8 lines)
- `addons/point_of_sale/data/ir_config_parameter_data.xml` (6 lines)
- `addons/point_of_sale/data/ir_cron_data.xml` (43 lines)
- `addons/point_of_sale/data/mail_template_data.xml` (40 lines)
- `addons/point_of_sale/data/orders_demo.xml` (386 lines)
- `addons/point_of_sale/data/point_of_sale_data.xml` (135 lines)
- `addons/point_of_sale/data/point_of_sale_tour.xml` (8 lines)
- `addons/point_of_sale/data/pos_note_data.xml` (23 lines)
- `addons/point_of_sale/data/scenarios/bakery_category_data.xml` (16 lines)
- `addons/point_of_sale/data/scenarios/bakery_data.xml` (202 lines)
- `addons/point_of_sale/data/scenarios/clothes_category_data.xml` (29 lines)
- `addons/point_of_sale/data/scenarios/clothes_data.xml` (541 lines)
- `addons/point_of_sale/data/scenarios/furniture_category_data.xml` (22 lines)
- `addons/point_of_sale/data/scenarios/furniture_data.xml` (240 lines)
- `addons/point_of_sale/doc/barcode_test_sheet.pdf` (1,363 lines)
- `addons/point_of_sale/doc/barcode_test_sheet.svg` (525 lines)
- `addons/point_of_sale/doc/barcode_test_sheet2.svg` (1,108 lines)
- `addons/point_of_sale/doc/barcode_test_sheet4.pdf` (1,908 lines)
- `addons/point_of_sale/doc/barcode_test_sheet4.svg` (1,210 lines)
- `addons/point_of_sale/doc/barcode_test_sheet_new.svg` (506 lines)
- `addons/point_of_sale/i18n/af.po` (11,783 lines)
- `addons/point_of_sale/i18n/ar.po` (12,298 lines)
- `addons/point_of_sale/i18n/az.po` (12,148 lines)
- `addons/point_of_sale/i18n/bg.po` (12,069 lines)
- `addons/point_of_sale/i18n/bs.po` (11,961 lines)
- `addons/point_of_sale/i18n/ca.po` (12,353 lines)
- `addons/point_of_sale/i18n/cs.po` (12,269 lines)
- `addons/point_of_sale/i18n/da.po` (12,274 lines)
- `addons/point_of_sale/i18n/de.po` (12,841 lines)
- `addons/point_of_sale/i18n/el.po` (11,992 lines)
- `addons/point_of_sale/i18n/es.po` (12,766 lines)
- `addons/point_of_sale/i18n/es_419.po` (12,660 lines)
- `addons/point_of_sale/i18n/es_CL.po` (863 lines)
- `addons/point_of_sale/i18n/et.po` (12,160 lines)
- `addons/point_of_sale/i18n/eu.po` (11,780 lines)
- `addons/point_of_sale/i18n/fa.po` (12,139 lines)
- `addons/point_of_sale/i18n/fi.po` (12,554 lines)
- `addons/point_of_sale/i18n/fr.po` (12,847 lines)
- `addons/point_of_sale/i18n/fr_CA.po` (543 lines)
- `addons/point_of_sale/i18n/gl.po` (11,778 lines)
- `addons/point_of_sale/i18n/gu.po` (11,794 lines)
- `addons/point_of_sale/i18n/he.po` (12,060 lines)
- `addons/point_of_sale/i18n/hi.po` (11,983 lines)
- `addons/point_of_sale/i18n/hr.po` (12,067 lines)
- `addons/point_of_sale/i18n/hu.po` (12,032 lines)
- `addons/point_of_sale/i18n/id.po` (12,673 lines)
- `addons/point_of_sale/i18n/is.po` (11,825 lines)
- `addons/point_of_sale/i18n/it.po` (12,793 lines)
- `addons/point_of_sale/i18n/ja.po` (12,292 lines)
- `addons/point_of_sale/i18n/ka.po` (11,782 lines)
- `addons/point_of_sale/i18n/kab.po` (11,950 lines)
- `addons/point_of_sale/i18n/km.po` (11,784 lines)
- `addons/point_of_sale/i18n/ko.po` (12,229 lines)
- `addons/point_of_sale/i18n/ku.po` (11,959 lines)
- `addons/point_of_sale/i18n/lb.po` (11,781 lines)
- `addons/point_of_sale/i18n/lo.po` (12,340 lines)
- `addons/point_of_sale/i18n/lt.po` (12,030 lines)
- `addons/point_of_sale/i18n/lv.po` (11,976 lines)
- `addons/point_of_sale/i18n/mk.po` (11,793 lines)
- `addons/point_of_sale/i18n/mn.po` (12,120 lines)
- `addons/point_of_sale/i18n/my.po` (11,954 lines)
- `addons/point_of_sale/i18n/nb.po` (12,038 lines)
- `addons/point_of_sale/i18n/nl.po` (12,756 lines)
- `addons/point_of_sale/i18n/pl.po` (12,742 lines)
- `addons/point_of_sale/i18n/point_of_sale.pot` (11,900 lines)
- `addons/point_of_sale/i18n/pt.po` (12,363 lines)
- `addons/point_of_sale/i18n/pt_BR.po` (12,744 lines)
- `addons/point_of_sale/i18n/ro.po` (12,327 lines)
- `addons/point_of_sale/i18n/ru.po` (12,380 lines)
- `addons/point_of_sale/i18n/sk.po` (12,016 lines)
- `addons/point_of_sale/i18n/sl.po` (12,020 lines)
- `addons/point_of_sale/i18n/sr@latin.po` (11,967 lines)
- `addons/point_of_sale/i18n/sv.po` (12,247 lines)
- `addons/point_of_sale/i18n/th.po` (12,329 lines)
- `addons/point_of_sale/i18n/tr.po` (12,450 lines)
- `addons/point_of_sale/i18n/uk.po` (12,177 lines)
- `addons/point_of_sale/i18n/uz.po` (13,738 lines)
- `addons/point_of_sale/i18n/vi.po` (12,329 lines)
- `addons/point_of_sale/i18n/zh_CN.po` (12,294 lines)
- `addons/point_of_sale/i18n/zh_TW.po` (12,053 lines)
- `addons/point_of_sale/models/__init__.py` (56 lines)
- `addons/point_of_sale/models/account_account.py` (16 lines)
- `addons/point_of_sale/models/account_bank_statement.py` (11 lines)
- `addons/point_of_sale/models/account_bank_statement_line.py` (12 lines)
- `addons/point_of_sale/models/account_cash_rounding.py` (27 lines)
- `addons/point_of_sale/models/account_fiscal_position.py` (24 lines)
- `addons/point_of_sale/models/account_journal.py` (68 lines)
- `addons/point_of_sale/models/account_move.py` (121 lines)
- `addons/point_of_sale/models/account_move_line.py` (13 lines)
- `addons/point_of_sale/models/account_payment.py` (35 lines)
- `addons/point_of_sale/models/account_tax.py` (62 lines)
- `addons/point_of_sale/models/account_tax_group.py` (14 lines)
- `addons/point_of_sale/models/barcode_rule.py` (23 lines)
- `addons/point_of_sale/models/decimal_precision.py` (10 lines)
- `addons/point_of_sale/models/digest.py` (28 lines)
- `addons/point_of_sale/models/ir_http.py` (10 lines)
- `addons/point_of_sale/models/ir_sequence.py` (21 lines)
- `addons/point_of_sale/models/ir_ui_view.py` (45 lines)
- `addons/point_of_sale/models/pos_bill.py` (27 lines)
- `addons/point_of_sale/models/pos_bus_mixin.py` (40 lines)
- `addons/point_of_sale/models/pos_category.py` (156 lines)
- `addons/point_of_sale/models/pos_config.py` (1,499 lines)
- `addons/point_of_sale/models/pos_load_mixin.py` (138 lines)
- `addons/point_of_sale/models/pos_note.py` (28 lines)
- `addons/point_of_sale/models/pos_order.py` (1,829 lines)
- `addons/point_of_sale/models/pos_order_line.py` (335 lines)
- `addons/point_of_sale/models/pos_payment.py` (101 lines)
- `addons/point_of_sale/models/pos_payment_method.py` (603 lines)
- `addons/point_of_sale/models/pos_prep_line.py` (35 lines)
- `addons/point_of_sale/models/pos_prep_order.py` (55 lines)
- `addons/point_of_sale/models/pos_preset.py` (143 lines)
- `addons/point_of_sale/models/pos_printer.py` (123 lines)
- `addons/point_of_sale/models/pos_session.py` (1,330 lines)
- `addons/point_of_sale/models/pos_snooze.py` (63 lines)
- `addons/point_of_sale/models/product_attribute.py` (71 lines)
- `addons/point_of_sale/models/product_category.py` (11 lines)
- `addons/point_of_sale/models/product_combo.py` (56 lines)
- `addons/point_of_sale/models/product_combo_item.py` (23 lines)
- `addons/point_of_sale/models/product_pricelist.py` (72 lines)
- `addons/point_of_sale/models/product_product.py` (81 lines)
- `addons/point_of_sale/models/product_tag.py` (29 lines)
- `addons/point_of_sale/models/product_template.py` (374 lines)
- `addons/point_of_sale/models/product_uom.py` (14 lines)
- `addons/point_of_sale/models/report_sale_details.py` (546 lines)
- `addons/point_of_sale/models/res_company.py` (83 lines)
- `addons/point_of_sale/models/res_config_settings.py` (336 lines)
- `addons/point_of_sale/models/res_country.py` (10 lines)
- `addons/point_of_sale/models/res_country_state.py` (14 lines)
- `addons/point_of_sale/models/res_currency.py` (16 lines)
- `addons/point_of_sale/models/res_groups.py` (13 lines)
- `addons/point_of_sale/models/res_lang.py` (10 lines)
- `addons/point_of_sale/models/res_partner.py` (139 lines)
- `addons/point_of_sale/models/res_users.py` (30 lines)
- `addons/point_of_sale/models/resource_calendar_attendance.py` (15 lines)
- `addons/point_of_sale/models/uom.py` (18 lines)
- `addons/point_of_sale/receipt/__init__.py` (3 lines)
- `addons/point_of_sale/receipt/pos_cash_move_receipt.xml` (39 lines)
- `addons/point_of_sale/receipt/pos_order_change_receipt.xml` (104 lines)
- `addons/point_of_sale/receipt/pos_order_change_receipt_zpl.xml` (106 lines)
- `addons/point_of_sale/receipt/pos_order_receipt.py` (624 lines)
- `addons/point_of_sale/receipt/pos_order_receipt.xml` (251 lines)
- `addons/point_of_sale/receipt/pos_receipt_common.xml` (137 lines)
- `addons/point_of_sale/receipt/pos_sale_details_receipt.xml` (122 lines)
- `addons/point_of_sale/receipt/pos_tip_receipt.xml` (69 lines)
- `addons/point_of_sale/report/__init__.py` (5 lines)
- `addons/point_of_sale/report/pos_invoice.py` (30 lines)
- `addons/point_of_sale/report/pos_order_report.py` (128 lines)
- `addons/point_of_sale/security/ir.access.csv` (64 lines)
- `addons/point_of_sale/security/point_of_sale_security.xml` (30 lines)
- `addons/point_of_sale/static/description/icon.png` (17 lines)
- `addons/point_of_sale/static/description/icon.svg` (1 lines)

Additional files not expanded here: 725. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
