# Module: pos_hr

- **Module ID:** MOD-433
- **Path:** `addons/pos_hr`
- **Manifest:** `addons/pos_hr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and HR


This module allows Employees (and not users) to log in to the Point of Sale application using a barcode, a PIN number or both.
The actual till still requires one user but an unlimited number of employees can log on to that till and process sales.
    

Declared dependencies: `point_of_sale`, `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 23 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 31 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "hr"
  ],
  "data": [
    "views/pos_config.xml",
    "views/pos_order_view.xml",
    "views/pos_payment_view.xml",
    "views/pos_order_report_view.xml",
    "views/single_employee_sales_report.xml",
    "views/res_config_settings_views.xml",
    "views/point_of_sale_dashboard.xml",
    "views/pos_session_view.xml",
    "wizard/pos_daily_sales_reports.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_hr/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_hr/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_hr/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_hr/__init__.py` (9 lines)
- `addons/pos_hr/__manifest__.py` (41 lines)
- `addons/pos_hr/i18n/ar.po` (513 lines)
- `addons/pos_hr/i18n/az.po` (465 lines)
- `addons/pos_hr/i18n/bg.po` (468 lines)
- `addons/pos_hr/i18n/bs.po` (460 lines)
- `addons/pos_hr/i18n/ca.po` (485 lines)
- `addons/pos_hr/i18n/cs.po` (511 lines)
- `addons/pos_hr/i18n/da.po` (514 lines)
- `addons/pos_hr/i18n/de.po` (547 lines)
- `addons/pos_hr/i18n/el.po` (466 lines)
- `addons/pos_hr/i18n/es.po` (527 lines)
- `addons/pos_hr/i18n/es_419.po` (525 lines)
- `addons/pos_hr/i18n/et.po` (497 lines)
- `addons/pos_hr/i18n/fa.po` (475 lines)
- `addons/pos_hr/i18n/fi.po` (517 lines)
- `addons/pos_hr/i18n/fr.po` (523 lines)
- `addons/pos_hr/i18n/he.po` (502 lines)
- `addons/pos_hr/i18n/hi.po` (465 lines)
- `addons/pos_hr/i18n/hr.po` (490 lines)
- `addons/pos_hr/i18n/hu.po` (473 lines)
- `addons/pos_hr/i18n/id.po` (519 lines)
- `addons/pos_hr/i18n/it.po` (529 lines)
- `addons/pos_hr/i18n/ja.po` (518 lines)
- `addons/pos_hr/i18n/kab.po` (459 lines)
- `addons/pos_hr/i18n/ko.po` (509 lines)
- `addons/pos_hr/i18n/ku.po` (462 lines)
- `addons/pos_hr/i18n/lo.po` (478 lines)
- `addons/pos_hr/i18n/lt.po` (473 lines)
- `addons/pos_hr/i18n/lv.po` (459 lines)
- `addons/pos_hr/i18n/mn.po` (471 lines)
- `addons/pos_hr/i18n/my.po` (462 lines)
- `addons/pos_hr/i18n/nb.po` (478 lines)
- `addons/pos_hr/i18n/nl.po` (542 lines)
- `addons/pos_hr/i18n/pl.po` (529 lines)
- `addons/pos_hr/i18n/pos_hr.pot` (452 lines)
- `addons/pos_hr/i18n/pt.po` (486 lines)
- `addons/pos_hr/i18n/pt_BR.po` (546 lines)
- `addons/pos_hr/i18n/ro.po` (506 lines)
- `addons/pos_hr/i18n/ru.po` (521 lines)
- `addons/pos_hr/i18n/sk.po` (458 lines)
- `addons/pos_hr/i18n/sl.po` (477 lines)
- `addons/pos_hr/i18n/sr@latin.po` (466 lines)
- `addons/pos_hr/i18n/sv.po` (501 lines)
- `addons/pos_hr/i18n/th.po` (496 lines)
- `addons/pos_hr/i18n/tr.po` (527 lines)
- `addons/pos_hr/i18n/uk.po` (498 lines)
- `addons/pos_hr/i18n/uz.po` (571 lines)
- `addons/pos_hr/i18n/vi.po` (509 lines)
- `addons/pos_hr/i18n/zh_CN.po` (519 lines)
- `addons/pos_hr/i18n/zh_TW.po` (508 lines)
- `addons/pos_hr/models/__init__.py` (13 lines)
- `addons/pos_hr/models/account_bank_statement.py` (8 lines)
- `addons/pos_hr/models/hr_employee.py` (99 lines)
- `addons/pos_hr/models/pos_config.py` (110 lines)
- `addons/pos_hr/models/pos_order.py` (27 lines)
- `addons/pos_hr/models/pos_order_receipt.py` (10 lines)
- `addons/pos_hr/models/pos_payment.py` (15 lines)
- `addons/pos_hr/models/pos_session.py` (102 lines)
- `addons/pos_hr/models/product_product.py` (11 lines)
- `addons/pos_hr/models/res_config_settings.py` (65 lines)
- `addons/pos_hr/models/res_partner.py` (21 lines)
- `addons/pos_hr/models/single_employee_sales_report.py` (32 lines)
- `addons/pos_hr/report/__init__.py` (3 lines)
- `addons/pos_hr/report/pos_order_report.py` (13 lines)
- `addons/pos_hr/static/src/app/components/navbar/cashier_name/cashier_name.js` (29 lines)
- `addons/pos_hr/static/src/app/components/navbar/cashier_name/cashier_name.xml` (10 lines)
- `addons/pos_hr/static/src/app/components/navbar/navbar.js` (17 lines)
- `addons/pos_hr/static/src/app/components/navbar/navbar.xml` (23 lines)
- `addons/pos_hr/static/src/app/components/popups/cash_move_popup/cash_move_popup.js` (17 lines)
- `addons/pos_hr/static/src/app/components/popups/cashier_selection_popup/cashier_selection_popup.js` (35 lines)
- `addons/pos_hr/static/src/app/components/popups/cashier_selection_popup/cashier_selection_popup.xml` (56 lines)
- `addons/pos_hr/static/src/app/components/popups/closing_popup/closing_popup.js` (15 lines)
- `addons/pos_hr/static/src/app/components/popups/closing_popup/closing_popup.xml` (49 lines)
- `addons/pos_hr/static/src/app/models/data_service_options.js` (8 lines)
- `addons/pos_hr/static/src/app/models/pos_order.js` (9 lines)
- `addons/pos_hr/static/src/app/plugins/access_right_plugin.js` (226 lines)
- `addons/pos_hr/static/src/app/screens/login_screen/login_screen.js` (96 lines)
- `addons/pos_hr/static/src/app/screens/login_screen/login_screen.xml` (31 lines)
- `addons/pos_hr/static/src/app/screens/order_details_dialog.js` (19 lines)
- `addons/pos_hr/static/src/app/services/pos_store.js` (236 lines)
- `addons/pos_hr/static/src/app/utils/order_payment_validation.js` (12 lines)
- `addons/pos_hr/static/tests/tours/pos_hr_tour.js` (481 lines)
- `addons/pos_hr/static/tests/tours/utils/cashier_selection_popup_util.js` (30 lines)
- `addons/pos_hr/static/tests/tours/utils/pos_hr_helpers.js` (73 lines)
- `addons/pos_hr/static/tests/unit/components/navbar/cashier_name.test.js` (28 lines)
- `addons/pos_hr/static/tests/unit/components/popups/cash_move_popup.test.js` (34 lines)
- `addons/pos_hr/static/tests/unit/components/popups/cashier_selection_popup.test.js` (65 lines)
- `addons/pos_hr/static/tests/unit/components/popups/product_info_popup.test.js` (58 lines)
- `addons/pos_hr/static/tests/unit/components/screens/feedback_screen.test.js` (20 lines)
- `addons/pos_hr/static/tests/unit/components/screens/login_screen.test.js` (22 lines)
- `addons/pos_hr/static/tests/unit/components/screens/payment_screen.test.js` (47 lines)
- `addons/pos_hr/static/tests/unit/components/screens/ticket_screen.test.js` (27 lines)
- `addons/pos_hr/static/tests/unit/data/hr_employee.data.js` (55 lines)
- `addons/pos_hr/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/pos_hr/static/tests/unit/data/pos_order.data.js` (8 lines)
- `addons/pos_hr/static/tests/unit/data/pos_session.data.js` (11 lines)
- `addons/pos_hr/static/tests/unit/models/pos_order.test.js` (14 lines)
- `addons/pos_hr/static/tests/unit/services/access_right_plugin.test.js` (81 lines)
- `addons/pos_hr/static/tests/unit/services/pos_store.test.js` (175 lines)
- `addons/pos_hr/static/tests/unit/utils.js` (25 lines)
- `addons/pos_hr/tests/__init__.py` (7 lines)
- `addons/pos_hr/tests/test_frontend.py` (334 lines)
- `addons/pos_hr/tests/test_point_of_sale_flow.py` (55 lines)
- `addons/pos_hr/tests/test_res_config_settings.py` (129 lines)
- `addons/pos_hr/tests/test_synchronisation.py` (30 lines)
- `addons/pos_hr/views/point_of_sale_dashboard.xml` (16 lines)
- `addons/pos_hr/views/pos_config.xml` (29 lines)
- `addons/pos_hr/views/pos_order_report_view.xml` (24 lines)
- `addons/pos_hr/views/pos_order_view.xml` (41 lines)
- `addons/pos_hr/views/pos_payment_view.xml` (13 lines)
- `addons/pos_hr/views/pos_session_view.xml` (13 lines)
- `addons/pos_hr/views/res_config_settings_views.xml` (28 lines)
- `addons/pos_hr/views/single_employee_sales_report.xml` (47 lines)
- `addons/pos_hr/wizard/__init__.py` (3 lines)
- `addons/pos_hr/wizard/pos_daily_sales_reports.py` (29 lines)
- `addons/pos_hr/wizard/pos_daily_sales_reports.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
