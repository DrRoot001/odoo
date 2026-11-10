# Module: sale_timesheet

- **Module ID:** MOD-536
- **Path:** `addons/sale_timesheet`
- **Manifest:** `addons/sale_timesheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Sell based on timesheets


Allows to sell timesheets in your sales order
=============================================

This module set the right product on all timesheet lines
according to the order/contract you work on. This allows to
have real delivered quantities in sales orders.


Declared dependencies: `sale_project`, `hr_timesheet`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 47 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 16 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 18 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 22 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_project",
    "hr_timesheet"
  ],
  "data": [
    "data/sale_service_data.xml",
    "security/sale_timesheet_security.xml",
    "views/account_analytic_line_views.xml",
    "views/account_invoice_views.xml",
    "views/sale_order_views.xml",
    "views/product_views.xml",
    "views/project_task_views.xml",
    "views/res_config_settings_views.xml",
    "views/sale_timesheet_portal_templates.xml",
    "views/project_sharing_views.xml",
    "views/project_portal_templates.xml",
    "report/timesheets_analysis_views.xml",
    "report/report_timesheet_templates.xml",
    "report/project_report_view.xml",
    "wizard/sale_make_invoice_advance_views.xml",
    "security/ir.access.csv",
    "data/mail_template_data.xml"
  ],
  "demo": [
    "data/sale_service_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "sale_timesheet/static/src/scss/sale_timesheet_portal.scss"
    ],
    "web.assets_backend": [
      "sale_timesheet/static/src/components/**/*"
    ],
    "web.assets_tests": [
      "sale_timesheet/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "sale_timesheet/static/tests/**/*",
      [
        "remove",
        "sale_timesheet/static/tests/tours/**/*"
      ]
    ],
    "project.webclient": [
      "sale_timesheet/static/src/components/so_line_field/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_timesheet/__init__.py` (33 lines)
- `addons/sale_timesheet/__manifest__.py` (61 lines)
- `addons/sale_timesheet/controllers/__init__.py` (4 lines)
- `addons/sale_timesheet/controllers/portal.py` (137 lines)
- `addons/sale_timesheet/data/mail_template_data.xml` (12 lines)
- `addons/sale_timesheet/data/sale_service_data.xml` (66 lines)
- `addons/sale_timesheet/data/sale_service_demo.xml` (2,827 lines)
- `addons/sale_timesheet/i18n/af.po` (1,575 lines)
- `addons/sale_timesheet/i18n/am.po` (1,571 lines)
- `addons/sale_timesheet/i18n/ar.po` (1,662 lines)
- `addons/sale_timesheet/i18n/az.po` (1,564 lines)
- `addons/sale_timesheet/i18n/bg.po` (1,567 lines)
- `addons/sale_timesheet/i18n/bs.po` (1,556 lines)
- `addons/sale_timesheet/i18n/ca.po` (1,666 lines)
- `addons/sale_timesheet/i18n/cs.po` (1,646 lines)
- `addons/sale_timesheet/i18n/da.po` (1,658 lines)
- `addons/sale_timesheet/i18n/de.po` (1,760 lines)
- `addons/sale_timesheet/i18n/el.po` (1,567 lines)
- `addons/sale_timesheet/i18n/es.po` (1,686 lines)
- `addons/sale_timesheet/i18n/es_419.po` (1,725 lines)
- `addons/sale_timesheet/i18n/es_CL.po` (42 lines)
- `addons/sale_timesheet/i18n/et.po` (1,660 lines)
- `addons/sale_timesheet/i18n/eu.po` (1,573 lines)
- `addons/sale_timesheet/i18n/fa.po` (1,585 lines)
- `addons/sale_timesheet/i18n/fi.po` (1,718 lines)
- `addons/sale_timesheet/i18n/fo.po` (1,573 lines)
- `addons/sale_timesheet/i18n/fr.po` (1,729 lines)
- `addons/sale_timesheet/i18n/fr_BE.po` (30 lines)
- `addons/sale_timesheet/i18n/fr_CA.po` (31 lines)
- `addons/sale_timesheet/i18n/gl.po` (1,573 lines)
- `addons/sale_timesheet/i18n/gu.po` (1,575 lines)
- `addons/sale_timesheet/i18n/he.po` (1,587 lines)
- `addons/sale_timesheet/i18n/hi.po` (1,565 lines)
- `addons/sale_timesheet/i18n/hr.po` (1,576 lines)
- `addons/sale_timesheet/i18n/hu.po` (1,671 lines)
- `addons/sale_timesheet/i18n/hy.po` (1,573 lines)
- `addons/sale_timesheet/i18n/id.po` (1,688 lines)
- `addons/sale_timesheet/i18n/is.po` (1,575 lines)
- `addons/sale_timesheet/i18n/it.po` (1,737 lines)
- `addons/sale_timesheet/i18n/ja.po` (1,697 lines)
- `addons/sale_timesheet/i18n/ka.po` (1,577 lines)
- `addons/sale_timesheet/i18n/kab.po` (1,552 lines)
- `addons/sale_timesheet/i18n/km.po` (1,576 lines)
- `addons/sale_timesheet/i18n/ko.po` (1,659 lines)
- `addons/sale_timesheet/i18n/ku.po` (1,551 lines)
- `addons/sale_timesheet/i18n/lo.po` (1,657 lines)
- `addons/sale_timesheet/i18n/lt.po` (1,585 lines)
- `addons/sale_timesheet/i18n/lv.po` (1,565 lines)
- `addons/sale_timesheet/i18n/mk.po` (1,575 lines)
- `addons/sale_timesheet/i18n/mn.po` (1,571 lines)
- `addons/sale_timesheet/i18n/my.po` (1,553 lines)
- `addons/sale_timesheet/i18n/nb.po` (1,568 lines)
- `addons/sale_timesheet/i18n/nl.po` (1,736 lines)
- `addons/sale_timesheet/i18n/pl.po` (1,739 lines)
- `addons/sale_timesheet/i18n/pt.po` (1,666 lines)
- `addons/sale_timesheet/i18n/pt_BR.po` (1,728 lines)
- `addons/sale_timesheet/i18n/ro.po` (1,656 lines)
- `addons/sale_timesheet/i18n/ru.po` (1,680 lines)
- `addons/sale_timesheet/i18n/sale_timesheet.pot` (1,520 lines)
- `addons/sale_timesheet/i18n/sk.po` (1,586 lines)
- `addons/sale_timesheet/i18n/sl.po` (1,575 lines)
- `addons/sale_timesheet/i18n/sr@latin.po` (1,561 lines)
- `addons/sale_timesheet/i18n/sv.po` (1,662 lines)
- `addons/sale_timesheet/i18n/th.po` (1,651 lines)
- `addons/sale_timesheet/i18n/tr.po` (1,693 lines)
- `addons/sale_timesheet/i18n/uk.po` (1,646 lines)
- `addons/sale_timesheet/i18n/uz.po` (1,879 lines)
- `addons/sale_timesheet/i18n/vi.po` (1,690 lines)
- `addons/sale_timesheet/i18n/zh_CN.po` (1,650 lines)
- `addons/sale_timesheet/i18n/zh_TW.po` (1,615 lines)
- `addons/sale_timesheet/models/__init__.py` (18 lines)
- `addons/sale_timesheet/models/account_analytic_line.py` (288 lines)
- `addons/sale_timesheet/models/account_move.py` (111 lines)
- `addons/sale_timesheet/models/account_move_line.py` (42 lines)
- `addons/sale_timesheet/models/account_move_reversal.py` (26 lines)
- `addons/sale_timesheet/models/account_move_send.py` (16 lines)
- `addons/sale_timesheet/models/hr_employee.py` (15 lines)
- `addons/sale_timesheet/models/hr_employee_departure.py` (11 lines)
- `addons/sale_timesheet/models/product_product.py` (58 lines)
- `addons/sale_timesheet/models/product_template.py` (110 lines)
- `addons/sale_timesheet/models/project_project.py` (297 lines)
- `addons/sale_timesheet/models/project_sale_line_employee_map.py` (142 lines)
- `addons/sale_timesheet/models/project_task.py` (147 lines)
- `addons/sale_timesheet/models/res_config_settings.py` (10 lines)
- `addons/sale_timesheet/models/sale_order.py` (159 lines)
- `addons/sale_timesheet/models/sale_order_line.py` (213 lines)
- `addons/sale_timesheet/report/__init__.py` (5 lines)
- `addons/sale_timesheet/report/project_report.py` (25 lines)
- `addons/sale_timesheet/report/project_report_view.xml` (37 lines)
- `addons/sale_timesheet/report/report_timesheet_templates.xml` (92 lines)
- `addons/sale_timesheet/report/timesheets_analysis_report.py` (59 lines)
- `addons/sale_timesheet/report/timesheets_analysis_views.xml` (209 lines)
- `addons/sale_timesheet/security/ir.access.csv` (5 lines)
- `addons/sale_timesheet/security/sale_timesheet_security.xml` (18 lines)
- `addons/sale_timesheet/static/description/icon.png` (27 lines)
- `addons/sale_timesheet/static/description/icon.svg` (1 lines)
- `addons/sale_timesheet/static/description/icon_hi.png` (137 lines)
- `addons/sale_timesheet/static/img/employee_jjo-image.webp` (39 lines)
- `addons/sale_timesheet/static/img/employee_jsm-image.webp` (41 lines)
- `addons/sale_timesheet/static/img/product_product_time_product.png` (43 lines)
- `addons/sale_timesheet/static/src/components/so_line_field/so_line_field.js` (33 lines)
- `addons/sale_timesheet/static/src/components/so_line_field/so_line_field.xml` (9 lines)
- `addons/sale_timesheet/static/src/scss/sale_timesheet_portal.scss` (15 lines)
- `addons/sale_timesheet/static/tests/sale_timesheet_test_helpers.js` (44 lines)
- `addons/sale_timesheet/static/tests/so_line_create_button.test.js` (171 lines)
- `addons/sale_timesheet/static/tests/so_line_field.test.js` (110 lines)
- `addons/sale_timesheet/static/tests/tours/sale_timesheet_tour.js` (301 lines)
- `addons/sale_timesheet/tests/__init__.py` (24 lines)
- `addons/sale_timesheet/tests/common.py` (295 lines)
- `addons/sale_timesheet/tests/test_account_analytic_line.py` (149 lines)
- `addons/sale_timesheet/tests/test_analytic_to_sale_timesheet.py` (94 lines)
- `addons/sale_timesheet/tests/test_edit_so_line_timesheet.py` (70 lines)
- `addons/sale_timesheet/tests/test_performance.py` (44 lines)
- `addons/sale_timesheet/tests/test_project.py` (287 lines)
- `addons/sale_timesheet/tests/test_project_billing.py` (368 lines)
- `addons/sale_timesheet/tests/test_project_pricing_type.py` (113 lines)
- `addons/sale_timesheet/tests/test_reinvoice.py` (415 lines)
- `addons/sale_timesheet/tests/test_report_timesheet.py` (62 lines)
- `addons/sale_timesheet/tests/test_sale_service.py` (1,071 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet.py` (2,048 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_accrued_entries.py` (138 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_portal.py` (46 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_product_product.py` (31 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_product_template.py` (31 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_report.py` (238 lines)
- `addons/sale_timesheet/tests/test_sale_timesheet_ui.py` (37 lines)
- `addons/sale_timesheet/tests/test_so_line_determined_in_timesheet.py` (327 lines)
- `addons/sale_timesheet/tests/test_task_analysis.py` (32 lines)
- `addons/sale_timesheet/tests/test_upsell_warning.py` (335 lines)
- `addons/sale_timesheet/views/account_analytic_line_views.xml` (280 lines)
- `addons/sale_timesheet/views/account_invoice_views.xml` (80 lines)
- `addons/sale_timesheet/views/product_views.xml` (56 lines)
- `addons/sale_timesheet/views/project_portal_templates.xml` (35 lines)
- `addons/sale_timesheet/views/project_sharing_views.xml` (48 lines)
- `addons/sale_timesheet/views/project_task_views.xml` (266 lines)
- `addons/sale_timesheet/views/res_config_settings_views.xml` (23 lines)
- `addons/sale_timesheet/views/sale_order_views.xml` (30 lines)
- `addons/sale_timesheet/views/sale_timesheet_portal_templates.xml` (119 lines)
- `addons/sale_timesheet/wizard/__init__.py` (4 lines)
- `addons/sale_timesheet/wizard/sale_make_invoice_advance.py` (50 lines)
- `addons/sale_timesheet/wizard/sale_make_invoice_advance_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
