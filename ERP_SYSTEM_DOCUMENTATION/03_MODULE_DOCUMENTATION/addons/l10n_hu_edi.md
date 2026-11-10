# Module: l10n_hu_edi

- **Module ID:** MOD-220
- **Path:** `addons/l10n_hu_edi`
- **Manifest:** `addons/l10n_hu_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_hu']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


* Electronically report invoices to the NAV (Hungarian Tax Agency) when issuing physical (paper) invoices.
* Electronically receive vendor bills from the NAV.
* Perform the Tax Audit Export (Adóhatósági Ellenőrzési Adatszolgáltatás) in NAV 3.0 format.
* NAV Documentation: https://onlineszamla.nav.gov.hu/files/container/download/2025.10.09.%20EN_Online%20Invoice%20System%203.0%20Interface%20Specification%20.pdf
    

Declared dependencies: `account_debit_note`, `l10n_hu`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 57 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_debit_note",
    "l10n_hu"
  ],
  "data": [
    "data/uom.uom.csv",
    "data/template_requests.xml",
    "data/template_invoice.xml",
    "data/ir_cron.xml",
    "views/report_templates.xml",
    "views/report_invoice.xml",
    "views/account_move_views.xml",
    "views/product_template_views.xml",
    "views/account_tax_views.xml",
    "views/uom_uom_views.xml",
    "views/res_partner_views.xml",
    "views/res_company_views.xml",
    "views/res_config_settings_views.xml",
    "wizard/l10n_hu_edi_cancellation.xml",
    "wizard/l10n_hu_edi_receive_bills_wizard_views.xml",
    "wizard/l10n_hu_edi_tax_audit_export.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_partner.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_hu_edi/static/src/views/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_hu_edi/__init__.py` (4 lines)
- `addons/l10n_hu_edi/__manifest__.py` (44 lines)
- `addons/l10n_hu_edi/data/ir_cron.xml` (16 lines)
- `addons/l10n_hu_edi/data/neutralize.sql` (8 lines)
- `addons/l10n_hu_edi/data/template/account.tax-hu.csv` (40 lines)
- `addons/l10n_hu_edi/data/template_invoice.xml` (206 lines)
- `addons/l10n_hu_edi/data/template_requests.xml` (125 lines)
- `addons/l10n_hu_edi/data/uom.uom.csv` (10 lines)
- `addons/l10n_hu_edi/demo/demo_partner.xml` (65 lines)
- `addons/l10n_hu_edi/i18n/hu.po` (1,612 lines)
- `addons/l10n_hu_edi/i18n/l10n_hu_edi.pot` (1,505 lines)
- `addons/l10n_hu_edi/models/__init__.py` (12 lines)
- `addons/l10n_hu_edi/models/account_move.py` (1,469 lines)
- `addons/l10n_hu_edi/models/account_move_send.py` (107 lines)
- `addons/l10n_hu_edi/models/account_tax.py` (66 lines)
- `addons/l10n_hu_edi/models/l10n_hu_edi_connection.py` (475 lines)
- `addons/l10n_hu_edi/models/product.py` (27 lines)
- `addons/l10n_hu_edi/models/res_company.py` (270 lines)
- `addons/l10n_hu_edi/models/res_config_settings.py` (49 lines)
- `addons/l10n_hu_edi/models/res_partner.py` (50 lines)
- `addons/l10n_hu_edi/models/template_hu.py` (28 lines)
- `addons/l10n_hu_edi/models/uom_uom.py` (29 lines)
- `addons/l10n_hu_edi/security/ir.access.csv` (4 lines)
- `addons/l10n_hu_edi/static/img/gipsz_jakab.jpg` (170 lines)
- `addons/l10n_hu_edi/static/img/hun_flag.jpg` (21 lines)
- `addons/l10n_hu_edi/static/img/logo-mol-colorful.88751645.svg` (8 lines)
- `addons/l10n_hu_edi/static/img/magyaros_karoly.jpg` (874 lines)
- `addons/l10n_hu_edi/static/img/tvk.png` (302 lines)
- `addons/l10n_hu_edi/static/src/views/sync_with_nav_btn/sync_with_nav_btn.js` (46 lines)
- `addons/l10n_hu_edi/static/src/views/sync_with_nav_btn/sync_with_nav_btn.xml` (15 lines)
- `addons/l10n_hu_edi/tests/__init__.py` (11 lines)
- `addons/l10n_hu_edi/tests/common.py` (470 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/batch_modifications.xml` (330 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/credit_note.xml` (128 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/credit_note_original_bill.xml` (421 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/credit_note_receive.xml` (133 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/debit_note.xml` (204 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/debit_note_original_bill.xml` (294 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_advance.xml` (118 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_complex_eur.xml` (234 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_complex_huf.xml` (272 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_final.xml` (150 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_simple.xml` (119 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_simple_discount.xml` (123 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/invoice_tax_price_include.xml` (146 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/normal_invoice.xml` (193 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/query_invoice_data_response.xml` (38 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/query_invoice_data_response_gzip.xml` (35 lines)
- `addons/l10n_hu_edi/tests/invoice_xmls/simplified_invoice.xml` (150 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/BATCH_MOD_2026_0002_1.xml` (35 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/BATCH_MOD_2026_0002_2.xml` (35 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/INV_2026_00003.xml` (34 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/INV_2026_00004.xml` (34 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/manageAnnulment_request.xml` (33 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/manageAnnulment_response.xml` (26 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/manageInvoice_request.xml` (35 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/manageInvoice_response.xml` (26 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryInvoiceData_batch_request.xml` (31 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryInvoiceData_request.xml` (30 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryInvoiceDigest_request.xml` (35 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryInvoiceDigest_response.xml` (116 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionList_request.xml` (31 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionList_response.xml` (39 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_request.xml` (28 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response.xml` (33 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response_annulment_done.xml` (45 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response_annulment_pending.xml` (45 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response_error.xml` (62 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response_original.xml` (35 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/queryTransactionStatus_response_warning.xml` (54 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/tokenExchange_request.xml` (26 lines)
- `addons/l10n_hu_edi/tests/mocked_requests/tokenExchange_response.xml` (28 lines)
- `addons/l10n_hu_edi/tests/test_account_move_sync_tax_lines.py` (99 lines)
- `addons/l10n_hu_edi/tests/test_bill_xml_upload.py` (316 lines)
- `addons/l10n_hu_edi/tests/test_credit_debit_notes.py` (45 lines)
- `addons/l10n_hu_edi/tests/test_flows_live.py` (173 lines)
- `addons/l10n_hu_edi/tests/test_flows_mocked.py` (449 lines)
- `addons/l10n_hu_edi/tests/test_invoice_report.py` (39 lines)
- `addons/l10n_hu_edi/tests/test_invoice_xml.py` (257 lines)
- `addons/l10n_hu_edi/tests/test_res_partner.py` (37 lines)
- `addons/l10n_hu_edi/views/account_move_views.xml` (78 lines)
- `addons/l10n_hu_edi/views/account_tax_views.xml` (16 lines)
- `addons/l10n_hu_edi/views/product_template_views.xml` (22 lines)
- `addons/l10n_hu_edi/views/report_invoice.xml` (135 lines)
- `addons/l10n_hu_edi/views/report_templates.xml` (118 lines)
- `addons/l10n_hu_edi/views/res_company_views.xml` (16 lines)
- `addons/l10n_hu_edi/views/res_config_settings_views.xml` (53 lines)
- `addons/l10n_hu_edi/views/res_partner_views.xml` (19 lines)
- `addons/l10n_hu_edi/views/uom_uom_views.xml` (15 lines)
- `addons/l10n_hu_edi/wizard/__init__.py` (5 lines)
- `addons/l10n_hu_edi/wizard/account_move_debit.py` (13 lines)
- `addons/l10n_hu_edi/wizard/account_move_reversal.py` (28 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_cancellation.py` (48 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_cancellation.xml` (25 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_receive_bills_wizard.py` (44 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_receive_bills_wizard_views.xml` (22 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_tax_audit_export.py` (119 lines)
- `addons/l10n_hu_edi/wizard/l10n_hu_edi_tax_audit_export.xml` (47 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
