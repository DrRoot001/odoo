# Module: pos_stock

- **Module ID:** MOD-464
- **Path:** `addons/pos_stock`
- **Manifest:** `addons/pos_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Stock integration for PoS

No manifest description declared.

Declared dependencies: `point_of_sale`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 18 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 17 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 48 | Client behavior/assets. |
| Tests | 16 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "stock_account"
  ],
  "data": [
    "security/pos_stock_security.xml",
    "data/pos_stock_data.xml",
    "views/pos_order_view.xml",
    "views/product_view.xml",
    "views/pos_config_view.xml",
    "views/pos_session_view.xml",
    "views/res_config_settings_views.xml",
    "views/stock_reference_views.xml",
    "receipt/pos_order_receipt.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_stock/static/src/**/*",
      [
        "remove",
        "pos_stock/static/src/customer_display/**/*"
      ]
    ],
    "point_of_sale.customer_display_assets": [
      "pos_stock/static/src/customer_display/**/*"
    ],
    "web.assets_tests": [
      "pos_stock/static/tests/pos/tours/**/*"
    ],
    "web.assets_unit_tests_setup": [
      [
        "remove",
        "pos_stock/static/src/app/components/popups/select_lot_popup/select_lot_popup.scss"
      ],
      "pos_stock/static/src/customer_display/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_stock/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_stock/__init__.py` (7 lines)
- `addons/pos_stock/__manifest__.py` (43 lines)
- `addons/pos_stock/data/pos_stock_data.xml` (8 lines)
- `addons/pos_stock/i18n/ar.po` (689 lines)
- `addons/pos_stock/i18n/az.po` (687 lines)
- `addons/pos_stock/i18n/bg.po` (687 lines)
- `addons/pos_stock/i18n/bs.po` (688 lines)
- `addons/pos_stock/i18n/ca.po` (688 lines)
- `addons/pos_stock/i18n/cs.po` (688 lines)
- `addons/pos_stock/i18n/da.po` (687 lines)
- `addons/pos_stock/i18n/de.po` (718 lines)
- `addons/pos_stock/i18n/el.po` (687 lines)
- `addons/pos_stock/i18n/es.po` (715 lines)
- `addons/pos_stock/i18n/es_419.po` (717 lines)
- `addons/pos_stock/i18n/et.po` (687 lines)
- `addons/pos_stock/i18n/fa.po` (687 lines)
- `addons/pos_stock/i18n/fi.po` (693 lines)
- `addons/pos_stock/i18n/fr.po` (716 lines)
- `addons/pos_stock/i18n/he.po` (688 lines)
- `addons/pos_stock/i18n/hi.po` (687 lines)
- `addons/pos_stock/i18n/hr.po` (688 lines)
- `addons/pos_stock/i18n/hu.po` (687 lines)
- `addons/pos_stock/i18n/id.po` (712 lines)
- `addons/pos_stock/i18n/it.po` (713 lines)
- `addons/pos_stock/i18n/ja.po` (709 lines)
- `addons/pos_stock/i18n/kab.po` (687 lines)
- `addons/pos_stock/i18n/ko.po` (687 lines)
- `addons/pos_stock/i18n/ku.po` (687 lines)
- `addons/pos_stock/i18n/lo.po` (705 lines)
- `addons/pos_stock/i18n/lt.po` (689 lines)
- `addons/pos_stock/i18n/lv.po` (688 lines)
- `addons/pos_stock/i18n/mn.po` (687 lines)
- `addons/pos_stock/i18n/my.po` (688 lines)
- `addons/pos_stock/i18n/nb.po` (687 lines)
- `addons/pos_stock/i18n/nl.po` (716 lines)
- `addons/pos_stock/i18n/pl.po` (688 lines)
- `addons/pos_stock/i18n/pos_stock.pot` (679 lines)
- `addons/pos_stock/i18n/pt.po` (687 lines)
- `addons/pos_stock/i18n/pt_BR.po` (717 lines)
- `addons/pos_stock/i18n/ro.po` (688 lines)
- `addons/pos_stock/i18n/ru.po` (688 lines)
- `addons/pos_stock/i18n/sk.po` (687 lines)
- `addons/pos_stock/i18n/sl.po` (688 lines)
- `addons/pos_stock/i18n/sr@latin.po` (689 lines)
- `addons/pos_stock/i18n/sv.po` (688 lines)
- `addons/pos_stock/i18n/th.po` (696 lines)
- `addons/pos_stock/i18n/tr.po` (688 lines)
- `addons/pos_stock/i18n/uk.po` (688 lines)
- `addons/pos_stock/i18n/uz.po` (687 lines)
- `addons/pos_stock/i18n/vi.po` (687 lines)
- `addons/pos_stock/i18n/zh_CN.po` (702 lines)
- `addons/pos_stock/i18n/zh_TW.po` (688 lines)
- `addons/pos_stock/models/__init__.py` (17 lines)
- `addons/pos_stock/models/account_move.py` (48 lines)
- `addons/pos_stock/models/account_move_line.py` (19 lines)
- `addons/pos_stock/models/pos_config.py` (49 lines)
- `addons/pos_stock/models/pos_order.py` (119 lines)
- `addons/pos_stock/models/pos_order_line.py` (185 lines)
- `addons/pos_stock/models/pos_pack_operation_lot.py` (25 lines)
- `addons/pos_stock/models/pos_session.py` (223 lines)
- `addons/pos_stock/models/product_category.py` (12 lines)
- `addons/pos_stock/models/product_removal.py` (10 lines)
- `addons/pos_stock/models/product_template.py` (65 lines)
- `addons/pos_stock/models/res_company.py` (11 lines)
- `addons/pos_stock/models/res_config_settings.py` (12 lines)
- `addons/pos_stock/models/stock_move.py` (185 lines)
- `addons/pos_stock/models/stock_picking.py` (203 lines)
- `addons/pos_stock/models/stock_reference.py` (9 lines)
- `addons/pos_stock/models/stock_rule.py` (16 lines)
- `addons/pos_stock/models/stock_warehouse.py` (47 lines)
- `addons/pos_stock/receipt/__init__.py` (3 lines)
- `addons/pos_stock/receipt/pos_order_receipt.py` (31 lines)
- `addons/pos_stock/receipt/pos_order_receipt.xml` (22 lines)
- `addons/pos_stock/security/ir.access.csv` (8 lines)
- `addons/pos_stock/security/pos_stock_security.xml` (8 lines)
- `addons/pos_stock/static/src/app/components/orderline/orderline.js` (22 lines)
- `addons/pos_stock/static/src/app/components/orderline/orderline.xml` (15 lines)
- `addons/pos_stock/static/src/app/components/popups/date_picker_popup/date_picker_popup.js` (49 lines)
- `addons/pos_stock/static/src/app/components/popups/date_picker_popup/date_picker_popup.xml` (24 lines)
- `addons/pos_stock/static/src/app/components/popups/product_info_popup/product_info_popup.xml` (44 lines)
- `addons/pos_stock/static/src/app/components/popups/select_lot_popup/select_lot_popup.js` (159 lines)
- `addons/pos_stock/static/src/app/components/popups/select_lot_popup/select_lot_popup.scss` (4 lines)
- `addons/pos_stock/static/src/app/components/popups/select_lot_popup/select_lot_popup.xml` (36 lines)
- `addons/pos_stock/static/src/app/components/product_info_banner/product_info_banner.js` (12 lines)
- `addons/pos_stock/static/src/app/components/product_info_banner/product_info_banner.xml` (32 lines)
- `addons/pos_stock/static/src/app/models/accounting/product_template_accounting.js` (30 lines)
- `addons/pos_stock/static/src/app/models/data_service_options.js` (12 lines)
- `addons/pos_stock/static/src/app/models/pos_order.js` (43 lines)
- `addons/pos_stock/static/src/app/models/pos_order_line.js` (133 lines)
- `addons/pos_stock/static/src/app/models/product_template.js` (17 lines)
- `addons/pos_stock/static/src/app/screens/payment_screen/payment_screen.js` (24 lines)
- `addons/pos_stock/static/src/app/screens/payment_screen/payment_screen.xml` (15 lines)
- `addons/pos_stock/static/src/app/screens/product_screen/order_summary/order_summary.js` (18 lines)
- `addons/pos_stock/static/src/app/screens/product_screen/order_summary/order_summary.xml` (15 lines)
- `addons/pos_stock/static/src/app/screens/ticket_screen/ticket_screen.js` (22 lines)
- `addons/pos_stock/static/src/app/services/pos_store.js` (310 lines)
- `addons/pos_stock/static/src/app/utils/generate_printer_data.js` (22 lines)
- `addons/pos_stock/static/src/app/utils/order_payment_validation.js` (49 lines)
- `addons/pos_stock/static/src/customer_display/customer_display.xml` (8 lines)
- `addons/pos_stock/static/tests/pos/tours/OrderWithLots_tour.js` (70 lines)
- `addons/pos_stock/static/tests/pos/tours/barcode_scanning_tour.js` (20 lines)
- `addons/pos_stock/static/tests/pos/tours/chrome_tour.js` (50 lines)
- `addons/pos_stock/static/tests/pos/tours/feedback_screen_tour.js` (214 lines)
- `addons/pos_stock/static/tests/pos/tours/order_receipt.js` (55 lines)
- `addons/pos_stock/static/tests/pos/tours/payment_screen_tour.js` (47 lines)
- `addons/pos_stock/static/tests/pos/tours/pos_combo_tour.js` (29 lines)
- `addons/pos_stock/static/tests/pos/tours/product_screen_tour.js` (146 lines)
- `addons/pos_stock/static/tests/pos/tours/shipping_date_tour.js` (34 lines)
- `addons/pos_stock/static/tests/pos/tours/ticket_screen_tour.js` (187 lines)
- `addons/pos_stock/static/tests/pos/tours/utils/feedback_screen_util.js` (42 lines)
- `addons/pos_stock/static/tests/pos/tours/utils/payment_screen_util.js` (46 lines)
- `addons/pos_stock/static/tests/pos/tours/utils/product_screen_util.js` (169 lines)
- `addons/pos_stock/static/tests/unit/accounting/price.test.js` (54 lines)
- `addons/pos_stock/static/tests/unit/components/payment_screen.test.js` (44 lines)
- `addons/pos_stock/static/tests/unit/components/popup/select_lot_popup.test.js` (45 lines)
- `addons/pos_stock/static/tests/unit/customer_display/customer_display.test.js` (32 lines)
- `addons/pos_stock/static/tests/unit/data/decimal_precision.data.js` (13 lines)
- `addons/pos_stock/static/tests/unit/data/generate_model_definitions.js` (19 lines)
- `addons/pos_stock/static/tests/unit/data/pos_config.data.js` (10 lines)
- `addons/pos_stock/static/tests/unit/data/pos_order.data.js` (27 lines)
- `addons/pos_stock/static/tests/unit/data/pos_order_line.data.js` (8 lines)
- `addons/pos_stock/static/tests/unit/data/pos_pack_operation_lot.data.js` (13 lines)
- `addons/pos_stock/static/tests/unit/data/pos_session.data.js` (25 lines)
- `addons/pos_stock/static/tests/unit/data/product_pricelist.data.js` (11 lines)
- `addons/pos_stock/static/tests/unit/data/product_pricelist_item.data.js` (21 lines)
- `addons/pos_stock/static/tests/unit/data/product_product.data.js` (41 lines)
- `addons/pos_stock/static/tests/unit/data/product_template.data.js` (114 lines)
- `addons/pos_stock/static/tests/unit/data/stock_picking_type.data.js` (18 lines)
- `addons/pos_stock/static/tests/unit/data/stock_route.data.js` (9 lines)
- `addons/pos_stock/static/tests/unit/data/stock_warehouse.data.js` (9 lines)
- `addons/pos_stock/static/tests/unit/models/pos_order_line.test.js` (93 lines)
- `addons/pos_stock/static/tests/unit/related_models/orm_serialization.test.js` (115 lines)
- `addons/pos_stock/tests/__init__.py` (14 lines)
- `addons/pos_stock/tests/common.py` (86 lines)
- `addons/pos_stock/tests/test_anglo_saxon.py` (560 lines)
- `addons/pos_stock/tests/test_continental.py` (112 lines)
- `addons/pos_stock/tests/test_frontend.py` (474 lines)
- `addons/pos_stock/tests/test_pos_accounting.py` (146 lines)
- `addons/pos_stock/tests/test_pos_picking_backorder.py` (66 lines)
- `addons/pos_stock/tests/test_pos_stock.py` (18 lines)
- `addons/pos_stock/tests/test_pos_stock_account.py` (299 lines)
- `addons/pos_stock/tests/test_pos_stock_basic_config.py` (82 lines)
- `addons/pos_stock/tests/test_pos_stock_flow.py` (1,721 lines)
- `addons/pos_stock/tests/test_pos_stock_margin.py` (157 lines)
- `addons/pos_stock/tests/test_pos_stock_order_receipt.py` (30 lines)
- `addons/pos_stock/tests/test_pos_stock_other_currency_config.py` (120 lines)
- `addons/pos_stock/tests/test_pos_stock_products_with_tax.py` (209 lines)
- `addons/pos_stock/tests/test_res_config_settings.py` (32 lines)
- `addons/pos_stock/views/pos_config_view.xml` (15 lines)
- `addons/pos_stock/views/pos_order_view.xml` (27 lines)
- `addons/pos_stock/views/pos_session_view.xml` (18 lines)
- `addons/pos_stock/views/product_view.xml` (15 lines)
- `addons/pos_stock/views/res_config_settings_views.xml` (39 lines)
- `addons/pos_stock/views/stock_reference_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
