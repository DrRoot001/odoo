# Module: stock

- **Module ID:** MOD-559
- **Path:** `addons/stock`
- **Manifest:** `addons/stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage your stock and logistics activities

No manifest description declared.

Declared dependencies: `product`, `barcodes_gs1_nomenclature`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 96 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 29 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 107 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 55 | Client behavior/assets. |
| Tests | 32 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "product",
    "barcodes_gs1_nomenclature",
    "digest"
  ],
  "data": [
    "security/stock_security.xml",
    "data/digest_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_templates.xml",
    "data/default_barcode_patterns.xml",
    "data/stock_data.xml",
    "data/stock_sequence_data.xml",
    "data/stock_traceability_report_data.xml",
    "report/report_stock_quantity.xml",
    "report/report_stock_reception.xml",
    "report/stock_report_views.xml",
    "report/report_package_barcode.xml",
    "report/report_lot_barcode.xml",
    "report/report_location_barcode.xml",
    "report/report_picking_batch.xml",
    "report/report_stockpicking_operations.xml",
    "report/report_deliveryslip.xml",
    "report/report_stockinventory.xml",
    "report/report_stock_rule.xml",
    "report/package_templates.xml",
    "report/picking_templates.xml",
    "report/product_templates.xml",
    "report/report_return_slip.xml",
    "report/stock_allocation_report.xml",
    "data/mail_template_data.xml",
    "views/stock_menu_views.xml",
    "wizard/stock_add_to_wave_views.xml",
    "wizard/stock_inventory_conflict.xml",
    "wizard/stock_backorder_confirmation_views.xml",
    "wizard/stock_zero_demand_confirmation_views.xml",
    "wizard/stock_request_count.xml",
    "wizard/stock_replenishment_info.xml",
    "wizard/stock_rules_report_views.xml",
    "wizard/stock_warn_insufficient_qty_views.xml",
    "wizard/product_replenish_views.xml",
    "wizard/product_label_layout_views.xml",
    "wizard/stock_orderpoint_snooze_views.xml",
    "wizard/stock_orderpoint_suggest.xml",
    "wizard/stock_package_destination_views.xml",
    "wizard/stock_picking_to_batch_views.xml",
    "wizard/stock_inventory_adjustment_name.xml",
    "wizard/stock_inventory_warning.xml",
    "wizard/stock_label_type.xml",
    "wizard/stock_lot_label_layout.xml",
    "wizard/stock_quant_relocate.xml",
    "wizard/stock_put_in_pack_views.xml",
    "views/res_partner_views.xml",
    "views/product_strategy_views.xml",
    "views/stock_lot_views.xml",
    "views/stock_quant_views.xml",
    "views/stock_warehouse_views.xml",
    "views/stock_move_line_views.xml",
    "views/stock_move_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_picking_batch_views.xml",
    "views/stock_picking_type_views.xml",
    "views/product_views.xml",
    "views/stock_location_views.xml",
    "views/stock_orderpoint_views.xml",
    "views/stock_storage_category_views.xml",
    "views/res_config_settings_views.xml",
    "views/report_stock_traceability.xml",
    "views/stock_template.xml",
    "views/stock_rule_views.xml",
    "views/stock_scrap_reason_tag_views.xml",
    "views/stock_package_history_views.xml",
    "views/stock_package_type_view.xml",
    "views/stock_package_views.xml",
    "views/stock_forecasted.xml",
    "views/stock_reference_views.xml",
    "views/uom_uom_views.xml",
    "views/digest_digest_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/stock_demo_pre.xml",
    "data/stock_demo.xml",
    "data/stock_demo2.xml",
    "data/stock_demo3_batch.xml",
    "data/stock_orderpoint_demo.xml",
    "data/stock_storage_category_demo.xml"
  ],
  "assets": {
    "web.report_assets_common": [
      "stock/static/src/scss/report_stock_reception_labels.scss",
      "stock/static/src/scss/report_stock_rule.scss",
      "stock/static/src/scss/report_stockpicking_operations.scss"
    ],
    "web.assets_backend": [
      "stock/static/src/**/*.js",
      "stock/static/src/**/*.xml",
      "stock/static/src/**/*.scss",
      [
        "remove",
        "stock/static/src/stock_forecasted/forecasted_graph.*"
      ]
    ],
    "web.assets_backend_lazy": [
      "stock/static/src/stock_forecasted/forecasted_graph.*"
    ],
    "web.assets_frontend": [
      "stock/static/src/scss/stock_traceability_report.scss"
    ],
    "web.assets_tests": [
      "stock/static/tests/tours/*.js"
    ],
    "web.assets_unit_tests": [
      "stock/static/tests/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/stock/__init__.py` (92 lines)
- `addons/stock/__manifest__.py` (129 lines)
- `addons/stock/controllers/__init__.py` (1 lines)
- `addons/stock/controllers/main.py` (40 lines)
- `addons/stock/data/default_barcode_patterns.xml` (40 lines)
- `addons/stock/data/digest_data.xml` (45 lines)
- `addons/stock/data/mail_message_subtype_data.xml` (19 lines)
- `addons/stock/data/mail_template_data.xml` (83 lines)
- `addons/stock/data/mail_templates.xml` (32 lines)
- `addons/stock/data/stock_data.xml` (108 lines)
- `addons/stock/data/stock_demo.xml` (217 lines)
- `addons/stock/data/stock_demo2.xml` (732 lines)
- `addons/stock/data/stock_demo3_batch.xml` (131 lines)
- `addons/stock/data/stock_demo_pre.xml` (141 lines)
- `addons/stock/data/stock_orderpoint_demo.xml` (65 lines)
- `addons/stock/data/stock_sequence_data.xml` (69 lines)
- `addons/stock/data/stock_storage_category_demo.xml` (29 lines)
- `addons/stock/data/stock_traceability_report_data.xml` (10 lines)
- `addons/stock/i18n/af.po` (12,052 lines)
- `addons/stock/i18n/ar.po` (13,193 lines)
- `addons/stock/i18n/az.po` (12,407 lines)
- `addons/stock/i18n/bg.po` (12,537 lines)
- `addons/stock/i18n/bs.po` (14,278 lines)
- `addons/stock/i18n/ca.po` (12,975 lines)
- `addons/stock/i18n/cs.po` (13,244 lines)
- `addons/stock/i18n/da.po` (13,541 lines)
- `addons/stock/i18n/de.po` (13,745 lines)
- `addons/stock/i18n/el.po` (13,252 lines)
- `addons/stock/i18n/es.po` (13,541 lines)
- `addons/stock/i18n/es_419.po` (13,583 lines)
- `addons/stock/i18n/es_CL.po` (1,424 lines)
- `addons/stock/i18n/et.po` (13,181 lines)
- `addons/stock/i18n/fa.po` (12,885 lines)
- `addons/stock/i18n/fi.po` (13,477 lines)
- `addons/stock/i18n/fr.po` (13,478 lines)
- `addons/stock/i18n/gl.po` (12,054 lines)
- `addons/stock/i18n/gu.po` (12,075 lines)
- `addons/stock/i18n/he.po` (12,732 lines)
- `addons/stock/i18n/hi.po` (12,605 lines)
- `addons/stock/i18n/hr.po` (13,702 lines)
- `addons/stock/i18n/hu.po` (12,555 lines)
- `addons/stock/i18n/id.po` (13,493 lines)
- `addons/stock/i18n/is.po` (12,066 lines)
- `addons/stock/i18n/it.po` (13,521 lines)
- `addons/stock/i18n/ja.po` (13,273 lines)
- `addons/stock/i18n/kab.po` (12,323 lines)
- `addons/stock/i18n/km.po` (12,060 lines)
- `addons/stock/i18n/ko.po` (13,131 lines)
- `addons/stock/i18n/ku.po` (12,261 lines)
- `addons/stock/i18n/lb.po` (12,053 lines)
- `addons/stock/i18n/lo.po` (12,947 lines)
- `addons/stock/i18n/lt.po` (12,489 lines)
- `addons/stock/i18n/lv.po` (12,481 lines)
- `addons/stock/i18n/mk.po` (12,093 lines)
- `addons/stock/i18n/mn.po` (13,282 lines)
- `addons/stock/i18n/my.po` (12,277 lines)
- `addons/stock/i18n/nb.po` (12,816 lines)
- `addons/stock/i18n/nl.po` (13,613 lines)
- `addons/stock/i18n/pl.po` (13,328 lines)
- `addons/stock/i18n/pt.po` (13,355 lines)
- `addons/stock/i18n/pt_BR.po` (13,585 lines)
- `addons/stock/i18n/ro.po` (13,468 lines)
- `addons/stock/i18n/ru.po` (13,267 lines)
- `addons/stock/i18n/sk.po` (13,165 lines)
- `addons/stock/i18n/sl.po` (12,625 lines)
- `addons/stock/i18n/sr@latin.po` (12,287 lines)
- `addons/stock/i18n/stock.pot` (12,102 lines)
- `addons/stock/i18n/sv.po` (13,099 lines)
- `addons/stock/i18n/th.po` (13,161 lines)
- `addons/stock/i18n/tr.po` (13,297 lines)
- `addons/stock/i18n/uk.po` (12,988 lines)
- `addons/stock/i18n/uz.po` (14,901 lines)
- `addons/stock/i18n/vi.po` (13,195 lines)
- `addons/stock/i18n/zh_CN.po` (13,173 lines)
- `addons/stock/i18n/zh_TW.po` (12,817 lines)
- `addons/stock/models/__init__.py` (31 lines)
- `addons/stock/models/barcode.py` (20 lines)
- `addons/stock/models/digest.py` (45 lines)
- `addons/stock/models/ir_actions_report.py` (22 lines)
- `addons/stock/models/product.py` (1,389 lines)
- `addons/stock/models/product_strategy.py` (183 lines)
- `addons/stock/models/res_company.py` (252 lines)
- `addons/stock/models/res_config_settings.py` (163 lines)
- `addons/stock/models/res_groups.py` (23 lines)
- `addons/stock/models/res_partner.py` (44 lines)
- `addons/stock/models/res_users.py` (12 lines)
- `addons/stock/models/stock_location.py` (614 lines)
- `addons/stock/models/stock_lot.py` (431 lines)
- `addons/stock/models/stock_move.py` (3,026 lines)
- `addons/stock/models/stock_move_line.py` (1,767 lines)
- `addons/stock/models/stock_orderpoint.py` (887 lines)
- `addons/stock/models/stock_package.py` (574 lines)
- `addons/stock/models/stock_package_history.py` (42 lines)
- `addons/stock/models/stock_package_type.py` (127 lines)
- `addons/stock/models/stock_picking.py` (2,127 lines)
- `addons/stock/models/stock_picking_batch.py` (491 lines)
- `addons/stock/models/stock_picking_type.py` (736 lines)
- `addons/stock/models/stock_quant.py` (1,619 lines)
- `addons/stock/models/stock_reference.py` (15 lines)
- `addons/stock/models/stock_replenish_mixin.py` (40 lines)
- `addons/stock/models/stock_rule.py` (741 lines)
- `addons/stock/models/stock_scrap_reason_tag.py` (16 lines)
- `addons/stock/models/stock_storage_category.py` (71 lines)
- `addons/stock/models/stock_warehouse.py` (1,172 lines)
- `addons/stock/populate/benchmarks.xml` (336 lines)
- `addons/stock/populate/populate_demo.xml` (171 lines)
- `addons/stock/report/__init__.py` (7 lines)
- `addons/stock/report/package_templates.xml` (55 lines)
- `addons/stock/report/picking_templates.xml` (14 lines)
- `addons/stock/report/product_templates.xml` (42 lines)
- `addons/stock/report/report_deliveryslip.xml` (325 lines)
- `addons/stock/report/report_location_barcode.xml` (36 lines)
- `addons/stock/report/report_lot_barcode.xml` (70 lines)
- `addons/stock/report/report_package_barcode.xml` (217 lines)
- `addons/stock/report/report_picking_batch.xml` (134 lines)
- `addons/stock/report/report_return_slip.xml` (67 lines)
- `addons/stock/report/report_stock_quantity.py` (194 lines)
- `addons/stock/report/report_stock_quantity.xml` (16 lines)
- `addons/stock/report/report_stock_reception.xml` (26 lines)
- `addons/stock/report/report_stock_rule.py` (140 lines)
- `addons/stock/report/report_stock_rule.xml` (182 lines)
- `addons/stock/report/report_stockinventory.xml` (52 lines)
- `addons/stock/report/report_stockpicking_operations.xml` (310 lines)
- `addons/stock/report/stock_allocation_report.py` (480 lines)
- `addons/stock/report/stock_allocation_report.xml` (8 lines)
- `addons/stock/report/stock_forecasted.py` (518 lines)
- `addons/stock/report/stock_report_views.xml` (72 lines)
- `addons/stock/report/stock_traceability.py` (296 lines)
- `addons/stock/security/ir.access.csv` (91 lines)
- `addons/stock/security/stock_security.xml` (69 lines)
- `addons/stock/static/description/icon.png` (10 lines)
- `addons/stock/static/description/icon.svg` (1 lines)
- `addons/stock/static/description/icon_hi.png` (51 lines)
- `addons/stock/static/img/barcode_scanner.png` (280 lines)
- `addons/stock/static/img/cable_management.jpg` (1,026 lines)
- `addons/stock/static/img/empty_list.png` (418 lines)
- `addons/stock/static/img/replenishment.svg` (256 lines)
- `addons/stock/static/img/res_partner_address_41.webp` (28 lines)
- `addons/stock/static/img/shapes/batch-picking.svg` (109 lines)
- `addons/stock/static/img/shapes/cluster-picking.svg` (97 lines)
- `addons/stock/static/img/shapes/wave-picking.svg` (87 lines)
- `addons/stock/static/src/allocation_report/allocation_report.js` (384 lines)
- `addons/stock/static/src/allocation_report/allocation_report.scss` (7 lines)
- `addons/stock/static/src/allocation_report/allocation_report.xml` (84 lines)
- `addons/stock/static/src/allocation_report/out_line/out_line.js` (91 lines)
- `addons/stock/static/src/allocation_report/out_line/out_line.xml` (124 lines)
- `addons/stock/static/src/allocation_report/product_line/product_line.js` (89 lines)
- `addons/stock/static/src/allocation_report/product_line/product_line.xml` (70 lines)
- `addons/stock/static/src/client_actions/multi_print.js` (38 lines)
- `addons/stock/static/src/client_actions/stock_traceability_report_backend.js` (236 lines)
- `addons/stock/static/src/client_actions/stock_traceability_report_backend.xml` (88 lines)
- `addons/stock/static/src/components/stock_overview/stock_overview.js` (49 lines)
- `addons/stock/static/src/fields/stock_action_field.js` (101 lines)
- `addons/stock/static/src/fields/stock_action_field.xml` (21 lines)
- `addons/stock/static/src/fields/stock_move_line_x2_many_field.js` (190 lines)
- `addons/stock/static/src/fields/stock_picking_locked_statusbar_field.js` (25 lines)
- `addons/stock/static/src/fields/stock_picking_locked_statusbar_field.xml` (30 lines)
- `addons/stock/static/src/img/barcode.gif` (384 lines)
- `addons/stock/static/src/picking_type_dashboard_graph/picking_type_dashboard_graph_field.js` (110 lines)
- `addons/stock/static/src/picking_type_dashboard_graph/picking_type_dashboard_graph_field.scss` (5 lines)

Additional files not expanded here: 185. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
