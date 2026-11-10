# Module: stock_account

- **Module ID:** MOD-560
- **Path:** `addons/stock_account`
- **Manifest:** `addons/stock_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Inventory, Logistic, Valuation, Accounting


WMS Accounting module
======================
This module makes the link between the 'stock' and 'account' modules and allows you to create accounting entries to value your stock movements

Key Features
------------
* Stock Valuation (periodical or automatic)
* Invoice from Picking

Dashboard / Reports for Warehouse Management includes:
------------------------------------------------------
* Stock Inventory Value at given date (support dates in the past)
    

Declared dependencies: `stock`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 16 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock",
    "account"
  ],
  "data": [
    "security/stock_account_security.xml",
    "data/stock_account_data.xml",
    "views/account_move_views.xml",
    "views/res_config_settings_views.xml",
    "views/report_invoice.xml",
    "views/stock_quant_views.xml",
    "views/product_views.xml",
    "views/product_value_views.xml",
    "views/stock_location_views.xml",
    "views/stock_lot_views.xml",
    "views/stock_move_views.xml",
    "wizard/stock_inventory_adjustment_name_views.xml",
    "report/account_invoice_report_view.xml",
    "report/stock_avco_audit_report_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "stock_account/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/stock_account/__init__.py` (60 lines)
- `addons/stock_account/__manifest__.py` (50 lines)
- `addons/stock_account/data/stock_account_data.xml` (7 lines)
- `addons/stock_account/i18n/af.po` (1,223 lines)
- `addons/stock_account/i18n/am.po` (1,219 lines)
- `addons/stock_account/i18n/ar.po` (1,159 lines)
- `addons/stock_account/i18n/az.po` (1,052 lines)
- `addons/stock_account/i18n/bg.po` (1,067 lines)
- `addons/stock_account/i18n/bs.po` (1,028 lines)
- `addons/stock_account/i18n/ca.po` (1,137 lines)
- `addons/stock_account/i18n/cs.po` (1,083 lines)
- `addons/stock_account/i18n/da.po` (1,115 lines)
- `addons/stock_account/i18n/de.po` (1,330 lines)
- `addons/stock_account/i18n/el.po` (1,058 lines)
- `addons/stock_account/i18n/es.po` (1,289 lines)
- `addons/stock_account/i18n/es_419.po` (1,303 lines)
- `addons/stock_account/i18n/es_CL.po` (186 lines)
- `addons/stock_account/i18n/et.po` (1,209 lines)
- `addons/stock_account/i18n/eu.po` (1,221 lines)
- `addons/stock_account/i18n/fa.po` (1,105 lines)
- `addons/stock_account/i18n/fi.po` (1,276 lines)
- `addons/stock_account/i18n/fo.po` (1,221 lines)
- `addons/stock_account/i18n/fr.po` (1,297 lines)
- `addons/stock_account/i18n/fr_BE.po` (86 lines)
- `addons/stock_account/i18n/fr_CA.po` (107 lines)
- `addons/stock_account/i18n/gl.po` (1,221 lines)
- `addons/stock_account/i18n/gu.po` (1,225 lines)
- `addons/stock_account/i18n/he.po` (1,116 lines)
- `addons/stock_account/i18n/hi.po` (1,049 lines)
- `addons/stock_account/i18n/hr.po` (1,068 lines)
- `addons/stock_account/i18n/hu.po` (1,091 lines)
- `addons/stock_account/i18n/id.po` (1,237 lines)
- `addons/stock_account/i18n/is.po` (1,224 lines)
- `addons/stock_account/i18n/it.po` (1,304 lines)
- `addons/stock_account/i18n/ja.po` (1,267 lines)
- `addons/stock_account/i18n/ka.po` (1,225 lines)
- `addons/stock_account/i18n/kab.po` (1,014 lines)
- `addons/stock_account/i18n/km.po` (1,226 lines)
- `addons/stock_account/i18n/ko.po` (1,167 lines)
- `addons/stock_account/i18n/ku.po` (1,032 lines)
- `addons/stock_account/i18n/lo.po` (1,059 lines)
- `addons/stock_account/i18n/lt.po` (1,092 lines)
- `addons/stock_account/i18n/lv.po` (1,036 lines)
- `addons/stock_account/i18n/mk.po` (1,227 lines)
- `addons/stock_account/i18n/mn.po` (1,142 lines)
- `addons/stock_account/i18n/my.po` (1,048 lines)
- `addons/stock_account/i18n/nb.po` (1,103 lines)
- `addons/stock_account/i18n/nl.po` (1,325 lines)
- `addons/stock_account/i18n/pl.po` (1,140 lines)
- `addons/stock_account/i18n/pt.po` (1,123 lines)
- `addons/stock_account/i18n/pt_BR.po` (1,310 lines)
- `addons/stock_account/i18n/ro.po` (1,240 lines)
- `addons/stock_account/i18n/ru.po` (1,264 lines)
- `addons/stock_account/i18n/sk.po` (1,065 lines)
- `addons/stock_account/i18n/sl.po` (1,069 lines)
- `addons/stock_account/i18n/sq.po` (1,221 lines)
- `addons/stock_account/i18n/sr@latin.po` (1,048 lines)
- `addons/stock_account/i18n/stock_account.pot` (1,004 lines)
- `addons/stock_account/i18n/sv.po` (1,139 lines)
- `addons/stock_account/i18n/ta.po` (1,223 lines)
- `addons/stock_account/i18n/th.po` (1,117 lines)
- `addons/stock_account/i18n/tr.po` (1,291 lines)
- `addons/stock_account/i18n/uk.po` (1,117 lines)
- `addons/stock_account/i18n/uz.po` (1,355 lines)
- `addons/stock_account/i18n/vi.po` (1,146 lines)
- `addons/stock_account/i18n/zh_CN.po` (1,174 lines)
- `addons/stock_account/i18n/zh_TW.po` (1,128 lines)
- `addons/stock_account/models/__init__.py` (19 lines)
- `addons/stock_account/models/account_move.py` (98 lines)
- `addons/stock_account/models/account_move_line.py` (71 lines)
- `addons/stock_account/models/analytic_account.py` (110 lines)
- `addons/stock_account/models/product.py` (776 lines)
- `addons/stock_account/models/product_value.py` (131 lines)
- `addons/stock_account/models/res_company.py` (139 lines)
- `addons/stock_account/models/res_config_settings.py` (10 lines)
- `addons/stock_account/models/res_groups.py` (13 lines)
- `addons/stock_account/models/stock_location.py` (35 lines)
- `addons/stock_account/models/stock_lot.py` (128 lines)
- `addons/stock_account/models/stock_move.py` (840 lines)
- `addons/stock_account/models/stock_move_line.py` (55 lines)
- `addons/stock_account/models/stock_picking.py` (37 lines)
- `addons/stock_account/models/stock_picking_type.py` (9 lines)
- `addons/stock_account/models/stock_quant.py` (108 lines)
- `addons/stock_account/report/__init__.py` (5 lines)
- `addons/stock_account/report/account_invoice_report_view.xml` (10 lines)
- `addons/stock_account/report/account_stock_valuation_report.py` (62 lines)
- `addons/stock_account/report/stock_avco_audit_report.py` (143 lines)
- `addons/stock_account/report/stock_avco_audit_report_views.xml` (29 lines)
- `addons/stock_account/report/stock_forecasted.py` (35 lines)
- `addons/stock_account/security/ir.access.csv` (13 lines)
- `addons/stock_account/security/stock_account_security.xml` (7 lines)
- `addons/stock_account/static/src/fields/boolean_confirm.js` (57 lines)
- `addons/stock_account/static/src/fields/boolean_confirm.xml` (12 lines)
- `addons/stock_account/static/src/stock_account_forecasted/forecasted_header.js` (39 lines)
- `addons/stock_account/static/src/stock_account_forecasted/forecasted_header.xml` (13 lines)
- `addons/stock_account/static/src/stock_valuation/stock_valuation_report.js` (35 lines)
- `addons/stock_account/static/src/views/stock_account_move_list_view.js` (78 lines)
- `addons/stock_account/tests/__init__.py` (6 lines)
- `addons/stock_account/tests/common.py` (480 lines)
- `addons/stock_account/tests/test_account_move.py` (514 lines)
- `addons/stock_account/tests/test_anglo_saxon_valuation_reconciliation_common.py` (85 lines)
- `addons/stock_account/tests/test_lot_valuation.py` (970 lines)
- `addons/stock_account/tests/test_multicompany_lot_valuation.py` (74 lines)
- `addons/stock_account/tests/test_stockvaluation.py` (4,039 lines)
- `addons/stock_account/tests/test_stockvaluationlayer.py` (1,190 lines)
- `addons/stock_account/views/account_move_views.xml` (19 lines)
- `addons/stock_account/views/product_value_views.xml` (82 lines)
- `addons/stock_account/views/product_views.xml` (65 lines)
- `addons/stock_account/views/report_invoice.xml` (29 lines)
- `addons/stock_account/views/res_config_settings_views.xml` (25 lines)
- `addons/stock_account/views/stock_location_views.xml` (21 lines)
- `addons/stock_account/views/stock_lot_views.xml` (19 lines)
- `addons/stock_account/views/stock_move_views.xml` (98 lines)
- `addons/stock_account/views/stock_quant_views.xml` (38 lines)
- `addons/stock_account/wizard/__init__.py` (3 lines)
- `addons/stock_account/wizard/stock_inventory_adjustment_name.py` (21 lines)
- `addons/stock_account/wizard/stock_inventory_adjustment_name_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
