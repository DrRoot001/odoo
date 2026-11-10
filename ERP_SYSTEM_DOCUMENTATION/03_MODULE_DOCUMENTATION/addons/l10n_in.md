# Module: l10n_in

- **Module ID:** MOD-227
- **Path:** `addons/l10n_in`
- **Manifest:** `addons/l10n_in/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Indian Accounting: Chart of Account.
====================================

Indian accounting chart and localization.

Odoo allows to manage Indian Accounting by providing Two Formats Of Chart of Accounts i.e Indian Chart Of Accounts - Standard and Indian Chart Of Accounts - Schedule VI.

Note: The Schedule VI has been revised by MCA and is applicable for all Balance Sheet made after
31st March, 2011. The Format has done away with earlier two options of format of Balance
Sheet, now only Vertical format has been permitted Which is Supported By Odoo.
  

Declared dependencies: `account_tax_python`, `account_debit_note`, `account`, `l10n_account_withholding_tax`, `iap`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 19 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 31 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_tax_python",
    "account_debit_note",
    "account",
    "l10n_account_withholding_tax",
    "iap"
  ],
  "data": [
    "security/l10n_in_security.xml",
    "data/iap_service_data.xml",
    "data/account.account.tag.csv",
    "data/l10n_in_chart_data.xml",
    "data/l10n_in.port.code.csv",
    "data/res_country_state_data.xml",
    "data/res_country_group.xml",
    "data/uom_data.xml",
    "data/res_partner_industry.xml",
    "data/account_tax_report_tcs_data.xml",
    "data/account_tax_report_tds_data.xml",
    "data/account_tax_report_tcs_it_act_25_data.xml",
    "data/account_tax_report_tds_it_act_25_data.xml",
    "data/account_report_data.xml",
    "views/l10n_in_pan_entity_views.xml",
    "views/account_invoice_views.xml",
    "views/account_move_line_views.xml",
    "views/account_journal_views.xml",
    "views/res_config_settings_views.xml",
    "views/product_template_view.xml",
    "views/port_code_views.xml",
    "views/res_company_views.xml",
    "views/report_invoice.xml",
    "views/res_country_state_view.xml",
    "views/res_partner_views.xml",
    "views/account_tax_views.xml",
    "views/uom_uom_views.xml",
    "views/base_document_layout_views.xml",
    "wizard/account_paymnet_register_views.xml",
    "wizard/account_move_reversal.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/product_demo.xml",
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_in/static/src/components/**/*",
      "l10n_in/static/src/helpers/*.js"
    ],
    "web.assets_frontend": [
      "l10n_in/static/src/components/tests_shared_js_python/*",
      "l10n_in/static/src/helpers/*.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_in/__init__.py` (14 lines)
- `addons/l10n_in/__manifest__.py` (80 lines)
- `addons/l10n_in/data/account.account.tag.csv` (47 lines)
- `addons/l10n_in/data/account_report_data.xml` (25 lines)
- `addons/l10n_in/data/account_tax_report_tcs_data.xml` (159 lines)
- `addons/l10n_in/data/account_tax_report_tcs_it_act_25_data.xml` (128 lines)
- `addons/l10n_in/data/account_tax_report_tds_data.xml` (328 lines)
- `addons/l10n_in/data/account_tax_report_tds_it_act_25_data.xml` (579 lines)
- `addons/l10n_in/data/iap_service_data.xml` (12 lines)
- `addons/l10n_in/data/l10n_in.port.code.csv` (635 lines)
- `addons/l10n_in/data/l10n_in_chart_data.xml` (25 lines)
- `addons/l10n_in/data/neutralize.sql` (3 lines)
- `addons/l10n_in/data/res_country_group.xml` (11 lines)
- `addons/l10n_in/data/res_country_state_data.xml` (128 lines)
- `addons/l10n_in/data/res_partner_industry.xml` (11 lines)
- `addons/l10n_in/data/template/account.account-in.csv` (114 lines)
- `addons/l10n_in/data/template/account.account-in_sch3.csv` (286 lines)
- `addons/l10n_in/data/template/account.fiscal.position-in.csv` (3 lines)
- `addons/l10n_in/data/template/account.tax-in.csv` (1,137 lines)
- `addons/l10n_in/data/template/account.tax.group-in.csv` (11 lines)
- `addons/l10n_in/data/uom_data.xml` (87 lines)
- `addons/l10n_in/demo/__init__.py` (3 lines)
- `addons/l10n_in/demo/account_demo.py` (728 lines)
- `addons/l10n_in/demo/demo_company.xml` (38 lines)
- `addons/l10n_in/demo/product_demo.xml` (97 lines)
- `addons/l10n_in/i18n/hi.po` (3,137 lines)
- `addons/l10n_in/i18n/l10n_in.pot` (3,099 lines)
- `addons/l10n_in/migrations/2.1/end-migrate.py` (35 lines)
- `addons/l10n_in/migrations/9.0.2.0/pre-set_tags_and_taxes_updatable.py` (8 lines)
- `addons/l10n_in/migrations/saas~19.5.2.2/pre-10-migrate.py` (103 lines)
- `addons/l10n_in/models/__init__.py` (20 lines)
- `addons/l10n_in/models/account_account.py` (14 lines)
- `addons/l10n_in/models/account_invoice.py` (640 lines)
- `addons/l10n_in/models/account_journal.py` (26 lines)
- `addons/l10n_in/models/account_move_line.py` (317 lines)
- `addons/l10n_in/models/account_payment.py` (12 lines)
- `addons/l10n_in/models/account_tax.py` (141 lines)
- `addons/l10n_in/models/company.py` (246 lines)
- `addons/l10n_in/models/iap_account.py` (30 lines)
- `addons/l10n_in/models/l10n_in_pan_entity.py` (89 lines)
- `addons/l10n_in/models/l10n_in_report_handler.py` (17 lines)
- `addons/l10n_in/models/port_code.py` (17 lines)
- `addons/l10n_in/models/product_template.py` (41 lines)
- `addons/l10n_in/models/res_config_settings.py` (194 lines)
- `addons/l10n_in/models/res_country_state.py` (7 lines)
- `addons/l10n_in/models/res_groups.py` (13 lines)
- `addons/l10n_in/models/res_partner.py` (269 lines)
- `addons/l10n_in/models/template_in.py` (203 lines)
- `addons/l10n_in/models/uom_uom.py` (8 lines)
- `addons/l10n_in/security/ir.access.csv` (4 lines)
- `addons/l10n_in/security/l10n_in_security.xml` (6 lines)
- `addons/l10n_in/static/src/components/hsn_autocomplete/hsn_autocomplete.js` (116 lines)
- `addons/l10n_in/static/src/components/hsn_autocomplete/hsn_autocomplete.xml` (18 lines)
- `addons/l10n_in/static/src/components/tests_shared_js_python/tests_shared_js_python.js` (14 lines)
- `addons/l10n_in/static/src/helpers/hsn_summary.js` (99 lines)
- `addons/l10n_in/static/src/img/Google_Pay-Logo.svg` (1 lines)
- `addons/l10n_in/static/src/img/Paytm-Logo.svg` (1 lines)
- `addons/l10n_in/static/src/img/PhonePe-Logo.svg` (1 lines)
- `addons/l10n_in/static/src/img/Upi-logo.svg` (1 lines)
- `addons/l10n_in/tests/__init__.py` (8 lines)
- `addons/l10n_in/tests/common.py` (278 lines)
- `addons/l10n_in/tests/test_check_status.py` (88 lines)
- `addons/l10n_in/tests/test_gstr_section.py` (126 lines)
- `addons/l10n_in/tests/test_hsn_summary.py` (770 lines)
- `addons/l10n_in/tests/test_invoice_label.py` (74 lines)
- `addons/l10n_in/tests/test_l10n_in_company.py` (115 lines)
- `addons/l10n_in/tests/test_l10n_in_fiscal_position.py` (244 lines)
- `addons/l10n_in/tests/test_partner_details_on_invoice.py` (137 lines)
- `addons/l10n_in/views/account_invoice_views.xml` (85 lines)
- `addons/l10n_in/views/account_journal_views.xml` (23 lines)
- `addons/l10n_in/views/account_move_line_views.xml` (37 lines)
- `addons/l10n_in/views/account_tax_views.xml` (17 lines)
- `addons/l10n_in/views/base_document_layout_views.xml` (17 lines)
- `addons/l10n_in/views/l10n_in_pan_entity_views.xml` (59 lines)
- `addons/l10n_in/views/port_code_views.xml` (48 lines)
- `addons/l10n_in/views/product_template_view.xml` (20 lines)
- `addons/l10n_in/views/report_invoice.xml` (233 lines)
- `addons/l10n_in/views/res_company_views.xml` (33 lines)
- `addons/l10n_in/views/res_config_settings_views.xml` (190 lines)
- `addons/l10n_in/views/res_country_state_view.xml` (26 lines)
- `addons/l10n_in/views/res_partner_views.xml` (86 lines)
- `addons/l10n_in/views/uom_uom_views.xml` (13 lines)
- `addons/l10n_in/wizard/__init__.py` (2 lines)
- `addons/l10n_in/wizard/account_move_reversal.py` (30 lines)
- `addons/l10n_in/wizard/account_move_reversal.xml` (15 lines)
- `addons/l10n_in/wizard/account_payment_register.py` (31 lines)
- `addons/l10n_in/wizard/account_paymnet_register_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
