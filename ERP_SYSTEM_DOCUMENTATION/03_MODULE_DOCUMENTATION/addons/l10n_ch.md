# Module: l10n_ch

- **Module ID:** MOD-146
- **Path:** `addons/l10n_ch`
- **Manifest:** `addons/l10n_ch/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Swiss localization
==================
This module defines a chart of account for Switzerland (Swiss PME/KMU 2015), taxes and enables the generation of a QR-bill when you print an invoice or send it by mail.
The QR bill is attached to the invoice and eases its payment.

A QR-bill will be generated if:
    - The partner set on your invoice has a complete address (street, city, postal code and country) in Switzerland
    - The option to generate the Swiss QR-code is selected on the invoice (done by default)
    - A correct account number/QR IBAN is set on your bank journal
    - (when using a QR-IBAN): the payment reference of the invoice is a QR-reference

The generation of the QR-bill is automatic if you meet the previous criteria. The QR-bill will be appended after the invoice when printing or sending by mail.

    

Declared dependencies: `account`, `account_edi_ubl_cii`, `l10n_din5008`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 25 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii",
    "l10n_din5008"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "report/swissqr_report.xml",
    "views/res_bank_view.xml",
    "views/account_invoice.xml",
    "views/setup_wizard_views.xml",
    "views/qr_invoice_wizard_view.xml",
    "views/account_payment_view.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/account_cash_rounding.xml",
    "demo/demo_company.xml",
    "demo/res_partner_demo.xml"
  ],
  "assets": {
    "web.report_assets_common": [
      "l10n_ch/static/src/scss/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ch/__init__.py` (23 lines)
- `addons/l10n_ch/__manifest__.py` (55 lines)
- `addons/l10n_ch/data/account_tax_report_data.xml` (605 lines)
- `addons/l10n_ch/data/template/account.account-ch.csv` (241 lines)
- `addons/l10n_ch/data/template/account.asset-ch.csv` (21 lines)
- `addons/l10n_ch/data/template/account.fiscal.position-ch.csv` (3 lines)
- `addons/l10n_ch/data/template/account.tax-ch.csv` (71 lines)
- `addons/l10n_ch/data/template/account.tax.group-ch.csv` (9 lines)
- `addons/l10n_ch/demo/account_cash_rounding.xml` (10 lines)
- `addons/l10n_ch/demo/demo_company.xml` (43 lines)
- `addons/l10n_ch/demo/res_partner_demo.xml` (20 lines)
- `addons/l10n_ch/i18n/de.po` (567 lines)
- `addons/l10n_ch/i18n/fr.po` (535 lines)
- `addons/l10n_ch/i18n/it.po` (555 lines)
- `addons/l10n_ch/i18n/l10n_ch.pot` (484 lines)
- `addons/l10n_ch/migrations/0.0.0/pre-migrate-qr-template.py` (20 lines)
- `addons/l10n_ch/migrations/11.1/end-migrate_update_taxes.py` (21 lines)
- `addons/l10n_ch/migrations/11.2/pre-migrate.py` (13 lines)
- `addons/l10n_ch/migrations/11.3/end-migrate.py` (8 lines)
- `addons/l10n_ch/migrations/9.0.9.0/pre-set_tags_and_taxes_updatable.py` (9 lines)
- `addons/l10n_ch/models/__init__.py` (8 lines)
- `addons/l10n_ch/models/account_invoice.py` (119 lines)
- `addons/l10n_ch/models/account_journal.py` (25 lines)
- `addons/l10n_ch/models/account_move_send.py` (46 lines)
- `addons/l10n_ch/models/account_payment.py` (37 lines)
- `addons/l10n_ch/models/ir_actions_report.py` (82 lines)
- `addons/l10n_ch/models/res_bank.py` (293 lines)
- `addons/l10n_ch/models/template_ch.py` (51 lines)
- `addons/l10n_ch/report/__init__.py` (3 lines)
- `addons/l10n_ch/report/swissqr_report.py` (22 lines)
- `addons/l10n_ch/report/swissqr_report.xml` (235 lines)
- `addons/l10n_ch/security/ir.access.csv` (2 lines)
- `addons/l10n_ch/static/src/font/LiberationSans-Bold.woff` (1,474 lines)
- `addons/l10n_ch/static/src/font/LiberationSans-Regular.woff` (1,409 lines)
- `addons/l10n_ch/static/src/font/liberation_sans_license.txt` (102 lines)
- `addons/l10n_ch/static/src/font/ocrb-license.txt` (4 lines)
- `addons/l10n_ch/static/src/font/ocrb.otf` (93 lines)
- `addons/l10n_ch/static/src/img/CH-Cross_7mm.png` (166 lines)
- `addons/l10n_ch/static/src/img/background_virgin_isr.png` (163 lines)
- `addons/l10n_ch/static/src/img/background_virgin_isr_bank.png` (187 lines)
- `addons/l10n_ch/static/src/img/scissors_h.png` (15 lines)
- `addons/l10n_ch/static/src/img/scissors_v.png` (83 lines)
- `addons/l10n_ch/static/src/scss/report_swissqr.scss` (193 lines)
- `addons/l10n_ch/tests/__init__.py` (7 lines)
- `addons/l10n_ch/tests/test_ch_qr_code.py` (132 lines)
- `addons/l10n_ch/tests/test_gen_qrr_reference.py` (103 lines)
- `addons/l10n_ch/tests/test_l10n_ch_qr_print.py` (335 lines)
- `addons/l10n_ch/tests/test_swissqr.py` (234 lines)
- `addons/l10n_ch/views/account_invoice.xml` (14 lines)
- `addons/l10n_ch/views/account_payment_view.xml` (17 lines)
- `addons/l10n_ch/views/qr_invoice_wizard_view.xml` (33 lines)
- `addons/l10n_ch/views/res_bank_view.xml` (15 lines)
- `addons/l10n_ch/views/res_config_settings_views.xml` (23 lines)
- `addons/l10n_ch/views/setup_wizard_views.xml` (15 lines)
- `addons/l10n_ch/wizard/__init__.py` (4 lines)
- `addons/l10n_ch/wizard/qr_invoice_wizard.py` (92 lines)
- `addons/l10n_ch/wizard/setup_wizards.py` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
