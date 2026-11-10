# Module: mrp

- **Module ID:** MOD-377
- **Path:** `addons/mrp`
- **Manifest:** `addons/mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manufacturing Orders & BOMs

No manifest description declared.

Declared dependencies: `product`, `stock`, `resource`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 69 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 24 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 62 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 52 | Client behavior/assets. |
| Tests | 25 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "product",
    "stock",
    "resource"
  ],
  "data": [
    "security/mrp_security.xml",
    "data/digest_data.xml",
    "data/mail_templates.xml",
    "data/mrp_data.xml",
    "data/mail_message_subtype_data.xml",
    "wizard/change_production_qty_views.xml",
    "wizard/mrp_workcenter_block_view.xml",
    "wizard/stock_warn_insufficient_qty_views.xml",
    "wizard/mrp_production_backorder.xml",
    "wizard/mrp_consumption_warning_views.xml",
    "wizard/mrp_production_split.xml",
    "wizard/mrp_production_serial_numbers.xml",
    "views/mrp_views_menus.xml",
    "views/stock_move_views.xml",
    "views/mrp_workorder_views.xml",
    "views/mrp_workcenter_views.xml",
    "views/mrp_bom_views.xml",
    "views/mrp_production_views.xml",
    "views/mrp_routing_views.xml",
    "views/product_views.xml",
    "views/stock_orderpoint_views.xml",
    "views/stock_warehouse_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_rule_views.xml",
    "views/mrp_unbuild_views.xml",
    "views/res_config_settings_views.xml",
    "wizard/stock_replenishment_info.xml",
    "report/report_deliveryslip.xml",
    "report/mrp_report_views_main.xml",
    "report/mrp_report_bom_structure.xml",
    "report/mrp_report_mo_overview.xml",
    "report/mrp_production_templates.xml",
    "report/report_stock_rule.xml",
    "report/mrp_zebra_production_templates.xml",
    "report/mrp_workorder_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/mrp_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mrp/static/src/**/*"
    ],
    "web.assets_tests": [
      "mrp/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "mrp/static/tests/**/*"
    ],
    "web.report_assets_common": [
      "mrp/static/src/scss/mrp_report_bom_structure.scss",
      "mrp/static/src/scss/mrp_report_mo.scss"
    ]
  }
}
```

### Representative source files

- `addons/mrp/README.md` (62 lines)
- `addons/mrp/__init__.py` (28 lines)
- `addons/mrp/__manifest__.py` (73 lines)
- `addons/mrp/data/digest_data.xml` (17 lines)
- `addons/mrp/data/mail_message_subtype_data.xml` (8 lines)
- `addons/mrp/data/mail_templates.xml` (54 lines)
- `addons/mrp/data/mrp_data.xml` (96 lines)
- `addons/mrp/data/mrp_demo.xml` (804 lines)
- `addons/mrp/i18n/af.po` (7,189 lines)
- `addons/mrp/i18n/am.po` (7,185 lines)
- `addons/mrp/i18n/ar.po` (7,859 lines)
- `addons/mrp/i18n/az.po` (7,565 lines)
- `addons/mrp/i18n/bg.po` (7,551 lines)
- `addons/mrp/i18n/bs.po` (7,467 lines)
- `addons/mrp/i18n/ca.po` (7,941 lines)
- `addons/mrp/i18n/cs.po` (7,820 lines)
- `addons/mrp/i18n/da.po` (7,924 lines)
- `addons/mrp/i18n/de.po` (8,075 lines)
- `addons/mrp/i18n/el.po` (7,952 lines)
- `addons/mrp/i18n/es.po` (8,095 lines)
- `addons/mrp/i18n/es_419.po` (8,004 lines)
- `addons/mrp/i18n/es_CL.po` (389 lines)
- `addons/mrp/i18n/et.po` (7,927 lines)
- `addons/mrp/i18n/eu.po` (7,185 lines)
- `addons/mrp/i18n/fa.po` (7,789 lines)
- `addons/mrp/i18n/fi.po` (8,068 lines)
- `addons/mrp/i18n/fo.po` (7,185 lines)
- `addons/mrp/i18n/fr.po` (8,079 lines)
- `addons/mrp/i18n/fr_CA.po` (322 lines)
- `addons/mrp/i18n/gl.po` (7,188 lines)
- `addons/mrp/i18n/gu.po` (7,201 lines)
- `addons/mrp/i18n/he.po` (7,804 lines)
- `addons/mrp/i18n/hi.po` (7,529 lines)
- `addons/mrp/i18n/hr.po` (7,671 lines)
- `addons/mrp/i18n/hu.po` (7,544 lines)
- `addons/mrp/i18n/id.po` (8,119 lines)
- `addons/mrp/i18n/is.po` (7,196 lines)
- `addons/mrp/i18n/it.po` (8,210 lines)
- `addons/mrp/i18n/ja.po` (7,809 lines)
- `addons/mrp/i18n/ka.po` (7,188 lines)
- `addons/mrp/i18n/kab.po` (7,425 lines)
- `addons/mrp/i18n/km.po` (7,194 lines)
- `addons/mrp/i18n/ko.po` (7,840 lines)
- `addons/mrp/i18n/ku.po` (7,424 lines)
- `addons/mrp/i18n/lb.po` (7,187 lines)
- `addons/mrp/i18n/lo.po` (7,799 lines)
- `addons/mrp/i18n/lt.po` (7,557 lines)
- `addons/mrp/i18n/lv.po` (7,449 lines)
- `addons/mrp/i18n/mk.po` (7,188 lines)
- `addons/mrp/i18n/mn.po` (7,770 lines)
- `addons/mrp/i18n/mrp.pot` (7,352 lines)
- `addons/mrp/i18n/my.po` (7,421 lines)
- `addons/mrp/i18n/nb.po` (7,814 lines)
- `addons/mrp/i18n/nl.po` (8,007 lines)
- `addons/mrp/i18n/pl.po` (7,907 lines)
- `addons/mrp/i18n/pt.po` (7,814 lines)
- `addons/mrp/i18n/pt_BR.po` (8,099 lines)
- `addons/mrp/i18n/ro.po` (8,001 lines)
- `addons/mrp/i18n/ru.po` (7,994 lines)
- `addons/mrp/i18n/sk.po` (7,572 lines)
- `addons/mrp/i18n/sl.po` (7,597 lines)
- `addons/mrp/i18n/sq.po` (7,185 lines)
- `addons/mrp/i18n/sr@latin.po` (7,455 lines)
- `addons/mrp/i18n/sv.po` (7,906 lines)
- `addons/mrp/i18n/th.po` (7,917 lines)
- `addons/mrp/i18n/tr.po` (7,955 lines)
- `addons/mrp/i18n/uk.po` (7,830 lines)
- `addons/mrp/i18n/uz.po` (8,985 lines)
- `addons/mrp/i18n/vi.po` (7,964 lines)
- `addons/mrp/i18n/zh_CN.po` (7,895 lines)
- `addons/mrp/i18n/zh_TW.po` (7,760 lines)
- `addons/mrp/models/__init__.py` (27 lines)
- `addons/mrp/models/mrp_bom.py` (890 lines)
- `addons/mrp/models/mrp_production.py` (3,398 lines)
- `addons/mrp/models/mrp_routing.py` (215 lines)
- `addons/mrp/models/mrp_unbuild.py` (355 lines)
- `addons/mrp/models/mrp_workcenter.py` (659 lines)
- `addons/mrp/models/mrp_workorder.py` (1,172 lines)
- `addons/mrp/models/product.py` (457 lines)
- `addons/mrp/models/product_uom.py` (33 lines)
- `addons/mrp/models/res_company.py` (34 lines)
- `addons/mrp/models/res_config_settings.py` (39 lines)
- `addons/mrp/models/res_groups.py` (15 lines)
- `addons/mrp/models/stock_lot.py` (19 lines)
- `addons/mrp/models/stock_move.py` (724 lines)
- `addons/mrp/models/stock_move_line.py` (159 lines)
- `addons/mrp/models/stock_orderpoint.py` (256 lines)
- `addons/mrp/models/stock_package.py` (12 lines)
- `addons/mrp/models/stock_package_history.py` (7 lines)
- `addons/mrp/models/stock_picking.py` (227 lines)
- `addons/mrp/models/stock_quant.py` (14 lines)
- `addons/mrp/models/stock_reference.py` (9 lines)
- `addons/mrp/models/stock_replenish_mixin.py` (18 lines)
- `addons/mrp/models/stock_rule.py` (267 lines)
- `addons/mrp/models/stock_warehouse.py` (332 lines)
- `addons/mrp/report/__init__.py` (8 lines)
- `addons/mrp/report/mrp_production_templates.xml` (213 lines)
- `addons/mrp/report/mrp_report_bom_structure.py` (892 lines)
- `addons/mrp/report/mrp_report_bom_structure.xml` (151 lines)
- `addons/mrp/report/mrp_report_mo_overview.py` (859 lines)
- `addons/mrp/report/mrp_report_mo_overview.xml` (214 lines)
- `addons/mrp/report/mrp_report_views_main.xml` (51 lines)
- `addons/mrp/report/mrp_workorder_templates.xml` (52 lines)
- `addons/mrp/report/mrp_zebra_production_templates.xml` (21 lines)
- `addons/mrp/report/report_deliveryslip.xml` (89 lines)
- `addons/mrp/report/report_stock_rule.py` (17 lines)
- `addons/mrp/report/report_stock_rule.xml` (32 lines)
- `addons/mrp/report/stock_allocation_report.py` (45 lines)
- `addons/mrp/report/stock_forecasted.py` (53 lines)
- `addons/mrp/report/stock_traceability.py` (63 lines)
- `addons/mrp/security/ir.access.csv` (59 lines)
- `addons/mrp/security/mrp_security.xml` (39 lines)
- `addons/mrp/static/description/icon.png` (14 lines)
- `addons/mrp/static/description/icon.svg` (1 lines)
- `addons/mrp/static/description/icon_hi.png` (78 lines)
- `addons/mrp/static/img/assebly-worksheet.pdf` (951 lines)
- `addons/mrp/static/img/cutting-worksheet-1.pdf` (329 lines)
- `addons/mrp/static/img/cutting-worksheet-2.pdf` (480 lines)
- `addons/mrp/static/img/cutting-worksheet-3.pdf` (491 lines)
- `addons/mrp/static/img/cutting-worksheet-4.pdf` (394 lines)
- `addons/mrp/static/img/product_product_computer_desk_bolt.png` (373 lines)
- `addons/mrp/static/img/product_product_computer_desk_screw.png` (346 lines)
- `addons/mrp/static/img/product_product_drawer_black.png` (639 lines)
- `addons/mrp/static/img/product_product_drawer_case_black.png` (220 lines)
- `addons/mrp/static/img/product_product_plastic_laminate.png` (131 lines)
- `addons/mrp/static/img/product_product_ply_veneer.png` (166 lines)
- `addons/mrp/static/img/product_product_table_kit.png` (206 lines)
- `addons/mrp/static/img/product_product_wood_panel.png` (439 lines)
- `addons/mrp/static/img/product_product_wood_ply.png` (590 lines)
- `addons/mrp/static/img/product_product_wood_wear.png` (274 lines)
- `addons/mrp/static/img/routing.svg` (5 lines)
- `addons/mrp/static/img/routing_shopfloor.png` (620 lines)
- `addons/mrp/static/img/table.png` (138 lines)
- `addons/mrp/static/img/table_leg.png` (12 lines)
- `addons/mrp/static/img/table_top.png` (123 lines)
- `addons/mrp/static/src/allocation_report/allocation_report.js` (19 lines)
- `addons/mrp/static/src/components/bom_overview/mrp_bom_overview.js` (177 lines)
- `addons/mrp/static/src/components/bom_overview/mrp_bom_overview.xml` (35 lines)
- `addons/mrp/static/src/components/bom_overview_components_block/mrp_bom_overview_components_block.js` (98 lines)
- `addons/mrp/static/src/components/bom_overview_components_block/mrp_bom_overview_components_block.xml` (45 lines)
- `addons/mrp/static/src/components/bom_overview_control_panel/mrp_bom_overview_control_panel.js` (107 lines)
- `addons/mrp/static/src/components/bom_overview_control_panel/mrp_bom_overview_control_panel.xml` (60 lines)
- `addons/mrp/static/src/components/bom_overview_display_filter/mrp_bom_overview_display_filter.js` (31 lines)
- `addons/mrp/static/src/components/bom_overview_display_filter/mrp_bom_overview_display_filter.xml` (15 lines)
- `addons/mrp/static/src/components/bom_overview_extra_block/mrp_bom_overview_extra_block.js` (64 lines)
- `addons/mrp/static/src/components/bom_overview_extra_block/mrp_bom_overview_extra_block.xml` (22 lines)
- `addons/mrp/static/src/components/bom_overview_line/mrp_bom_overview_line.js` (165 lines)
- `addons/mrp/static/src/components/bom_overview_line/mrp_bom_overview_line.xml` (59 lines)
- `addons/mrp/static/src/components/bom_overview_special_line/mrp_bom_overview_special_line.js` (50 lines)
- `addons/mrp/static/src/components/bom_overview_special_line/mrp_bom_overview_special_line.xml` (31 lines)
- `addons/mrp/static/src/components/bom_overview_table/mrp_bom_overview_table.js` (73 lines)
- `addons/mrp/static/src/components/bom_overview_table/mrp_bom_overview_table.xml` (75 lines)
- `addons/mrp/static/src/components/mo_overview/mrp_mo_overview.js` (189 lines)
- `addons/mrp/static/src/components/mo_overview/mrp_mo_overview.xml` (108 lines)
- `addons/mrp/static/src/components/mo_overview_byproducts_block/mrp_mo_overview_byproducts_block.js` (33 lines)
- `addons/mrp/static/src/components/mo_overview_byproducts_block/mrp_mo_overview_byproducts_block.xml` (29 lines)
- `addons/mrp/static/src/components/mo_overview_components_block/mrp_mo_overview_components_block.js` (134 lines)
- `addons/mrp/static/src/components/mo_overview_components_block/mrp_mo_overview_components_block.xml` (43 lines)
- `addons/mrp/static/src/components/mo_overview_display_filter/mrp_mo_overview_display_filter.js` (36 lines)
- `addons/mrp/static/src/components/mo_overview_line/mo_overview_colors.js` (59 lines)

Additional files not expanded here: 123. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
