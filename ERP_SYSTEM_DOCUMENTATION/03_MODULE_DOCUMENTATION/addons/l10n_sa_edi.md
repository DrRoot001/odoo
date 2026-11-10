# Module: l10n_sa_edi

- **Module ID:** MOD-311
- **Path:** `addons/l10n_sa_edi`
- **Manifest:** `addons/l10n_sa_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

E-Invoicing, Universal Business Language


E-invoice implementation for Saudi Arabia; Integration with ZATCA
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_sa`, `certificate`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 17 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 23 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_sa",
    "certificate"
  ],
  "data": [
    "data/ubl_21_zatca.xml",
    "data/res_country_data.xml",
    "data/transaction_type_data.xml",
    "wizard/l10n_sa_edi_otp_wizard.xml",
    "views/account_tax_views.xml",
    "views/account_journal_views.xml",
    "views/res_company_views.xml",
    "views/res_config_settings_view.xml",
    "views/report_invoice.xml",
    "views/account_move_views.xml",
    "views/portal_address_templates.xml",
    "views/report_templates.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_sa_edi/static/src/interactions/**/*"
    ],
    "web.assets_backend": [
      "l10n_sa_edi/static/src/scss/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_sa_edi/__init__.py` (4 lines)
- `addons/l10n_sa_edi/__manifest__.py` (42 lines)
- `addons/l10n_sa_edi/controllers/__init__.py` (1 lines)
- `addons/l10n_sa_edi/controllers/portal.py` (79 lines)
- `addons/l10n_sa_edi/data/neutralize.sql` (3 lines)
- `addons/l10n_sa_edi/data/pre-hash_invoice.xsl` (19 lines)
- `addons/l10n_sa_edi/data/res_country_data.xml` (38 lines)
- `addons/l10n_sa_edi/data/template/account.tax-sa.csv` (17 lines)
- `addons/l10n_sa_edi/data/transaction_type_data.xml` (16 lines)
- `addons/l10n_sa_edi/data/ubl_21_zatca.xml` (115 lines)
- `addons/l10n_sa_edi/demo/__init__.py` (1 lines)
- `addons/l10n_sa_edi/demo/account_demo.py` (48 lines)
- `addons/l10n_sa_edi/i18n/ar.po` (1,675 lines)
- `addons/l10n_sa_edi/i18n/l10n_sa_edi.pot` (1,547 lines)
- `addons/l10n_sa_edi/migrations/0.3/end-migrate.py` (22 lines)
- `addons/l10n_sa_edi/models/__init__.py` (16 lines)
- `addons/l10n_sa_edi/models/account_chart_template.py` (10 lines)
- `addons/l10n_sa_edi/models/account_edi_xml_ubl_21_zatca.py` (284 lines)
- `addons/l10n_sa_edi/models/account_journal.py` (673 lines)
- `addons/l10n_sa_edi/models/account_move.py` (332 lines)
- `addons/l10n_sa_edi/models/account_move_send.py` (103 lines)
- `addons/l10n_sa_edi/models/account_tax.py` (41 lines)
- `addons/l10n_sa_edi/models/certificate.py` (166 lines)
- `addons/l10n_sa_edi/models/ir_attachment.py` (52 lines)
- `addons/l10n_sa_edi/models/l10n_sa_edi_document.py` (547 lines)
- `addons/l10n_sa_edi/models/l10n_sa_edi_log.py` (32 lines)
- `addons/l10n_sa_edi/models/l10n_sa_edi_transaction_type.py` (17 lines)
- `addons/l10n_sa_edi/models/res_company.py` (78 lines)
- `addons/l10n_sa_edi/models/res_config_settings.py` (19 lines)
- `addons/l10n_sa_edi/models/res_partner.py` (73 lines)
- `addons/l10n_sa_edi/models/zatca_mixin.py` (75 lines)
- `addons/l10n_sa_edi/models/zatca_ubl_mixin.py` (454 lines)
- `addons/l10n_sa_edi/security/ir.access.csv` (7 lines)
- `addons/l10n_sa_edi/static/src/interactions/address.js` (42 lines)
- `addons/l10n_sa_edi/static/src/scss/form_view.scss` (21 lines)
- `addons/l10n_sa_edi/tests/__init__.py` (5 lines)
- `addons/l10n_sa_edi/tests/common.py` (390 lines)
- `addons/l10n_sa_edi/tests/compliance/simplified/credit.xml` (196 lines)
- `addons/l10n_sa_edi/tests/compliance/simplified/debit.xml` (197 lines)
- `addons/l10n_sa_edi/tests/compliance/simplified/invoice.xml` (192 lines)
- `addons/l10n_sa_edi/tests/compliance/standard/credit.xml` (229 lines)
- `addons/l10n_sa_edi/tests/compliance/standard/debit.xml` (230 lines)
- `addons/l10n_sa_edi/tests/compliance/standard/invoice.xml` (223 lines)
- `addons/l10n_sa_edi/tests/test_account_move_send.py` (98 lines)
- `addons/l10n_sa_edi/tests/test_edi_zatca.py` (872 lines)
- `addons/l10n_sa_edi/tests/test_files/downpayment_credit_note.xml` (223 lines)
- `addons/l10n_sa_edi/tests/test_files/downpayment_invoice.xml` (218 lines)
- `addons/l10n_sa_edi/tests/test_files/final_credit_note.xml` (266 lines)
- `addons/l10n_sa_edi/tests/test_files/final_invoice.xml` (261 lines)
- `addons/l10n_sa_edi/tests/test_files/invoice_global_discount.xml` (208 lines)
- `addons/l10n_sa_edi/tests/test_invoice.py` (52 lines)
- `addons/l10n_sa_edi/tests/test_sa_edi_additional_identifiers.py` (26 lines)
- `addons/l10n_sa_edi/views/account_journal_views.xml` (62 lines)
- `addons/l10n_sa_edi/views/account_move_views.xml` (79 lines)
- `addons/l10n_sa_edi/views/account_tax_views.xml` (14 lines)
- `addons/l10n_sa_edi/views/portal_address_templates.xml` (64 lines)
- `addons/l10n_sa_edi/views/report_invoice.xml` (36 lines)
- `addons/l10n_sa_edi/views/report_templates.xml` (8 lines)
- `addons/l10n_sa_edi/views/res_company_views.xml` (24 lines)
- `addons/l10n_sa_edi/views/res_config_settings_view.xml` (43 lines)
- `addons/l10n_sa_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_sa_edi/wizard/l10n_sa_edi_otp_wizard.py` (28 lines)
- `addons/l10n_sa_edi/wizard/l10n_sa_edi_otp_wizard.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
