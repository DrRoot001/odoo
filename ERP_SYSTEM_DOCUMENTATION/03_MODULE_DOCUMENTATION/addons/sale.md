# Module: sale

- **Module ID:** MOD-509
- **Path:** `addons/sale`
- **Manifest:** `addons/sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Sales internal machinery


This module contains all the common features of Sales Management and eCommerce.
    

Declared dependencies: `sales_team`, `account_payment`, `utm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 76 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 21 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 64 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 69 | Client behavior/assets. |
| Tests | 37 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 14 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sales_team",
    "account_payment",
    "utm"
  ],
  "data": [
    "security/res_groups.xml",
    "report/account_invoice_report_views.xml",
    "report/ir_actions_report_templates.xml",
    "report/ir_actions_report.xml",
    "report/sale_report_views.xml",
    "data/ir_cron.xml",
    "data/ir_sequence_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_template_data.xml",
    "data/portal_entry_data.xml",
    "data/sale_tour.xml",
    "data/ir_config_parameter.xml",
    "wizard/account_accrued_orders_wizard_views.xml",
    "wizard/mass_cancel_orders_views.xml",
    "wizard/payment_link_wizard_views.xml",
    "wizard/res_config_settings_views.xml",
    "wizard/sale_make_invoice_advance_views.xml",
    "wizard/sale_order_discount_views.xml",
    "views/sale_order_views.xml",
    "views/account_views.xml",
    "views/account_analytic_line_views.xml",
    "views/crm_team_views.xml",
    "views/mail_activity_views.xml",
    "views/payment_views.xml",
    "views/product_document_views.xml",
    "views/product_template_views.xml",
    "views/product_views.xml",
    "views/res_partner_views.xml",
    "views/sale_order_line_views.xml",
    "views/sale_portal_templates.xml",
    "views/utm_campaign_views.xml",
    "views/sale_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/product_demo.xml",
    "data/sale_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale/static/src/scss/sale_onboarding.scss",
      "sale/static/src/scss/services_and_material.scss",
      "sale/static/src/js/badge_extra_price/*",
      "sale/static/src/js/sale_action_helper/*",
      "sale/static/src/js/combo_configurator_dialog/*",
      "sale/static/src/scss/sale_order_line_kanban.scss",
      "sale/static/src/js/discount_menu_widget.js",
      "sale/static/src/js/combo_menu_widget.js",
      "sale/static/src/xml/discount_menu_widget.xml",
      "sale/static/src/xml/combo_menu_widget.xml",
      "sale/static/src/js/extra_total_field/*",
      "sale/static/src/js/labeled_field_short_labels.js",
      "sale/static/src/js/labeled_float_field/*",
      "sale/static/src/js/labeled_monetary_field/*",
      "sale/static/src/js/labeled_percentage_field/*",
      "sale/static/src/js/models/*",
      "sale/static/src/js/product/*",
      "sale/static/src/js/product_card/*",
      "sale/static/src/js/product_configurator_dialog/*",
      "sale/static/src/js/product_list/*",
      "sale/static/src/js/product_template_attribute_line/*",
      "sale/static/src/js/quantity_availability/*",
      "sale/static/src/js/quantity_buttons/*",
      "sale/static/src/js/sale_line_number/*",
      "sale/static/src/js/sale_order_line_field/*",
      "sale/static/src/js/section_line_record/*",
      "sale/static/src/js/tours/sale.js",
      "sale/static/src/js/upload_rfq_cog_menu/*",
      "sale/static/src/js/sale_product_mixin.js",
      "sale/static/src/js/sale_product_field/*",
      "sale/static/src/js/sale_utils.js",
      "sale/static/src/js/combo_configurator_utils.js",
      "sale/static/src/js/sale_label_text/*",
      "sale/static/src/js/date_filter_button/**/*",
      "sale/static/src/js/dashboard/**/*",
      [
        "remove",
        "sale/static/src/js/dashboard/**/*.dark.scss"
      ],
      "sale/static/src/views/**/*"
    ],
    "web.assets_web_dark": [
      "sale/static/src/js/dashboard/**/*.dark.scss",
      "sale/static/src/scss/services_and_material.dark.scss"
    ],
    "web.assets_frontend": [
      "sale/static/src/interactions/**/*",
      "sale/static/src/scss/sale_portal.scss"
    ],
    "web.assets_tests": [
      "sale/static/tests/tours/**/*",
      "sale/static/src/js/tours/combo_configurator_tour_utils.js",
      "sale/static/src/js/tours/product_configurator_tour_utils.js",
      "sale/static/src/js/tours/tour_utils.js"
    ],
    "web.assets_unit_tests": [
      "sale/static/tests/mock_server/**/*",
      "sale/static/tests/sale_test_helpers.js",
      "sale/static/tests/**/*.test.js"
    ],
    "web.report_assets_common": [
      "sale/static/src/scss/sale_report.scss"
    ]
  }
}
```

### Representative source files

- `addons/sale/README.md` (99 lines)
- `addons/sale/__init__.py` (33 lines)
- `addons/sale/__manifest__.py` (117 lines)
- `addons/sale/const.py` (4 lines)
- `addons/sale/controllers/__init__.py` (3 lines)
- `addons/sale/controllers/combo_configurator.py` (247 lines)
- `addons/sale/controllers/portal.py` (539 lines)
- `addons/sale/controllers/product_configurator.py` (469 lines)
- `addons/sale/data/ir_config_parameter.xml` (19 lines)
- `addons/sale/data/ir_cron.xml` (26 lines)
- `addons/sale/data/ir_sequence_data.xml` (12 lines)
- `addons/sale/data/mail_message_subtype_data.xml` (65 lines)
- `addons/sale/data/mail_template_data.xml` (457 lines)
- `addons/sale/data/portal_entry_data.xml` (20 lines)
- `addons/sale/data/product_demo.xml` (182 lines)
- `addons/sale/data/sale_demo.xml` (706 lines)
- `addons/sale/data/sale_tour.xml` (10 lines)
- `addons/sale/i18n/af.po` (5,930 lines)
- `addons/sale/i18n/am.po` (5,926 lines)
- `addons/sale/i18n/ar.po` (8,273 lines)
- `addons/sale/i18n/az.po` (6,335 lines)
- `addons/sale/i18n/bg.po` (6,221 lines)
- `addons/sale/i18n/bs.po` (6,830 lines)
- `addons/sale/i18n/ca.po` (8,429 lines)
- `addons/sale/i18n/cs.po` (6,558 lines)
- `addons/sale/i18n/da.po` (6,362 lines)
- `addons/sale/i18n/de.po` (8,711 lines)
- `addons/sale/i18n/el.po` (6,240 lines)
- `addons/sale/i18n/en_AU.po` (99 lines)
- `addons/sale/i18n/es.po` (8,546 lines)
- `addons/sale/i18n/es_419.po` (8,602 lines)
- `addons/sale/i18n/es_CL.po` (624 lines)
- `addons/sale/i18n/et.po` (7,300 lines)
- `addons/sale/i18n/eu.po` (5,943 lines)
- `addons/sale/i18n/fa.po` (6,301 lines)
- `addons/sale/i18n/fi.po` (8,609 lines)
- `addons/sale/i18n/fo.po` (5,926 lines)
- `addons/sale/i18n/fr.po` (7,691 lines)
- `addons/sale/i18n/fr_CA.po` (303 lines)
- `addons/sale/i18n/gl.po` (5,928 lines)
- `addons/sale/i18n/gu.po` (5,940 lines)
- `addons/sale/i18n/he.po` (6,296 lines)
- `addons/sale/i18n/hi.po` (6,233 lines)
- `addons/sale/i18n/hr.po` (6,394 lines)
- `addons/sale/i18n/hu.po` (6,375 lines)
- `addons/sale/i18n/id.po` (8,635 lines)
- `addons/sale/i18n/is.po` (5,960 lines)
- `addons/sale/i18n/it.po` (8,649 lines)
- `addons/sale/i18n/ja.po` (7,386 lines)
- `addons/sale/i18n/ka.po` (5,929 lines)
- `addons/sale/i18n/kab.po` (6,127 lines)
- `addons/sale/i18n/km.po` (5,935 lines)
- `addons/sale/i18n/ko.po` (6,406 lines)
- `addons/sale/i18n/ku.po` (6,088 lines)
- `addons/sale/i18n/lb.po` (5,928 lines)
- `addons/sale/i18n/lo.po` (7,481 lines)
- `addons/sale/i18n/lt.po` (6,230 lines)
- `addons/sale/i18n/lv.po` (6,570 lines)
- `addons/sale/i18n/mk.po` (5,955 lines)
- `addons/sale/i18n/mn.po` (7,619 lines)
- `addons/sale/i18n/my.po` (6,097 lines)
- `addons/sale/i18n/nb.po` (6,261 lines)
- `addons/sale/i18n/nl.po` (8,642 lines)
- `addons/sale/i18n/pl.po` (8,663 lines)
- `addons/sale/i18n/pt.po` (7,606 lines)
- `addons/sale/i18n/pt_BR.po` (8,600 lines)
- `addons/sale/i18n/ro.po` (6,398 lines)
- `addons/sale/i18n/ru.po` (7,321 lines)
- `addons/sale/i18n/sale.pot` (5,762 lines)
- `addons/sale/i18n/sk.po` (6,667 lines)
- `addons/sale/i18n/sl.po` (6,193 lines)
- `addons/sale/i18n/sq.po` (5,930 lines)
- `addons/sale/i18n/sr@latin.po` (6,089 lines)
- `addons/sale/i18n/sv.po` (6,382 lines)
- `addons/sale/i18n/th.po` (8,350 lines)
- `addons/sale/i18n/tr.po` (7,338 lines)
- `addons/sale/i18n/uk.po` (6,451 lines)
- `addons/sale/i18n/uz.po` (7,114 lines)
- `addons/sale/i18n/vi.po` (6,487 lines)
- `addons/sale/i18n/zh_CN.po` (8,464 lines)
- `addons/sale/i18n/zh_TW.po` (6,370 lines)
- `addons/sale/models/__init__.py` (25 lines)
- `addons/sale/models/account_analytic_applicability.py` (12 lines)
- `addons/sale/models/account_analytic_line.py` (261 lines)
- `addons/sale/models/account_move.py` (317 lines)
- `addons/sale/models/account_move_line.py` (308 lines)
- `addons/sale/models/crm_team.py` (50 lines)
- `addons/sale/models/ir_actions_report.py` (58 lines)
- `addons/sale/models/ir_config_parameter.py` (45 lines)
- `addons/sale/models/payment_provider.py` (15 lines)
- `addons/sale/models/payment_transaction.py` (273 lines)
- `addons/sale/models/product_category.py` (22 lines)
- `addons/sale/models/product_document.py` (25 lines)
- `addons/sale/models/product_pricelist_item.py` (16 lines)
- `addons/sale/models/product_product.py` (181 lines)
- `addons/sale/models/product_template.py` (385 lines)
- `addons/sale/models/res_company.py` (134 lines)
- `addons/sale/models/res_groups.py` (17 lines)
- `addons/sale/models/res_partner.py` (123 lines)
- `addons/sale/models/sale_order.py` (2,930 lines)
- `addons/sale/models/sale_order_line.py` (2,401 lines)
- `addons/sale/models/utm_campaign.py` (122 lines)
- `addons/sale/populate/benchmarks.xml` (169 lines)
- `addons/sale/populate/populate_demo.xml` (57 lines)
- `addons/sale/report/__init__.py` (3 lines)
- `addons/sale/report/account_invoice_report.py` (16 lines)
- `addons/sale/report/account_invoice_report_views.xml` (40 lines)
- `addons/sale/report/ir_actions_report.xml` (25 lines)
- `addons/sale/report/ir_actions_report_templates.xml` (508 lines)
- `addons/sale/report/sale_report.py` (220 lines)
- `addons/sale/report/sale_report_views.xml` (207 lines)
- `addons/sale/security/ir.access.csv` (55 lines)
- `addons/sale/security/res_groups.xml` (23 lines)
- `addons/sale/static/description/icon.png` (15 lines)
- `addons/sale/static/description/icon.svg` (1 lines)
- `addons/sale/static/description/icon_hi.png` (20 lines)
- `addons/sale/static/img/advance_product_0-image.jpg` (25 lines)
- `addons/sale/static/img/btn_paynowcc_lg.gif` (22 lines)
- `addons/sale/static/img/floor_protection-image.jpg` (301 lines)
- `addons/sale/static/src/img/bag.svg` (9 lines)
- `addons/sale/static/src/img/onboarding_quotation_order_tooltip.jpg` (172 lines)
- `addons/sale/static/src/img/sales_quotation_thumbnail.webp` (46 lines)
- `addons/sale/static/src/img/services_and_material_empty_dark.svg` (1,022 lines)
- `addons/sale/static/src/img/services_and_material_empty_light.svg` (1,021 lines)
- `addons/sale/static/src/interactions/portal_prepayment.js` (65 lines)
- `addons/sale/static/src/interactions/sale_portal.js` (11 lines)
- `addons/sale/static/src/interactions/sale_sidebar.js` (26 lines)
- `addons/sale/static/src/js/badge_extra_price/badge_extra_price.js` (19 lines)
- `addons/sale/static/src/js/badge_extra_price/badge_extra_price.xml` (9 lines)
- `addons/sale/static/src/js/combo_configurator_dialog/combo_configurator_dialog.js` (278 lines)
- `addons/sale/static/src/js/combo_configurator_dialog/combo_configurator_dialog.scss` (11 lines)
- `addons/sale/static/src/js/combo_configurator_dialog/combo_configurator_dialog.xml` (119 lines)
- `addons/sale/static/src/js/combo_configurator_utils.js` (89 lines)
- `addons/sale/static/src/js/combo_menu_widget.js` (45 lines)
- `addons/sale/static/src/js/dashboard/dashboard.dark.scss` (10 lines)
- `addons/sale/static/src/js/dashboard/dashboard.js` (178 lines)
- `addons/sale/static/src/js/dashboard/dashboard.scss` (63 lines)
- `addons/sale/static/src/js/dashboard/dashboard.xml` (60 lines)
- `addons/sale/static/src/js/date_filter_button/date_filter_button.js` (30 lines)
- `addons/sale/static/src/js/date_filter_button/date_filter_button.xml` (24 lines)
- `addons/sale/static/src/js/discount_menu_widget.js` (40 lines)
- `addons/sale/static/src/js/extra_total_field/extra_total_field.js` (26 lines)
- `addons/sale/static/src/js/extra_total_field/extra_total_field.xml` (27 lines)
- `addons/sale/static/src/js/labeled_field_short_labels.js` (36 lines)
- `addons/sale/static/src/js/labeled_float_field/labeled_float_field.js` (24 lines)
- `addons/sale/static/src/js/labeled_float_field/labeled_float_field.xml` (16 lines)
- `addons/sale/static/src/js/labeled_monetary_field/labeled_monetary_field.js` (28 lines)
- `addons/sale/static/src/js/labeled_monetary_field/labeled_monetary_field.xml` (16 lines)
- `addons/sale/static/src/js/labeled_percentage_field/labeled_percentage_field.js` (27 lines)
- `addons/sale/static/src/js/labeled_percentage_field/labeled_percentage_field.xml` (16 lines)
- `addons/sale/static/src/js/models/product_combo.js` (41 lines)
- `addons/sale/static/src/js/models/product_combo_item.js` (51 lines)
- `addons/sale/static/src/js/models/product_product.js` (77 lines)
- `addons/sale/static/src/js/models/product_template_attribute_line.js` (73 lines)
- `addons/sale/static/src/js/models/product_template_attribute_value.js` (14 lines)
- `addons/sale/static/src/js/product/product.js` (93 lines)
- `addons/sale/static/src/js/product/product.scss` (60 lines)
- `addons/sale/static/src/js/product/product.xml` (138 lines)
- `addons/sale/static/src/js/product_card/product_card.js` (28 lines)
- `addons/sale/static/src/js/product_card/product_card.scss` (17 lines)

Additional files not expanded here: 146. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
