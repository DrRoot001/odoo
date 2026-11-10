# Module: l10n_ar

- **Module ID:** MOD-120
- **Path:** `addons/l10n_ar`
- **Manifest:** `addons/l10n_ar/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Functional
----------

This module add accounting features for the Argentinean localization, which represent the minimal configuration needed for a company  to operate in Argentina and under the ARCA (Administración Federal de Ingresos Públicos) regulations and guidelines.

Follow the next configuration steps for Production:

1. Go to your company and configure your VAT number and ARCA Responsibility Type
2. Go to Accounting / Settings and set the Chart of Account that you will like to use.
3. Create your Sale journals taking into account ARCA POS info.

Demo data for testing:

* 3 companies were created, one for each ARCA responsibility type with the respective Chart of Account installed. Choose the company that fix you in order to make tests:

  * (AR) Responsable Inscripto
  * (AR) Exento
  * (AR) Monotributo

* Journal sales configured to Pre printed and Expo invoices in all companies
* Invoices and other documents examples already validated in “(AR) Responsable Inscripto” company
* Partners example for the different responsibility types:

  * ADHOC (IVA Responsable Inscripto)
  * Servicios Globales (IVA Sujeto Exento)
  * Gritti (Monotributo)
  * Montana Sur. IVA Liberado in Zona Franca
  * Barcelona food (Cliente del Exterior)
  * Odoo (Proveedor del Exterior)

Highlights:

* Chart of account will not be automatically installed, each CoA Template depends on the ARCA Responsibility of the company, you will need to install the CoA for your needs.
* No sales journals will be generated when installing a CoA, you will need to configure your journals manually.
* The Document type will be properly pre selected when creating an invoice depending on the fiscal responsibility of the issuer and receiver of the document and the related journal.
* A CBU account type has been added and also CBU Validation


Technical
---------

This module adds both models and fields that will be eventually used for the electronic invoice module. Here is a summary of the main features:

Master Data:

* Chart of Account: one for each ARCA responsibility that is related to a legal entity:

  * Responsable Inscripto (RI)
  * Exento (EX)
  * Monotributo (Mono)

* Argentinean Taxes and Account Tax Groups (VAT taxes with the existing aliquots and other types)
* ARCA Responsibility Types
* Fiscal Positions (in order to map taxes)
* Legal Documents Types in Argentina
* Identification Types valid in Argentina.
* Country ARCA codes and Country VAT codes for legal entities, natural persons and others
* Currency ARCA codes
* Unit of measures ARCA codes
* Partners: Consumidor Final and ARCA


Declared dependencies: `l10n_latam_invoice_document`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 35 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 21 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 32 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_latam_invoice_document",
    "account"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/l10n_ar_afip_responsibility_type_data.xml",
    "data/l10n_ar.arca.activity.csv",
    "data/account_chart_template_data2.xml",
    "data/uom_uom_data.xml",
    "data/l10n_latam.document.type.csv",
    "data/l10n_latam.document.type.xml",
    "data/res_partner_data.xml",
    "data/res.currency.csv",
    "data/res.country.csv",
    "views/account_move_view.xml",
    "views/account_account_view.xml",
    "views/res_partner_view.xml",
    "views/res_company_view.xml",
    "views/res_country_view.xml",
    "views/afip_menuitem.xml",
    "views/l10n_ar_afip_responsibility_type_view.xml",
    "views/l10n_ar_arca_activity_view.xml",
    "views/res_currency_view.xml",
    "views/account_fiscal_position_view.xml",
    "views/uom_uom_view.xml",
    "views/account_journal_view.xml",
    "views/l10n_latam_document_type_view.xml",
    "views/portal_address_templates.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_view.xml",
    "report/invoice_report_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/exento_demo.xml",
    "demo/mono_demo.xml",
    "demo/respinsc_demo.xml",
    "demo/res_partner_demo.xml",
    "demo/product_product_demo.xml",
    "demo/account_tax_demo.xml",
    "demo/account_customer_invoice_demo.xml",
    "demo/account_customer_refund_demo.xml",
    "demo/account_supplier_invoice_demo.xml",
    "demo/account_supplier_refund_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ar/__init__.py` (7 lines)
- `addons/l10n_ar/__manifest__.py` (120 lines)
- `addons/l10n_ar/controllers/__init__.py` (3 lines)
- `addons/l10n_ar/controllers/portal.py` (59 lines)
- `addons/l10n_ar/data/account.account.tag.csv` (3 lines)
- `addons/l10n_ar/data/account_chart_template_data2.xml` (4 lines)
- `addons/l10n_ar/data/l10n_ar.arca.activity.csv` (959 lines)
- `addons/l10n_ar/data/l10n_ar_afip_responsibility_type_data.xml` (81 lines)
- `addons/l10n_ar/data/l10n_latam.document.type.csv` (147 lines)
- `addons/l10n_ar/data/l10n_latam.document.type.xml` (9 lines)
- `addons/l10n_ar/data/res.country.csv` (229 lines)
- `addons/l10n_ar/data/res.currency.csv` (44 lines)
- `addons/l10n_ar/data/res_partner_data.xml` (21 lines)
- `addons/l10n_ar/data/template/account.account-ar_base.csv` (286 lines)
- `addons/l10n_ar/data/template/account.account-ar_ex.csv` (67 lines)
- `addons/l10n_ar/data/template/account.account-ar_ri.csv` (31 lines)
- `addons/l10n_ar/data/template/account.depreciation.model-ar_base.csv` (5 lines)
- `addons/l10n_ar/data/template/account.fiscal.position-ar_ri.csv` (5 lines)
- `addons/l10n_ar/data/template/account.tax-ar_base.csv` (105 lines)
- `addons/l10n_ar/data/template/account.tax-ar_ex.csv` (109 lines)
- `addons/l10n_ar/data/template/account.tax-ar_ri.csv` (89 lines)
- `addons/l10n_ar/data/template/account.tax.group-ar_base.csv` (41 lines)
- `addons/l10n_ar/data/template/account.tax.group-ar_ex.csv` (42 lines)
- `addons/l10n_ar/data/template/account.tax.group-ar_ri.csv` (41 lines)
- `addons/l10n_ar/data/uom_uom_data.xml` (61 lines)
- `addons/l10n_ar/demo/__init__.py` (3 lines)
- `addons/l10n_ar/demo/account_customer_invoice_demo.xml` (278 lines)
- `addons/l10n_ar/demo/account_customer_refund_demo.xml` (34 lines)
- `addons/l10n_ar/demo/account_demo.py` (65 lines)
- `addons/l10n_ar/demo/account_supplier_invoice_demo.xml` (337 lines)
- `addons/l10n_ar/demo/account_supplier_refund_demo.xml` (36 lines)
- `addons/l10n_ar/demo/account_tax_demo.xml` (15 lines)
- `addons/l10n_ar/demo/adhoc_jjs.jpeg` (135 lines)
- `addons/l10n_ar/demo/adhoc_logo.png` (75 lines)
- `addons/l10n_ar/demo/exento_demo.xml` (53 lines)
- `addons/l10n_ar/demo/gritti_logo.png` (97 lines)
- `addons/l10n_ar/demo/mono_demo.xml` (53 lines)
- `addons/l10n_ar/demo/odoo_logo.jpg` (45 lines)
- `addons/l10n_ar/demo/product_product_demo.xml` (135 lines)
- `addons/l10n_ar/demo/res_partner_demo.xml` (136 lines)
- `addons/l10n_ar/demo/respinsc_demo.xml` (69 lines)
- `addons/l10n_ar/i18n/es_419.po` (1,717 lines)
- `addons/l10n_ar/i18n/l10n_ar.pot` (1,471 lines)
- `addons/l10n_ar/models/__init__.py` (21 lines)
- `addons/l10n_ar/models/account_account.py` (14 lines)
- `addons/l10n_ar/models/account_chart_template.py` (57 lines)
- `addons/l10n_ar/models/account_fiscal_position.py` (19 lines)
- `addons/l10n_ar/models/account_journal.py` (191 lines)
- `addons/l10n_ar/models/account_move.py` (572 lines)
- `addons/l10n_ar/models/account_move_line.py` (51 lines)
- `addons/l10n_ar/models/account_tax_group.py` (53 lines)
- `addons/l10n_ar/models/l10n_ar_afip_responsibility_type.py` (18 lines)
- `addons/l10n_ar/models/l10n_ar_arca_activity.py` (30 lines)
- `addons/l10n_ar/models/l10n_latam_document_type.py` (82 lines)
- `addons/l10n_ar/models/res_company.py` (38 lines)
- `addons/l10n_ar/models/res_config_settings.py` (10 lines)
- `addons/l10n_ar/models/res_country.py` (18 lines)
- `addons/l10n_ar/models/res_currency.py` (8 lines)
- `addons/l10n_ar/models/res_partner.py` (180 lines)
- `addons/l10n_ar/models/res_partner_bank.py` (22 lines)
- `addons/l10n_ar/models/template_ar_base.py` (106 lines)
- `addons/l10n_ar/models/template_ar_ex.py` (31 lines)
- `addons/l10n_ar/models/template_ar_ri.py` (33 lines)
- `addons/l10n_ar/models/uom_uom.py` (8 lines)
- `addons/l10n_ar/report/__init__.py` (3 lines)
- `addons/l10n_ar/report/invoice_report.py` (21 lines)
- `addons/l10n_ar/report/invoice_report_view.xml` (47 lines)
- `addons/l10n_ar/security/ir.access.csv` (4 lines)
- `addons/l10n_ar/tests/__init__.py` (4 lines)
- `addons/l10n_ar/tests/common.py` (665 lines)
- `addons/l10n_ar/tests/test_manual.py` (581 lines)
- `addons/l10n_ar/tests/test_res_partner.py` (201 lines)
- `addons/l10n_ar/tools/__init__.py` (2 lines)
- `addons/l10n_ar/tools/partner_identifiers.py` (140 lines)
- `addons/l10n_ar/views/account_account_view.xml` (24 lines)
- `addons/l10n_ar/views/account_fiscal_position_view.xml` (15 lines)
- `addons/l10n_ar/views/account_journal_view.xml` (19 lines)
- `addons/l10n_ar/views/account_move_view.xml` (34 lines)
- `addons/l10n_ar/views/afip_menuitem.xml` (6 lines)
- `addons/l10n_ar/views/l10n_ar_afip_responsibility_type_view.xml` (37 lines)
- `addons/l10n_ar/views/l10n_ar_arca_activity_view.xml` (36 lines)
- `addons/l10n_ar/views/l10n_latam_document_type_view.xml` (51 lines)
- `addons/l10n_ar/views/portal_address_templates.xml` (34 lines)
- `addons/l10n_ar/views/report_invoice.xml` (324 lines)
- `addons/l10n_ar/views/res_company_view.xml` (19 lines)
- `addons/l10n_ar/views/res_config_settings_view.xml` (24 lines)
- `addons/l10n_ar/views/res_country_view.xml` (32 lines)
- `addons/l10n_ar/views/res_currency_view.xml` (15 lines)
- `addons/l10n_ar/views/res_partner_view.xml` (49 lines)
- `addons/l10n_ar/views/uom_uom_view.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
