# Module: pos_loyalty

- **Module ID:** MOD-436
- **Path:** `addons/pos_loyalty`
- **Manifest:** `addons/pos_loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Use Coupons, Gift Cards and Loyalty programs in Point of Sale

No manifest description declared.

Declared dependencies: `loyalty`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 54 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "loyalty",
    "point_of_sale"
  ],
  "data": [
    "data/default_barcode_patterns.xml",
    "data/gift_card_data.xml",
    "views/loyalty_card_views.xml",
    "views/loyalty_mail_views.xml",
    "views/pos_loyalty_menu_views.xml",
    "views/res_config_settings_view.xml",
    "views/loyalty_program_views.xml",
    "views/res_partner_views.xml",
    "receipt/pos_order_receipt.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/pos_loyalty_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "pos_loyalty/static/src/portal/*"
    ],
    "point_of_sale._assets_pos": [
      "pos_loyalty/static/src/app/**/*"
    ],
    "point_of_sale.customer_display_assets": [
      "pos_loyalty/static/src/customer_display/**/*"
    ],
    "web.assets_tests": [
      "pos_loyalty/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "pos_loyalty/static/src/customer_display/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_loyalty/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_loyalty/__init__.py` (9 lines)
- `addons/pos_loyalty/__manifest__.py` (49 lines)
- `addons/pos_loyalty/data/default_barcode_patterns.xml` (12 lines)
- `addons/pos_loyalty/data/gift_card_data.xml` (15 lines)
- `addons/pos_loyalty/data/pos_loyalty_demo.xml` (97 lines)
- `addons/pos_loyalty/i18n/ar.po` (726 lines)
- `addons/pos_loyalty/i18n/az.po` (714 lines)
- `addons/pos_loyalty/i18n/bg.po` (715 lines)
- `addons/pos_loyalty/i18n/bs.po` (716 lines)
- `addons/pos_loyalty/i18n/ca.po` (728 lines)
- `addons/pos_loyalty/i18n/cs.po` (727 lines)
- `addons/pos_loyalty/i18n/da.po` (727 lines)
- `addons/pos_loyalty/i18n/de.po` (759 lines)
- `addons/pos_loyalty/i18n/el.po` (715 lines)
- `addons/pos_loyalty/i18n/es.po` (732 lines)
- `addons/pos_loyalty/i18n/es_419.po` (738 lines)
- `addons/pos_loyalty/i18n/et.po` (715 lines)
- `addons/pos_loyalty/i18n/fa.po` (714 lines)
- `addons/pos_loyalty/i18n/fi.po` (731 lines)
- `addons/pos_loyalty/i18n/fr.po` (738 lines)
- `addons/pos_loyalty/i18n/he.po` (715 lines)
- `addons/pos_loyalty/i18n/hi.po` (714 lines)
- `addons/pos_loyalty/i18n/hr.po` (715 lines)
- `addons/pos_loyalty/i18n/hu.po` (715 lines)
- `addons/pos_loyalty/i18n/id.po` (741 lines)
- `addons/pos_loyalty/i18n/it.po` (737 lines)
- `addons/pos_loyalty/i18n/ja.po` (734 lines)
- `addons/pos_loyalty/i18n/kab.po` (715 lines)
- `addons/pos_loyalty/i18n/ko.po` (725 lines)
- `addons/pos_loyalty/i18n/ku.po` (714 lines)
- `addons/pos_loyalty/i18n/lo.po` (726 lines)
- `addons/pos_loyalty/i18n/lt.po` (716 lines)
- `addons/pos_loyalty/i18n/lv.po` (715 lines)
- `addons/pos_loyalty/i18n/mn.po` (714 lines)
- `addons/pos_loyalty/i18n/my.po` (715 lines)
- `addons/pos_loyalty/i18n/nb.po` (715 lines)
- `addons/pos_loyalty/i18n/nl.po` (749 lines)
- `addons/pos_loyalty/i18n/pl.po` (732 lines)
- `addons/pos_loyalty/i18n/pos_loyalty.pot` (711 lines)
- `addons/pos_loyalty/i18n/pt.po` (728 lines)
- `addons/pos_loyalty/i18n/pt_BR.po` (749 lines)
- `addons/pos_loyalty/i18n/ro.po` (728 lines)
- `addons/pos_loyalty/i18n/ru.po` (734 lines)
- `addons/pos_loyalty/i18n/sk.po` (714 lines)
- `addons/pos_loyalty/i18n/sl.po` (716 lines)
- `addons/pos_loyalty/i18n/sr@latin.po` (715 lines)
- `addons/pos_loyalty/i18n/sv.po` (727 lines)
- `addons/pos_loyalty/i18n/th.po` (722 lines)
- `addons/pos_loyalty/i18n/tr.po` (732 lines)
- `addons/pos_loyalty/i18n/uk.po` (715 lines)
- `addons/pos_loyalty/i18n/uz.po` (803 lines)
- `addons/pos_loyalty/i18n/vi.po` (728 lines)
- `addons/pos_loyalty/i18n/zh_CN.po` (724 lines)
- `addons/pos_loyalty/i18n/zh_TW.po` (722 lines)
- `addons/pos_loyalty/models/__init__.py` (15 lines)
- `addons/pos_loyalty/models/account_move_line.py` (23 lines)
- `addons/pos_loyalty/models/barcode_rule.py` (10 lines)
- `addons/pos_loyalty/models/loyalty_card.py` (105 lines)
- `addons/pos_loyalty/models/loyalty_mail.py` (12 lines)
- `addons/pos_loyalty/models/loyalty_program.py` (123 lines)
- `addons/pos_loyalty/models/loyalty_reward.py` (122 lines)
- `addons/pos_loyalty/models/loyalty_rule.py` (141 lines)
- `addons/pos_loyalty/models/pos_config.py` (47 lines)
- `addons/pos_loyalty/models/pos_order.py` (396 lines)
- `addons/pos_loyalty/models/pos_order_line.py` (49 lines)
- `addons/pos_loyalty/models/pos_session.py` (21 lines)
- `addons/pos_loyalty/models/product_product.py` (34 lines)
- `addons/pos_loyalty/models/product_template.py` (19 lines)
- `addons/pos_loyalty/receipt/__init__.py` (1 lines)
- `addons/pos_loyalty/receipt/pos_order_receipt.py` (64 lines)
- `addons/pos_loyalty/receipt/pos_order_receipt.xml` (31 lines)
- `addons/pos_loyalty/security/ir.access.csv` (14 lines)
- `addons/pos_loyalty/static/img/simple_pen.png` (304 lines)
- `addons/pos_loyalty/static/src/app/components/popups/manage_giftcard_popup/manage_giftcard_popup.js` (151 lines)
- `addons/pos_loyalty/static/src/app/components/popups/manage_giftcard_popup/manage_giftcard_popup.xml` (63 lines)
- `addons/pos_loyalty/static/src/app/css/Loyalty.scss` (55 lines)
- `addons/pos_loyalty/static/src/app/models/data_service_options.js` (27 lines)
- `addons/pos_loyalty/static/src/app/models/loyalty_card.js` (19 lines)
- `addons/pos_loyalty/static/src/app/models/loyalty_program.js` (147 lines)
- `addons/pos_loyalty/static/src/app/models/loyalty_reward.js` (229 lines)
- `addons/pos_loyalty/static/src/app/models/loyalty_rule.js` (151 lines)
- `addons/pos_loyalty/static/src/app/models/pos_order.js` (505 lines)
- `addons/pos_loyalty/static/src/app/models/pos_order_line.js` (181 lines)
- `addons/pos_loyalty/static/src/app/plugins/pos_data_plugin.js` (23 lines)
- `addons/pos_loyalty/static/src/app/screens/partner_list_screen/partner_line/partner_line.js` (52 lines)
- `addons/pos_loyalty/static/src/app/screens/partner_list_screen/partner_line/partner_line.xml` (10 lines)
- `addons/pos_loyalty/static/src/app/screens/partner_list_screen/partner_list_screen.js` (23 lines)
- `addons/pos_loyalty/static/src/app/screens/product_screen/control_buttons/control_buttons.js` (235 lines)
- `addons/pos_loyalty/static/src/app/screens/product_screen/control_buttons/control_buttons.xml` (70 lines)
- `addons/pos_loyalty/static/src/app/screens/product_screen/order_summary/order_summary.js` (80 lines)
- `addons/pos_loyalty/static/src/app/screens/product_screen/order_summary/order_summary.xml` (36 lines)
- `addons/pos_loyalty/static/src/app/screens/product_screen/product_screen.js` (28 lines)
- `addons/pos_loyalty/static/src/app/screens/ticket_screen/ticket_screen.js` (74 lines)
- `addons/pos_loyalty/static/src/app/services/customer_display_plugin.js` (32 lines)
- `addons/pos_loyalty/static/src/app/services/pos_store.js` (292 lines)
- `addons/pos_loyalty/static/src/app/utils/order_payment_validation.js` (40 lines)
- `addons/pos_loyalty/static/src/app/utils/printer/generate_printer_data.js` (72 lines)
- `addons/pos_loyalty/static/src/customer_display/customer_display.xml` (32 lines)
- `addons/pos_loyalty/static/src/portal/loyalty_card_dialog.xml` (16 lines)
- `addons/pos_loyalty/static/tests/tours/e_wallet_program_tour.js` (230 lines)
- `addons/pos_loyalty/static/tests/tours/gift_card_program_tour.js` (356 lines)
- `addons/pos_loyalty/static/tests/tours/loyalty_history_tour.js` (37 lines)
- `addons/pos_loyalty/static/tests/tours/loyalty_mirror_tour.js` (165 lines)
- `addons/pos_loyalty/static/tests/tours/multiple_gift_wallet_programs_tour.js` (76 lines)
- `addons/pos_loyalty/static/tests/tours/order_receipt.js` (38 lines)
- `addons/pos_loyalty/static/tests/tours/pos_loyalty_loyalty_program_tour.js` (414 lines)
- `addons/pos_loyalty/static/tests/tours/pos_loyalty_reward_button_tour.js` (365 lines)
- `addons/pos_loyalty/static/tests/tours/pos_loyalty_tour.js` (902 lines)
- `addons/pos_loyalty/static/tests/tours/pos_loyalty_validity_tour.js` (39 lines)
- `addons/pos_loyalty/static/tests/tours/service_fee_payment_reward_tour.js` (64 lines)
- `addons/pos_loyalty/static/tests/tours/service_fee_promotion_tour.js` (98 lines)
- `addons/pos_loyalty/static/tests/tours/utils/pos_loyalty_util.js` (268 lines)
- `addons/pos_loyalty/static/tests/unit/components/manage_giftcard_popup.test.js` (48 lines)
- `addons/pos_loyalty/static/tests/unit/components/order_receipt.test.js` (52 lines)
- `addons/pos_loyalty/static/tests/unit/components/screens/control_buttons.test.js` (56 lines)
- `addons/pos_loyalty/static/tests/unit/components/screens/order_summary.test.js` (36 lines)
- `addons/pos_loyalty/static/tests/unit/components/screens/partner_line.test.js` (40 lines)
- `addons/pos_loyalty/static/tests/unit/customer_display/customer_display.test.js` (37 lines)
- `addons/pos_loyalty/static/tests/unit/data/barcode_nomenclature.data.js` (9 lines)
- `addons/pos_loyalty/static/tests/unit/data/barcode_rule.data.js` (15 lines)
- `addons/pos_loyalty/static/tests/unit/data/loyalty_card.data.js` (52 lines)
- `addons/pos_loyalty/static/tests/unit/data/loyalty_program.data.js` (214 lines)
- `addons/pos_loyalty/static/tests/unit/data/loyalty_reward.data.js` (148 lines)
- `addons/pos_loyalty/static/tests/unit/data/loyalty_rule.data.js` (103 lines)
- `addons/pos_loyalty/static/tests/unit/data/pos_order.data.js` (110 lines)
- `addons/pos_loyalty/static/tests/unit/data/pos_order_line.data.js` (14 lines)
- `addons/pos_loyalty/static/tests/unit/data/pos_session.data.js` (14 lines)
- `addons/pos_loyalty/static/tests/unit/data/product_product.data.js` (27 lines)
- `addons/pos_loyalty/static/tests/unit/data/product_template.data.js` (18 lines)
- `addons/pos_loyalty/static/tests/unit/models/pos_order.test.js` (399 lines)
- `addons/pos_loyalty/static/tests/unit/models/pos_order_line.test.js` (59 lines)
- `addons/pos_loyalty/static/tests/unit/receipt_utils.js` (23 lines)
- `addons/pos_loyalty/static/tests/unit/screens/ticket_screen.test.js` (48 lines)
- `addons/pos_loyalty/static/tests/unit/utils.js` (28 lines)
- `addons/pos_loyalty/tests/__init__.py` (12 lines)
- `addons/pos_loyalty/tests/common.py` (35 lines)
- `addons/pos_loyalty/tests/test_frontend.py` (3,817 lines)
- `addons/pos_loyalty/tests/test_gift_card_communication.py` (240 lines)
- `addons/pos_loyalty/tests/test_loyalty_history.py` (208 lines)
- `addons/pos_loyalty/tests/test_loyalty_mirror.py` (342 lines)
- `addons/pos_loyalty/tests/test_order_receipt.py` (77 lines)
- `addons/pos_loyalty/tests/test_pos_loyalty_points.py` (345 lines)
- `addons/pos_loyalty/tests/test_product_loading.py` (108 lines)
- `addons/pos_loyalty/tests/test_service_fee.py` (157 lines)
- `addons/pos_loyalty/tests/test_unlink_reward.py` (27 lines)
- `addons/pos_loyalty/views/loyalty_card_views.xml` (13 lines)
- `addons/pos_loyalty/views/loyalty_mail_views.xml` (13 lines)
- `addons/pos_loyalty/views/loyalty_program_views.xml` (41 lines)
- `addons/pos_loyalty/views/pos_loyalty_menu_views.xml` (20 lines)
- `addons/pos_loyalty/views/res_config_settings_view.xml` (20 lines)
- `addons/pos_loyalty/views/res_partner_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
