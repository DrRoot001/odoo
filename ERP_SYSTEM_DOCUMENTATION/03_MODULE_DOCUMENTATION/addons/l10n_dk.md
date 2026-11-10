# Module: l10n_dk

- **Module ID:** MOD-164
- **Path:** `addons/l10n_dk`
- **Manifest:** `addons/l10n_dk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.



Localization Module for Denmark
===============================

This is the module to manage the **accounting chart for Denmark**. Cover both one-man business as well as I/S, IVS, ApS and A/S
Also provides Nemhandel registration and invoice sending throught the Odoo Access Point

    

Declared dependencies: `account`, `account_edi_proxy_client`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 20 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_proxy_client",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/account.account.tag.csv",
    "data/cron.xml",
    "data/nemhandel_onboarding_tour.xml",
    "views/account_journal_views.xml",
    "views/account_move_views.xml",
    "views/nemhandel_response_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "wizard/nemhandel_registration_views.xml",
    "wizard/nemhandel_rejection_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/nemhandel_mode_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_dk/static/src/components/**/*",
      "l10n_dk/static/src/tours/nemhandel_onboarding.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_dk/__init__.py` (12 lines)
- `addons/l10n_dk/__manifest__.py` (52 lines)
- `addons/l10n_dk/controllers/__init__.py` (1 lines)
- `addons/l10n_dk/controllers/webhooks.py` (62 lines)
- `addons/l10n_dk/data/account.account.tag.csv` (490 lines)
- `addons/l10n_dk/data/account_tax_report_data.xml` (248 lines)
- `addons/l10n_dk/data/cron.xml` (38 lines)
- `addons/l10n_dk/data/nemhandel_onboarding_tour.xml` (11 lines)
- `addons/l10n_dk/data/neutralize.sql` (3 lines)
- `addons/l10n_dk/data/template/account.account-dk.csv` (489 lines)
- `addons/l10n_dk/data/template/account.fiscal.position-dk.csv` (9 lines)
- `addons/l10n_dk/data/template/account.tax-dk.csv` (352 lines)
- `addons/l10n_dk/data/template/account.tax.group-dk.csv` (2 lines)
- `addons/l10n_dk/demo/demo_company.xml` (43 lines)
- `addons/l10n_dk/demo/nemhandel_mode_demo.xml` (7 lines)
- `addons/l10n_dk/i18n/da.po` (1,200 lines)
- `addons/l10n_dk/i18n/l10n_dk.pot` (1,152 lines)
- `addons/l10n_dk/migrations/1.2/end-migrate.py` (7 lines)
- `addons/l10n_dk/migrations/1.3/end-migrate.py` (9 lines)
- `addons/l10n_dk/migrations/1.4/end-migrate.py` (8 lines)
- `addons/l10n_dk/migrations/1.4/post-migrate.py` (105 lines)
- `addons/l10n_dk/models/__init__.py` (12 lines)
- `addons/l10n_dk/models/account_account.py` (35 lines)
- `addons/l10n_dk/models/account_edi_proxy_user.py` (565 lines)
- `addons/l10n_dk/models/account_edi_xml_oioubl_21.py` (310 lines)
- `addons/l10n_dk/models/account_journal.py` (57 lines)
- `addons/l10n_dk/models/account_move.py` (140 lines)
- `addons/l10n_dk/models/account_move_send.py` (135 lines)
- `addons/l10n_dk/models/nemhandel_response.py` (25 lines)
- `addons/l10n_dk/models/res_company.py` (150 lines)
- `addons/l10n_dk/models/res_config_settings.py` (69 lines)
- `addons/l10n_dk/models/res_partner.py` (298 lines)
- `addons/l10n_dk/models/template_dk.py` (46 lines)
- `addons/l10n_dk/security/ir.access.csv` (4 lines)
- `addons/l10n_dk/static/src/components/verification_code_widget/verification_code_widget.js` (56 lines)
- `addons/l10n_dk/static/src/components/verification_code_widget/verification_code_widget.xml` (18 lines)
- `addons/l10n_dk/static/src/tours/nemhandel_onboarding.js` (25 lines)
- `addons/l10n_dk/tests/__init__.py` (3 lines)
- `addons/l10n_dk/tests/assets/document` (1 lines)
- `addons/l10n_dk/tests/assets/enc_key` (1 lines)
- `addons/l10n_dk/tests/assets/private_key.pem` (28 lines)
- `addons/l10n_dk/tests/common.py` (156 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_invoice_child_partner.xml` (287 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_invoice_discount.xml` (246 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_invoice_foreign_partner_be.xml` (295 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_invoice_foreign_partner_fr.xml` (285 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_invoice_partner_dk.xml` (276 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_refund_foreign_partner_fr.xml` (283 lines)
- `addons/l10n_dk/tests/test_files/from_odoo/oioubl_out_refund_partner_dk.xml` (275 lines)
- `addons/l10n_dk/tests/test_nemhandel_messages.py` (284 lines)
- `addons/l10n_dk/tests/test_nemhandel_participant.py` (76 lines)
- `addons/l10n_dk/tests/test_xml_oioubl_21.py` (252 lines)
- `addons/l10n_dk/tools/__init__.py` (1 lines)
- `addons/l10n_dk/tools/demo_utils.py` (164 lines)
- `addons/l10n_dk/views/account_journal_views.xml` (29 lines)
- `addons/l10n_dk/views/account_move_views.xml` (85 lines)
- `addons/l10n_dk/views/nemhandel_response_views.xml` (28 lines)
- `addons/l10n_dk/views/res_config_settings_views.xml` (70 lines)
- `addons/l10n_dk/views/res_partner_views.xml` (40 lines)
- `addons/l10n_dk/wizard/__init__.py` (4 lines)
- `addons/l10n_dk/wizard/account_move_send_batch_wizard.py` (11 lines)
- `addons/l10n_dk/wizard/account_move_send_wizard.py` (53 lines)
- `addons/l10n_dk/wizard/nemhandel_registration.py` (283 lines)
- `addons/l10n_dk/wizard/nemhandel_registration_views.xml` (102 lines)
- `addons/l10n_dk/wizard/nemhandel_rejection_wizard.py` (18 lines)
- `addons/l10n_dk/wizard/nemhandel_rejection_wizard_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
