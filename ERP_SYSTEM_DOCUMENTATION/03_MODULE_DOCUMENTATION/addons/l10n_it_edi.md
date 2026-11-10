# Module: l10n_it_edi

- **Module ID:** MOD-241
- **Path:** `addons/l10n_it_edi`
- **Manifest:** `addons/l10n_it_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_it']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


E-invoice implementation
    

Declared dependencies: `l10n_it`, `account_edi_proxy_client`, `account_debit_note`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 68 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 14 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_it",
    "account_edi_proxy_client",
    "account_debit_note"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/invoice_it_simplified_template.xml",
    "data/invoice_it_template.xml",
    "data/ir_cron.xml",
    "data/l10n_it.document.type.csv",
    "views/account_payment_method.xml",
    "views/account_tax_view.xml",
    "views/l10n_it_document_type.xml",
    "views/l10n_it_view.xml",
    "views/portal_address_templates.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/account_invoice_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_it_edi/static/src/interactions/**/*"
    ],
    "web.assets_tests": [
      "l10n_it_edi/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_it_edi/__init__.py` (28 lines)
- `addons/l10n_it_edi/__manifest__.py` (45 lines)
- `addons/l10n_it_edi/controllers/__init__.py` (3 lines)
- `addons/l10n_it_edi/controllers/portal.py` (32 lines)
- `addons/l10n_it_edi/data/account.account.tag.csv` (2 lines)
- `addons/l10n_it_edi/data/account_invoice_demo.xml` (77 lines)
- `addons/l10n_it_edi/data/invoice_it_simplified_template.xml` (118 lines)
- `addons/l10n_it_edi/data/invoice_it_template.xml` (266 lines)
- `addons/l10n_it_edi/data/ir_cron.xml` (11 lines)
- `addons/l10n_it_edi/data/l10n_it.document.type.csv` (23 lines)
- `addons/l10n_it_edi/data/neutralize.sql` (3 lines)
- `addons/l10n_it_edi/data/pkey.key` (52 lines)
- `addons/l10n_it_edi/data/template/account.tax-it.csv` (15 lines)
- `addons/l10n_it_edi/demo/__init__.py` (1 lines)
- `addons/l10n_it_edi/demo/account_demo.py` (22 lines)
- `addons/l10n_it_edi/i18n/it.po` (2,473 lines)
- `addons/l10n_it_edi/i18n/l10n_it_edi.pot` (2,141 lines)
- `addons/l10n_it_edi/migrations/0.5/post-moving-account-taxes.py` (22 lines)
- `addons/l10n_it_edi/models/__init__.py` (12 lines)
- `addons/l10n_it_edi/models/account_chart_template.py` (18 lines)
- `addons/l10n_it_edi/models/account_edi_proxy_user.py` (60 lines)
- `addons/l10n_it_edi/models/account_journal.py` (42 lines)
- `addons/l10n_it_edi/models/account_move.py` (2,751 lines)
- `addons/l10n_it_edi/models/account_move_send.py` (154 lines)
- `addons/l10n_it_edi/models/account_payment_method_line.py` (53 lines)
- `addons/l10n_it_edi/models/account_tax.py` (120 lines)
- `addons/l10n_it_edi/models/ddt.py` (18 lines)
- `addons/l10n_it_edi/models/l10n_it_document_type.py` (27 lines)
- `addons/l10n_it_edi/models/res_company.py` (204 lines)
- `addons/l10n_it_edi/models/res_config_settings.py` (71 lines)
- `addons/l10n_it_edi/models/res_partner.py` (253 lines)
- `addons/l10n_it_edi/security/ir.access.csv` (3 lines)
- `addons/l10n_it_edi/static/src/interactions/address.js` (30 lines)
- `addons/l10n_it_edi/static/tests/tours/l10n_it_edi_address_codice_fiscale.js` (72 lines)
- `addons/l10n_it_edi/tests/__init__.py` (15 lines)
- `addons/l10n_it_edi/tests/common.py` (236 lines)
- `addons/l10n_it_edi/tests/export_xmls/bill_reverse_charge.xml` (99 lines)
- `addons/l10n_it_edi/tests/export_xmls/bill_reverse_charge_2.xml` (111 lines)
- `addons/l10n_it_edi/tests/export_xmls/bill_reverse_charge_san_marino.xml` (111 lines)
- `addons/l10n_it_edi/tests/export_xmls/credit_note_export_document_type.xml` (101 lines)
- `addons/l10n_it_edi/tests/export_xmls/credit_note_negative_price.xml` (100 lines)
- `addons/l10n_it_edi/tests/export_xmls/credit_note_refund_no_reconcile.xml` (101 lines)
- `addons/l10n_it_edi/tests/export_xmls/credit_note_reverse_charge.xml` (119 lines)
- `addons/l10n_it_edi/tests/export_xmls/enasarco_tax_invoice.xml` (159 lines)
- `addons/l10n_it_edi/tests/export_xmls/export_foreign_currency_global_discount.xml` (131 lines)
- `addons/l10n_it_edi/tests/export_xmls/export_foreign_currency_global_simple_discount.xml` (135 lines)
- `addons/l10n_it_edi/tests/export_xmls/export_foreign_currency_simple_discount.xml` (116 lines)
- `addons/l10n_it_edi/tests/export_xmls/inps_tax_invoice.xml` (161 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_below_400_codice_simplified.xml` (70 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_decimal_precision_product.xml` (99 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_exclude_postdated_moves.xml` (92 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_external_reverse_charge.xml` (114 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_fully_discounted.xml` (103 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_internal_reverse_charge.xml` (137 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_lowercase_fields.xml` (94 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_negative_price.xml` (107 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_non_latin_and_latin.xml` (115 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_partially_discounted.xml` (123 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_price_included_taxes.xml` (116 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_total_400_VAT_simplified.xml` (62 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_vat_not_equals_codice.xml` (99 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_with_attachment.xml` (105 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_with_multiple_product_description_fields.xml` (99 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_with_oss_tax.xml` (117 lines)
- `addons/l10n_it_edi/tests/export_xmls/invoice_with_rounding_line.xml` (116 lines)
- `addons/l10n_it_edi/tests/export_xmls/it_edi_debit_note.xml` (102 lines)
- `addons/l10n_it_edi/tests/export_xmls/pension_fund_tax_invoice.xml` (156 lines)
- `addons/l10n_it_edi/tests/export_xmls/prezzio_unitario_converted_company_currency.xml` (110 lines)
- `addons/l10n_it_edi/tests/export_xmls/split_payment.xml` (105 lines)
- `addons/l10n_it_edi/tests/export_xmls/split_payment_cn.xml` (92 lines)
- `addons/l10n_it_edi/tests/export_xmls/test_export_invoice_with_two_downpayments.xml` (127 lines)
- `addons/l10n_it_edi/tests/export_xmls/withholding_23_ret20.xml` (133 lines)
- `addons/l10n_it_edi/tests/export_xmls/withholding_23_ret50.xml` (133 lines)
- `addons/l10n_it_edi/tests/export_xmls/withholding_tax_invoice.xml` (133 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_enasa.xml` (160 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_pfun2.xml` (144 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_pfun3.xml` (149 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_pfund.xml` (159 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_ret20.xml` (129 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_ret50.xml` (129 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT00470550013_withh.xml` (129 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567888_FPR01.xml` (137 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567889_FPR03.xml` (140 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_DISC1.xml` (147 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPMAP.xml` (76 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR01.xml` (121 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR01.xml.p7m` (157 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR02.xml` (114 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR03.xml` (159 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR04.xml` (121 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567890_FPR05.xml` (75 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567891_FPR01.xml` (135 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01234567892_FPR01.xml` (64 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01654010345_10099.xml` (193 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT01654010345_10099.xml.p7m` (229 lines)
- `addons/l10n_it_edi/tests/import_xmls/IT09633951000_NpFwF.xml.p7m` (378 lines)
- `addons/l10n_it_edi/tests/test_account_move_document_type.py` (70 lines)
- `addons/l10n_it_edi/tests/test_account_move_payment_method.py` (43 lines)
- `addons/l10n_it_edi/tests/test_account_move_send.py` (464 lines)
- `addons/l10n_it_edi/tests/test_download_docs.py` (27 lines)
- `addons/l10n_it_edi/tests/test_edi_address.py` (23 lines)
- `addons/l10n_it_edi/tests/test_edi_export.py` (1,002 lines)
- `addons/l10n_it_edi/tests/test_edi_import.py` (1,163 lines)
- `addons/l10n_it_edi/tests/test_edi_pa.py` (70 lines)
- `addons/l10n_it_edi/tests/test_edi_reverse_charge.py` (406 lines)
- `addons/l10n_it_edi/tests/test_it_document_type.py` (55 lines)
- `addons/l10n_it_edi/tests/test_res_partner.py` (227 lines)
- `addons/l10n_it_edi/tests/test_withholding.py` (655 lines)
- `addons/l10n_it_edi/tools/__init__.py` (4 lines)
- `addons/l10n_it_edi/tools/remove_signature.py` (370 lines)
- `addons/l10n_it_edi/views/account_payment_method.xml` (19 lines)
- `addons/l10n_it_edi/views/account_tax_view.xml` (20 lines)
- `addons/l10n_it_edi/views/l10n_it_document_type.xml` (36 lines)
- `addons/l10n_it_edi/views/l10n_it_view.xml` (234 lines)
- `addons/l10n_it_edi/views/portal_address_templates.xml` (31 lines)
- `addons/l10n_it_edi/views/report_invoice.xml` (77 lines)
- `addons/l10n_it_edi/views/res_config_settings_views.xml` (38 lines)
- `addons/l10n_it_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_it_edi/wizard/account_payment_register.py` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
