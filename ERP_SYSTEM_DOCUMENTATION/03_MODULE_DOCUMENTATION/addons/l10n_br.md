# Module: l10n_br

- **Module ID:** MOD-139
- **Path:** `addons/l10n_br`
- **Manifest:** `addons/l10n_br/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Base module for the Brazilian localization
==========================================

This module consists of:

- Generic Brazilian chart of accounts
- Brazilian taxes such as:

  - IPI
  - ICMS
  - PIS
  - COFINS
  - ISS
  - IR
  - CSLL

- Document Types as NFC-e, NFS-e, etc.
- Identification Documents as CNPJ and CPF

In addition to this module, the Brazilian Localizations is also
extended and complemented with several additional modules.

Brazil - Accounting Reports (l10n_br_reports)
---------------------------------------------
Adds a simple tax report that helps check the tax amount per tax group
in a given period of time. Also adds the P&L and BS adapted for the
Brazilian market.

Avatax Brazil (l10n_br_avatax)
------------------------------
Add Brazilian tax calculation via Avatax and all necessary fields needed to
configure Odoo in order to properly use Avatax and send the needed fiscal
information to retrieve the correct taxes.

Avatax for SOs in Brazil (l10n_br_avatax_sale)
----------------------------------------------
Same as the l10n_br_avatax module with the extension to the sales order module.

Electronic invoicing through Avatax (l10n_br_edi)
-------------------------------------------------
Create electronic sales invoices with Avatax.


Declared dependencies: `account`, `account_qr_code_emv`, `l10n_latam_invoice_document`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 24 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_qr_code_emv",
    "l10n_latam_invoice_document"
  ],
  "data": [
    "views/res_partner_views.xml",
    "data/account_tax_report_data.xml",
    "data/res_country_data.xml",
    "data/res.city.csv",
    "data/l10n_br.zip.range.csv",
    "data/l10n_latam.document.type.csv",
    "views/account_view.xml",
    "views/account_fiscal_position_views.xml",
    "views/ir_ui_menu_brazil.xml",
    "views/portal_address_templates.xml",
    "views/res_company_views.xml",
    "views/account_journal_views.xml",
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_city_view.xml",
    "views/report_invoice.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_br/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_br/__init__.py` (6 lines)
- `addons/l10n_br/__manifest__.py` (87 lines)
- `addons/l10n_br/data/account_tax_report_data.xml` (1,597 lines)
- `addons/l10n_br/data/l10n_br.zip.range.csv` (5,574 lines)
- `addons/l10n_br/data/l10n_latam.document.type.csv` (32 lines)
- `addons/l10n_br/data/res.city.csv` (5,571 lines)
- `addons/l10n_br/data/res_country_data.xml` (9 lines)
- `addons/l10n_br/data/template/account.account-br.csv` (1,201 lines)
- `addons/l10n_br/data/template/account.depreciation.model-br.csv` (7 lines)
- `addons/l10n_br/data/template/account.fiscal.position-br.csv` (7 lines)
- `addons/l10n_br/data/template/account.tax-br.csv` (1,293 lines)
- `addons/l10n_br/data/template/account.tax.group-br.csv` (161 lines)
- `addons/l10n_br/demo/__init__.py` (1 lines)
- `addons/l10n_br/demo/account_demo.py` (21 lines)
- `addons/l10n_br/demo/demo_company.xml` (41 lines)
- `addons/l10n_br/i18n/l10n_br.pot` (1,191 lines)
- `addons/l10n_br/i18n/pt_BR.po` (1,262 lines)
- `addons/l10n_br/migrations/1.1/end-migrate-update_taxes.py` (8 lines)
- `addons/l10n_br/models/__init__.py` (12 lines)
- `addons/l10n_br/models/account.py` (16 lines)
- `addons/l10n_br/models/account_fiscal_position.py` (44 lines)
- `addons/l10n_br/models/account_journal.py` (19 lines)
- `addons/l10n_br/models/account_move.py` (47 lines)
- `addons/l10n_br/models/l10n_br_zip_range.py` (41 lines)
- `addons/l10n_br/models/res_city.py` (26 lines)
- `addons/l10n_br/models/res_company.py` (16 lines)
- `addons/l10n_br/models/res_country.py` (14 lines)
- `addons/l10n_br/models/res_partner.py` (38 lines)
- `addons/l10n_br/models/res_partner_bank.py` (144 lines)
- `addons/l10n_br/models/template_br.py` (94 lines)
- `addons/l10n_br/security/ir.access.csv` (3 lines)
- `addons/l10n_br/static/src/interactions/address.js` (98 lines)
- `addons/l10n_br/tests/__init__.py` (4 lines)
- `addons/l10n_br/tests/test_l10n_br_fiscal_position.py` (48 lines)
- `addons/l10n_br/tests/test_l10n_br_pix.py` (112 lines)
- `addons/l10n_br/tools/__init__.py` (2 lines)
- `addons/l10n_br/tools/partner_identifiers.py` (17 lines)
- `addons/l10n_br/views/account_fiscal_position_views.xml` (15 lines)
- `addons/l10n_br/views/account_journal_views.xml` (15 lines)
- `addons/l10n_br/views/account_view.xml` (17 lines)
- `addons/l10n_br/views/ir_ui_menu_brazil.xml` (8 lines)
- `addons/l10n_br/views/portal_address_templates.xml` (69 lines)
- `addons/l10n_br/views/report_invoice.xml` (30 lines)
- `addons/l10n_br/views/res_bank_views.xml` (15 lines)
- `addons/l10n_br/views/res_city_view.xml` (18 lines)
- `addons/l10n_br/views/res_company_views.xml` (15 lines)
- `addons/l10n_br/views/res_config_settings_views.xml` (22 lines)
- `addons/l10n_br/views/res_partner_views.xml` (71 lines)
- `addons/l10n_br/wizard/__init__.py` (2 lines)
- `addons/l10n_br/wizard/account_move_reversal.py` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
