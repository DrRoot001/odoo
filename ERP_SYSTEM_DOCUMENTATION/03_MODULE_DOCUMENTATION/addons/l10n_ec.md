# Module: l10n_ec

- **Module ID:** MOD-168
- **Path:** `addons/l10n_ec`
- **Manifest:** `addons/l10n_ec/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Functional
----------

This module adds accounting features for Ecuadorian localization, which
represent the minimum requirements to operate a business in Ecuador in compliance
with local regulation bodies such as the ecuadorian tax authority -SRI- and the
Superintendency of Companies -Super Intendencia de Compañías-

Follow the next configuration steps:
1. Go to your company and configure your country as Ecuador
2. Install the invoicing or accounting module, everything will be handled automatically

Highlights:
* Ecuadorian chart of accounts will be automatically installed, based on example provided by Super Intendencia de Compañías
* List of taxes (including withholds) will also be installed, you can switch off the ones your company doesn't use
* Fiscal position, document types, list of local banks, list of local states, etc, will also be installed

Technical
---------
Master Data:
* Chart of Accounts, based on recomendation by Super Cías
* Ecuadorian Taxes, Tax Tags, and Tax Groups
* Ecuadorian Fiscal Positions
* Document types (there are about 41 purchase documents types in Ecuador)
* Identification types
* Ecuador banks
* Partners: Consumidor Final, SRI, IESS, and also basic VAT validation


Declared dependencies: `base`, `account_debit_note`, `l10n_latam_invoice_document`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "account_debit_note",
    "l10n_latam_invoice_document",
    "account"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/res_partner_data.xml",
    "data/l10n_latam.document.type.csv",
    "data/l10n_ec.sri.payment.csv",
    "views/root_sri_menu.xml",
    "views/account_tax_view.xml",
    "views/l10n_latam_document_type_view.xml",
    "views/l10n_ec_sri_payment.xml",
    "views/account_journal_view.xml",
    "views/res_partner_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ec/__init__.py` (5 lines)
- `addons/l10n_ec/__manifest__.py` (64 lines)
- `addons/l10n_ec/data/account_tax_report_data.xml` (3,846 lines)
- `addons/l10n_ec/data/l10n_ec.sri.payment.csv` (9 lines)
- `addons/l10n_ec/data/l10n_latam.document.type.csv` (38 lines)
- `addons/l10n_ec/data/res_partner_data.xml` (26 lines)
- `addons/l10n_ec/data/template/account.account-ec.csv` (615 lines)
- `addons/l10n_ec/data/template/account.depreciation.model-ec.csv` (8 lines)
- `addons/l10n_ec/data/template/account.fiscal.position-ec.csv` (3 lines)
- `addons/l10n_ec/data/template/account.tax-ec.csv` (729 lines)
- `addons/l10n_ec/data/template/account.tax.group-ec.csv` (18 lines)
- `addons/l10n_ec/demo/__init__.py` (1 lines)
- `addons/l10n_ec/demo/account_demo.py` (25 lines)
- `addons/l10n_ec/demo/demo_company.xml` (36 lines)
- `addons/l10n_ec/i18n/es_419.po` (627 lines)
- `addons/l10n_ec/i18n/l10n_ec.pot` (544 lines)
- `addons/l10n_ec/models/__init__.py` (10 lines)
- `addons/l10n_ec/models/account_journal.py` (34 lines)
- `addons/l10n_ec/models/account_move.py` (204 lines)
- `addons/l10n_ec/models/account_tax.py` (21 lines)
- `addons/l10n_ec/models/account_tax_group.py` (32 lines)
- `addons/l10n_ec/models/l10n_ec_sri_payment.py` (16 lines)
- `addons/l10n_ec/models/l10n_latam_document_type.py` (40 lines)
- `addons/l10n_ec/models/res_company.py` (11 lines)
- `addons/l10n_ec/models/res_partner.py` (83 lines)
- `addons/l10n_ec/models/template_ec.py` (100 lines)
- `addons/l10n_ec/security/ir.access.csv` (4 lines)
- `addons/l10n_ec/static/img/logo_iess.png` (84 lines)
- `addons/l10n_ec/static/img/logo_sri.png` (50 lines)
- `addons/l10n_ec/tests/__init__.py` (2 lines)
- `addons/l10n_ec/tests/test_account_move.py` (43 lines)
- `addons/l10n_ec/tools/__init__.py` (2 lines)
- `addons/l10n_ec/tools/partner_identifiers.py` (17 lines)
- `addons/l10n_ec/views/account_journal_view.xml` (30 lines)
- `addons/l10n_ec/views/account_tax_view.xml` (17 lines)
- `addons/l10n_ec/views/l10n_ec_sri_payment.xml` (45 lines)
- `addons/l10n_ec/views/l10n_latam_document_type_view.xml` (28 lines)
- `addons/l10n_ec/views/res_partner_view.xml` (15 lines)
- `addons/l10n_ec/views/root_sri_menu.xml` (8 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
