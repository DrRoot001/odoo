# Module: account

- **Module ID:** MOD-001
- **Path:** `addons/account`
- **Manifest:** `addons/account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Invoices & Payments


Invoicing & Payments
====================
The specific and easy-to-use Invoicing system in Odoo allows you to keep track of your accounting, even when you are not an accountant. It provides an easy way to follow up on your vendors and customers.

You could use this simplified accounting in case you work with an (external) account to keep your books, and you still want to keep track of payments. This module also offers you an easy method of registering payments, without having to encode complete abstracts of account.
    

Declared dependencies: `base_setup`, `onboarding`, `product`, `analytic`, `portal`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 173 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 57 | Files under `models/` or `models.py`. |
| Controller-path Python files | 6 | Files under `controllers/` or `controllers.py`. |
| XML files | 138 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 115 | Client behavior/assets. |
| Tests | 80 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 10 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "onboarding",
    "product",
    "analytic",
    "portal",
    "digest"
  ],
  "data": [
    "security/account_security.xml",
    "data/account_data.xml",
    "data/digest_data.xml",
    "views/account_report.xml",
    "data/mail_template_data.xml",
    "data/onboarding_data.xml",
    "data/account_tour.xml",
    "data/ir_sequence.xml",
    "data/res_country_group.xml",
    "data/portal_entry_data.xml",
    "views/account_payment_view.xml",
    "wizard/account_automatic_entry_wizard_views.xml",
    "wizard/account_autopost_bills_wizard.xml",
    "wizard/account_unreconcile_view.xml",
    "wizard/account_move_reversal_view.xml",
    "wizard/account_resequence_views.xml",
    "wizard/account_payment_register_views.xml",
    "views/account_move_views.xml",
    "wizard/setup_wizards_view.xml",
    "views/account_account_views.xml",
    "views/account_journal_views.xml",
    "views/account_account_tag_views.xml",
    "views/account_bank_statement_views.xml",
    "views/account_reconcile_model_views.xml",
    "views/account_tax_views.xml",
    "views/account_full_reconcile_views.xml",
    "views/account_payment_term_views.xml",
    "views/account_payment_method.xml",
    "views/res_partner_bank_views.xml",
    "views/report_statement.xml",
    "views/terms_template.xml",
    "wizard/account_validate_move_view.xml",
    "views/res_company_views.xml",
    "views/product_view.xml",
    "views/account_analytic_plan_views.xml",
    "views/account_analytic_account_views.xml",
    "views/account_analytic_distribution_model_views.xml",
    "views/account_analytic_line_views.xml",
    "views/report_invoice.xml",
    "report/account_invoice_report_view.xml",
    "views/account_cash_rounding_view.xml",
    "views/ir_actions_views.xml",
    "views/ir_module_views.xml",
    "views/base_document_layout_views.xml",
    "views/res_config_settings_views.xml",
    "views/partner_view.xml",
    "views/account_journal_dashboard_view.xml",
    "views/account_portal_templates.xml",
    "views/report_payment_receipt_templates.xml",
    "data/service_cron.xml",
    "views/account_incoterms_view.xml",
    "data/account_incoterms_data.xml",
    "views/digest_views.xml",
    "wizard/account_move_send_wizard.xml",
    "wizard/account_move_send_batch_wizard.xml",
    "report/account_hash_integrity_templates.xml",
    "report/account_stock_valuation_report.xml",
    "views/res_currency.xml",
    "views/res_country_group_view.xml",
    "views/account_menuitem.xml",
    "wizard/account_secure_entries_wizard.xml",
    "views/mail_message_views.xml",
    "wizard/accrued_orders.xml",
    "views/bill_preview_template.xml",
    "data/account_reports_data.xml",
    "views/uom_uom_views.xml",
    "views/product_views.xml",
    "views/tests_shared_js_python.xml",
    "views/account_lock_exception_views.xml",
    "views/report_templates.xml",
    "wizard/account_merge_wizard_views.xml",
    "data/ir_config_parameter_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/account_demo.xml",
    "demo/res_partner_bank_demo.xml"
  ],
  "assets": {
    "web._assets_primary_variables": [
      "account/static/src/scss/variables.scss"
    ],
    "web.assets_backend": [
      "account/static/src/css/account_bank_and_cash.css",
      "account/static/src/css/account.css",
      "account/static/src/css/account_payment.scss",
      "account/static/src/scss/account.scss",
      "account/static/src/scss/account_journal_dashboard.scss",
      "account/static/src/scss/account_searchpanel.scss",
      "account/static/src/scss/account_payment_term.scss",
      "account/static/src/scss/account_reconcile_model.scss",
      "account/static/src/scss/account_multi_ledger.scss",
      "account/static/src/scss/account_move_send_wizard.scss",
      "account/static/src/scss/account_type_selection.scss",
      "account/static/src/components/**/*",
      "account/static/src/services/*.js",
      "account/static/src/views/**/*",
      "account/static/src/js/tours/*",
      "account/static/src/js/search/search_bar/search_bar.js",
      "account/static/src/helpers/*.js",
      "account/static/src/webclient/**/*",
      [
        "remove",
        "account/static/src/**/*.dark.scss"
      ]
    ],
    "web.assets_web_dark": [
      "account/static/src/**/*.dark.scss"
    ],
    "web.assets_unit_tests": [
      "account/static/tests/**/*",
      [
        "remove",
        "account/static/tests/tours/**/*"
      ]
    ],
    "web.assets_frontend": [
      "account/static/src/interactions/**/*",
      "account/static/src/components/tests_shared_js_python/*",
      "account/static/src/helpers/*.js"
    ],
    "web.assets_tests": [
      "account/static/tests/tours/**/*"
    ],
    "web.report_assets_common": [
      "account/static/src/css/report_invoice.css"
    ],
    "web.report_assets_pdf": [
      "account/static/src/css/report_invoice.css"
    ]
  }
}
```

### Representative source files

- `addons/account/README.md` (68 lines)
- `addons/account/__init__.py` (33 lines)
- `addons/account/__manifest__.py` (151 lines)
- `addons/account/controllers/__init__.py` (8 lines)
- `addons/account/controllers/download_docs.py` (111 lines)
- `addons/account/controllers/portal.py` (292 lines)
- `addons/account/controllers/terms.py` (29 lines)
- `addons/account/controllers/tests_shared_js_python.py` (16 lines)
- `addons/account/controllers/webmanifest.py` (9 lines)
- `addons/account/data/account_data.xml` (316 lines)
- `addons/account/data/account_incoterms_data.xml` (50 lines)
- `addons/account/data/account_reports_data.xml` (64 lines)
- `addons/account/data/account_tour.xml` (7 lines)
- `addons/account/data/digest_data.xml` (23 lines)
- `addons/account/data/ir_config_parameter_data.xml` (13 lines)
- `addons/account/data/ir_sequence.xml` (12 lines)
- `addons/account/data/mail_template_data.xml` (522 lines)
- `addons/account/data/onboarding_data.xml` (88 lines)
- `addons/account/data/portal_entry_data.xml` (22 lines)
- `addons/account/data/res_country_group.xml` (35 lines)
- `addons/account/data/service_cron.xml` (33 lines)
- `addons/account/data/template/account.account-generic_coa.csv` (46 lines)
- `addons/account/data/template/account.fiscal.position-generic_coa.csv` (3 lines)
- `addons/account/data/template/account.tax-generic_coa.csv` (17 lines)
- `addons/account/data/template/account.tax.group-generic_coa.csv` (3 lines)
- `addons/account/demo/__init__.py` (3 lines)
- `addons/account/demo/account_demo.py` (585 lines)
- `addons/account/demo/account_demo.xml` (84 lines)
- `addons/account/demo/res_partner_bank_demo.xml` (30 lines)
- `addons/account/doc/account_anglo_saxon.ods` (229 lines)
- `addons/account/doc/account_anglo_saxon.pdf` (537 lines)
- `addons/account/i18n/account.pot` (21,767 lines)
- `addons/account/i18n/af.po` (23,392 lines)
- `addons/account/i18n/am.po` (23,388 lines)
- `addons/account/i18n/ar.po` (24,807 lines)
- `addons/account/i18n/az.po` (22,378 lines)
- `addons/account/i18n/bg.po` (22,628 lines)
- `addons/account/i18n/bs.po` (26,422 lines)
- `addons/account/i18n/ca.po` (23,286 lines)
- `addons/account/i18n/cs.po` (24,612 lines)
- `addons/account/i18n/da.po` (24,667 lines)
- `addons/account/i18n/de.po` (25,487 lines)
- `addons/account/i18n/el.po` (22,443 lines)
- `addons/account/i18n/en_AU.po` (25 lines)
- `addons/account/i18n/en_NZ.po` (78 lines)
- `addons/account/i18n/es.po` (28,271 lines)
- `addons/account/i18n/es_419.po` (26,642 lines)
- `addons/account/i18n/es_CL.po` (882 lines)
- `addons/account/i18n/et.po` (22,814 lines)
- `addons/account/i18n/eu.po` (23,391 lines)
- `addons/account/i18n/fa.po` (22,954 lines)
- `addons/account/i18n/fi.po` (25,434 lines)
- `addons/account/i18n/fo.po` (23,391 lines)
- `addons/account/i18n/fr.po` (25,387 lines)
- `addons/account/i18n/fr_BE.po` (150 lines)
- `addons/account/i18n/fr_CA.po` (619 lines)
- `addons/account/i18n/gl.po` (23,391 lines)
- `addons/account/i18n/gu.po` (23,877 lines)
- `addons/account/i18n/he.po` (22,687 lines)
- `addons/account/i18n/hi.po` (23,015 lines)
- `addons/account/i18n/hr.po` (24,605 lines)
- `addons/account/i18n/hu.po` (23,095 lines)
- `addons/account/i18n/id.po` (25,314 lines)
- `addons/account/i18n/is.po` (23,448 lines)
- `addons/account/i18n/it.po` (25,364 lines)
- `addons/account/i18n/ja.po` (25,184 lines)
- `addons/account/i18n/ka.po` (23,391 lines)
- `addons/account/i18n/kab.po` (22,221 lines)
- `addons/account/i18n/km.po` (23,402 lines)
- `addons/account/i18n/ko.po` (23,898 lines)
- `addons/account/i18n/ku.po` (22,390 lines)
- `addons/account/i18n/lb.po` (23,393 lines)
- `addons/account/i18n/lo.po` (24,330 lines)
- `addons/account/i18n/lt.po` (22,499 lines)
- `addons/account/i18n/lv.po` (23,256 lines)
- `addons/account/i18n/mk.po` (23,391 lines)
- `addons/account/i18n/mn.po` (24,845 lines)
- `addons/account/i18n/my.po` (22,132 lines)
- `addons/account/i18n/nb.po` (22,842 lines)
- `addons/account/i18n/nl.po` (25,238 lines)
- `addons/account/i18n/pl.po` (24,430 lines)
- `addons/account/i18n/pt.po` (24,309 lines)
- `addons/account/i18n/pt_BR.po` (26,093 lines)
- `addons/account/i18n/ro.po` (24,672 lines)
- `addons/account/i18n/ru.po` (24,476 lines)
- `addons/account/i18n/sk.po` (25,753 lines)
- `addons/account/i18n/sl.po` (23,105 lines)
- `addons/account/i18n/sq.po` (23,395 lines)
- `addons/account/i18n/sr@latin.po` (22,196 lines)
- `addons/account/i18n/sv.po` (25,203 lines)
- `addons/account/i18n/th.po` (24,150 lines)
- `addons/account/i18n/tr.po` (25,101 lines)
- `addons/account/i18n/uk.po` (23,702 lines)
- `addons/account/i18n/uz.po` (26,594 lines)
- `addons/account/i18n/vi.po` (24,358 lines)
- `addons/account/i18n/zh_CN.po` (24,338 lines)
- `addons/account/i18n/zh_TW.po` (23,648 lines)
- `addons/account/migrations/1.5/pre-migrate.py` (8 lines)
- `addons/account/migrations/1.6/pre-migrate.py` (8 lines)
- `addons/account/models/__init__.py` (56 lines)
- `addons/account/models/account_account.py` (1,551 lines)
- `addons/account/models/account_account_tag.py` (139 lines)
- `addons/account/models/account_analytic_account.py` (78 lines)
- `addons/account/models/account_analytic_distribution_model.py` (70 lines)
- `addons/account/models/account_analytic_line.py` (185 lines)
- `addons/account/models/account_analytic_plan.py` (80 lines)
- `addons/account/models/account_bank_statement.py` (488 lines)
- `addons/account/models/account_bank_statement_line.py` (877 lines)
- `addons/account/models/account_cash_rounding.py` (129 lines)
- `addons/account/models/account_code_mapping.py` (90 lines)
- `addons/account/models/account_document_import_mixin.py` (567 lines)
- `addons/account/models/account_full_reconcile.py` (62 lines)
- `addons/account/models/account_incoterms.py` (25 lines)
- `addons/account/models/account_journal.py` (1,424 lines)
- `addons/account/models/account_journal_dashboard.py` (1,401 lines)
- `addons/account/models/account_lock_exception.py` (280 lines)
- `addons/account/models/account_move.py` (8,413 lines)
- `addons/account/models/account_move_line.py` (4,158 lines)
- `addons/account/models/account_move_line_tax_details.py` (231 lines)
- `addons/account/models/account_move_send.py` (924 lines)
- `addons/account/models/account_partial_reconcile.py` (744 lines)
- `addons/account/models/account_payment.py` (1,330 lines)
- `addons/account/models/account_payment_method.py` (166 lines)
- `addons/account/models/account_payment_term.py` (360 lines)
- `addons/account/models/account_reconcile_model.py` (229 lines)
- `addons/account/models/account_report.py` (1,080 lines)
- `addons/account/models/account_root.py` (40 lines)
- `addons/account/models/account_tax.py` (5,268 lines)
- `addons/account/models/chart_template.py` (1,598 lines)
- `addons/account/models/company.py` (1,635 lines)
- `addons/account/models/decimal_precision.py` (15 lines)
- `addons/account/models/digest.py` (38 lines)
- `addons/account/models/ir_actions_report.py` (99 lines)
- `addons/account/models/ir_attachment.py` (89 lines)
- `addons/account/models/ir_http.py` (11 lines)
- `addons/account/models/ir_module.py` (140 lines)
- `addons/account/models/kpi_provider.py` (81 lines)
- `addons/account/models/mail_message.py` (161 lines)
- `addons/account/models/mail_template.py` (16 lines)
- `addons/account/models/merge_partner_automatic.py` (9 lines)
- `addons/account/models/onboarding_onboarding.py` (29 lines)
- `addons/account/models/onboarding_onboarding_step.py` (119 lines)
- `addons/account/models/partner.py` (1,258 lines)
- `addons/account/models/product.py` (715 lines)
- `addons/account/models/product_catalog_line_mixin.py` (46 lines)
- `addons/account/models/product_catalog_mixin.py` (303 lines)
- `addons/account/models/res_config_settings.py` (337 lines)
- `addons/account/models/res_country_group.py` (12 lines)
- `addons/account/models/res_currency.py` (185 lines)
- `addons/account/models/res_currency_rate_consolidation_mixin.py` (59 lines)
- `addons/account/models/res_groups.py` (14 lines)
- `addons/account/models/res_partner_bank.py` (415 lines)
- `addons/account/models/res_users.py` (21 lines)
- `addons/account/models/sequence_mixin.py` (513 lines)
- `addons/account/models/template_generic_coa.py` (67 lines)
- `addons/account/models/uom_uom.py` (56 lines)
- `addons/account/populate/benchmarks.xml` (189 lines)
- `addons/account/populate/populate_demo.xml` (237 lines)
- `addons/account/report/__init__.py` (6 lines)
- `addons/account/report/account_hash_integrity_templates.py` (22 lines)

Additional files not expanded here: 393. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
