# Module: pos_sale

- **Module ID:** MOD-450
- **Path:** `addons/pos_sale`
- **Manifest:** `addons/pos_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and Sales



This module adds a custom Sales Team for the Point of Sale. This enables you to view and manage your point of sale sales with more ease.


Declared dependencies: `point_of_sale`, `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 30 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "sale_management"
  ],
  "data": [
    "data/pos_sale_data.xml",
    "views/point_of_sale_report.xml",
    "views/sale_order_views.xml",
    "views/pos_order_views.xml",
    "views/sales_team_views.xml",
    "views/res_config_settings_views.xml",
    "receipt/pos_order_receipt.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_sale/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_sale/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_sale/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_sale/__init__.py` (6 lines)
- `addons/pos_sale/__manifest__.py` (39 lines)
- `addons/pos_sale/data/pos_sale_data.xml` (34 lines)
- `addons/pos_sale/i18n/ar.po` (485 lines)
- `addons/pos_sale/i18n/az.po` (461 lines)
- `addons/pos_sale/i18n/bg.po` (457 lines)
- `addons/pos_sale/i18n/bs.po` (461 lines)
- `addons/pos_sale/i18n/ca.po` (482 lines)
- `addons/pos_sale/i18n/cs.po` (489 lines)
- `addons/pos_sale/i18n/da.po` (472 lines)
- `addons/pos_sale/i18n/de.po` (517 lines)
- `addons/pos_sale/i18n/el.po` (462 lines)
- `addons/pos_sale/i18n/es.po` (517 lines)
- `addons/pos_sale/i18n/es_419.po` (507 lines)
- `addons/pos_sale/i18n/et.po` (477 lines)
- `addons/pos_sale/i18n/fa.po` (467 lines)
- `addons/pos_sale/i18n/fi.po` (500 lines)
- `addons/pos_sale/i18n/fr.po` (515 lines)
- `addons/pos_sale/i18n/gu.po` (488 lines)
- `addons/pos_sale/i18n/he.po` (474 lines)
- `addons/pos_sale/i18n/hi.po` (457 lines)
- `addons/pos_sale/i18n/hr.po` (469 lines)
- `addons/pos_sale/i18n/hu.po` (469 lines)
- `addons/pos_sale/i18n/id.po` (504 lines)
- `addons/pos_sale/i18n/is.po` (487 lines)
- `addons/pos_sale/i18n/it.po` (514 lines)
- `addons/pos_sale/i18n/ja.po` (496 lines)
- `addons/pos_sale/i18n/kab.po` (458 lines)
- `addons/pos_sale/i18n/km.po` (488 lines)
- `addons/pos_sale/i18n/ko.po` (476 lines)
- `addons/pos_sale/i18n/ku.po` (457 lines)
- `addons/pos_sale/i18n/lo.po` (470 lines)
- `addons/pos_sale/i18n/lt.po` (468 lines)
- `addons/pos_sale/i18n/lv.po` (471 lines)
- `addons/pos_sale/i18n/mn.po` (467 lines)
- `addons/pos_sale/i18n/my.po` (458 lines)
- `addons/pos_sale/i18n/nb.po` (464 lines)
- `addons/pos_sale/i18n/nl.po` (509 lines)
- `addons/pos_sale/i18n/pl.po` (512 lines)
- `addons/pos_sale/i18n/pos_sale.pot` (453 lines)
- `addons/pos_sale/i18n/pt.po` (476 lines)
- `addons/pos_sale/i18n/pt_BR.po` (520 lines)
- `addons/pos_sale/i18n/ro.po` (482 lines)
- `addons/pos_sale/i18n/ru.po` (484 lines)
- `addons/pos_sale/i18n/sk.po` (466 lines)
- `addons/pos_sale/i18n/sl.po` (467 lines)
- `addons/pos_sale/i18n/sr@latin.po` (463 lines)
- `addons/pos_sale/i18n/sv.po` (474 lines)
- `addons/pos_sale/i18n/th.po` (469 lines)
- `addons/pos_sale/i18n/tr.po` (496 lines)
- `addons/pos_sale/i18n/uk.po` (472 lines)
- `addons/pos_sale/i18n/uz.po` (550 lines)
- `addons/pos_sale/i18n/vi.po` (484 lines)
- `addons/pos_sale/i18n/zh_CN.po` (501 lines)
- `addons/pos_sale/i18n/zh_TW.po` (479 lines)
- `addons/pos_sale/models/__init__.py` (14 lines)
- `addons/pos_sale/models/account_move.py` (35 lines)
- `addons/pos_sale/models/account_move_line.py` (46 lines)
- `addons/pos_sale/models/crm_team.py` (7 lines)
- `addons/pos_sale/models/pos_config.py` (80 lines)
- `addons/pos_sale/models/pos_order.py` (168 lines)
- `addons/pos_sale/models/pos_order_line.py` (54 lines)
- `addons/pos_sale/models/pos_session.py` (16 lines)
- `addons/pos_sale/models/product_template.py` (11 lines)
- `addons/pos_sale/models/res_config_settings.py` (11 lines)
- `addons/pos_sale/models/res_partner.py` (9 lines)
- `addons/pos_sale/models/sale_order.py` (253 lines)
- `addons/pos_sale/receipt/__init__.py` (1 lines)
- `addons/pos_sale/receipt/pos_order_receipt.py` (16 lines)
- `addons/pos_sale/receipt/pos_order_receipt.xml` (23 lines)
- `addons/pos_sale/report/__init__.py` (4 lines)
- `addons/pos_sale/report/sale_report.py` (110 lines)
- `addons/pos_sale/security/ir.access.csv` (4 lines)
- `addons/pos_sale/static/src/app/components/orderline/orderline.scss` (4 lines)
- `addons/pos_sale/static/src/app/components/orderline/orderline.xml` (21 lines)
- `addons/pos_sale/static/src/app/components/screens/product_screen/control_buttons/control_buttons.js` (43 lines)
- `addons/pos_sale/static/src/app/components/screens/product_screen/control_buttons/control_buttons.xml` (15 lines)
- `addons/pos_sale/static/src/app/models/data_service_options.js` (28 lines)
- `addons/pos_sale/static/src/app/models/pos_order.js` (13 lines)
- `addons/pos_sale/static/src/app/models/pos_order_line.js` (54 lines)
- `addons/pos_sale/static/src/app/services/pos_store.js` (423 lines)
- `addons/pos_sale/static/src/app/utils/order_payment_validation.js` (18 lines)
- `addons/pos_sale/static/src/app/utils/printer/generate_printer_data.js` (17 lines)
- `addons/pos_sale/static/src/css/popups/product_info_popup.css` (16 lines)
- `addons/pos_sale/static/tests/tours/pos_sale_tour.js` (126 lines)
- `addons/pos_sale/static/tests/tours/test_taxes_downpayment.js` (337 lines)
- `addons/pos_sale/static/tests/tours/utils/pos_sale_utils.js` (74 lines)
- `addons/pos_sale/static/tests/unit/components/orderline.test.js` (55 lines)
- `addons/pos_sale/static/tests/unit/data/account_tax.data.js` (36 lines)
- `addons/pos_sale/static/tests/unit/data/pos_config.data.js` (12 lines)
- `addons/pos_sale/static/tests/unit/data/pos_order_line.data.js` (13 lines)
- `addons/pos_sale/static/tests/unit/data/pos_session.data.js` (8 lines)
- `addons/pos_sale/static/tests/unit/data/product_attribute.data.js` (11 lines)
- `addons/pos_sale/static/tests/unit/data/product_attribute_custom_value.data.js` (10 lines)
- `addons/pos_sale/static/tests/unit/data/product_product.data.js` (53 lines)
- `addons/pos_sale/static/tests/unit/data/product_template.data.js` (144 lines)
- `addons/pos_sale/static/tests/unit/data/product_template_attribute_line.data.js` (11 lines)
- `addons/pos_sale/static/tests/unit/data/product_template_attribute_value.data.js` (17 lines)
- `addons/pos_sale/static/tests/unit/data/res_partner.data.js` (8 lines)
- `addons/pos_sale/static/tests/unit/data/sale_order.data.js` (364 lines)
- `addons/pos_sale/static/tests/unit/data/sale_order_line.data.js` (593 lines)
- `addons/pos_sale/static/tests/unit/models/pos_order_line.test.js` (87 lines)
- `addons/pos_sale/static/tests/unit/scenarios/pos_sale_flow.test.js` (308 lines)
- `addons/pos_sale/static/tests/unit/scenarios/quotation_list_flow.test.js` (74 lines)
- `addons/pos_sale/static/tests/unit/scenarios/sale_warning_flow.test.js` (49 lines)
- `addons/pos_sale/static/tests/unit/services/pos_store.test.js` (276 lines)
- `addons/pos_sale/static/tests/unit/ui_utils.js` (66 lines)
- `addons/pos_sale/tests/__init__.py` (6 lines)
- `addons/pos_sale/tests/test_pos_sale_flow.py` (1,712 lines)
- `addons/pos_sale/tests/test_pos_sale_report.py` (150 lines)
- `addons/pos_sale/tests/test_taxes_downpayment.py` (161 lines)
- `addons/pos_sale/views/point_of_sale_report.xml` (19 lines)
- `addons/pos_sale/views/pos_order_views.xml` (41 lines)
- `addons/pos_sale/views/res_config_settings_views.xml` (40 lines)
- `addons/pos_sale/views/sale_order_views.xml` (28 lines)
- `addons/pos_sale/views/sales_team_views.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
