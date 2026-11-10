# Module: l10n_account_edi_ubl_cii_tests

- **Module ID:** MOD-114
- **Path:** `addons/l10n_account_edi_ubl_cii_tests`
- **Manifest:** `addons/l10n_account_edi_ubl_cii_tests/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module tests the module 'account_edi_ubl_cii', it is separated since dependencies to some
localizations were required. Its name begins with 'l10n' to not overload runbot.

The test files are separated by sources, they were taken from:

* the factur-x doc (form the FNFE)
* the peppol-bis-invoice-3 doc (the github repository: https://github.com/OpenPEPPOL/peppol-bis-invoice-3/tree/master/rules/examples contains examples)
* odoo, these files pass all validation tests (using ecosio or the FNFE validator)

We test that the external examples are correctly imported (currency, total amount and total tax match).
We also test that generating xml from odoo with given parameters gives exactly the same xml as the expected,
valid ones.
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_fr_account`, `l10n_be`, `l10n_de`, `l10n_nl`, `l10n_au`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 42 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_fr_account",
    "l10n_be",
    "l10n_de",
    "l10n_nl",
    "l10n_au"
  ]
}
```

### Representative source files

- `addons/l10n_account_edi_ubl_cii_tests/__init__.py` (2 lines)
- `addons/l10n_account_edi_ubl_cii_tests/__manifest__.py` (28 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/__init__.py` (11 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/common.py` (248 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_factur-x_doc/facturx_credit_note_type380.xml` (193 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_factur-x_doc/facturx_credit_note_type381.xml` (193 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_factur-x_doc/facturx_invoice_basis_quantity.xml` (441 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_factur-x_doc/facturx_invoice_negative_amounts.xml` (325 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/a_nz_out_invoice.xml` (194 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/a_nz_out_invoice_attacheddocument_b64.xml` (179 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/a_nz_out_invoice_attacheddocument_description.xml` (256 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/a_nz_out_refund.xml` (193 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_ecotaxes_case1.xml` (160 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_ecotaxes_case2.xml` (166 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_ecotaxes_case3.xml` (160 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_ecotaxes_case4.xml` (165 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_ecotaxes_case5.xml` (178 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_out_invoice.xml` (211 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_out_invoice_no_prices.xml` (171 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_out_invoice_quantity_and_or_unit_price_zero.xml` (182 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_out_refund.xml` (209 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/bis3_pay_term.xml` (238 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_ecotaxes_case1.xml` (170 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_ecotaxes_case2.xml` (178 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_ecotaxes_case3.xml` (170 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_out_invoice.xml` (232 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_out_invoice_tax_incl.xml` (259 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_out_refund.xml` (231 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_positive_discount_price_unit.xml` (189 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/facturx_test_import_partner.xml` (127 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/nlcius_out_invoice.xml` (208 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/nlcius_out_refund.xml` (212 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/sg_out_invoice.xml` (188 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/sg_out_refund.xml` (187 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/ubl_test_import_partner.xml` (104 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/xrechnung_ubl_out_invoice.xml` (206 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/xrechnung_ubl_out_refund.xml` (205 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/zugferd_out_invoice.xml` (220 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/zugferd_out_invoice_gln.xml` (144 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/zugferd_out_invoice_without_vat.xml` (148 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_odoo/zugferd_out_refund.xml` (219 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_peppol-bis-invoice-3_doc/bis3_allowance.xml` (369 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_peppol-bis-invoice-3_doc/bis3_credit_note.xml` (224 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_peppol-bis-invoice-3_doc/bis3_invoice_ignore_lineextensionamount.xml` (43 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_peppol-bis-invoice-3_doc/bis3_invoice_negative_amounts.xml` (224 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_files/from_peppol-bis-invoice-3_doc/bis3_tax_exempt_gbp.xml` (114 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_cii_de.py` (113 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_cii_fr.py` (578 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_cii_us.py` (71 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_attacheddocument.py` (77 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_au.py` (190 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_be.py` (642 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_de.py` (503 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_nl.py` (244 lines)
- `addons/l10n_account_edi_ubl_cii_tests/tests/test_xml_ubl_sg.py` (144 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
