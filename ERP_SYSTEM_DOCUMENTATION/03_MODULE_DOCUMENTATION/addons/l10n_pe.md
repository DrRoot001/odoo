# Module: l10n_pe

- **Module ID:** MOD-290
- **Path:** `addons/l10n_pe`
- **Manifest:** `addons/l10n_pe/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `l10n_latam_invoice_document`, `account_debit_note`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 20 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_latam_invoice_document",
    "account_debit_note",
    "account"
  ],
  "data": [
    "views/account_tax_view.xml",
    "views/res_city_view.xml",
    "views/portal_address_templates.xml",
    "data/l10n_latam_document_type_data.xml",
    "data/res.city.csv",
    "data/l10n_pe.res.city.district.csv",
    "data/res_country_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_partner.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_pe/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_pe/README.rst` (68 lines)
- `addons/l10n_pe/__init__.py` (6 lines)
- `addons/l10n_pe/__manifest__.py` (36 lines)
- `addons/l10n_pe/controllers/__init__.py` (3 lines)
- `addons/l10n_pe/controllers/portal.py` (39 lines)
- `addons/l10n_pe/data/l10n_latam_document_type_data.xml` (663 lines)
- `addons/l10n_pe/data/l10n_pe.res.city.district.csv` (1,876 lines)
- `addons/l10n_pe/data/res.city.csv` (197 lines)
- `addons/l10n_pe/data/res_country_data.xml` (47 lines)
- `addons/l10n_pe/data/template/account.account-pe.csv` (1,261 lines)
- `addons/l10n_pe/data/template/account.asset-pe.csv` (9 lines)
- `addons/l10n_pe/data/template/account.fiscal.position-pe.csv` (3 lines)
- `addons/l10n_pe/data/template/account.tax-pe.csv` (70 lines)
- `addons/l10n_pe/data/template/account.tax.group-pe.csv` (16 lines)
- `addons/l10n_pe/demo/__init__.py` (1 lines)
- `addons/l10n_pe/demo/account_demo.py` (149 lines)
- `addons/l10n_pe/demo/demo_company.xml` (36 lines)
- `addons/l10n_pe/demo/demo_partner.xml` (9 lines)
- `addons/l10n_pe/i18n/es_419.po` (629 lines)
- `addons/l10n_pe/i18n/l10n_pe.pot` (504 lines)
- `addons/l10n_pe/migrations/3.1/end-migrate_upgrade_taxes.py` (8 lines)
- `addons/l10n_pe/models/__init__.py` (9 lines)
- `addons/l10n_pe/models/account_move.py` (67 lines)
- `addons/l10n_pe/models/account_tax.py` (41 lines)
- `addons/l10n_pe/models/res_city.py` (9 lines)
- `addons/l10n_pe/models/res_city_district.py` (14 lines)
- `addons/l10n_pe/models/res_company.py` (12 lines)
- `addons/l10n_pe/models/res_country.py` (13 lines)
- `addons/l10n_pe/models/res_partner.py` (92 lines)
- `addons/l10n_pe/models/template_pe.py` (60 lines)
- `addons/l10n_pe/security/ir.access.csv` (2 lines)
- `addons/l10n_pe/static/src/interactions/address.js` (19 lines)
- `addons/l10n_pe/tests/__init__.py` (1 lines)
- `addons/l10n_pe/tests/test_l10n_latam_doc_types.py` (127 lines)
- `addons/l10n_pe/tools/__init__.py` (2 lines)
- `addons/l10n_pe/tools/partner_identifiers.py` (89 lines)
- `addons/l10n_pe/views/account_tax_view.xml` (19 lines)
- `addons/l10n_pe/views/portal_address_templates.xml` (32 lines)
- `addons/l10n_pe/views/res_city_view.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
