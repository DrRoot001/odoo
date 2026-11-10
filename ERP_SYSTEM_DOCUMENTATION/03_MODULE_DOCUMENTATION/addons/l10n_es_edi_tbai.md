# Module: l10n_es_edi_tbai

- **Module ID:** MOD-177
- **Path:** `addons/l10n_es_edi_tbai`
- **Manifest:** `addons/l10n_es_edi_tbai/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module sends invoices and vendor bills to the "Diputaciones
Forales" of Araba/Álava, Bizkaia and Gipuzkoa.

Invoices and bills get converted to XML and regularly sent to the
Basque government servers which provides them with a unique identifier.
A hash chain ensures the continuous nature of the invoice/bill
sequences. QR codes are added to emitted (sent/printed) invoices,
bills and tickets to allow anyone to check they have been declared.

You need to configure your certificate and the tax agency.
    

Declared dependencies: `l10n_es`, `certificate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 29 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_es",
    "certificate"
  ],
  "data": [
    "data/template_invoice.xml",
    "data/template_LROE_bizkaia.xml",
    "data/ir_config_parameter.xml",
    "views/account_move_view.xml",
    "views/l10n_es_edi_tbai_certificate_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "views/res_company_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_certificate.xml",
    "demo/demo_res_partner.xml",
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_es_edi_tbai/__init__.py` (4 lines)
- `addons/l10n_es_edi_tbai/__manifest__.py` (46 lines)
- `addons/l10n_es_edi_tbai/const.py` (4 lines)
- `addons/l10n_es_edi_tbai/data/ir_config_parameter.xml` (9 lines)
- `addons/l10n_es_edi_tbai/data/neutralize.sql` (3 lines)
- `addons/l10n_es_edi_tbai/data/template_LROE_bizkaia.xml` (209 lines)
- `addons/l10n_es_edi_tbai/data/template_invoice.xml` (265 lines)
- `addons/l10n_es_edi_tbai/demo/certificates/Bizkaia-IZDesa2025.p12` (45 lines)
- `addons/l10n_es_edi_tbai/demo/certificates/araba_1234.p12` (69 lines)
- `addons/l10n_es_edi_tbai/demo/certificates/gipuzkoa_Iz3np32024.p12` (48 lines)
- `addons/l10n_es_edi_tbai/demo/demo_certificate.xml` (10 lines)
- `addons/l10n_es_edi_tbai/demo/demo_company.xml` (7 lines)
- `addons/l10n_es_edi_tbai/demo/demo_res_partner.xml` (19 lines)
- `addons/l10n_es_edi_tbai/i18n/es.po` (807 lines)
- `addons/l10n_es_edi_tbai/i18n/l10n_es_edi_tbai.pot` (703 lines)
- `addons/l10n_es_edi_tbai/models/__init__.py` (12 lines)
- `addons/l10n_es_edi_tbai/models/account_move.py` (382 lines)
- `addons/l10n_es_edi_tbai/models/account_move_line.py` (10 lines)
- `addons/l10n_es_edi_tbai/models/account_move_send.py` (63 lines)
- `addons/l10n_es_edi_tbai/models/account_tax.py` (27 lines)
- `addons/l10n_es_edi_tbai/models/certificate.py` (25 lines)
- `addons/l10n_es_edi_tbai/models/l10n_es_edi_tbai_agencies.py` (76 lines)
- `addons/l10n_es_edi_tbai/models/l10n_es_edi_tbai_document.py` (892 lines)
- `addons/l10n_es_edi_tbai/models/res_company.py` (184 lines)
- `addons/l10n_es_edi_tbai/models/res_config_settings.py` (12 lines)
- `addons/l10n_es_edi_tbai/models/xml_utils.py` (88 lines)
- `addons/l10n_es_edi_tbai/security/ir.access.csv` (3 lines)
- `addons/l10n_es_edi_tbai/tests/__init__.py` (11 lines)
- `addons/l10n_es_edi_tbai/tests/common.py` (264 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_cancel.xml` (27 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_fecha_operacion.xml` (84 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post.xml` (83 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post_in.xml` (50 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post_in_140.xml` (51 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post_in_ic.xml` (55 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post_in_nd.xml` (50 lines)
- `addons/l10n_es_edi_tbai/tests/document_xmls/xml_post_refund.xml` (95 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/cancel_bill_failure_bi.xml` (31 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/cancel_bill_success_bi.xml` (33 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/cancel_invoice_failure_bi.xml` (28 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/cancel_invoice_success_bi.xml` (33 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/cancel_invoice_success_gi.xml` (16 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/post_bill_success_bi.xml` (33 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/post_invoice_failure_bi.xml` (28 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/post_invoice_success_bi.xml` (33 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/post_invoice_success_gi.xml` (16 lines)
- `addons/l10n_es_edi_tbai/tests/response_xmls/post_or_cancel_invoice_failure_gi.xml` (14 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_tbai_send_bill_bizkaia.py` (101 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_tbai_send_invoice.py` (216 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_tbai_send_invoice_bizkaia.py` (107 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_tbai_user_errors.py` (159 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_web_services.py` (67 lines)
- `addons/l10n_es_edi_tbai/tests/test_edi_xml.py` (423 lines)
- `addons/l10n_es_edi_tbai/tests/test_move_reversal.py` (78 lines)
- `addons/l10n_es_edi_tbai/tests/test_tbai_recipient_id_types.py` (129 lines)
- `addons/l10n_es_edi_tbai/views/account_move_view.xml` (62 lines)
- `addons/l10n_es_edi_tbai/views/l10n_es_edi_tbai_certificate_views.xml` (50 lines)
- `addons/l10n_es_edi_tbai/views/report_invoice.xml` (14 lines)
- `addons/l10n_es_edi_tbai/views/res_company_views.xml` (25 lines)
- `addons/l10n_es_edi_tbai/views/res_config_settings_views.xml` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
