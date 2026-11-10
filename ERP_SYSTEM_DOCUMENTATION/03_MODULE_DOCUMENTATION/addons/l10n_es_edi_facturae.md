# Module: l10n_es_edi_facturae

- **Module ID:** MOD-175
- **Path:** `addons/l10n_es_edi_facturae`
- **Manifest:** `addons/l10n_es_edi_facturae/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module create the Facturae file required to send the invoices information to the General State Administrations.
It allows the export and signature of the signing of Facturae files.
The current version of Facturae supported is the 3.2.2

for more informations, see https://www.facturae.gob.es/face/Paginas/FACE.aspx
    

Declared dependencies: `certificate`, `l10n_es`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 24 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "certificate",
    "l10n_es"
  ],
  "data": [
    "data/uom.uom.csv",
    "data/facturae_templates.xml",
    "data/l10n_es_edi_facturae.ac_role_type.csv",
    "data/signature_templates.xml",
    "views/l10n_es_edi_facturae_views.xml",
    "views/res_partner_views.xml",
    "views/account_tax_views.xml",
    "views/account_move_views.xml",
    "views/uom_uom_views.xml",
    "views/account_menuitem.xml",
    "wizard/account_move_reversal_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/l10n_es_edi_facturae_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_es_edi_facturae/__init__.py` (7 lines)
- `addons/l10n_es_edi_facturae/__manifest__.py` (40 lines)
- `addons/l10n_es_edi_facturae/data/facturae_templates.xml` (331 lines)
- `addons/l10n_es_edi_facturae/data/l10n_es_edi_facturae.ac_role_type.csv` (10 lines)
- `addons/l10n_es_edi_facturae/data/signature_templates.xml` (91 lines)
- `addons/l10n_es_edi_facturae/data/template/account.tax-es_common.csv` (253 lines)
- `addons/l10n_es_edi_facturae/data/uom.uom.csv` (14 lines)
- `addons/l10n_es_edi_facturae/demo/certificate_demo.pfx` (35 lines)
- `addons/l10n_es_edi_facturae/demo/l10n_es_edi_facturae_demo.xml` (43 lines)
- `addons/l10n_es_edi_facturae/i18n/es.po` (1,164 lines)
- `addons/l10n_es_edi_facturae/i18n/l10n_es_edi_facturae.pot` (1,080 lines)
- `addons/l10n_es_edi_facturae/models/__init__.py` (8 lines)
- `addons/l10n_es_edi_facturae/models/account_chart_template.py` (10 lines)
- `addons/l10n_es_edi_facturae/models/account_move.py` (918 lines)
- `addons/l10n_es_edi_facturae/models/account_move_send.py` (136 lines)
- `addons/l10n_es_edi_facturae/models/account_tax.py` (37 lines)
- `addons/l10n_es_edi_facturae/models/certificate.py` (27 lines)
- `addons/l10n_es_edi_facturae/models/res_company.py` (40 lines)
- `addons/l10n_es_edi_facturae/models/res_partner.py` (87 lines)
- `addons/l10n_es_edi_facturae/models/uom_uom.py` (45 lines)
- `addons/l10n_es_edi_facturae/security/ir.access.csv` (2 lines)
- `addons/l10n_es_edi_facturae/tests/__init__.py` (1 lines)
- `addons/l10n_es_edi_facturae/tests/data/certificate_test.pfx` (31 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_ac_document.xml` (259 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_in_invoice_document.xml` (298 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_invoice_payment_means.xml` (211 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_invoice_period_document.xml` (215 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_out_invoice_4_decimals.xml` (211 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_out_invoice_negative.xml` (264 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_out_invoice_round_2.xml` (253 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_out_invoice_round_glob.xml` (274 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_out_invoice_withhold.xml` (211 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_refund_document.xml` (241 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_signed_document.xml` (333 lines)
- `addons/l10n_es_edi_facturae/tests/data/expected_simplified_document.xml` (212 lines)
- `addons/l10n_es_edi_facturae/tests/data/import_multiple_invoices.xml` (333 lines)
- `addons/l10n_es_edi_facturae/tests/data/import_withholding_invoice.xml` (255 lines)
- `addons/l10n_es_edi_facturae/tests/test_edi_xml.py` (827 lines)
- `addons/l10n_es_edi_facturae/views/account_menuitem.xml` (10 lines)
- `addons/l10n_es_edi_facturae/views/account_move_views.xml` (20 lines)
- `addons/l10n_es_edi_facturae/views/account_tax_views.xml` (28 lines)
- `addons/l10n_es_edi_facturae/views/l10n_es_edi_facturae_views.xml` (35 lines)
- `addons/l10n_es_edi_facturae/views/res_partner_views.xml` (18 lines)
- `addons/l10n_es_edi_facturae/views/uom_uom_views.xml` (23 lines)
- `addons/l10n_es_edi_facturae/wizard/__init__.py` (2 lines)
- `addons/l10n_es_edi_facturae/wizard/account_move_reversal.py` (31 lines)
- `addons/l10n_es_edi_facturae/wizard/account_move_reversal_view.xml` (30 lines)
- `addons/l10n_es_edi_facturae/wizard/account_move_send_wizard.py` (14 lines)
- `addons/l10n_es_edi_facturae/xml_utils.py` (65 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
