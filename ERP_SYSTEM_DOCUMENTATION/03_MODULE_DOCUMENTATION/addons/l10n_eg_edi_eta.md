# Module: l10n_eg_edi_eta

- **Module ID:** MOD-172
- **Path:** `addons/l10n_eg_edi_eta`
- **Manifest:** `addons/l10n_eg_edi_eta/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Egypt Tax Authority Invoice Integration


Egypt Tax Authority Invoice Integration
==============================================================================
Integrates with the ETA portal to automatically send and sign the Invoices to the Tax Authority.
    

Declared dependencies: `l10n_eg`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_eg"
  ],
  "data": [
    "data/l10n_eg_edi.activity.type.csv",
    "data/l10n_eg_edi.uom.code.csv",
    "data/uom.uom.csv",
    "views/l10n_eg_edi_activity_type_view.xml",
    "views/uom_uom_view.xml",
    "views/account_move_view.xml",
    "views/account_journal_view.xml",
    "views/eta_thumb_drive.xml",
    "views/product_template_views.xml",
    "views/res_config_settings_view.xml",
    "views/report_invoice.xml",
    "wizards/l10n_eg_edi_cancel_wizard.xml",
    "data/res_country_data.xml",
    "views/res_company_view.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_eg_edi_eta/static/src/**/*.js"
    ]
  },
  "external_dependencies": {
    "python": [
      "asn1crypto"
    ],
    "apt": {
      "asn1crypto": "python3-asn1crypto"
    }
  }
}
```

### Representative source files

- `addons/l10n_eg_edi_eta/__init__.py` (11 lines)
- `addons/l10n_eg_edi_eta/__manifest__.py` (46 lines)
- `addons/l10n_eg_edi_eta/data/l10n_eg_edi.activity.type.csv` (436 lines)
- `addons/l10n_eg_edi_eta/data/l10n_eg_edi.uom.code.csv` (144 lines)
- `addons/l10n_eg_edi_eta/data/neutralize.sql` (4 lines)
- `addons/l10n_eg_edi_eta/data/res_country_data.xml` (31 lines)
- `addons/l10n_eg_edi_eta/data/uom.uom.csv` (26 lines)
- `addons/l10n_eg_edi_eta/i18n/ar.po` (1,968 lines)
- `addons/l10n_eg_edi_eta/i18n/l10n_eg_edi_eta.pot` (1,847 lines)
- `addons/l10n_eg_edi_eta/lib/eta_client.py` (134 lines)
- `addons/l10n_eg_edi_eta/models/__init__.py` (13 lines)
- `addons/l10n_eg_edi_eta/models/account_journal.py` (13 lines)
- `addons/l10n_eg_edi_eta/models/account_move.py` (836 lines)
- `addons/l10n_eg_edi_eta/models/account_move_send.py` (57 lines)
- `addons/l10n_eg_edi_eta/models/eta_activity_type.py` (15 lines)
- `addons/l10n_eg_edi_eta/models/eta_submission.py` (56 lines)
- `addons/l10n_eg_edi_eta/models/eta_thumb_drive.py` (159 lines)
- `addons/l10n_eg_edi_eta/models/ir_attachment.py` (29 lines)
- `addons/l10n_eg_edi_eta/models/product_template.py` (65 lines)
- `addons/l10n_eg_edi_eta/models/res_company.py` (24 lines)
- `addons/l10n_eg_edi_eta/models/res_config_settings.py` (9 lines)
- `addons/l10n_eg_edi_eta/models/res_currency_rate.py` (24 lines)
- `addons/l10n_eg_edi_eta/models/res_partner.py` (33 lines)
- `addons/l10n_eg_edi_eta/models/uom_uom.py` (16 lines)
- `addons/l10n_eg_edi_eta/security/ir.access.csv` (7 lines)
- `addons/l10n_eg_edi_eta/static/src/client_action/sign_invoice.js` (131 lines)
- `addons/l10n_eg_edi_eta/tests/__init__.py` (1 lines)
- `addons/l10n_eg_edi_eta/tests/common.py` (110 lines)
- `addons/l10n_eg_edi_eta/tests/test_edi_json.py` (908 lines)
- `addons/l10n_eg_edi_eta/tools/__init__.py` (0 lines)
- `addons/l10n_eg_edi_eta/tools/eta_serialize.py` (22 lines)
- `addons/l10n_eg_edi_eta/views/account_journal_view.xml` (20 lines)
- `addons/l10n_eg_edi_eta/views/account_move_view.xml` (129 lines)
- `addons/l10n_eg_edi_eta/views/eta_thumb_drive.xml` (28 lines)
- `addons/l10n_eg_edi_eta/views/l10n_eg_edi_activity_type_view.xml` (24 lines)
- `addons/l10n_eg_edi_eta/views/product_template_views.xml` (63 lines)
- `addons/l10n_eg_edi_eta/views/report_invoice.xml` (15 lines)
- `addons/l10n_eg_edi_eta/views/res_company_view.xml` (16 lines)
- `addons/l10n_eg_edi_eta/views/res_config_settings_view.xml` (47 lines)
- `addons/l10n_eg_edi_eta/views/uom_uom_view.xml` (14 lines)
- `addons/l10n_eg_edi_eta/wizards/__init__.py` (1 lines)
- `addons/l10n_eg_edi_eta/wizards/l10n_eg_edi_cancel_wizard.py` (13 lines)
- `addons/l10n_eg_edi_eta/wizards/l10n_eg_edi_cancel_wizard.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
