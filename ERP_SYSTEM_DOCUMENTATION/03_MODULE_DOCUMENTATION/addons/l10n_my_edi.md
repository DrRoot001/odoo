# Module: l10n_my_edi

- **Module ID:** MOD-279
- **Path:** `addons/l10n_my_edi`
- **Manifest:** `addons/l10n_my_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_my']`
- **License:** `LGPL-3`

## Purpose and dependencies

E-invoicing using MyInvois


    This modules allows the user to send their invoices to the MyInvois system.
    

Declared dependencies: `l10n_my`, `l10n_my_ubl_pint`, `account_edi_proxy_client`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 27 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 27 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_my",
    "l10n_my_ubl_pint",
    "account_edi_proxy_client"
  ],
  "data": [
    "data/ir_cron.xml",
    "data/l10n_my_edi.industry_classification.csv",
    "data/res_partner.xml",
    "views/account_journal_dashboard_view.xml",
    "views/account_move_view.xml",
    "views/account_tax_view.xml",
    "views/l10n_my_edi_industrial_classification_views.xml",
    "views/myinvois_document_views.xml",
    "views/product_template_view.xml",
    "views/report_invoice.xml",
    "views/res_company_view.xml",
    "views/res_config_settings_view.xml",
    "views/res_partner_view.xml",
    "views/account_portal_templates.xml",
    "wizard/myinvois_consolidate_invoice_wizard.xml",
    "wizard/myinvois_document_status_update_wizard.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_my_edi/__init__.py` (4 lines)
- `addons/l10n_my_edi/__manifest__.py` (37 lines)
- `addons/l10n_my_edi/controllers/__init__.py` (2 lines)
- `addons/l10n_my_edi/controllers/portal.py` (16 lines)
- `addons/l10n_my_edi/data/ir_cron.xml` (14 lines)
- `addons/l10n_my_edi/data/l10n_my_edi.industry_classification.csv` (1,175 lines)
- `addons/l10n_my_edi/data/neutralize.sql` (6 lines)
- `addons/l10n_my_edi/data/res_partner.xml` (18 lines)
- `addons/l10n_my_edi/i18n/l10n_my_edi.pot` (1,915 lines)
- `addons/l10n_my_edi/i18n/ms.po` (1,941 lines)
- `addons/l10n_my_edi/models/__init__.py` (14 lines)
- `addons/l10n_my_edi/models/account_edi_proxy_user.py` (82 lines)
- `addons/l10n_my_edi/models/account_edi_xml_ubl_my.py` (835 lines)
- `addons/l10n_my_edi/models/account_journal_dashboard.py` (24 lines)
- `addons/l10n_my_edi/models/account_move.py` (276 lines)
- `addons/l10n_my_edi/models/account_move_line.py` (37 lines)
- `addons/l10n_my_edi/models/account_move_send.py` (19 lines)
- `addons/l10n_my_edi/models/account_tax.py` (50 lines)
- `addons/l10n_my_edi/models/l10n_my_edi_industry_classification.py` (30 lines)
- `addons/l10n_my_edi/models/myinvois_document.py` (1,465 lines)
- `addons/l10n_my_edi/models/product_template.py` (94 lines)
- `addons/l10n_my_edi/models/res_company.py` (107 lines)
- `addons/l10n_my_edi/models/res_config_settings.py` (86 lines)
- `addons/l10n_my_edi/models/res_partner.py` (146 lines)
- `addons/l10n_my_edi/security/ir.access.csv` (9 lines)
- `addons/l10n_my_edi/tests/__init__.py` (6 lines)
- `addons/l10n_my_edi/tests/expected_xmls/bill_import.xml` (174 lines)
- `addons/l10n_my_edi/tests/expected_xmls/credit_note.xml` (173 lines)
- `addons/l10n_my_edi/tests/expected_xmls/credit_note_company_currency.xml` (167 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice.xml` (165 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_foreigner.xml` (164 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_import.xml` (165 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_multicurrency.xml` (170 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_optional_fields.xml` (189 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_self_billing.xml` (164 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_tax_exempt.xml` (170 lines)
- `addons/l10n_my_edi/tests/expected_xmls/invoice_with_so.xml` (165 lines)
- `addons/l10n_my_edi/tests/expected_xmls/refund_note_company_currency.xml` (167 lines)
- `addons/l10n_my_edi/tests/test_branch.py` (62 lines)
- `addons/l10n_my_edi/tests/test_consolidated_invoices.py` (707 lines)
- `addons/l10n_my_edi/tests/test_file_generation.py` (1,050 lines)
- `addons/l10n_my_edi/tests/test_file_generation_common.py` (94 lines)
- `addons/l10n_my_edi/tests/test_submissions.py` (1,122 lines)
- `addons/l10n_my_edi/views/account_journal_dashboard_view.xml` (15 lines)
- `addons/l10n_my_edi/views/account_move_view.xml` (86 lines)
- `addons/l10n_my_edi/views/account_portal_templates.xml` (41 lines)
- `addons/l10n_my_edi/views/account_tax_view.xml` (14 lines)
- `addons/l10n_my_edi/views/l10n_my_edi_industrial_classification_views.xml` (16 lines)
- `addons/l10n_my_edi/views/myinvois_document_views.xml` (111 lines)
- `addons/l10n_my_edi/views/product_template_view.xml` (15 lines)
- `addons/l10n_my_edi/views/report_invoice.xml` (32 lines)
- `addons/l10n_my_edi/views/res_company_view.xml` (25 lines)
- `addons/l10n_my_edi/views/res_config_settings_view.xml` (76 lines)
- `addons/l10n_my_edi/views/res_partner_view.xml` (30 lines)
- `addons/l10n_my_edi/wizard/__init__.py` (3 lines)
- `addons/l10n_my_edi/wizard/myinvois_consolidate_invoice_wizard.py` (131 lines)
- `addons/l10n_my_edi/wizard/myinvois_consolidate_invoice_wizard.xml` (23 lines)
- `addons/l10n_my_edi/wizard/myinvois_document_status_update_wizard.py` (31 lines)
- `addons/l10n_my_edi/wizard/myinvois_document_status_update_wizard.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
