# Module: account_peppol

- **Module ID:** MOD-011
- **Path:** `addons/account_peppol`
- **Manifest:** `addons/account_peppol/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account_edi_ubl_cii']`
- **License:** `LGPL-3`

## Purpose and dependencies

This module is used to send/receive documents with Peppol


- Register as a Peppol participant
- Send and receive documents via Peppol network in Peppol BIS Billing 3.0 format
    

Declared dependencies: `account_edi_proxy_client`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 37 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_proxy_client",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/cron.xml",
    "data/mail_templates_email_layouts.xml",
    "data/peppol_clarification_data.xml",
    "data/res_partner_data.xml",
    "views/account_move_views.xml",
    "views/account_peppol_response_views.xml",
    "views/account_portal_templates.xml",
    "views/peppol_authentication_views.xml",
    "views/res_partner_views.xml",
    "views/res_config_settings_views.xml",
    "wizard/peppol_registration_views.xml",
    "wizard/peppol_rejection_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/account_peppol_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "account_peppol/static/src/components/**/*",
      "account_peppol/static/src/web/**/*",
      "account_peppol/static/src/css/**/*"
    ],
    "web.assets_frontend": [
      "account_peppol/static/src/interactions/*"
    ]
  },
  "external_dependencies": {
    "python": [
      "phonenumbers"
    ],
    "apt": {
      "phonenumbers": "python3-phonenumbers"
    }
  }
}
```

### Representative source files

- `addons/account_peppol/__init__.py` (11 lines)
- `addons/account_peppol/__manifest__.py` (60 lines)
- `addons/account_peppol/controllers/__init__.py` (3 lines)
- `addons/account_peppol/controllers/authentication.py` (83 lines)
- `addons/account_peppol/controllers/portal.py` (76 lines)
- `addons/account_peppol/controllers/webhooks.py` (62 lines)
- `addons/account_peppol/data/cron.xml` (48 lines)
- `addons/account_peppol/data/mail_templates_email_layouts.xml` (109 lines)
- `addons/account_peppol/data/neutralize.sql` (4 lines)
- `addons/account_peppol/data/peppol_clarification_data.xml` (155 lines)
- `addons/account_peppol/data/res_partner_data.xml` (4 lines)
- `addons/account_peppol/demo/account_peppol_demo.xml` (7 lines)
- `addons/account_peppol/exceptions.py` (174 lines)
- `addons/account_peppol/i18n/account_peppol.pot` (2,654 lines)
- `addons/account_peppol/i18n/ar.po` (3,215 lines)
- `addons/account_peppol/i18n/az.po` (2,694 lines)
- `addons/account_peppol/i18n/bg.po` (2,695 lines)
- `addons/account_peppol/i18n/bs.po` (2,696 lines)
- `addons/account_peppol/i18n/ca.po` (2,949 lines)
- `addons/account_peppol/i18n/cs.po` (3,113 lines)
- `addons/account_peppol/i18n/da.po` (3,126 lines)
- `addons/account_peppol/i18n/de.po` (3,309 lines)
- `addons/account_peppol/i18n/el.po` (2,695 lines)
- `addons/account_peppol/i18n/es.po` (3,144 lines)
- `addons/account_peppol/i18n/es_419.po` (3,268 lines)
- `addons/account_peppol/i18n/et.po` (2,707 lines)
- `addons/account_peppol/i18n/fa.po` (2,727 lines)
- `addons/account_peppol/i18n/fi.po` (3,227 lines)
- `addons/account_peppol/i18n/fr.po` (3,266 lines)
- `addons/account_peppol/i18n/he.po` (2,695 lines)
- `addons/account_peppol/i18n/hi.po` (3,029 lines)
- `addons/account_peppol/i18n/hr.po` (2,695 lines)
- `addons/account_peppol/i18n/hu.po` (2,695 lines)
- `addons/account_peppol/i18n/id.po` (3,078 lines)
- `addons/account_peppol/i18n/it.po` (3,271 lines)
- `addons/account_peppol/i18n/ja.po` (3,200 lines)
- `addons/account_peppol/i18n/kab.po` (2,695 lines)
- `addons/account_peppol/i18n/ko.po` (3,026 lines)
- `addons/account_peppol/i18n/ku.po` (2,703 lines)
- `addons/account_peppol/i18n/lo.po` (3,019 lines)
- `addons/account_peppol/i18n/lt.po` (2,696 lines)
- `addons/account_peppol/i18n/lv.po` (2,699 lines)
- `addons/account_peppol/i18n/mn.po` (2,694 lines)
- `addons/account_peppol/i18n/my.po` (2,695 lines)
- `addons/account_peppol/i18n/nb.po` (2,695 lines)
- `addons/account_peppol/i18n/nl.po` (3,263 lines)
- `addons/account_peppol/i18n/pl.po` (3,191 lines)
- `addons/account_peppol/i18n/pt.po` (3,055 lines)
- `addons/account_peppol/i18n/pt_BR.po` (3,253 lines)
- `addons/account_peppol/i18n/ro.po` (3,094 lines)
- `addons/account_peppol/i18n/ru.po` (3,161 lines)
- `addons/account_peppol/i18n/sk.po` (2,695 lines)
- `addons/account_peppol/i18n/sl.po` (2,776 lines)
- `addons/account_peppol/i18n/sr@latin.po` (2,695 lines)
- `addons/account_peppol/i18n/sv.po` (3,251 lines)
- `addons/account_peppol/i18n/th.po` (2,969 lines)
- `addons/account_peppol/i18n/tr.po` (3,204 lines)
- `addons/account_peppol/i18n/uk.po` (2,780 lines)
- `addons/account_peppol/i18n/uz.po` (3,281 lines)
- `addons/account_peppol/i18n/vi.po` (3,068 lines)
- `addons/account_peppol/i18n/zh_CN.po` (3,064 lines)
- `addons/account_peppol/i18n/zh_TW.po` (2,980 lines)
- `addons/account_peppol/models/__init__.py` (11 lines)
- `addons/account_peppol/models/account_edi_common.py` (18 lines)
- `addons/account_peppol/models/account_edi_proxy_user.py` (902 lines)
- `addons/account_peppol/models/account_edi_ubl_xml.py` (16 lines)
- `addons/account_peppol/models/account_journal.py` (82 lines)
- `addons/account_peppol/models/account_move.py` (205 lines)
- `addons/account_peppol/models/account_move_send.py` (388 lines)
- `addons/account_peppol/models/account_peppol_clarification.py` (15 lines)
- `addons/account_peppol/models/account_peppol_response.py` (33 lines)
- `addons/account_peppol/models/res_company.py` (358 lines)
- `addons/account_peppol/models/res_config_settings.py` (183 lines)
- `addons/account_peppol/models/res_partner.py` (318 lines)
- `addons/account_peppol/security/ir.access.csv` (6 lines)
- `addons/account_peppol/static/img/itsme.svg` (11 lines)
- `addons/account_peppol/static/src/components/peppol_auth/peppol_auth_callback_action.js` (15 lines)
- `addons/account_peppol/static/src/components/peppol_auth/peppol_auth_service.js` (43 lines)
- `addons/account_peppol/static/src/components/peppol_filterable_selection/peppol_non_focusable_selection.js` (21 lines)
- `addons/account_peppol/static/src/components/peppol_filterable_selection/peppol_non_focusable_selection.xml` (16 lines)
- `addons/account_peppol/static/src/components/peppol_info/peppol_info.js` (44 lines)
- `addons/account_peppol/static/src/components/peppol_info/peppol_info.xml` (39 lines)
- `addons/account_peppol/static/src/css/account_peppol.scss` (12 lines)
- `addons/account_peppol/static/src/interactions/invoice_sending_method.js` (28 lines)
- `addons/account_peppol/static/src/web/account_move_form_controller.js` (65 lines)
- `addons/account_peppol/static/src/web/account_move_list_controller.js` (127 lines)
- `addons/account_peppol/tests/__init__.py` (10 lines)
- `addons/account_peppol/tests/assets/enc_key` (1 lines)
- `addons/account_peppol/tests/assets/incoming_invoice` (1 lines)
- `addons/account_peppol/tests/assets/incoming_self_billed_invoice` (1 lines)
- `addons/account_peppol/tests/assets/peppol_identification_test.pdf` (220 lines)
- `addons/account_peppol/tests/assets/private_key.pem` (28 lines)
- `addons/account_peppol/tests/assets/response_document` (1 lines)
- `addons/account_peppol/tests/common.py` (283 lines)
- `addons/account_peppol/tests/test_account_journal.py` (25 lines)
- `addons/account_peppol/tests/test_account_move.py` (114 lines)
- `addons/account_peppol/tests/test_peppol_kyc.py` (175 lines)
- `addons/account_peppol/tests/test_peppol_messages.py` (1,111 lines)
- `addons/account_peppol/tests/test_peppol_out_of_sync_resolution.py` (45 lines)
- `addons/account_peppol/tests/test_peppol_participant.py` (501 lines)
- `addons/account_peppol/tests/test_ubl_export_bis3_be.py` (45 lines)
- `addons/account_peppol/tools/__init__.py` (4 lines)
- `addons/account_peppol/tools/demo_bill` (1 lines)
- `addons/account_peppol/tools/demo_utils.py` (186 lines)
- `addons/account_peppol/tools/enc_key` (1 lines)
- `addons/account_peppol/tools/peppol_errors.py` (92 lines)
- `addons/account_peppol/tools/peppol_iap_connector.py` (72 lines)
- `addons/account_peppol/tools/private_key.pem` (28 lines)
- `addons/account_peppol/views/account_move_views.xml` (76 lines)
- `addons/account_peppol/views/account_peppol_response_views.xml` (28 lines)
- `addons/account_peppol/views/account_portal_templates.xml` (36 lines)
- `addons/account_peppol/views/peppol_authentication_views.xml` (14 lines)
- `addons/account_peppol/views/res_config_settings_views.xml` (132 lines)
- `addons/account_peppol/views/res_partner_views.xml` (52 lines)
- `addons/account_peppol/wizard/__init__.py` (6 lines)
- `addons/account_peppol/wizard/account_move_send_batch_wizard.py` (14 lines)
- `addons/account_peppol/wizard/account_move_send_wizard.py` (86 lines)
- `addons/account_peppol/wizard/peppol_registration.py` (539 lines)
- `addons/account_peppol/wizard/peppol_registration_views.xml` (89 lines)
- `addons/account_peppol/wizard/peppol_rejection_wizard.py` (43 lines)
- `addons/account_peppol/wizard/peppol_rejection_wizard_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
