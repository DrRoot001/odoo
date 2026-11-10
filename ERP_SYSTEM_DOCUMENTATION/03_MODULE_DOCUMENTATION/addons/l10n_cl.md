# Module: l10n_cl

- **Module ID:** MOD-149
- **Path:** `addons/l10n_cl`
- **Manifest:** `addons/l10n_cl/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chilean accounting chart and tax localization.
Plan contable chileno e impuestos de acuerdo a disposiciones vigentes.
    

Declared dependencies: `contacts`, `l10n_latam_invoice_document`, `uom`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 20 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 17 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "contacts",
    "l10n_latam_invoice_document",
    "uom",
    "account"
  ],
  "data": [
    "views/account_move_view.xml",
    "views/account_tax_view.xml",
    "views/res_country_view.xml",
    "views/res_company_view.xml",
    "views/report_invoice.xml",
    "views/res_partner.xml",
    "views/res_config_settings_view.xml",
    "data/l10n_cl_chart_data.xml",
    "data/account_tax_report_data.xml",
    "data/account_tax_tags_data.xml",
    "data/l10n_latam.document.type.csv",
    "data/product_data.xml",
    "data/uom_data.xml",
    "data/res.city.csv",
    "data/res.country.csv",
    "data/res.currency.csv",
    "data/res_country.xml",
    "data/res_currency_data.xml",
    "data/res_partner.xml"
  ],
  "demo": [
    "demo/partner_demo.xml",
    "demo/company_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_cl/__init__.py` (5 lines)
- `addons/l10n_cl/__manifest__.py` (47 lines)
- `addons/l10n_cl/data/account_tax_report_data.xml` (374 lines)
- `addons/l10n_cl/data/account_tax_tags_data.xml` (266 lines)
- `addons/l10n_cl/data/l10n_cl_chart_data.xml` (142 lines)
- `addons/l10n_cl/data/l10n_latam.document.type.csv` (59 lines)
- `addons/l10n_cl/data/product_data.xml` (24 lines)
- `addons/l10n_cl/data/res.city.csv` (347 lines)
- `addons/l10n_cl/data/res.country.csv` (168 lines)
- `addons/l10n_cl/data/res.currency.csv` (28 lines)
- `addons/l10n_cl/data/res_country.xml` (7 lines)
- `addons/l10n_cl/data/res_currency_data.xml` (34 lines)
- `addons/l10n_cl/data/res_partner.xml` (29 lines)
- `addons/l10n_cl/data/template/account.account-cl.csv` (212 lines)
- `addons/l10n_cl/data/template/account.depreciation.model-cl.csv` (5 lines)
- `addons/l10n_cl/data/template/account.fiscal.position-cl.csv` (26 lines)
- `addons/l10n_cl/data/template/account.tax-cl.csv` (109 lines)
- `addons/l10n_cl/data/template/account.tax.group-cl.csv` (6 lines)
- `addons/l10n_cl/data/uom_data.xml` (28 lines)
- `addons/l10n_cl/demo/__init__.py` (3 lines)
- `addons/l10n_cl/demo/account_demo.py` (440 lines)
- `addons/l10n_cl/demo/bmya_icon.png` (78 lines)
- `addons/l10n_cl/demo/company_demo.xml` (37 lines)
- `addons/l10n_cl/demo/partner_demo.xml` (120 lines)
- `addons/l10n_cl/i18n/es_419.po` (2,356 lines)
- `addons/l10n_cl/i18n/l10n_cl.pot` (2,296 lines)
- `addons/l10n_cl/migrations/3.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_cl/models/__init__.py` (11 lines)
- `addons/l10n_cl/models/account_move.py` (296 lines)
- `addons/l10n_cl/models/account_move_line.py` (142 lines)
- `addons/l10n_cl/models/account_tax.py` (9 lines)
- `addons/l10n_cl/models/l10n_latam_document_type.py` (43 lines)
- `addons/l10n_cl/models/res_company.py` (15 lines)
- `addons/l10n_cl/models/res_country.py` (11 lines)
- `addons/l10n_cl/models/res_currency.py` (9 lines)
- `addons/l10n_cl/models/res_partner.py` (37 lines)
- `addons/l10n_cl/models/template_cl.py` (69 lines)
- `addons/l10n_cl/models/uom_uom.py` (9 lines)
- `addons/l10n_cl/static/sii_logo.jpeg` (41 lines)
- `addons/l10n_cl/static/tgr_logo.png` (39 lines)
- `addons/l10n_cl/tests/__init__.py` (1 lines)
- `addons/l10n_cl/tests/test_latam_document_type.py` (112 lines)
- `addons/l10n_cl/tools/__init__.py` (2 lines)
- `addons/l10n_cl/tools/partner_identifiers.py` (18 lines)
- `addons/l10n_cl/views/account_move_view.xml` (79 lines)
- `addons/l10n_cl/views/account_tax_view.xml` (26 lines)
- `addons/l10n_cl/views/report_invoice.xml` (267 lines)
- `addons/l10n_cl/views/res_company_view.xml` (17 lines)
- `addons/l10n_cl/views/res_config_settings_view.xml` (17 lines)
- `addons/l10n_cl/views/res_country_view.xml` (29 lines)
- `addons/l10n_cl/views/res_partner.xml` (57 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
