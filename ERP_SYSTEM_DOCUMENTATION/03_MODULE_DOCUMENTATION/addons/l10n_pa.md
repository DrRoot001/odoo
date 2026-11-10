# Module: l10n_pa

- **Module ID:** MOD-289
- **Path:** `addons/l10n_pa`
- **Manifest:** `addons/l10n_pa/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Panamenian accounting chart and tax localization.

Plan contable panameño e impuestos de acuerdo a disposiciones vigentes

Con la Colaboración de
- AHMNET CORP http://www.ahmnet.com

    

Declared dependencies: `account`, `base_address_extended`, `contacts`, `l10n_latam_invoice_document`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "base_address_extended",
    "contacts",
    "l10n_latam_invoice_document"
  ],
  "data": [
    "views/res_partner_views.xml",
    "views/res_company_views.xml",
    "views/res_city_views.xml",
    "views/res_city_corregimiento_views.xml",
    "data/res_country_data.xml",
    "data/l10n_latam.document.type.csv",
    "data/res.city.csv",
    "data/l10n_pa.res.city.corregimiento.csv",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_partner.xml",
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_pa/__init__.py` (4 lines)
- `addons/l10n_pa/__manifest__.py` (41 lines)
- `addons/l10n_pa/data/l10n_latam.document.type.csv` (10 lines)
- `addons/l10n_pa/data/l10n_pa.res.city.corregimiento.csv` (648 lines)
- `addons/l10n_pa/data/res.city.csv` (80 lines)
- `addons/l10n_pa/data/res_country_data.xml` (9 lines)
- `addons/l10n_pa/data/template/account.account-pa.csv` (148 lines)
- `addons/l10n_pa/data/template/account.depreciation.model-pa.csv` (5 lines)
- `addons/l10n_pa/data/template/account.fiscal.position-pa.csv` (4 lines)
- `addons/l10n_pa/data/template/account.tax-pa.csv` (61 lines)
- `addons/l10n_pa/data/template/account.tax.group-pa.csv` (9 lines)
- `addons/l10n_pa/demo/__init__.py` (2 lines)
- `addons/l10n_pa/demo/account_demo.py` (31 lines)
- `addons/l10n_pa/demo/demo_company.xml` (38 lines)
- `addons/l10n_pa/demo/demo_partner.xml` (48 lines)
- `addons/l10n_pa/i18n/es_419.po` (645 lines)
- `addons/l10n_pa/i18n/l10n_pa.pot` (628 lines)
- `addons/l10n_pa/models/__init__.py` (6 lines)
- `addons/l10n_pa/models/res_city.py` (14 lines)
- `addons/l10n_pa/models/res_city_corregimiento.py` (30 lines)
- `addons/l10n_pa/models/res_company.py` (15 lines)
- `addons/l10n_pa/models/res_partner.py` (46 lines)
- `addons/l10n_pa/models/template_pa.py` (50 lines)
- `addons/l10n_pa/security/ir.access.csv` (3 lines)
- `addons/l10n_pa/tools/__init__.py` (2 lines)
- `addons/l10n_pa/tools/partner_identifiers.py` (14 lines)
- `addons/l10n_pa/views/res_city_corregimiento_views.xml` (75 lines)
- `addons/l10n_pa/views/res_city_views.xml` (17 lines)
- `addons/l10n_pa/views/res_company_views.xml` (22 lines)
- `addons/l10n_pa/views/res_partner_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
