# Module: sale_stock

- **Module ID:** MOD-533
- **Path:** `addons/sale_stock`
- **Manifest:** `addons/sale_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Quotation, Sales Orders, Delivery & Invoicing Control


Manage sales quotations and orders
==================================

This module makes the link between the sales and warehouses management applications.

Preferences
-----------
* Shipping: Choice of delivery at once or partial delivery
* Invoicing: choose how invoices will be paid
* Incoterms: International Commercial terms



Declared dependencies: `sale`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 40 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 24 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 17 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "stock_account"
  ],
  "data": [
    "views/product_views.xml",
    "views/sale_order_views.xml",
    "views/sale_order_line_views.xml",
    "views/stock_route_views.xml",
    "views/return_reason_views.xml",
    "views/res_config_settings_views.xml",
    "views/sale_stock_portal_template.xml",
    "views/stock_lot_views.xml",
    "views/res_users_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_reference_views.xml",
    "report/stock_report_deliveryslip.xml",
    "report/return_label.xml",
    "data/mail_templates.xml",
    "data/return_reason_data.xml",
    "data/sale_stock_data.xml",
    "wizard/stock_replenishment_info.xml",
    "wizard/stock_rules_report_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/sale_order_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_stock/static/src/**/*",
      [
        "remove",
        "sale_stock/static/src/interactions/*"
      ],
      [
        "remove",
        "sale_stock/static/src/return_order_dialog/*"
      ]
    ],
    "web.assets_frontend": [
      "sale/static/src/js/quantity_buttons/*",
      "sale_stock/static/src/interactions/*",
      "sale_stock/static/src/return_order_dialog/*"
    ],
    "web.assets_tests": [
      "sale_stock/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/sale_stock/__init__.py` (48 lines)
- `addons/sale_stock/__manifest__.py` (67 lines)
- `addons/sale_stock/controllers/__init__.py` (4 lines)
- `addons/sale_stock/controllers/portal.py` (51 lines)
- `addons/sale_stock/controllers/return_order.py` (156 lines)
- `addons/sale_stock/data/mail_templates.xml` (57 lines)
- `addons/sale_stock/data/return_reason_data.xml` (25 lines)
- `addons/sale_stock/data/sale_order_demo.xml` (167 lines)
- `addons/sale_stock/data/sale_stock_data.xml` (8 lines)
- `addons/sale_stock/i18n/af.po` (1,025 lines)
- `addons/sale_stock/i18n/am.po` (1,021 lines)
- `addons/sale_stock/i18n/ar.po` (1,052 lines)
- `addons/sale_stock/i18n/az.po` (1,001 lines)
- `addons/sale_stock/i18n/bg.po` (1,029 lines)
- `addons/sale_stock/i18n/bs.po` (1,050 lines)
- `addons/sale_stock/i18n/ca.po` (1,061 lines)
- `addons/sale_stock/i18n/cs.po` (1,041 lines)
- `addons/sale_stock/i18n/da.po` (1,057 lines)
- `addons/sale_stock/i18n/de.po` (1,096 lines)
- `addons/sale_stock/i18n/el.po` (1,012 lines)
- `addons/sale_stock/i18n/es.po` (1,089 lines)
- `addons/sale_stock/i18n/es_419.po` (1,081 lines)
- `addons/sale_stock/i18n/es_CL.po` (53 lines)
- `addons/sale_stock/i18n/et.po` (1,069 lines)
- `addons/sale_stock/i18n/eu.po` (1,023 lines)
- `addons/sale_stock/i18n/fa.po` (1,067 lines)
- `addons/sale_stock/i18n/fi.po` (1,094 lines)
- `addons/sale_stock/i18n/fo.po` (1,023 lines)
- `addons/sale_stock/i18n/fr.po` (1,080 lines)
- `addons/sale_stock/i18n/fr_CA.po` (30 lines)
- `addons/sale_stock/i18n/gl.po` (1,023 lines)
- `addons/sale_stock/i18n/gu.po` (1,025 lines)
- `addons/sale_stock/i18n/he.po` (1,046 lines)
- `addons/sale_stock/i18n/hi.po` (1,103 lines)
- `addons/sale_stock/i18n/hr.po` (1,093 lines)
- `addons/sale_stock/i18n/hu.po` (1,073 lines)
- `addons/sale_stock/i18n/id.po` (1,081 lines)
- `addons/sale_stock/i18n/is.po` (1,025 lines)
- `addons/sale_stock/i18n/it.po` (1,086 lines)
- `addons/sale_stock/i18n/ja.po` (1,057 lines)
- `addons/sale_stock/i18n/kab.po` (1,015 lines)
- `addons/sale_stock/i18n/km.po` (1,024 lines)
- `addons/sale_stock/i18n/ko.po` (1,061 lines)
- `addons/sale_stock/i18n/ku.po` (986 lines)
- `addons/sale_stock/i18n/lo.po` (1,048 lines)
- `addons/sale_stock/i18n/lt.po` (1,043 lines)
- `addons/sale_stock/i18n/lv.po` (1,027 lines)
- `addons/sale_stock/i18n/mk.po` (1,028 lines)
- `addons/sale_stock/i18n/mn.po` (1,060 lines)
- `addons/sale_stock/i18n/my.po` (1,003 lines)
- `addons/sale_stock/i18n/nb.po` (1,029 lines)
- `addons/sale_stock/i18n/nl.po` (1,088 lines)
- `addons/sale_stock/i18n/pl.po` (1,077 lines)
- `addons/sale_stock/i18n/pt.po` (1,053 lines)
- `addons/sale_stock/i18n/pt_BR.po` (1,091 lines)
- `addons/sale_stock/i18n/ro.po` (1,065 lines)
- `addons/sale_stock/i18n/ru.po` (1,070 lines)
- `addons/sale_stock/i18n/sale_stock.pot` (976 lines)
- `addons/sale_stock/i18n/sk.po` (1,096 lines)
- `addons/sale_stock/i18n/sl.po` (1,026 lines)
- `addons/sale_stock/i18n/sr@latin.po` (994 lines)
- `addons/sale_stock/i18n/sv.po` (1,070 lines)
- `addons/sale_stock/i18n/th.po` (1,065 lines)
- `addons/sale_stock/i18n/tr.po` (1,074 lines)
- `addons/sale_stock/i18n/uk.po` (1,058 lines)
- `addons/sale_stock/i18n/uz.po` (1,147 lines)
- `addons/sale_stock/i18n/vi.po` (1,066 lines)
- `addons/sale_stock/i18n/zh_CN.po` (1,078 lines)
- `addons/sale_stock/i18n/zh_TW.po` (1,051 lines)
- `addons/sale_stock/models/__init__.py` (12 lines)
- `addons/sale_stock/models/account_move.py` (143 lines)
- `addons/sale_stock/models/product_template.py` (18 lines)
- `addons/sale_stock/models/res_company.py` (17 lines)
- `addons/sale_stock/models/res_config_settings.py` (23 lines)
- `addons/sale_stock/models/res_users.py` (14 lines)
- `addons/sale_stock/models/return_reason.py` (12 lines)
- `addons/sale_stock/models/sale_order.py` (357 lines)
- `addons/sale_stock/models/sale_order_line.py` (468 lines)
- `addons/sale_stock/models/stock.py` (440 lines)
- `addons/sale_stock/models/stock_reference.py` (9 lines)
- `addons/sale_stock/report/__init__.py` (5 lines)
- `addons/sale_stock/report/report_stock_rule.py` (15 lines)
- `addons/sale_stock/report/return_label.xml` (104 lines)
- `addons/sale_stock/report/sale_report.py` (12 lines)
- `addons/sale_stock/report/stock_forecasted.py` (55 lines)
- `addons/sale_stock/report/stock_report_deliveryslip.xml` (19 lines)
- `addons/sale_stock/security/ir.access.csv` (19 lines)
- `addons/sale_stock/static/src/interactions/return_order.js` (22 lines)
- `addons/sale_stock/static/src/product_catalog/kanban_record.js` (29 lines)
- `addons/sale_stock/static/src/product_catalog/sale_order_line/sale_order_line.js` (22 lines)
- `addons/sale_stock/static/src/return_order_dialog/return_label_info.xml` (19 lines)
- `addons/sale_stock/static/src/return_order_dialog/return_order_dialog.js` (146 lines)
- `addons/sale_stock/static/src/return_order_dialog/return_order_dialog.scss` (16 lines)
- `addons/sale_stock/static/src/return_order_dialog/return_order_dialog.xml` (86 lines)
- `addons/sale_stock/static/src/sale_stock_forecasted/forecasted_details.xml` (34 lines)
- `addons/sale_stock/static/src/widgets/qty_at_date_widget.js` (140 lines)
- `addons/sale_stock/static/src/widgets/qty_at_date_widget.xml` (81 lines)
- `addons/sale_stock/static/src/xml/delay_alert.xml` (9 lines)
- `addons/sale_stock/static/tests/tours/barcode_duplication_tour.js` (26 lines)
- `addons/sale_stock/tests/__init__.py` (18 lines)
- `addons/sale_stock/tests/common.py` (59 lines)
- `addons/sale_stock/tests/test_analytic_to_sale_stock.py` (64 lines)
- `addons/sale_stock/tests/test_anglo_saxon_valuation.py` (1,826 lines)
- `addons/sale_stock/tests/test_anglo_saxon_valuation_reconciliation.py` (216 lines)
- `addons/sale_stock/tests/test_anglosaxon_account.py` (42 lines)
- `addons/sale_stock/tests/test_create_perf.py` (183 lines)
- `addons/sale_stock/tests/test_packaging_tours.py` (29 lines)
- `addons/sale_stock/tests/test_return_order.py` (166 lines)
- `addons/sale_stock/tests/test_sale_order_dates.py` (290 lines)
- `addons/sale_stock/tests/test_sale_stock.py` (2,994 lines)
- `addons/sale_stock/tests/test_sale_stock_access_rights.py` (52 lines)
- `addons/sale_stock/tests/test_sale_stock_accrued_entries.py` (1,074 lines)
- `addons/sale_stock/tests/test_sale_stock_lead_time.py` (294 lines)
- `addons/sale_stock/tests/test_sale_stock_multi_warehouse.py` (63 lines)
- `addons/sale_stock/tests/test_sale_stock_multicompany.py` (322 lines)
- `addons/sale_stock/tests/test_sale_stock_report.py` (780 lines)
- `addons/sale_stock/views/product_views.xml` (12 lines)
- `addons/sale_stock/views/res_config_settings_views.xml` (49 lines)
- `addons/sale_stock/views/res_users_views.xml` (40 lines)
- `addons/sale_stock/views/return_reason_views.xml` (23 lines)
- `addons/sale_stock/views/sale_order_line_views.xml` (15 lines)
- `addons/sale_stock/views/sale_order_views.xml` (113 lines)
- `addons/sale_stock/views/sale_stock_portal_template.xml` (112 lines)
- `addons/sale_stock/views/stock_lot_views.xml` (22 lines)
- `addons/sale_stock/views/stock_picking_views.xml` (102 lines)
- `addons/sale_stock/views/stock_reference_views.xml` (13 lines)
- `addons/sale_stock/views/stock_route_views.xml` (15 lines)
- `addons/sale_stock/wizard/__init__.py` (4 lines)
- `addons/sale_stock/wizard/stock_replenishment_info.py` (19 lines)
- `addons/sale_stock/wizard/stock_replenishment_info.xml` (17 lines)
- `addons/sale_stock/wizard/stock_rules_report.py` (16 lines)
- `addons/sale_stock/wizard/stock_rules_report_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
