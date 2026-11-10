# Module: stock_delivery

- **Module ID:** MOD-561
- **Path:** `addons/stock_delivery`
- **Manifest:** `addons/stock_delivery/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['sale_stock', 'delivery']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows you to add delivery methods in pickings.
===============================================

When creating invoices from picking, the system is able to add and compute the shipping line.


Declared dependencies: `printer`, `sale_stock`, `delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 30 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 21 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "printer",
    "sale_stock",
    "delivery"
  ],
  "data": [
    "data/mail_template_data.xml",
    "report/shipping_reports.xml",
    "views/ir_actions_report.xml",
    "views/product_template_view.xml",
    "views/product_product_view.xml",
    "views/delivery_view.xml",
    "views/delivery_portal_template.xml",
    "views/report_shipping.xml",
    "views/report_deliveryslip.xml",
    "views/report_package_barcode.xml",
    "wizard/choose_delivery_carrier_views.xml",
    "wizard/pay_on_delivery_views.xml",
    "wizard/stock_put_in_pack_views.xml",
    "views/stock_package_type_views.xml",
    "views/stock_picking_type_views.xml",
    "views/stock_rule_views.xml",
    "views/stock_move_line_views.xml",
    "views/stock_menu_views.xml",
    "report/product_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/delivery_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "stock_delivery/static/src/return_order_dialog/*"
    ],
    "web.assets_tests": [
      [
        "include",
        "printer.assets_tests"
      ]
    ]
  }
}
```

### Representative source files

- `addons/stock_delivery/__init__.py` (16 lines)
- `addons/stock_delivery/__manifest__.py` (49 lines)
- `addons/stock_delivery/data/delivery_demo.xml` (89 lines)
- `addons/stock_delivery/data/mail_template_data.xml` (8 lines)
- `addons/stock_delivery/i18n/ar.po` (963 lines)
- `addons/stock_delivery/i18n/az.po` (910 lines)
- `addons/stock_delivery/i18n/bg.po` (910 lines)
- `addons/stock_delivery/i18n/bs.po` (912 lines)
- `addons/stock_delivery/i18n/ca.po` (957 lines)
- `addons/stock_delivery/i18n/cs.po` (943 lines)
- `addons/stock_delivery/i18n/da.po` (927 lines)
- `addons/stock_delivery/i18n/de.po` (1,008 lines)
- `addons/stock_delivery/i18n/el.po` (919 lines)
- `addons/stock_delivery/i18n/es.po` (973 lines)
- `addons/stock_delivery/i18n/es_419.po` (985 lines)
- `addons/stock_delivery/i18n/et.po` (963 lines)
- `addons/stock_delivery/i18n/fa.po` (910 lines)
- `addons/stock_delivery/i18n/fi.po` (966 lines)
- `addons/stock_delivery/i18n/fr.po` (994 lines)
- `addons/stock_delivery/i18n/he.po` (911 lines)
- `addons/stock_delivery/i18n/hi.po` (910 lines)
- `addons/stock_delivery/i18n/hr.po` (911 lines)
- `addons/stock_delivery/i18n/hu.po` (928 lines)
- `addons/stock_delivery/i18n/id.po` (959 lines)
- `addons/stock_delivery/i18n/it.po` (985 lines)
- `addons/stock_delivery/i18n/ja.po` (961 lines)
- `addons/stock_delivery/i18n/kab.po` (911 lines)
- `addons/stock_delivery/i18n/ko.po` (957 lines)
- `addons/stock_delivery/i18n/ku.po` (910 lines)
- `addons/stock_delivery/i18n/lo.po` (954 lines)
- `addons/stock_delivery/i18n/lt.po` (912 lines)
- `addons/stock_delivery/i18n/lv.po` (911 lines)
- `addons/stock_delivery/i18n/mn.po` (910 lines)
- `addons/stock_delivery/i18n/my.po` (911 lines)
- `addons/stock_delivery/i18n/nb.po` (920 lines)
- `addons/stock_delivery/i18n/nl.po` (1,007 lines)
- `addons/stock_delivery/i18n/pl.po` (969 lines)
- `addons/stock_delivery/i18n/pt.po` (957 lines)
- `addons/stock_delivery/i18n/pt_BR.po` (1,001 lines)
- `addons/stock_delivery/i18n/ro.po` (967 lines)
- `addons/stock_delivery/i18n/ru.po` (971 lines)
- `addons/stock_delivery/i18n/sk.po` (910 lines)
- `addons/stock_delivery/i18n/sl.po` (926 lines)
- `addons/stock_delivery/i18n/sr@latin.po` (911 lines)
- `addons/stock_delivery/i18n/stock_delivery.pot` (899 lines)
- `addons/stock_delivery/i18n/sv.po` (954 lines)
- `addons/stock_delivery/i18n/th.po` (946 lines)
- `addons/stock_delivery/i18n/tr.po` (967 lines)
- `addons/stock_delivery/i18n/uk.po` (911 lines)
- `addons/stock_delivery/i18n/uz.po` (1,059 lines)
- `addons/stock_delivery/i18n/vi.po` (958 lines)
- `addons/stock_delivery/i18n/zh_CN.po` (955 lines)
- `addons/stock_delivery/i18n/zh_TW.po` (952 lines)
- `addons/stock_delivery/models/__init__.py` (14 lines)
- `addons/stock_delivery/models/delivery_carrier.py` (283 lines)
- `addons/stock_delivery/models/delivery_request_objects.py` (31 lines)
- `addons/stock_delivery/models/ir_actions_report.py` (87 lines)
- `addons/stock_delivery/models/product_product.py` (17 lines)
- `addons/stock_delivery/models/product_template.py` (40 lines)
- `addons/stock_delivery/models/res_partner.py` (12 lines)
- `addons/stock_delivery/models/sale_order.py` (56 lines)
- `addons/stock_delivery/models/stock_move.py` (154 lines)
- `addons/stock_delivery/models/stock_package.py` (53 lines)
- `addons/stock_delivery/models/stock_package_type.py` (33 lines)
- `addons/stock_delivery/models/stock_picking.py` (327 lines)
- `addons/stock_delivery/models/stock_picking_batch.py` (23 lines)
- `addons/stock_delivery/models/stock_picking_type.py` (35 lines)
- `addons/stock_delivery/report/product_templates.xml` (17 lines)
- `addons/stock_delivery/report/shipping_reports.xml` (24 lines)
- `addons/stock_delivery/security/ir.access.csv` (11 lines)
- `addons/stock_delivery/static/src/return_order_dialog/return_label_info.xml` (13 lines)
- `addons/stock_delivery/static/src/return_order_dialog/return_order_dialog.js` (55 lines)
- `addons/stock_delivery/tests/__init__.py` (9 lines)
- `addons/stock_delivery/tests/test_carrier_propagation.py` (376 lines)
- `addons/stock_delivery/tests/test_delivery_cost.py` (126 lines)
- `addons/stock_delivery/tests/test_delivery_picking_batch.py` (123 lines)
- `addons/stock_delivery/tests/test_delivery_stock_move.py` (347 lines)
- `addons/stock_delivery/tests/test_packing_delivery.py` (555 lines)
- `addons/stock_delivery/tests/test_pay_on_delivery.py` (110 lines)
- `addons/stock_delivery/tests/test_printer_tour.py` (86 lines)
- `addons/stock_delivery/views/delivery_portal_template.xml` (29 lines)
- `addons/stock_delivery/views/delivery_view.xml` (139 lines)
- `addons/stock_delivery/views/ir_actions_report.xml` (21 lines)
- `addons/stock_delivery/views/product_product_view.xml` (27 lines)
- `addons/stock_delivery/views/product_template_view.xml` (16 lines)
- `addons/stock_delivery/views/report_deliveryslip.xml` (78 lines)
- `addons/stock_delivery/views/report_package_barcode.xml` (49 lines)
- `addons/stock_delivery/views/report_shipping.xml` (17 lines)
- `addons/stock_delivery/views/stock_menu_views.xml` (17 lines)
- `addons/stock_delivery/views/stock_move_line_views.xml` (27 lines)
- `addons/stock_delivery/views/stock_package_type_views.xml` (30 lines)
- `addons/stock_delivery/views/stock_picking_type_views.xml` (48 lines)
- `addons/stock_delivery/views/stock_rule_views.xml` (15 lines)
- `addons/stock_delivery/wizard/__init__.py` (7 lines)
- `addons/stock_delivery/wizard/choose_delivery_carrier.py` (13 lines)
- `addons/stock_delivery/wizard/choose_delivery_carrier_views.xml` (17 lines)
- `addons/stock_delivery/wizard/pay_on_delivery.py` (44 lines)
- `addons/stock_delivery/wizard/pay_on_delivery_views.xml` (27 lines)
- `addons/stock_delivery/wizard/product_label_layout.py` (12 lines)
- `addons/stock_delivery/wizard/stock_package_label_layout.py` (26 lines)
- `addons/stock_delivery/wizard/stock_put_in_pack.py` (54 lines)
- `addons/stock_delivery/wizard/stock_put_in_pack_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
