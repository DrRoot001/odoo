# Module: purchase

- **Module ID:** MOD-493
- **Path:** `addons/purchase`
- **Manifest:** `addons/purchase/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Purchase orders, tenders and agreements

No manifest description declared.

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 15 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 33 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 21 | Client behavior/assets. |
| Tests | 13 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "security/purchase_security.xml",
    "data/digest_data.xml",
    "data/portal_entry_data.xml",
    "views/account_move_views.xml",
    "data/purchase_data.xml",
    "data/ir_cron_data.xml",
    "report/purchase_reports.xml",
    "views/product_views.xml",
    "views/purchase_views.xml",
    "views/purchase_bill_line_match_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "report/purchase_bill_views.xml",
    "report/purchase_report_views.xml",
    "data/mail_templates.xml",
    "data/mail_template_data.xml",
    "views/portal_templates.xml",
    "report/purchase_order_templates.xml",
    "report/purchase_quotation_templates.xml",
    "views/analytic_account_views.xml",
    "wizard/bill_to_po_wizard_views.xml",
    "data/purchase_tour.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/purchase_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "purchase/static/src/components/**/*",
      "purchase/static/src/product_catalog/**/*",
      "purchase/static/src/toaster_button/*",
      "purchase/static/src/views/*.js",
      "purchase/static/src/js/tours/purchase.js",
      "purchase/static/src/js/tours/purchase_steps.js",
      "purchase/static/src/**/*.xml",
      "purchase/static/src/**/*.scss"
    ],
    "web.assets_frontend": [
      "purchase/static/src/interactions/**/*",
      "purchase/static/src/scss/purchase_portal.scss"
    ],
    "web.assets_tests": [
      "purchase/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/purchase/README.md` (63 lines)
- `addons/purchase/__init__.py` (20 lines)
- `addons/purchase/__manifest__.py` (62 lines)
- `addons/purchase/controllers/__init__.py` (4 lines)
- `addons/purchase/controllers/portal.py` (216 lines)
- `addons/purchase/data/digest_data.xml` (28 lines)
- `addons/purchase/data/ir_cron_data.xml` (12 lines)
- `addons/purchase/data/mail_template_data.xml` (130 lines)
- `addons/purchase/data/mail_templates.xml` (47 lines)
- `addons/purchase/data/portal_entry_data.xml` (22 lines)
- `addons/purchase/data/purchase_data.xml` (43 lines)
- `addons/purchase/data/purchase_demo.xml` (361 lines)
- `addons/purchase/data/purchase_tour.xml` (7 lines)
- `addons/purchase/i18n/af.po` (3,938 lines)
- `addons/purchase/i18n/am.po` (3,934 lines)
- `addons/purchase/i18n/ar.po` (4,415 lines)
- `addons/purchase/i18n/az.po` (4,152 lines)
- `addons/purchase/i18n/bg.po` (4,243 lines)
- `addons/purchase/i18n/bs.po` (4,083 lines)
- `addons/purchase/i18n/ca.po` (4,237 lines)
- `addons/purchase/i18n/cs.po` (4,330 lines)
- `addons/purchase/i18n/da.po` (4,219 lines)
- `addons/purchase/i18n/de.po` (4,622 lines)
- `addons/purchase/i18n/el.po` (4,115 lines)
- `addons/purchase/i18n/en_AU.po` (74 lines)
- `addons/purchase/i18n/es.po` (4,566 lines)
- `addons/purchase/i18n/es_419.po` (4,597 lines)
- `addons/purchase/i18n/es_CL.po` (510 lines)
- `addons/purchase/i18n/et.po` (4,226 lines)
- `addons/purchase/i18n/eu.po` (3,936 lines)
- `addons/purchase/i18n/fa.po` (4,162 lines)
- `addons/purchase/i18n/fi.po` (4,553 lines)
- `addons/purchase/i18n/fo.po` (3,936 lines)
- `addons/purchase/i18n/fr.po` (4,518 lines)
- `addons/purchase/i18n/fr_CA.po` (216 lines)
- `addons/purchase/i18n/gl.po` (3,936 lines)
- `addons/purchase/i18n/gu.po` (3,955 lines)
- `addons/purchase/i18n/he.po` (4,184 lines)
- `addons/purchase/i18n/hi.po` (4,100 lines)
- `addons/purchase/i18n/hr.po` (4,202 lines)
- `addons/purchase/i18n/hu.po` (4,139 lines)
- `addons/purchase/i18n/id.po` (4,564 lines)
- `addons/purchase/i18n/is.po` (3,945 lines)
- `addons/purchase/i18n/it.po` (4,584 lines)
- `addons/purchase/i18n/ja.po` (4,419 lines)
- `addons/purchase/i18n/ka.po` (3,940 lines)
- `addons/purchase/i18n/kab.po` (4,076 lines)
- `addons/purchase/i18n/km.po` (3,945 lines)
- `addons/purchase/i18n/ko.po` (4,398 lines)
- `addons/purchase/i18n/ku.po` (4,164 lines)
- `addons/purchase/i18n/lb.po` (3,939 lines)
- `addons/purchase/i18n/lo.po` (4,462 lines)
- `addons/purchase/i18n/lt.po` (4,164 lines)
- `addons/purchase/i18n/lv.po` (4,119 lines)
- `addons/purchase/i18n/mk.po` (3,944 lines)
- `addons/purchase/i18n/mn.po` (4,608 lines)
- `addons/purchase/i18n/my.po` (4,076 lines)
- `addons/purchase/i18n/nb.po` (4,145 lines)
- `addons/purchase/i18n/nl.po` (4,577 lines)
- `addons/purchase/i18n/pl.po` (4,526 lines)
- `addons/purchase/i18n/pt.po` (4,332 lines)
- `addons/purchase/i18n/pt_BR.po` (4,590 lines)
- `addons/purchase/i18n/purchase.pot` (4,027 lines)
- `addons/purchase/i18n/ro.po` (4,234 lines)
- `addons/purchase/i18n/ru.po` (4,233 lines)
- `addons/purchase/i18n/sk.po` (4,132 lines)
- `addons/purchase/i18n/sl.po` (4,130 lines)
- `addons/purchase/i18n/sq.po` (3,936 lines)
- `addons/purchase/i18n/sr@latin.po` (4,102 lines)
- `addons/purchase/i18n/sv.po` (4,230 lines)
- `addons/purchase/i18n/th.po` (4,464 lines)
- `addons/purchase/i18n/tr.po` (4,421 lines)
- `addons/purchase/i18n/uk.po` (4,198 lines)
- `addons/purchase/i18n/uz.po` (4,798 lines)
- `addons/purchase/i18n/vi.po` (4,424 lines)
- `addons/purchase/i18n/zh_CN.po` (4,444 lines)
- `addons/purchase/i18n/zh_TW.po` (4,145 lines)
- `addons/purchase/models/__init__.py` (18 lines)
- `addons/purchase/models/account_invoice.py` (729 lines)
- `addons/purchase/models/account_tax.py` (22 lines)
- `addons/purchase/models/analytic_account.py` (34 lines)
- `addons/purchase/models/analytic_applicability.py` (14 lines)
- `addons/purchase/models/ir_actions_report.py` (56 lines)
- `addons/purchase/models/product.py` (286 lines)
- `addons/purchase/models/product_category.py` (22 lines)
- `addons/purchase/models/purchase_bill_line_match.py` (255 lines)
- `addons/purchase/models/purchase_order.py` (1,433 lines)
- `addons/purchase/models/purchase_order_line.py` (944 lines)
- `addons/purchase/models/res_company.py` (51 lines)
- `addons/purchase/models/res_config_settings.py` (45 lines)
- `addons/purchase/models/res_groups.py` (14 lines)
- `addons/purchase/models/res_partner.py` (79 lines)
- `addons/purchase/report/__init__.py` (5 lines)
- `addons/purchase/report/purchase_bill.py` (73 lines)
- `addons/purchase/report/purchase_bill_views.xml` (52 lines)
- `addons/purchase/report/purchase_order_templates.xml` (157 lines)
- `addons/purchase/report/purchase_quotation_templates.xml` (96 lines)
- `addons/purchase/report/purchase_report.py` (138 lines)
- `addons/purchase/report/purchase_report_views.xml` (111 lines)
- `addons/purchase/report/purchase_reports.xml` (26 lines)
- `addons/purchase/security/ir.access.csv` (36 lines)
- `addons/purchase/security/purchase_security.xml` (40 lines)
- `addons/purchase/static/description/icon.png` (5 lines)
- `addons/purchase/static/description/icon.svg` (1 lines)
- `addons/purchase/static/description/icon_hi.png` (17 lines)
- `addons/purchase/static/src/components/matching_tag/matching_tag.js` (29 lines)
- `addons/purchase/static/src/components/matching_tag/matching_tag.xml` (8 lines)
- `addons/purchase/static/src/components/monetary_field_no_zero/monetary_field_no_zero.js` (28 lines)
- `addons/purchase/static/src/components/open_match_line_widget/open_match_line_widget.js` (27 lines)
- `addons/purchase/static/src/components/open_match_line_widget/open_match_line_widget.xml` (8 lines)
- `addons/purchase/static/src/components/purchase_file_uploader/purchase_file_uploader.js` (90 lines)
- `addons/purchase/static/src/components/purchase_file_uploader/purchase_file_uploader.xml` (18 lines)
- `addons/purchase/static/src/components/purchase_line_match_field/purchase_line_match_field.js` (36 lines)
- `addons/purchase/static/src/components/purchase_line_match_field/purchase_line_match_field.xml` (10 lines)
- `addons/purchase/static/src/components/tax_totals/tax_totals.xml` (12 lines)
- `addons/purchase/static/src/img/calculator.svg` (19 lines)
- `addons/purchase/static/src/img/milk-OTDPurchase.gif` (143 lines)
- `addons/purchase/static/src/interactions/purchase_datetimepicker.js` (34 lines)
- `addons/purchase/static/src/interactions/purchase_sidebar.js` (21 lines)
- `addons/purchase/static/src/js/tours/purchase.js` (170 lines)
- `addons/purchase/static/src/js/tours/purchase_steps.js` (14 lines)
- `addons/purchase/static/src/product_catalog/kanban_record.js` (18 lines)
- `addons/purchase/static/src/product_catalog/kanban_renderer.js` (47 lines)
- `addons/purchase/static/src/product_catalog/kanban_renderer.xml` (22 lines)
- `addons/purchase/static/src/product_catalog/kanban_view.js` (11 lines)
- `addons/purchase/static/src/product_catalog/purchase_order_line/purchase_order_line.js` (9 lines)
- `addons/purchase/static/src/scss/purchase_portal.scss` (8 lines)
- `addons/purchase/static/src/toaster_button/toaster_button_widget.js` (36 lines)
- `addons/purchase/static/src/toaster_button/toaster_button_widget.xml` (11 lines)
- `addons/purchase/static/src/views/purchase_dashboard.js` (48 lines)
- `addons/purchase/static/src/views/purchase_dashboard.scss` (44 lines)
- `addons/purchase/static/src/views/purchase_dashboard.xml` (186 lines)
- `addons/purchase/static/src/views/purchase_kanbanview.js` (16 lines)
- `addons/purchase/static/src/views/purchase_kanbanview.xml` (7 lines)
- `addons/purchase/static/src/views/purchase_listview.js` (27 lines)
- `addons/purchase/static/src/views/purchase_listview.xml` (13 lines)
- `addons/purchase/static/tests/tours/purchase_catalog.js` (84 lines)
- `addons/purchase/static/tests/tours/purchase_flow_tour.js` (73 lines)
- `addons/purchase/static/tests/tours/purchase_order_duplicate_section_test_tour.js` (25 lines)
- `addons/purchase/static/tests/tours/tour_helper.js` (165 lines)
- `addons/purchase/static/xls/product_purchase.xls` (69 lines)
- `addons/purchase/static/xls/products_import_template.xlsx` (537 lines)
- `addons/purchase/static/xls/requests_for_quotation_import_template.xlsx` (51 lines)
- `addons/purchase/tests/__init__.py` (15 lines)
- `addons/purchase/tests/test_access_rights.py` (203 lines)
- `addons/purchase/tests/test_accrued_purchase_orders.py` (289 lines)
- `addons/purchase/tests/test_import_files.py` (56 lines)
- `addons/purchase/tests/test_purchase.py` (1,666 lines)
- `addons/purchase/tests/test_purchase_dashboard.py` (99 lines)
- `addons/purchase/tests/test_purchase_downpayment.py` (146 lines)
- `addons/purchase/tests/test_purchase_flow.py` (34 lines)
- `addons/purchase/tests/test_purchase_invoice.py` (1,545 lines)
- `addons/purchase/tests/test_purchase_order_product_catalog.py` (23 lines)
- `addons/purchase/tests/test_purchase_order_report.py` (321 lines)
- `addons/purchase/tests/test_purchase_order_tax_mode.py` (62 lines)
- `addons/purchase/tests/test_purchase_product_catalog.py` (227 lines)
- `addons/purchase/views/account_move_views.xml` (72 lines)
- `addons/purchase/views/analytic_account_views.xml` (19 lines)
- `addons/purchase/views/portal_templates.xml` (387 lines)
- `addons/purchase/views/product_views.xml` (277 lines)

Additional files not expanded here: 8. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
