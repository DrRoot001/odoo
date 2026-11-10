# Module: l10n_es_edi_verifactu

- **Module ID:** MOD-179
- **Path:** `addons/l10n_es_edi_verifactu`
- **Manifest:** `addons/l10n_es_edi_verifactu/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Module for sending Spanish Veri*Factu XML to the AEAT

No manifest description declared.

Declared dependencies: `l10n_es`, `certificate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
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
    "wizard/account_resequence_views.xml",
    "views/account_move_views.xml",
    "views/certificate_certificate_views.xml",
    "views/l10n_es_edi_verifactu_document_views.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml",
    "views/account_journal_dashboard_view.xml",
    "data/ir_cron.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_certificate.xml",
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_es_edi_verifactu/static/src/css/warning.scss"
    ]
  }
}
```

### Representative source files

- `addons/l10n_es_edi_verifactu/__init__.py` (4 lines)
- `addons/l10n_es_edi_verifactu/__manifest__.py` (31 lines)
- `addons/l10n_es_edi_verifactu/const.py` (14 lines)
- `addons/l10n_es_edi_verifactu/data/ir_cron.xml` (11 lines)
- `addons/l10n_es_edi_verifactu/data/neutralize.sql` (3 lines)
- `addons/l10n_es_edi_verifactu/data/template/account.tax-es_common.csv` (281 lines)
- `addons/l10n_es_edi_verifactu/demo/certificates/Certificado_PF_99999910G_CERTIFICADO_FISICA_PRUEBAS_5_Pre.pfx` (65 lines)
- `addons/l10n_es_edi_verifactu/demo/certificates/Certificado_RPJ_A39200019_CERTIFICADO_ENTIDAD_PRUEBAS_5_Pre.p12` (73 lines)
- `addons/l10n_es_edi_verifactu/demo/demo_certificate.xml` (10 lines)
- `addons/l10n_es_edi_verifactu/demo/demo_company.xml` (8 lines)
- `addons/l10n_es_edi_verifactu/i18n/es.po` (1,136 lines)
- `addons/l10n_es_edi_verifactu/i18n/l10n_es_edi_verifactu.pot` (921 lines)
- `addons/l10n_es_edi_verifactu/models/__init__.py` (12 lines)
- `addons/l10n_es_edi_verifactu/models/account_journal_dashboard.py` (28 lines)
- `addons/l10n_es_edi_verifactu/models/account_move.py` (295 lines)
- `addons/l10n_es_edi_verifactu/models/account_move_send.py` (137 lines)
- `addons/l10n_es_edi_verifactu/models/account_tax.py` (97 lines)
- `addons/l10n_es_edi_verifactu/models/certificate.py` (11 lines)
- `addons/l10n_es_edi_verifactu/models/res_company.py` (66 lines)
- `addons/l10n_es_edi_verifactu/models/res_config_settings.py` (18 lines)
- `addons/l10n_es_edi_verifactu/models/res_partner.py` (10 lines)
- `addons/l10n_es_edi_verifactu/models/verifactu_document.py` (1,341 lines)
- `addons/l10n_es_edi_verifactu/models/verifactu_issuer.py` (69 lines)
- `addons/l10n_es_edi_verifactu/security/ir.access.csv` (6 lines)
- `addons/l10n_es_edi_verifactu/static/src/css/warning.scss` (5 lines)
- `addons/l10n_es_edi_verifactu/tests/__init__.py` (4 lines)
- `addons/l10n_es_edi_verifactu/tests/common.py` (241 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_1.json` (74 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_1_correction_substitution.json` (87 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_1_credit_note.json` (83 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_1_reversal_for_substitution.json` (74 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_2.json` (79 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_3.json` (64 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_4.json` (84 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_cancellation_1.json` (49 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_export.json` (68 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_multi_currency_1.json` (77 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_invoice_simplified_partner.json` (58 lines)
- `addons/l10n_es_edi_verifactu/tests/files/test_multiple_invoices_with_predecessor.json` (191 lines)
- `addons/l10n_es_edi_verifactu/tests/responses/batch_single_accepted_cancellation.json` (39 lines)
- `addons/l10n_es_edi_verifactu/tests/responses/batch_single_accepted_registration.json` (39 lines)
- `addons/l10n_es_edi_verifactu/tests/responses/batch_single_duplicate_original_registered_with_errors.json` (44 lines)
- `addons/l10n_es_edi_verifactu/tests/responses/batch_single_registered_with_errors_registration.json` (39 lines)
- `addons/l10n_es_edi_verifactu/tests/responses/batch_single_rejected_registration.json` (39 lines)
- `addons/l10n_es_edi_verifactu/tests/test_document.py` (782 lines)
- `addons/l10n_es_edi_verifactu/tests/test_json.py` (499 lines)
- `addons/l10n_es_edi_verifactu/tests/test_verifactu_partner_id_types.py` (28 lines)
- `addons/l10n_es_edi_verifactu/views/account_journal_dashboard_view.xml` (24 lines)
- `addons/l10n_es_edi_verifactu/views/account_move_views.xml` (153 lines)
- `addons/l10n_es_edi_verifactu/views/certificate_certificate_views.xml` (50 lines)
- `addons/l10n_es_edi_verifactu/views/l10n_es_edi_verifactu_document_views.xml` (33 lines)
- `addons/l10n_es_edi_verifactu/views/report_invoice.xml` (15 lines)
- `addons/l10n_es_edi_verifactu/views/res_config_settings_views.xml` (53 lines)
- `addons/l10n_es_edi_verifactu/wizard/__init__.py` (4 lines)
- `addons/l10n_es_edi_verifactu/wizard/account_move_reversal.py` (14 lines)
- `addons/l10n_es_edi_verifactu/wizard/account_resequence.py` (16 lines)
- `addons/l10n_es_edi_verifactu/wizard/account_resequence_views.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
