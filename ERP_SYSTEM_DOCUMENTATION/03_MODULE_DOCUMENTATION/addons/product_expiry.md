# Module: product_expiry

- **Module ID:** MOD-472
- **Path:** `addons/product_expiry`
- **Manifest:** `addons/product_expiry/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Track different dates on products and production lots.
======================================================

Following dates can be tracked:
-------------------------------
    - end of life
    - best before date
    - removal date
    - alert date

Also implements the removal strategy First Expiry First Out (FEFO) widely used, for example, in food industries.


Declared dependencies: `stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock"
  ],
  "data": [
    "security/stock_security.xml",
    "views/production_lot_views.xml",
    "views/product_template_views.xml",
    "views/res_config_settings_views.xml",
    "views/stock_move_views.xml",
    "views/stock_quant_views.xml",
    "wizard/confirm_expiry_view.xml",
    "report/report_deliveryslip.xml",
    "report/report_lot_barcode.xml",
    "report/report_package_barcode.xml",
    "report/report_stock_traceability.xml",
    "data/product_expiry_data.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "product_expiry/static/tests/tours/*.js"
    ],
    "web.assets_backend": [
      "product_expiry/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/product_expiry/__init__.py` (16 lines)
- `addons/product_expiry/__manifest__.py` (45 lines)
- `addons/product_expiry/data/product_expiry_data.xml` (7 lines)
- `addons/product_expiry/i18n/am.po` (664 lines)
- `addons/product_expiry/i18n/ar.po` (769 lines)
- `addons/product_expiry/i18n/az.po` (642 lines)
- `addons/product_expiry/i18n/bg.po` (645 lines)
- `addons/product_expiry/i18n/bs.po` (646 lines)
- `addons/product_expiry/i18n/ca.po` (747 lines)
- `addons/product_expiry/i18n/cs.po` (739 lines)
- `addons/product_expiry/i18n/da.po` (729 lines)
- `addons/product_expiry/i18n/de.po` (792 lines)
- `addons/product_expiry/i18n/el.po` (646 lines)
- `addons/product_expiry/i18n/es.po` (789 lines)
- `addons/product_expiry/i18n/es_419.po` (790 lines)
- `addons/product_expiry/i18n/et.po` (777 lines)
- `addons/product_expiry/i18n/eu.po` (667 lines)
- `addons/product_expiry/i18n/fa.po` (645 lines)
- `addons/product_expiry/i18n/fi.po` (776 lines)
- `addons/product_expiry/i18n/fr.po` (779 lines)
- `addons/product_expiry/i18n/gl.po` (666 lines)
- `addons/product_expiry/i18n/gu.po` (668 lines)
- `addons/product_expiry/i18n/he.po` (663 lines)
- `addons/product_expiry/i18n/hi.po` (639 lines)
- `addons/product_expiry/i18n/hr.po` (652 lines)
- `addons/product_expiry/i18n/hu.po` (654 lines)
- `addons/product_expiry/i18n/id.po` (773 lines)
- `addons/product_expiry/i18n/is.po` (664 lines)
- `addons/product_expiry/i18n/it.po` (792 lines)
- `addons/product_expiry/i18n/ja.po` (767 lines)
- `addons/product_expiry/i18n/kab.po` (641 lines)
- `addons/product_expiry/i18n/km.po` (664 lines)
- `addons/product_expiry/i18n/ko.po` (755 lines)
- `addons/product_expiry/i18n/ku.po` (639 lines)
- `addons/product_expiry/i18n/lo.po` (690 lines)
- `addons/product_expiry/i18n/lt.po` (663 lines)
- `addons/product_expiry/i18n/lv.po` (647 lines)
- `addons/product_expiry/i18n/mk.po` (671 lines)
- `addons/product_expiry/i18n/mn.po` (661 lines)
- `addons/product_expiry/i18n/my.po` (640 lines)
- `addons/product_expiry/i18n/nb.po` (648 lines)
- `addons/product_expiry/i18n/nl.po` (793 lines)
- `addons/product_expiry/i18n/pl.po` (783 lines)
- `addons/product_expiry/i18n/product_expiry.pot` (622 lines)
- `addons/product_expiry/i18n/pt.po` (761 lines)
- `addons/product_expiry/i18n/pt_BR.po` (788 lines)
- `addons/product_expiry/i18n/ro.po` (743 lines)
- `addons/product_expiry/i18n/ru.po` (775 lines)
- `addons/product_expiry/i18n/sk.po` (650 lines)
- `addons/product_expiry/i18n/sl.po` (649 lines)
- `addons/product_expiry/i18n/sr@latin.po` (644 lines)
- `addons/product_expiry/i18n/sv.po` (741 lines)
- `addons/product_expiry/i18n/th.po` (761 lines)
- `addons/product_expiry/i18n/tr.po` (780 lines)
- `addons/product_expiry/i18n/uk.po` (740 lines)
- `addons/product_expiry/i18n/uz.po` (841 lines)
- `addons/product_expiry/i18n/vi.po` (770 lines)
- `addons/product_expiry/i18n/zh_CN.po` (767 lines)
- `addons/product_expiry/i18n/zh_TW.po` (738 lines)
- `addons/product_expiry/models/__init__.py` (13 lines)
- `addons/product_expiry/models/product_product.py` (59 lines)
- `addons/product_expiry/models/production_lot.py` (107 lines)
- `addons/product_expiry/models/res_config_settings.py` (27 lines)
- `addons/product_expiry/models/res_groups.py` (13 lines)
- `addons/product_expiry/models/stock_move.py` (101 lines)
- `addons/product_expiry/models/stock_move_line.py` (48 lines)
- `addons/product_expiry/models/stock_picking.py` (48 lines)
- `addons/product_expiry/models/stock_quant.py` (42 lines)
- `addons/product_expiry/models/stock_rule.py` (17 lines)
- `addons/product_expiry/report/__init__.py` (5 lines)
- `addons/product_expiry/report/report_deliveryslip.xml` (22 lines)
- `addons/product_expiry/report/report_lot_barcode.xml` (61 lines)
- `addons/product_expiry/report/report_package_barcode.xml` (16 lines)
- `addons/product_expiry/report/report_stock_quantity.py` (16 lines)
- `addons/product_expiry/report/report_stock_traceability.xml` (16 lines)
- `addons/product_expiry/report/stock_forecasted.py` (64 lines)
- `addons/product_expiry/report/stock_traceability.py` (18 lines)
- `addons/product_expiry/security/ir.access.csv` (2 lines)
- `addons/product_expiry/security/stock_security.xml` (8 lines)
- `addons/product_expiry/static/description/icon.png` (21 lines)
- `addons/product_expiry/static/description/icon.svg` (7 lines)
- `addons/product_expiry/static/img/product_product_from-image.jpg` (20 lines)
- `addons/product_expiry/static/img/product_product_jambon-image.jpg` (21 lines)
- `addons/product_expiry/static/img/product_product_lait-image.jpg` (31 lines)
- `addons/product_expiry/static/img/product_product_pain-image.jpg` (22 lines)
- `addons/product_expiry/static/src/forecasted_details.js` (40 lines)
- `addons/product_expiry/static/src/forecasted_details.xml` (25 lines)
- `addons/product_expiry/static/src/forecasted_header.js` (8 lines)
- `addons/product_expiry/static/src/forecasted_header.xml` (18 lines)
- `addons/product_expiry/static/src/stock_traceability_report_backend.js` (37 lines)
- `addons/product_expiry/static/src/stock_traceability_report_backend.xml` (16 lines)
- `addons/product_expiry/static/tests/tours/stock_picking_tour.js` (41 lines)
- `addons/product_expiry/tests/__init__.py` (5 lines)
- `addons/product_expiry/tests/test_generate_serial_numbers.py` (305 lines)
- `addons/product_expiry/tests/test_stock_lot.py` (861 lines)
- `addons/product_expiry/views/product_template_views.xml` (38 lines)
- `addons/product_expiry/views/production_lot_views.xml` (88 lines)
- `addons/product_expiry/views/res_config_settings_views.xml` (15 lines)
- `addons/product_expiry/views/stock_move_views.xml` (54 lines)
- `addons/product_expiry/views/stock_quant_views.xml` (67 lines)
- `addons/product_expiry/wizard/__init__.py` (4 lines)
- `addons/product_expiry/wizard/confirm_expiry.py` (52 lines)
- `addons/product_expiry/wizard/confirm_expiry_view.xml` (36 lines)
- `addons/product_expiry/wizard/stock_lot_label_layout.py` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
