# Module: repair

- **Module ID:** MOD-505
- **Path:** `addons/repair`
- **Manifest:** `addons/repair/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Repair damaged products


The aim is to have a complete module to manage all products repairs.
====================================================================

The following topics are covered by this module:
------------------------------------------------------
    * Add/remove products in the reparation
    * Impact for stocks
    * Warranty concept
    * Repair quotation report
    * Notes for the technician and for the final customer


Declared dependencies: `sale_stock`, `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_stock",
    "sale_management"
  ],
  "data": [
    "views/product_views.xml",
    "views/stock_move_views.xml",
    "views/repair_views.xml",
    "views/sale_order_views.xml",
    "views/stock_lot_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_warehouse_views.xml",
    "views/account_move_views.xml",
    "views/res_partner_views.xml",
    "report/repair_reports.xml",
    "report/repair_templates_repair_order.xml",
    "data/repair_data.xml",
    "security/ir.access.csv",
    "wizard/repair_consumption_warning_views.xml"
  ],
  "demo": [
    "data/repair_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "repair/static/src/**/*"
    ],
    "web.assets_tests": [
      "repair/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/repair/__init__.py` (17 lines)
- `addons/repair/__manifest__.py` (51 lines)
- `addons/repair/data/repair_data.xml` (24 lines)
- `addons/repair/data/repair_demo.xml` (69 lines)
- `addons/repair/i18n/af.po` (1,645 lines)
- `addons/repair/i18n/am.po` (1,641 lines)
- `addons/repair/i18n/ar.po` (1,721 lines)
- `addons/repair/i18n/az.po` (1,687 lines)
- `addons/repair/i18n/bg.po` (1,703 lines)
- `addons/repair/i18n/bs.po` (1,677 lines)
- `addons/repair/i18n/ca.po` (1,720 lines)
- `addons/repair/i18n/cs.po` (1,715 lines)
- `addons/repair/i18n/da.po` (1,701 lines)
- `addons/repair/i18n/de.po` (1,774 lines)
- `addons/repair/i18n/el.po` (1,731 lines)
- `addons/repair/i18n/es.po` (1,760 lines)
- `addons/repair/i18n/es_419.po` (1,760 lines)
- `addons/repair/i18n/es_CL.po` (152 lines)
- `addons/repair/i18n/et.po` (1,732 lines)
- `addons/repair/i18n/eu.po` (1,644 lines)
- `addons/repair/i18n/fa.po` (1,700 lines)
- `addons/repair/i18n/fi.po` (1,744 lines)
- `addons/repair/i18n/fo.po` (1,644 lines)
- `addons/repair/i18n/fr.po` (1,750 lines)
- `addons/repair/i18n/fr_BE.po` (125 lines)
- `addons/repair/i18n/fr_CA.po` (137 lines)
- `addons/repair/i18n/gl.po` (1,644 lines)
- `addons/repair/i18n/gu.po` (1,655 lines)
- `addons/repair/i18n/he.po` (1,720 lines)
- `addons/repair/i18n/hi.po` (1,678 lines)
- `addons/repair/i18n/hr.po` (1,715 lines)
- `addons/repair/i18n/hu.po` (1,699 lines)
- `addons/repair/i18n/id.po` (1,728 lines)
- `addons/repair/i18n/is.po` (1,655 lines)
- `addons/repair/i18n/it.po` (1,756 lines)
- `addons/repair/i18n/ja.po` (1,728 lines)
- `addons/repair/i18n/ka.po` (1,644 lines)
- `addons/repair/i18n/kab.po` (1,668 lines)
- `addons/repair/i18n/km.po` (1,653 lines)
- `addons/repair/i18n/ko.po` (1,722 lines)
- `addons/repair/i18n/ku.po` (1,677 lines)
- `addons/repair/i18n/lb.po` (1,646 lines)
- `addons/repair/i18n/lo.po` (1,714 lines)
- `addons/repair/i18n/lt.po` (1,710 lines)
- `addons/repair/i18n/lv.po` (1,689 lines)
- `addons/repair/i18n/mk.po` (1,644 lines)
- `addons/repair/i18n/mn.po` (1,703 lines)
- `addons/repair/i18n/my.po` (1,668 lines)
- `addons/repair/i18n/nb.po` (1,695 lines)
- `addons/repair/i18n/nl.po` (1,760 lines)
- `addons/repair/i18n/pl.po` (1,753 lines)
- `addons/repair/i18n/pt.po` (1,712 lines)
- `addons/repair/i18n/pt_BR.po` (1,777 lines)
- `addons/repair/i18n/repair.pot` (1,658 lines)
- `addons/repair/i18n/ro.po` (1,723 lines)
- `addons/repair/i18n/ru.po` (1,727 lines)
- `addons/repair/i18n/sk.po` (1,691 lines)
- `addons/repair/i18n/sl.po` (1,697 lines)
- `addons/repair/i18n/sq.po` (1,644 lines)
- `addons/repair/i18n/sr@latin.po` (1,687 lines)
- `addons/repair/i18n/sv.po` (1,730 lines)
- `addons/repair/i18n/ta.po` (1,645 lines)
- `addons/repair/i18n/te.po` (1,643 lines)
- `addons/repair/i18n/th.po` (1,712 lines)
- `addons/repair/i18n/tr.po` (1,738 lines)
- `addons/repair/i18n/uk.po` (1,708 lines)
- `addons/repair/i18n/uz.po` (1,960 lines)
- `addons/repair/i18n/vi.po` (1,723 lines)
- `addons/repair/i18n/zh_CN.po` (1,718 lines)
- `addons/repair/i18n/zh_TW.po` (1,705 lines)
- `addons/repair/models/__init__.py` (15 lines)
- `addons/repair/models/account_move.py` (17 lines)
- `addons/repair/models/account_move_line.py` (29 lines)
- `addons/repair/models/product.py` (40 lines)
- `addons/repair/models/repair.py` (826 lines)
- `addons/repair/models/repair_service_line.py` (178 lines)
- `addons/repair/models/res_partner.py` (44 lines)
- `addons/repair/models/sale_order.py` (136 lines)
- `addons/repair/models/stock_lot.py` (81 lines)
- `addons/repair/models/stock_move.py` (319 lines)
- `addons/repair/models/stock_move_line.py` (10 lines)
- `addons/repair/models/stock_picking.py` (223 lines)
- `addons/repair/models/stock_warehouse.py` (96 lines)
- `addons/repair/report/__init__.py` (5 lines)
- `addons/repair/report/repair_reports.xml` (14 lines)
- `addons/repair/report/repair_templates_repair_order.xml` (83 lines)
- `addons/repair/report/stock_forecasted.py` (30 lines)
- `addons/repair/report/stock_traceability.py` (26 lines)
- `addons/repair/security/ir.access.csv` (7 lines)
- `addons/repair/static/description/icon.png` (15 lines)
- `addons/repair/static/description/icon.svg` (1 lines)
- `addons/repair/static/description/icon_hi.png` (120 lines)
- `addons/repair/static/src/components/product_catalog/kanban_controller.js` (13 lines)
- `addons/repair/static/src/components/product_catalog/kanban_renderer.js` (12 lines)
- `addons/repair/static/tests/tours/repair_order.js` (47 lines)
- `addons/repair/tests/__init__.py` (6 lines)
- `addons/repair/tests/test_anglo_saxon_valuation.py` (108 lines)
- `addons/repair/tests/test_repair.py` (1,130 lines)
- `addons/repair/tests/test_rules_installation.py` (21 lines)
- `addons/repair/views/account_move_views.xml` (23 lines)
- `addons/repair/views/product_views.xml` (32 lines)
- `addons/repair/views/repair_views.xml` (451 lines)
- `addons/repair/views/res_partner_views.xml` (16 lines)
- `addons/repair/views/sale_order_views.xml` (24 lines)
- `addons/repair/views/stock_lot_views.xml` (39 lines)
- `addons/repair/views/stock_move_views.xml` (11 lines)
- `addons/repair/views/stock_picking_views.xml` (141 lines)
- `addons/repair/views/stock_warehouse_views.xml` (13 lines)
- `addons/repair/wizard/__init__.py` (1 lines)
- `addons/repair/wizard/repair_consumption_warning.py` (40 lines)
- `addons/repair/wizard/repair_consumption_warning_views.xml` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
