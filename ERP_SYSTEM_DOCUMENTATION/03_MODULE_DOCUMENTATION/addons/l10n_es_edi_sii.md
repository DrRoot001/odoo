# Module: l10n_es_edi_sii

- **Module ID:** MOD-176
- **Path:** `addons/l10n_es_edi_sii`
- **Manifest:** `addons/l10n_es_edi_sii/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module sends the taxes information (mostly VAT) of the
vendor bills and customer invoices to the SII.  It is called
Procedimiento G417 - IVA. Llevanza de libros registro.  It is
required for every company with a turnover of +6M€ and others can
already make use of it.  The invoices are automatically
sent after validation.

How the information is sent to the SII depends on the
configuration that is put in the taxes.  The taxes
that were in the chart template (l10n_es) are automatically
configured to have the right type.  It is possible however
that extra taxes need to be created for certain exempt/no sujeta reasons.

You need to configure your certificate and the tax agency.
    

Declared dependencies: `certificate`, `l10n_es`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
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
    "views/account_move_views.xml",
    "views/account_journal_dashboard_views.xml",
    "views/l10n_es_edi_sii_certificate_views.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_certificate.xml",
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_es_edi_sii/__init__.py` (4 lines)
- `addons/l10n_es_edi_sii/__manifest__.py` (44 lines)
- `addons/l10n_es_edi_sii/data/neutralize.sql` (3 lines)
- `addons/l10n_es_edi_sii/demo/certificates/aeat_1234.p12` (73 lines)
- `addons/l10n_es_edi_sii/demo/demo_certificate.xml` (12 lines)
- `addons/l10n_es_edi_sii/demo/demo_company.xml` (7 lines)
- `addons/l10n_es_edi_sii/i18n/es.po` (643 lines)
- `addons/l10n_es_edi_sii/i18n/l10n_es_edi_sii.pot` (608 lines)
- `addons/l10n_es_edi_sii/models/__init__.py` (9 lines)
- `addons/l10n_es_edi_sii/models/account_journal.py` (81 lines)
- `addons/l10n_es_edi_sii/models/account_move.py` (740 lines)
- `addons/l10n_es_edi_sii/models/account_move_send.py` (66 lines)
- `addons/l10n_es_edi_sii/models/certificate.py` (11 lines)
- `addons/l10n_es_edi_sii/models/l10n_es_edi_sii_document.py` (416 lines)
- `addons/l10n_es_edi_sii/models/res_company.py` (47 lines)
- `addons/l10n_es_edi_sii/models/res_config_settings.py` (11 lines)
- `addons/l10n_es_edi_sii/security/ir.access.csv` (3 lines)
- `addons/l10n_es_edi_sii/tests/__init__.py` (5 lines)
- `addons/l10n_es_edi_sii/tests/common.py` (79 lines)
- `addons/l10n_es_edi_sii/tests/test_account_journal.py` (131 lines)
- `addons/l10n_es_edi_sii/tests/test_edi_web_services.py` (69 lines)
- `addons/l10n_es_edi_sii/tests/test_edi_xml.py` (1,424 lines)
- `addons/l10n_es_edi_sii/views/account_journal_dashboard_views.xml` (28 lines)
- `addons/l10n_es_edi_sii/views/account_move_views.xml` (142 lines)
- `addons/l10n_es_edi_sii/views/l10n_es_edi_sii_certificate_views.xml` (47 lines)
- `addons/l10n_es_edi_sii/views/res_config_settings_views.xml` (44 lines)
- `addons/l10n_es_edi_sii/wizard/__init__.py` (1 lines)
- `addons/l10n_es_edi_sii/wizard/account_move_send_wizard.py` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
