# Module: purchase_stock

- **Module ID:** MOD-503
- **Path:** `addons/purchase_stock`
- **Manifest:** `addons/purchase_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Purchase Orders, Receipts, Vendor Bills for Stock

No manifest description declared.

Declared dependencies: `stock_account`, `purchase`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 48 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 22 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 16 | Client behavior/assets. |
| Tests | 24 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock_account",
    "purchase"
  ],
  "data": [
    "data/purchase_stock_data.xml",
    "data/mail_templates.xml",
    "report/vendor_delay_report.xml",
    "views/purchase_views.xml",
    "views/stock_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_rule_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/stock_lot_views.xml",
    "views/stock_orderpoint_views.xml",
    "views/stock_reference_views.xml",
    "views/product_views.xml",
    "report/purchase_report_views.xml",
    "report/purchase_report_templates.xml",
    "report/report_stock_rule.xml",
    "wizard/stock_replenishment_info.xml",
    "wizard/product_replenish_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/purchase_stock_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "purchase_stock/static/src/**/*"
    ],
    "web.assets_tests": [
      "purchase_stock/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "purchase_stock/static/tests/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/purchase_stock/__init__.py` (61 lines)
- `addons/purchase_stock/__manifest__.py` (50 lines)
- `addons/purchase_stock/data/mail_templates.xml` (49 lines)
- `addons/purchase_stock/data/purchase_stock_data.xml` (25 lines)
- `addons/purchase_stock/data/purchase_stock_demo.xml` (1,264 lines)
- `addons/purchase_stock/i18n/ar.po` (1,356 lines)
- `addons/purchase_stock/i18n/az.po` (1,300 lines)
- `addons/purchase_stock/i18n/bg.po` (1,317 lines)
- `addons/purchase_stock/i18n/bs.po` (1,289 lines)
- `addons/purchase_stock/i18n/ca.po` (1,349 lines)
- `addons/purchase_stock/i18n/cs.po` (1,362 lines)
- `addons/purchase_stock/i18n/da.po` (1,346 lines)
- `addons/purchase_stock/i18n/de.po` (1,394 lines)
- `addons/purchase_stock/i18n/el.po` (1,309 lines)
- `addons/purchase_stock/i18n/es.po` (1,372 lines)
- `addons/purchase_stock/i18n/es_419.po` (1,378 lines)
- `addons/purchase_stock/i18n/et.po` (1,381 lines)
- `addons/purchase_stock/i18n/fa.po` (1,323 lines)
- `addons/purchase_stock/i18n/fi.po` (1,383 lines)
- `addons/purchase_stock/i18n/fr.po` (1,379 lines)
- `addons/purchase_stock/i18n/gu.po` (1,287 lines)
- `addons/purchase_stock/i18n/he.po` (1,339 lines)
- `addons/purchase_stock/i18n/hi.po` (1,295 lines)
- `addons/purchase_stock/i18n/hr.po` (1,324 lines)
- `addons/purchase_stock/i18n/hu.po` (1,320 lines)
- `addons/purchase_stock/i18n/id.po` (1,366 lines)
- `addons/purchase_stock/i18n/is.po` (1,287 lines)
- `addons/purchase_stock/i18n/it.po` (1,376 lines)
- `addons/purchase_stock/i18n/ja.po` (1,363 lines)
- `addons/purchase_stock/i18n/kab.po` (1,286 lines)
- `addons/purchase_stock/i18n/ko.po` (1,335 lines)
- `addons/purchase_stock/i18n/ku.po` (1,292 lines)
- `addons/purchase_stock/i18n/lo.po` (1,330 lines)
- `addons/purchase_stock/i18n/lt.po` (1,321 lines)
- `addons/purchase_stock/i18n/lv.po` (1,286 lines)
- `addons/purchase_stock/i18n/mn.po` (1,376 lines)
- `addons/purchase_stock/i18n/my.po` (1,297 lines)
- `addons/purchase_stock/i18n/nb.po` (1,315 lines)
- `addons/purchase_stock/i18n/nl.po` (1,379 lines)
- `addons/purchase_stock/i18n/pl.po` (1,385 lines)
- `addons/purchase_stock/i18n/pt.po` (1,347 lines)
- `addons/purchase_stock/i18n/pt_BR.po` (1,381 lines)
- `addons/purchase_stock/i18n/purchase_stock.pot` (1,275 lines)
- `addons/purchase_stock/i18n/ro.po` (1,353 lines)
- `addons/purchase_stock/i18n/ru.po` (1,367 lines)
- `addons/purchase_stock/i18n/sk.po` (1,307 lines)
- `addons/purchase_stock/i18n/sl.po` (1,304 lines)
- `addons/purchase_stock/i18n/sr@latin.po` (1,294 lines)
- `addons/purchase_stock/i18n/sv.po` (1,338 lines)
- `addons/purchase_stock/i18n/th.po` (1,344 lines)
- `addons/purchase_stock/i18n/tr.po` (1,372 lines)
- `addons/purchase_stock/i18n/uk.po` (1,333 lines)
- `addons/purchase_stock/i18n/uz.po` (1,536 lines)
- `addons/purchase_stock/i18n/vi.po` (1,358 lines)
- `addons/purchase_stock/i18n/zh_CN.po` (1,345 lines)
- `addons/purchase_stock/i18n/zh_TW.po` (1,330 lines)
- `addons/purchase_stock/models/__init__.py` (15 lines)
- `addons/purchase_stock/models/account_move_line.py` (15 lines)
- `addons/purchase_stock/models/product.py` (337 lines)
- `addons/purchase_stock/models/purchase_order.py` (475 lines)
- `addons/purchase_stock/models/purchase_order_line.py` (495 lines)
- `addons/purchase_stock/models/res_company.py` (12 lines)
- `addons/purchase_stock/models/res_config_settings.py` (21 lines)
- `addons/purchase_stock/models/res_partner.py` (109 lines)
- `addons/purchase_stock/models/stock.py` (386 lines)
- `addons/purchase_stock/models/stock_move.py` (276 lines)
- `addons/purchase_stock/models/stock_reference.py` (9 lines)
- `addons/purchase_stock/models/stock_replenish_mixin.py` (18 lines)
- `addons/purchase_stock/models/stock_rule.py` (424 lines)
- `addons/purchase_stock/report/__init__.py` (7 lines)
- `addons/purchase_stock/report/purchase_report.py` (46 lines)
- `addons/purchase_stock/report/purchase_report_templates.xml` (36 lines)
- `addons/purchase_stock/report/purchase_report_views.xml` (15 lines)
- `addons/purchase_stock/report/report_stock_rule.py` (17 lines)
- `addons/purchase_stock/report/report_stock_rule.xml` (32 lines)
- `addons/purchase_stock/report/stock_allocation_report.py` (20 lines)
- `addons/purchase_stock/report/stock_forecasted.py` (38 lines)
- `addons/purchase_stock/report/vendor_delay_report.py` (74 lines)
- `addons/purchase_stock/report/vendor_delay_report.xml` (35 lines)
- `addons/purchase_stock/security/ir.access.csv` (10 lines)
- `addons/purchase_stock/static/src/js/tours/purchase_stock.js` (71 lines)
- `addons/purchase_stock/static/src/product_catalog/kanban_controller.js` (62 lines)
- `addons/purchase_stock/static/src/product_catalog/kanban_model.js` (37 lines)
- `addons/purchase_stock/static/src/product_catalog/kanban_renderer.js` (10 lines)
- `addons/purchase_stock/static/src/product_catalog/kanban_view.js` (13 lines)
- `addons/purchase_stock/static/src/product_catalog/record/kanban_record.js` (29 lines)
- `addons/purchase_stock/static/src/product_catalog/record/kanban_record.scss` (3 lines)
- `addons/purchase_stock/static/src/product_catalog/record/purchase_order_line.js` (8 lines)
- `addons/purchase_stock/static/src/product_catalog/search/search_model.js` (138 lines)
- `addons/purchase_stock/static/src/product_catalog/search/search_panel.js` (84 lines)
- `addons/purchase_stock/static/src/product_catalog/search/search_panel.scss` (27 lines)
- `addons/purchase_stock/static/src/product_catalog/search/search_panel.xml` (89 lines)
- `addons/purchase_stock/static/src/product_catalog/search/time_period_selection_fields.js` (63 lines)
- `addons/purchase_stock/static/src/product_catalog/utils.js` (8 lines)
- `addons/purchase_stock/static/src/purchase_dashboard/purchase_dashboard.xml` (20 lines)
- `addons/purchase_stock/static/src/purchase_stock_forecasted/forecasted_details.xml` (22 lines)
- `addons/purchase_stock/static/tests/product_catalog.test.js` (166 lines)
- `addons/purchase_stock/static/tests/purchase_stock.test.js` (72 lines)
- `addons/purchase_stock/static/tests/tours/product_replenishment.js` (58 lines)
- `addons/purchase_stock/static/tests/tours/purchase_catalog_suggest.js` (155 lines)
- `addons/purchase_stock/static/tests/tours/tour_helper.js` (160 lines)
- `addons/purchase_stock/tests/__init__.py` (25 lines)
- `addons/purchase_stock/tests/common.py` (94 lines)
- `addons/purchase_stock/tests/test_account.py` (429 lines)
- `addons/purchase_stock/tests/test_create_picking.py` (996 lines)
- `addons/purchase_stock/tests/test_move_cancel_propagation.py` (269 lines)
- `addons/purchase_stock/tests/test_old_rules.py` (289 lines)
- `addons/purchase_stock/tests/test_onchange_product.py` (118 lines)
- `addons/purchase_stock/tests/test_product_template.py` (51 lines)
- `addons/purchase_stock/tests/test_purchase_delete_order.py` (80 lines)
- `addons/purchase_stock/tests/test_purchase_lead_time.py` (479 lines)
- `addons/purchase_stock/tests/test_purchase_order.py` (1,118 lines)
- `addons/purchase_stock/tests/test_purchase_order_process.py` (203 lines)
- `addons/purchase_stock/tests/test_purchase_order_suggest.py` (735 lines)
- `addons/purchase_stock/tests/test_purchase_stock_accrued_entries.py` (629 lines)
- `addons/purchase_stock/tests/test_purchase_stock_report.py` (444 lines)
- `addons/purchase_stock/tests/test_reordering_rule.py` (1,561 lines)
- `addons/purchase_stock/tests/test_replenish_wizard.py` (645 lines)
- `addons/purchase_stock/tests/test_routes.py` (139 lines)
- `addons/purchase_stock/tests/test_stock.py` (23 lines)
- `addons/purchase_stock/tests/test_stock_orderpoint.py` (46 lines)
- `addons/purchase_stock/tests/test_stock_valuation.py` (311 lines)
- `addons/purchase_stock/tests/test_stockvaluation.py` (1,148 lines)
- `addons/purchase_stock/tests/test_supplier.py` (111 lines)
- `addons/purchase_stock/tests/test_uninstall.py` (42 lines)
- `addons/purchase_stock/views/product_views.xml` (88 lines)
- `addons/purchase_stock/views/purchase_views.xml` (104 lines)
- `addons/purchase_stock/views/res_config_settings_views.xml` (41 lines)
- `addons/purchase_stock/views/res_partner_views.xml` (32 lines)
- `addons/purchase_stock/views/stock_lot_views.xml` (22 lines)
- `addons/purchase_stock/views/stock_orderpoint_views.xml` (14 lines)
- `addons/purchase_stock/views/stock_picking_views.xml` (25 lines)
- `addons/purchase_stock/views/stock_reference_views.xml` (13 lines)
- `addons/purchase_stock/views/stock_rule_views.xml` (18 lines)
- `addons/purchase_stock/views/stock_views.xml` (40 lines)
- `addons/purchase_stock/wizard/__init__.py` (4 lines)
- `addons/purchase_stock/wizard/product_replenish.py` (114 lines)
- `addons/purchase_stock/wizard/product_replenish_views.xml` (18 lines)
- `addons/purchase_stock/wizard/stock_replenishment_info.py` (45 lines)
- `addons/purchase_stock/wizard/stock_replenishment_info.xml` (53 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
