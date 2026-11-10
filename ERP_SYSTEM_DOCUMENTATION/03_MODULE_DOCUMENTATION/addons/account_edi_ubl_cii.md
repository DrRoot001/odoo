# Module: account_edi_ubl_cii

- **Module ID:** MOD-006
- **Path:** `addons/account_edi_ubl_cii`
- **Manifest:** `addons/account_edi_ubl_cii/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Electronic invoicing module
===========================

Allows to export and import formats: E-FFF, UBL Bis 3, EHF3, NLCIUS, Factur-X (CII), XRechnung (UBL).
When generating the PDF on the invoice, the PDF will be embedded inside the xml for all UBL formats. This allows the
receiver to retrieve the PDF with only the xml file. Note that **EHF3 is fully implemented by UBL Bis 3** (`reference
<https://anskaffelser.dev/postaward/g3/spec/current/billing-3.0/norway/#_implementation>`_).

Note that E-FFF, NLCIUS and XRechnung (UBL) are only available for Belgian, Dutch and German companies,
respectively. UBL Bis 3 is only available for companies which country is present in the `EAS list
<https://docs.peppol.eu/poacc/billing/3.0/codelist/eas/>`_.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 73 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 23 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 198 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 36 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/uom_data.xml",
    "data/cii_22_templates.xml",
    "data/ir_config_parameter_data.xml",
    "views/account_tax_views.xml",
    "views/account_move_views.xml",
    "views/res_partner_views.xml",
    "views/uom_uom_views.xml",
    "report/account_edi_ubl_cii_report_templates.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "account_edi_ubl_cii/static/src/scss/**/*"
    ]
  }
}
```

### Representative source files

- `addons/account_edi_ubl_cii/__init__.py` (14 lines)
- `addons/account_edi_ubl_cii/__manifest__.py` (37 lines)
- `addons/account_edi_ubl_cii/data/cii_22_templates.xml` (430 lines)
- `addons/account_edi_ubl_cii/data/ir_config_parameter_data.xml` (9 lines)
- `addons/account_edi_ubl_cii/data/uom_data.xml` (93 lines)
- `addons/account_edi_ubl_cii/i18n/account_edi_ubl_cii.pot` (2,185 lines)
- `addons/account_edi_ubl_cii/i18n/ar.po` (2,493 lines)
- `addons/account_edi_ubl_cii/i18n/az.po` (2,199 lines)
- `addons/account_edi_ubl_cii/i18n/bg.po` (2,205 lines)
- `addons/account_edi_ubl_cii/i18n/bs.po` (2,208 lines)
- `addons/account_edi_ubl_cii/i18n/ca.po` (2,394 lines)
- `addons/account_edi_ubl_cii/i18n/cs.po` (2,307 lines)
- `addons/account_edi_ubl_cii/i18n/da.po` (2,410 lines)
- `addons/account_edi_ubl_cii/i18n/de.po` (2,547 lines)
- `addons/account_edi_ubl_cii/i18n/el.po` (2,200 lines)
- `addons/account_edi_ubl_cii/i18n/es.po` (2,477 lines)
- `addons/account_edi_ubl_cii/i18n/es_419.po` (2,565 lines)
- `addons/account_edi_ubl_cii/i18n/et.po` (2,219 lines)
- `addons/account_edi_ubl_cii/i18n/fa.po` (2,248 lines)
- `addons/account_edi_ubl_cii/i18n/fi.po` (2,508 lines)
- `addons/account_edi_ubl_cii/i18n/fr.po` (2,543 lines)
- `addons/account_edi_ubl_cii/i18n/fr_BE.po` (29 lines)
- `addons/account_edi_ubl_cii/i18n/he.po` (2,200 lines)
- `addons/account_edi_ubl_cii/i18n/hi.po` (2,372 lines)
- `addons/account_edi_ubl_cii/i18n/hr.po` (2,642 lines)
- `addons/account_edi_ubl_cii/i18n/hu.po` (2,201 lines)
- `addons/account_edi_ubl_cii/i18n/id.po` (2,445 lines)
- `addons/account_edi_ubl_cii/i18n/it.po` (2,538 lines)
- `addons/account_edi_ubl_cii/i18n/ja.po` (2,351 lines)
- `addons/account_edi_ubl_cii/i18n/kab.po` (2,207 lines)
- `addons/account_edi_ubl_cii/i18n/ko.po` (2,390 lines)
- `addons/account_edi_ubl_cii/i18n/ku.po` (2,205 lines)
- `addons/account_edi_ubl_cii/i18n/lo.po` (2,333 lines)
- `addons/account_edi_ubl_cii/i18n/lt.po` (2,203 lines)
- `addons/account_edi_ubl_cii/i18n/lv.po` (2,218 lines)
- `addons/account_edi_ubl_cii/i18n/mn.po` (2,200 lines)
- `addons/account_edi_ubl_cii/i18n/my.po` (2,201 lines)
- `addons/account_edi_ubl_cii/i18n/nb.po` (2,201 lines)
- `addons/account_edi_ubl_cii/i18n/nl.po` (2,538 lines)
- `addons/account_edi_ubl_cii/i18n/pl.po` (2,501 lines)
- `addons/account_edi_ubl_cii/i18n/pt.po` (2,406 lines)
- `addons/account_edi_ubl_cii/i18n/pt_BR.po` (2,532 lines)
- `addons/account_edi_ubl_cii/i18n/ro.po` (2,489 lines)
- `addons/account_edi_ubl_cii/i18n/ru.po` (2,498 lines)
- `addons/account_edi_ubl_cii/i18n/sk.po` (2,659 lines)
- `addons/account_edi_ubl_cii/i18n/sl.po` (2,377 lines)
- `addons/account_edi_ubl_cii/i18n/sr@latin.po` (2,202 lines)
- `addons/account_edi_ubl_cii/i18n/sv.po` (2,501 lines)
- `addons/account_edi_ubl_cii/i18n/th.po` (2,339 lines)
- `addons/account_edi_ubl_cii/i18n/tr.po` (2,504 lines)
- `addons/account_edi_ubl_cii/i18n/uk.po` (2,489 lines)
- `addons/account_edi_ubl_cii/i18n/uz.po` (2,648 lines)
- `addons/account_edi_ubl_cii/i18n/vi.po` (2,379 lines)
- `addons/account_edi_ubl_cii/i18n/zh_CN.po` (2,394 lines)
- `addons/account_edi_ubl_cii/i18n/zh_TW.po` (2,416 lines)
- `addons/account_edi_ubl_cii/models/__init__.py` (22 lines)
- `addons/account_edi_ubl_cii/models/account_edi_cii.py` (1,597 lines)
- `addons/account_edi_ubl_cii/models/account_edi_common.py` (2,115 lines)
- `addons/account_edi_ubl_cii/models/account_edi_ubl.py` (3,106 lines)
- `addons/account_edi_ubl_cii/models/account_edi_ubl_cen_en16931.py` (259 lines)
- `addons/account_edi_ubl_cii/models/account_edi_ubl_pint.py` (628 lines)
- `addons/account_edi_ubl_cii/models/account_edi_ubl_pint_eu.py` (170 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_cii_facturx.py` (503 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_20.py` (1,344 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_21.py` (75 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_a_nz.py` (59 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_bis3.py` (480 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_efff.py` (20 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_nlcius.py` (128 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_sg.py` (84 lines)
- `addons/account_edi_ubl_cii/models/account_edi_xml_ubl_xrechnung.py` (125 lines)
- `addons/account_edi_ubl_cii/models/account_move.py` (366 lines)
- `addons/account_edi_ubl_cii/models/account_move_send.py` (354 lines)
- `addons/account_edi_ubl_cii/models/account_tax.py` (133 lines)
- `addons/account_edi_ubl_cii/models/ir_actions_report.py` (30 lines)
- `addons/account_edi_ubl_cii/models/res_company.py` (17 lines)
- `addons/account_edi_ubl_cii/models/res_partner.py` (350 lines)
- `addons/account_edi_ubl_cii/models/uom_uom.py` (47 lines)
- `addons/account_edi_ubl_cii/report/account_edi_ubl_cii_report_templates.xml` (98 lines)
- `addons/account_edi_ubl_cii/static/src/scss/account_edi_ubl_cii.scss` (8 lines)
- `addons/account_edi_ubl_cii/tests/__init__.py` (35 lines)
- `addons/account_edi_ubl_cii/tests/common.py` (419 lines)
- `addons/account_edi_ubl_cii/tests/test_addresses.py` (26 lines)
- `addons/account_edi_ubl_cii/tests/test_autopost_bills.py` (148 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_export_facturx_fr.py` (654 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_facturx_fr_decode_invoice_line.py` (240 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr.py` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_cash_rounding.py` (73 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_group_lines_by_tax.py` (88 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_retrieve_account.py` (36 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_retrieve_analytic_distribution.py` (40 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_retrieve_partner.py` (67 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_retrieve_product.py` (69 lines)
- `addons/account_edi_ubl_cii/tests/test_cii_import_facturx_fr_retrieve_tax.py` (189 lines)
- `addons/account_edi_ubl_cii/tests/test_download_docs.py` (101 lines)
- `addons/account_edi_ubl_cii/tests/test_files/bis3_bill_group_by_tax.xml` (155 lines)
- `addons/account_edi_ubl_cii/tests/test_files/bis3_bill_vehicle_line.xml` (306 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/debit_note/be/test_export_debit_note.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/debit_note/ignore_schema.xml` (27 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_BR_CO_10_line_extension_amount_sum_lines.xml` (254 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_BR_E_08_line_extension_amount.xml` (194 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_BR_S_08_tax_subtotal_taxable_amount.xml` (175 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_PEPPOL_EN16931_R120_line_extension_amount_huge_number_of_decimals.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_allowance_charge_custom_tax_recycling_contribution.xml` (181 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_allowance_charge_fixed_tax_recycling_contribution.xml` (207 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_cash_rounding_add_invoice_line.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_cash_rounding_biggest_tax.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_custom_tax_emptying_turned_as_extra_invoice_lines.xml` (193 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_be_invoice_address.xml` (142 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_be_only_eas_endpoint.xml` (142 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_be_vat.xml` (142 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_be_vat_and_company_registry.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_be_vat_and_ref.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_lu_company_registry.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_lu_only_vat.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_nl_vat_eas_kvk_company_registry.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_nl_vat_eas_oin_company_registry.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_nl_vat_kvk_eas.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_customer_party_identifiers_partner_nl_vat_oin_eas.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_early_pay_discount_multiple_taxes.xml` (230 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_early_pay_discount_with_0_tax.xml` (177 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_early_pay_discount_with_discount_on_lines.xml` (890 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_early_pay_discount_with_recycling_contribution_tax.xml` (194 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_export_sections_as_invoice_lines.xml` (192 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_export_sections_with_price_included_taxes.xml` (163 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_fixed_tax_emptying_return_turned_as_extra_invoice_lines.xml` (193 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_fixed_tax_emptying_turned_as_extra_invoice_lines.xml` (193 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_item_description_name.xml` (152 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_manual_tax_amount.xml` (210 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_multiple_fixed_tax_emptying_turned_as_extra_invoice_lines.xml` (229 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_negative_discount_upsell.xml` (153 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_negative_price_unit.xml` (163 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_payee_financial_account.xml` (148 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_payment_mandate_active.xml` (151 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_payment_mandate_expired.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_price_amount_rounding_precision_with_price_included_taxes.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_price_amount_rounding_precision_with_price_included_taxes_plus_free_product.xml` (176 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_price_unit_more_decimals.xml` (145 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_product_commodity_code_cpv.xml` (148 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_product_commodity_code_intrastat.xml` (148 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_product_commodity_code_unspsc.xml` (148 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_send_and_print_additional_documents.xml` (151 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_sent_to_luxembourg_dig.xml` (143 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_sent_to_partner_with_gln.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_currency_code_tax_totals_foreign_currency.xml` (149 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_exempt.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_out_of_scope.xml` (133 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_subtotal_exempt_amount_round_globally.xml` (180 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_subtotal_exempt_amount_round_per_line.xml` (181 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_tax_withholding.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_with_discount_and_fixed_tax_emptying_return.xml` (183 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_with_fixed_tax_on_negative_line.xml` (175 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_with_global_discount_line_sale_order.xml` (160 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_invoice_with_vehicle_license_plate.xml` (175 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/be/test_sale_order_down_payment_first_invoice.xml` (146 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice/ignore_schema.xml` (27 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice_selfbilling/be/test_credit_note_self_billing_payment_mandate_active.xml` (150 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice_selfbilling/be/test_credit_note_self_billing_payment_mandate_expired.xml` (144 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice_selfbilling/be/test_credit_note_selfbilling.xml` (144 lines)
- `addons/account_edi_ubl_cii/tests/test_files/export/bis3/invoice_selfbilling/be/test_invoice_selfbilling.xml` (146 lines)

Additional files not expanded here: 163. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
