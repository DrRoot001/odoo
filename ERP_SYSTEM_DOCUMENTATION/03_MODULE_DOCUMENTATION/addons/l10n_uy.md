# Module: l10n_uy

- **Module ID:** MOD-338
- **Path:** `addons/l10n_uy`
- **Manifest:** `addons/l10n_uy/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


General Chart of Accounts.
==========================

This module adds accounting functionalities for the Uruguayan localization, representing the minimum required configuration for a company to operate in Uruguay under the regulations and guidelines provided by the DGI (Dirección General Impositiva).

Among the functionalities are:

* Uruguayan Generic Chart of Account
* Pre-configured VAT Taxes and Tax Groups.
* Legal document types in Uruguay.
* Valid contact identification types in Uruguay.
* Configuration and activation of Uruguayan Currencies  (UYU, UYI - Unidad Indexada Uruguaya).
* Frequently used default contacts already configured: DGI, Consumidor Final Uruguayo.

Configuration
-------------

Demo data for testing:

* Uruguayan company named "UY Company" with the Uruguayan chart of accounts already installed, pre configured taxes, document types and identification types.
* Uruguayan contacts for testing:

   * IEB Internacional
   * Consumidor Final Anónimo Uruguayo.



Declared dependencies: `account`, `l10n_latam_invoice_document`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_latam_invoice_document"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/l10n_latam.document.type.csv",
    "data/res_partner_data.xml",
    "data/res_currency_data.xml",
    "views/account_tax_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/res_partner_demo.xml",
    "demo/res_currency_rate_demo.xml",
    "demo/account_customer_refund_demo.xml",
    "demo/account_supplier_refund_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_uy/__init__.py` (5 lines)
- `addons/l10n_uy/__manifest__.py` (57 lines)
- `addons/l10n_uy/data/account_tax_report_data.xml` (305 lines)
- `addons/l10n_uy/data/l10n_latam.document.type.csv` (52 lines)
- `addons/l10n_uy/data/res_currency_data.xml` (8 lines)
- `addons/l10n_uy/data/res_partner_data.xml` (9 lines)
- `addons/l10n_uy/data/template/account.account-uy.csv` (168 lines)
- `addons/l10n_uy/data/template/account.depreciation.model-uy.csv` (6 lines)
- `addons/l10n_uy/data/template/account.fiscal.position-uy.csv` (3 lines)
- `addons/l10n_uy/data/template/account.tax-uy.csv` (49 lines)
- `addons/l10n_uy/data/template/account.tax.group-uy.csv` (5 lines)
- `addons/l10n_uy/demo/__init__.py` (3 lines)
- `addons/l10n_uy/demo/account_customer_refund_demo.xml` (47 lines)
- `addons/l10n_uy/demo/account_demo.py` (412 lines)
- `addons/l10n_uy/demo/account_supplier_refund_demo.xml` (40 lines)
- `addons/l10n_uy/demo/demo_company.xml` (36 lines)
- `addons/l10n_uy/demo/res_currency_rate_demo.xml` (11 lines)
- `addons/l10n_uy/demo/res_partner_demo.xml` (12 lines)
- `addons/l10n_uy/i18n/es_419.po` (318 lines)
- `addons/l10n_uy/i18n/l10n_uy.pot` (231 lines)
- `addons/l10n_uy/models/__init__.py` (7 lines)
- `addons/l10n_uy/models/account_move.py` (49 lines)
- `addons/l10n_uy/models/account_tax.py` (10 lines)
- `addons/l10n_uy/models/l10n_latam_document_type.py` (35 lines)
- `addons/l10n_uy/models/res_company.py` (11 lines)
- `addons/l10n_uy/models/res_partner.py` (25 lines)
- `addons/l10n_uy/models/template_uy.py` (73 lines)
- `addons/l10n_uy/tests/__init__.py` (2 lines)
- `addons/l10n_uy/tests/test_check_vat.py` (65 lines)
- `addons/l10n_uy/tests/test_doc_types.py` (66 lines)
- `addons/l10n_uy/tools/__init__.py` (2 lines)
- `addons/l10n_uy/tools/partner_identifiers.py` (75 lines)
- `addons/l10n_uy/views/account_tax_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
