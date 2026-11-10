# Module: mrp_subcontracting

- **Module ID:** MOD-383
- **Path:** `addons/mrp_subcontracting`
- **Manifest:** `addons/mrp_subcontracting/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Subcontract Productions

No manifest description declared.

Declared dependencies: `mrp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 28 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 25 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 12 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp"
  ],
  "data": [
    "data/mrp_subcontracting_data.xml",
    "data/portal_entry_data.xml",
    "views/mrp_bom_views.xml",
    "views/res_partner_views.xml",
    "views/stock_warehouse_views.xml",
    "views/stock_move_views.xml",
    "views/stock_quant_views.xml",
    "views/stock_picking_views.xml",
    "views/supplier_info_views.xml",
    "views/mrp_production_views.xml",
    "views/subcontracting_portal_views.xml",
    "views/subcontracting_portal_templates.xml",
    "report/mrp_report_bom_structure.xml",
    "report/mrp_report_mo_overview.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/mrp_subcontracting_demo.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "mrp_subcontracting/static/tests/tours/subcontracting_portal_tour.js"
    ],
    "web.assets_backend": [
      "mrp_subcontracting/static/src/components/**/*",
      "mrp_subcontracting/static/src/subcontracting_portal/move_list_view.js"
    ],
    "web.assets_frontend": [
      "mrp_subcontracting/static/src/scss/subcontracting_portal.scss"
    ],
    "mrp_subcontracting.webclient": [
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
        "web.icons_fonts"
      ],
      "web/static/src/webclient/navbar/navbar.scss",
      "web/static/src/scss/animation.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      "web/static/src/module_loader.js",
      "web/static/src/session.js",
      "web/static/lib/luxon/luxon.js",
      "web/static/src/libs/luxon.js",
      "web/static/lib/owl/owl.js",
      "web/static/src/owl2/owl3_compatibility_layer.js",
      "web/static/src/owl2/utils.js",
      "web/static/lib/owl/odoo_module.js",
      "web/static/lib/popper/popper.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/component-functions.js",
      "web/static/lib/bootstrap/js/dist/util/backdrop.js",
      "web/static/lib/bootstrap/js/dist/util/focustrap.js",
      "web/static/lib/bootstrap/js/dist/util/sanitizer.js",
      "web/static/lib/bootstrap/js/dist/util/scrollbar.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/util/template-factory.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/alert.js",
      "web/static/lib/bootstrap/js/dist/button.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/collapse.js",
      "web/static/lib/bootstrap/js/dist/dropdown.js",
      "web/static/lib/bootstrap/js/dist/modal.js",
      "web/static/lib/bootstrap/js/dist/offcanvas.js",
      "web/static/lib/bootstrap/js/dist/tooltip.js",
      "web/static/lib/bootstrap/js/dist/popover.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/lib/bootstrap/js/dist/tab.js",
      "web/static/lib/bootstrap/js/dist/toast.js",
      "web/static/src/libs/bootstrap.js",
      [
        "include",
        "web._assets_bootstrap"
      ],
      "base/static/src/css/modules.css",
      "web/static/src/core/utils/transitions.scss",
      "web/static/src/core/**/*",
      [
        "remove",
        "web/static/src/core/emoji_picker/emoji_data.js"
      ],
      "web/static/src/search/**/*",
      "web/static/src/views/*.js",
      "web/static/src/views/*.xml",
      "web/static/src/views/*.scss",
      "web/static/src/views/fields/**/*",
      "web/static/src/views/form/**/*",
      "web/static/src/views/card/**/*",
      "web/static/src/views/kanban/**/*",
      "web/static/src/views/list/**/*",
      "web/static/src/model/**/*",
      "web/static/src/views/view_button/**/*",
      "web/static/src/views/view_components/**/*",
      "web/static/src/views/view_dialogs/**/*",
      "web/static/src/views/widgets/**/*",
      "web/static/src/webclient/**/*",
      [
        "remove",
        "web/static/src/webclient/clickbot/clickbot.js"
      ],
      [
        "remove",
        "web/static/src/views/form/button_box/*.scss"
      ],
      [
        "remove",
        "web/static/src/webclient/share_target/*"
      ],
      [
        "remove",
        "web/static/src/webclient/actions/reports/**/*"
      ],
      "web/static/src/webclient/actions/reports/*.js",
      "web/static/src/webclient/actions/reports/*.xml",
      "web/static/src/env.js",
      "base/static/src/scss/res_partner.scss",
      "web/static/src/views/form/button_box/*.scss",
      "mrp_subcontracting/static/src/subcontracting_portal/*",
      "web/static/src/start.js",
      "stock/static/src/widgets/*",
      "stock/static/src/fields/*",
      "mrp_subcontracting/static/src/components/subcontracting_production_form_controller.js",
      "mrp_subcontracting/static/src/components/subcontracting_production_list_controller.js"
    ]
  }
}
```

### Representative source files

- `addons/mrp_subcontracting/__init__.py` (26 lines)
- `addons/mrp_subcontracting/__manifest__.py` (144 lines)
- `addons/mrp_subcontracting/controllers/__init__.py` (4 lines)
- `addons/mrp_subcontracting/controllers/portal.py` (112 lines)
- `addons/mrp_subcontracting/data/mrp_subcontracting_data.xml` (21 lines)
- `addons/mrp_subcontracting/data/mrp_subcontracting_demo.xml` (29 lines)
- `addons/mrp_subcontracting/data/portal_entry_data.xml` (12 lines)
- `addons/mrp_subcontracting/i18n/ar.po` (652 lines)
- `addons/mrp_subcontracting/i18n/az.po` (634 lines)
- `addons/mrp_subcontracting/i18n/bg.po` (633 lines)
- `addons/mrp_subcontracting/i18n/bs.po` (665 lines)
- `addons/mrp_subcontracting/i18n/ca.po` (652 lines)
- `addons/mrp_subcontracting/i18n/cs.po` (642 lines)
- `addons/mrp_subcontracting/i18n/da.po` (662 lines)
- `addons/mrp_subcontracting/i18n/de.po` (666 lines)
- `addons/mrp_subcontracting/i18n/el.po` (633 lines)
- `addons/mrp_subcontracting/i18n/es.po` (661 lines)
- `addons/mrp_subcontracting/i18n/es_419.po` (661 lines)
- `addons/mrp_subcontracting/i18n/et.po` (654 lines)
- `addons/mrp_subcontracting/i18n/fa.po` (636 lines)
- `addons/mrp_subcontracting/i18n/fi.po` (653 lines)
- `addons/mrp_subcontracting/i18n/fr.po` (665 lines)
- `addons/mrp_subcontracting/i18n/he.po` (658 lines)
- `addons/mrp_subcontracting/i18n/hi.po` (698 lines)
- `addons/mrp_subcontracting/i18n/hr.po` (652 lines)
- `addons/mrp_subcontracting/i18n/hu.po` (641 lines)
- `addons/mrp_subcontracting/i18n/id.po` (651 lines)
- `addons/mrp_subcontracting/i18n/it.po` (662 lines)
- `addons/mrp_subcontracting/i18n/ja.po` (651 lines)
- `addons/mrp_subcontracting/i18n/kab.po` (647 lines)
- `addons/mrp_subcontracting/i18n/ko.po` (647 lines)
- `addons/mrp_subcontracting/i18n/ku.po` (626 lines)
- `addons/mrp_subcontracting/i18n/lo.po` (637 lines)
- `addons/mrp_subcontracting/i18n/lt.po` (644 lines)
- `addons/mrp_subcontracting/i18n/lv.po` (655 lines)
- `addons/mrp_subcontracting/i18n/mn.po` (640 lines)
- `addons/mrp_subcontracting/i18n/mrp_subcontracting.pot` (620 lines)
- `addons/mrp_subcontracting/i18n/my.po` (630 lines)
- `addons/mrp_subcontracting/i18n/nb.po` (651 lines)
- `addons/mrp_subcontracting/i18n/nl.po` (663 lines)
- `addons/mrp_subcontracting/i18n/pl.po` (679 lines)
- `addons/mrp_subcontracting/i18n/pt.po` (660 lines)
- `addons/mrp_subcontracting/i18n/pt_BR.po` (661 lines)
- `addons/mrp_subcontracting/i18n/ro.po` (664 lines)
- `addons/mrp_subcontracting/i18n/ru.po` (661 lines)
- `addons/mrp_subcontracting/i18n/sk.po` (724 lines)
- `addons/mrp_subcontracting/i18n/sl.po` (633 lines)
- `addons/mrp_subcontracting/i18n/sr@latin.po` (629 lines)
- `addons/mrp_subcontracting/i18n/sv.po` (652 lines)
- `addons/mrp_subcontracting/i18n/th.po` (640 lines)
- `addons/mrp_subcontracting/i18n/tr.po` (673 lines)
- `addons/mrp_subcontracting/i18n/uk.po` (663 lines)
- `addons/mrp_subcontracting/i18n/uz.po` (750 lines)
- `addons/mrp_subcontracting/i18n/vi.po` (657 lines)
- `addons/mrp_subcontracting/i18n/zh_CN.po` (644 lines)
- `addons/mrp_subcontracting/i18n/zh_TW.po` (642 lines)
- `addons/mrp_subcontracting/models/__init__.py` (15 lines)
- `addons/mrp_subcontracting/models/mrp_bom.py` (27 lines)
- `addons/mrp_subcontracting/models/mrp_production.py` (142 lines)
- `addons/mrp_subcontracting/models/mrp_unbuild.py` (15 lines)
- `addons/mrp_subcontracting/models/product.py` (26 lines)
- `addons/mrp_subcontracting/models/res_company.py` (35 lines)
- `addons/mrp_subcontracting/models/res_partner.py` (63 lines)
- `addons/mrp_subcontracting/models/stock_location.py` (29 lines)
- `addons/mrp_subcontracting/models/stock_move.py` (319 lines)
- `addons/mrp_subcontracting/models/stock_move_line.py` (40 lines)
- `addons/mrp_subcontracting/models/stock_picking.py` (199 lines)
- `addons/mrp_subcontracting/models/stock_quant.py` (15 lines)
- `addons/mrp_subcontracting/models/stock_rule.py` (25 lines)
- `addons/mrp_subcontracting/models/stock_warehouse.py` (214 lines)
- `addons/mrp_subcontracting/report/__init__.py` (5 lines)
- `addons/mrp_subcontracting/report/mrp_report_bom_structure.py` (194 lines)
- `addons/mrp_subcontracting/report/mrp_report_bom_structure.xml` (42 lines)
- `addons/mrp_subcontracting/report/mrp_report_mo_overview.py` (68 lines)
- `addons/mrp_subcontracting/report/mrp_report_mo_overview.xml` (35 lines)
- `addons/mrp_subcontracting/security/ir.access.csv` (50 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_components_block/mrp_bom_overview_components_block.js` (7 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_components_block/mrp_bom_overview_components_block.xml` (17 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_line/mrp_bom_overview_line.xml` (15 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_special_line/mrp_bom_overview_special_line.js` (31 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_special_line/mrp_bom_overview_special_line.xml` (26 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_table/mrp_bom_overview_table.js` (22 lines)
- `addons/mrp_subcontracting/static/src/components/bom_overview_table/mrp_bom_overview_table.xml` (19 lines)
- `addons/mrp_subcontracting/static/src/components/mo_overview/mrp_mo_overview.js` (21 lines)
- `addons/mrp_subcontracting/static/src/components/mo_overview/mrp_mo_overview.xml` (12 lines)
- `addons/mrp_subcontracting/static/src/components/mo_overview_byproducts_block/mo_overview_byproducts_block.xml` (10 lines)
- `addons/mrp_subcontracting/static/src/components/mo_overview_line/mrp_mo_overview_line.xml` (16 lines)
- `addons/mrp_subcontracting/static/src/components/mo_overview_operations_block/mo_overview_operations_block.xml` (10 lines)
- `addons/mrp_subcontracting/static/src/components/stock_move_line_x2_many_field.js` (8 lines)
- `addons/mrp_subcontracting/static/src/components/subcontracting_production_form_controller.js` (34 lines)
- `addons/mrp_subcontracting/static/src/components/subcontracting_production_list_controller.js` (16 lines)
- `addons/mrp_subcontracting/static/src/img/manufacturing.svg` (16 lines)
- `addons/mrp_subcontracting/static/src/scss/subcontracting_portal.scss` (3 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/main.js` (28 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/move_list_view.js` (9 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/picking_form_controller.js` (15 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/picking_form_controller.xml` (8 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/subcontracting_portal.js` (54 lines)
- `addons/mrp_subcontracting/static/src/subcontracting_portal/subcontracting_portal.xml` (9 lines)
- `addons/mrp_subcontracting/static/tests/tours/subcontracting_portal_tour.js` (18 lines)
- `addons/mrp_subcontracting/tests/__init__.py` (4 lines)
- `addons/mrp_subcontracting/tests/common.py` (80 lines)
- `addons/mrp_subcontracting/tests/test_subcontracting.py` (1,877 lines)
- `addons/mrp_subcontracting/tests/test_subcontracting_portal_ui.py` (60 lines)
- `addons/mrp_subcontracting/views/mrp_bom_views.xml` (19 lines)
- `addons/mrp_subcontracting/views/mrp_production_views.xml` (117 lines)
- `addons/mrp_subcontracting/views/res_partner_views.xml` (25 lines)
- `addons/mrp_subcontracting/views/stock_move_views.xml` (155 lines)
- `addons/mrp_subcontracting/views/stock_picking_views.xml` (16 lines)
- `addons/mrp_subcontracting/views/stock_quant_views.xml` (16 lines)
- `addons/mrp_subcontracting/views/stock_warehouse_views.xml` (13 lines)
- `addons/mrp_subcontracting/views/subcontracting_portal_templates.xml` (83 lines)
- `addons/mrp_subcontracting/views/subcontracting_portal_views.xml` (57 lines)
- `addons/mrp_subcontracting/views/supplier_info_views.xml` (14 lines)
- `addons/mrp_subcontracting/wizard/__init__.py` (5 lines)
- `addons/mrp_subcontracting/wizard/change_production_qty.py` (13 lines)
- `addons/mrp_subcontracting/wizard/mrp_production_serial_numbers.py` (48 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
