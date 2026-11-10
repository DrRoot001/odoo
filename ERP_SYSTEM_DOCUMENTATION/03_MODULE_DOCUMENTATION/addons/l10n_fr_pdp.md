# Module: l10n_fr_pdp

- **Module ID:** MOD-194
- **Path:** `addons/l10n_fr_pdp`
- **Manifest:** `addons/l10n_fr_pdp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_fr_account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


        - Support for the mandatory electronic invoicing in France
        - Send and receive documents via the Odoo Approved Platform


Declared dependencies: `l10n_fr_account`, `account_peppol`, `iap`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 43 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 18 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 48 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_fr_account",
    "account_peppol",
    "iap"
  ],
  "data": [
    "data/ir_cron.xml",
    "views/account_move_views.xml",
    "views/account_peppol_response_views.xml",
    "views/l10n_fr_account_inherit.xml",
    "views/pdp_flow_views.xml",
    "views/pdp_send_wizard_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "wizard/pdp_registration_views.xml",
    "wizard/pdp_response_wizard_views.xml",
    "wizard/l10n_fr_pdp_partner_lookup.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_fr_pdp/static/src/js/**"
    ]
  }
}
```

### Representative source files

- `addons/l10n_fr_pdp/__init__.py` (40 lines)
- `addons/l10n_fr_pdp/__manifest__.py` (39 lines)
- `addons/l10n_fr_pdp/controllers/__init__.py` (2 lines)
- `addons/l10n_fr_pdp/controllers/routes.py` (45 lines)
- `addons/l10n_fr_pdp/controllers/webhooks.py` (25 lines)
- `addons/l10n_fr_pdp/data/ir_cron.xml` (32 lines)
- `addons/l10n_fr_pdp/i18n/fr.po` (3,164 lines)
- `addons/l10n_fr_pdp/i18n/l10n_fr_pdp.pot` (2,884 lines)
- `addons/l10n_fr_pdp/models/__init__.py` (17 lines)
- `addons/l10n_fr_pdp/models/account_edi_cii.py` (84 lines)
- `addons/l10n_fr_pdp/models/account_edi_common.py` (61 lines)
- `addons/l10n_fr_pdp/models/account_edi_proxy_user.py` (964 lines)
- `addons/l10n_fr_pdp/models/account_edi_ubl.py` (20 lines)
- `addons/l10n_fr_pdp/models/account_edi_xml_cii_facturx.py` (136 lines)
- `addons/l10n_fr_pdp/models/account_edi_xml_ubl_21_fr.py` (299 lines)
- `addons/l10n_fr_pdp/models/account_journal.py` (35 lines)
- `addons/l10n_fr_pdp/models/account_move.py` (747 lines)
- `addons/l10n_fr_pdp/models/account_move_send.py` (106 lines)
- `addons/l10n_fr_pdp/models/account_peppol_response.py` (90 lines)
- `addons/l10n_fr_pdp/models/account_tax.py` (14 lines)
- `addons/l10n_fr_pdp/models/ir_attachment.py` (16 lines)
- `addons/l10n_fr_pdp/models/pdp_flow.py` (637 lines)
- `addons/l10n_fr_pdp/models/pdp_flow_xml_builder.py` (679 lines)
- `addons/l10n_fr_pdp/models/res_company.py` (295 lines)
- `addons/l10n_fr_pdp/models/res_config_settings.py` (62 lines)
- `addons/l10n_fr_pdp/models/res_partner.py` (311 lines)
- `addons/l10n_fr_pdp/security/ir.access.csv` (9 lines)
- `addons/l10n_fr_pdp/static/src/js/pdp_info.js` (33 lines)
- `addons/l10n_fr_pdp/static/src/js/pdp_info.xml` (39 lines)
- `addons/l10n_fr_pdp/static/src/js/status_listener.js` (41 lines)
- `addons/l10n_fr_pdp/static/src/js/status_listener.xml` (4 lines)
- `addons/l10n_fr_pdp/tests/__init__.py` (8 lines)
- `addons/l10n_fr_pdp/tests/common.py` (281 lines)
- `addons/l10n_fr_pdp/tests/data/FACT_REPORT2025_S2F3.xml` (176 lines)
- `addons/l10n_fr_pdp/tests/data/FACT_REPORT2025_S2F4.xml` (176 lines)
- `addons/l10n_fr_pdp/tests/data/FFE1025A_PPF262_PPF2621025000000000000290.xml` (182 lines)
- `addons/l10n_fr_pdp/tests/data/FFE1025A_PPF262_PPF2621025000000000000292.xml` (76 lines)
- `addons/l10n_fr_pdp/tests/data/FFE1025A_PPF262_PPF2621025000000000000294.xml` (76 lines)
- `addons/l10n_fr_pdp/tests/test_cii_export_facturx_fr.py` (160 lines)
- `addons/l10n_fr_pdp/tests/test_cii_import_facturx_fr.py` (79 lines)
- `addons/l10n_fr_pdp/tests/test_files/assets/document` (1 lines)
- `addons/l10n_fr_pdp/tests/test_files/assets/document_factur_x_self_bill` (1 lines)
- `addons/l10n_fr_pdp/tests/test_files/assets/enc_key` (1 lines)
- `addons/l10n_fr_pdp/tests/test_files/assets/private_key.pem` (28 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/facturx_fr_out_downpayment_credit_note.xml` (197 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/facturx_fr_out_downpayment_invoice.xml` (201 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/facturx_fr_out_final_invoice.xml` (273 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/test_invoice_narration.xml` (177 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/test_invoice_narration_early_payment_discount.xml` (182 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/test_invoice_profile_id_goods.xml` (177 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/test_invoice_profile_id_mixed.xml` (201 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/facturx/invoice/fr/test_invoice_profile_id_services.xml` (177 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_credit_note.xml` (193 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_downpayment_credit_note.xml` (182 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_downpayment_invoice.xml` (179 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_final_invoice.xml` (237 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_invoice.xml` (193 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_invoice_b2g.xml` (195 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_invoice_rounding.xml` (168 lines)
- `addons/l10n_fr_pdp/tests/test_files/export/ubl_21_fr/invoice/fr/ubl_21_fr_out_no_vat_invoice.xml` (194 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_downpayment_credit_note.xml` (205 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_downpayment_invoice.xml` (209 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_final_invoice_copied_lines.xml` (281 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_final_invoice_prepaid_amount.xml` (223 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_partial_invoice_line_charges_price_details.xml` (35 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/facturx/invoice/fr/facturx_fr_in_partial_invoice_line_wrong_unit_price.xml` (24 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_downpayment_credit_note.xml` (193 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_downpayment_invoice.xml` (175 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_final_invoice_copied_lines.xml` (235 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_final_invoice_prepaid_amount.xml` (187 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_invoice_establishment.xml` (111 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_partial_invoice_en16931_customization_id.xml` (11 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_partial_invoice_line_charges_price_details.xml` (19 lines)
- `addons/l10n_fr_pdp/tests/test_files/import/ubl_21_fr/invoice/fr/ubl_21_fr_in_partial_invoice_line_wrong_unit_price.xml` (10 lines)
- `addons/l10n_fr_pdp/tests/test_flow_lifecycle.py` (3,069 lines)
- `addons/l10n_fr_pdp/tests/test_messages.py` (1,003 lines)
- `addons/l10n_fr_pdp/tests/test_partner.py` (398 lines)
- `addons/l10n_fr_pdp/tests/test_user.py` (243 lines)
- `addons/l10n_fr_pdp/tests/test_xml_ubl_21_fr.py` (245 lines)
- `addons/l10n_fr_pdp/tools/__init__.py` (1 lines)
- `addons/l10n_fr_pdp/tools/demo_utils.py` (110 lines)
- `addons/l10n_fr_pdp/utils/__init__.py` (2 lines)
- `addons/l10n_fr_pdp/utils/cdar.py` (26 lines)
- `addons/l10n_fr_pdp/utils/drom_com_territories.py` (148 lines)
- `addons/l10n_fr_pdp/views/account_move_views.xml` (301 lines)
- `addons/l10n_fr_pdp/views/account_peppol_response_views.xml` (34 lines)
- `addons/l10n_fr_pdp/views/l10n_fr_account_inherit.xml` (8 lines)
- `addons/l10n_fr_pdp/views/pdp_flow_views.xml` (154 lines)
- `addons/l10n_fr_pdp/views/pdp_send_wizard_views.xml` (31 lines)
- `addons/l10n_fr_pdp/views/res_config_settings_views.xml` (161 lines)
- `addons/l10n_fr_pdp/views/res_partner_views.xml` (29 lines)
- `addons/l10n_fr_pdp/wizard/__init__.py` (5 lines)
- `addons/l10n_fr_pdp/wizard/account_move_send_wizard.py` (81 lines)
- `addons/l10n_fr_pdp/wizard/l10n_fr_pdp_partner_lookup.py` (42 lines)
- `addons/l10n_fr_pdp/wizard/l10n_fr_pdp_partner_lookup.xml` (32 lines)
- `addons/l10n_fr_pdp/wizard/pdp_registration.py` (401 lines)
- `addons/l10n_fr_pdp/wizard/pdp_registration_views.xml` (101 lines)
- `addons/l10n_fr_pdp/wizard/pdp_response_wizard.py` (330 lines)
- `addons/l10n_fr_pdp/wizard/pdp_response_wizard_views.xml` (28 lines)
- `addons/l10n_fr_pdp/wizard/pdp_send_wizard.py` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
