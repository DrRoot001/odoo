# Module: l10n_es

- **Module ID:** MOD-174
- **Path:** `addons/l10n_es`
- **Manifest:** `addons/l10n_es/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Spanish charts of accounts (PGCE 2008).
========================================

    * Defines the following chart of account templates:
        * Spanish general chart of accounts 2008
        * Spanish general chart of accounts 2008 for small and medium companies
        * Spanish general chart of accounts 2008 for associations
    * Defines templates for sale and purchase VAT
    * Defines tax templates
    * Defines fiscal positions for spanish fiscal legislation
    * Defines tax reports mod 111, 115, 130 and 303

5.3: Update taxes starting Q4 2024 according to BOE-A-2024-12944 (Royal Decree 4/2024) https://www.boe.es/buscar/act.php?id=BOE-A-2024-12944


Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 20 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/res_partner_data.xml",
    "data/res_country_group.xml",
    "views/account_move_views.xml",
    "views/account_tax_views.xml",
    "views/res_config_settings_views.xml",
    "data/mod111.xml",
    "data/mod115.xml",
    "data/mod130.xml",
    "data/mod303.xml",
    "data/mod390/mod390_section1.xml",
    "data/mod390/mod390_section2.xml",
    "data/mod390/mod390_section3.xml",
    "data/mod390/mod390_section4.xml",
    "data/mod390/mod390_section5.xml",
    "data/mod390/mod390_section6.xml",
    "data/mod390/mod390_section7.xml",
    "data/mod390/mod390.xml",
    "data/mod420.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_partner.xml"
  ]
}
```

### Representative source files

- `addons/l10n_es/__init__.py` (3 lines)
- `addons/l10n_es/__manifest__.py` (56 lines)
- `addons/l10n_es/data/account.account.tag.csv` (19 lines)
- `addons/l10n_es/data/mod111.xml` (527 lines)
- `addons/l10n_es/data/mod115.xml` (102 lines)
- `addons/l10n_es/data/mod130.xml` (325 lines)
- `addons/l10n_es/data/mod303.xml` (1,099 lines)
- `addons/l10n_es/data/mod390/mod390.xml` (16 lines)
- `addons/l10n_es/data/mod390/mod390_section1.xml` (1,545 lines)
- `addons/l10n_es/data/mod390/mod390_section2.xml` (1,866 lines)
- `addons/l10n_es/data/mod390/mod390_section3.xml` (95 lines)
- `addons/l10n_es/data/mod390/mod390_section4.xml` (147 lines)
- `addons/l10n_es/data/mod390/mod390_section5.xml` (269 lines)
- `addons/l10n_es/data/mod390/mod390_section6.xml` (200 lines)
- `addons/l10n_es/data/mod390/mod390_section7.xml` (864 lines)
- `addons/l10n_es/data/mod420.xml` (438 lines)
- `addons/l10n_es/data/res_country_group.xml` (14 lines)
- `addons/l10n_es/data/res_partner_data.xml` (6 lines)
- `addons/l10n_es/data/template/account.account-es_assec.csv` (62 lines)
- `addons/l10n_es/data/template/account.account-es_common.csv` (642 lines)
- `addons/l10n_es/data/template/account.account-es_coop_full.csv` (107 lines)
- `addons/l10n_es/data/template/account.account-es_coop_pymes.csv` (65 lines)
- `addons/l10n_es/data/template/account.account-es_full.csv` (110 lines)
- `addons/l10n_es/data/template/account.account-es_pymes.csv` (10 lines)
- `addons/l10n_es/data/template/account.depreciation.model-es_common.csv` (7 lines)
- `addons/l10n_es/data/template/account.fiscal.position-es_common.csv` (39 lines)
- `addons/l10n_es/data/template/account.tax-es_common.csv` (1,071 lines)
- `addons/l10n_es/data/template/account.tax.group-es_common.csv` (50 lines)
- `addons/l10n_es/demo/demo_company.xml` (56 lines)
- `addons/l10n_es/demo/demo_partner.xml` (28 lines)
- `addons/l10n_es/i18n/es.po` (737 lines)
- `addons/l10n_es/i18n/l10n_es.pot` (685 lines)
- `addons/l10n_es/migrations/5.3/end-migrate_update_taxes.py` (26 lines)
- `addons/l10n_es/migrations/5.4/end-migrate.py` (7 lines)
- `addons/l10n_es/models/__init__.py` (12 lines)
- `addons/l10n_es/models/account_move.py` (215 lines)
- `addons/l10n_es/models/account_tax.py` (163 lines)
- `addons/l10n_es/models/res_company.py` (131 lines)
- `addons/l10n_es/models/res_config_settings.py` (31 lines)
- `addons/l10n_es/models/res_partner.py` (188 lines)
- `addons/l10n_es/models/template_es_assec.py` (27 lines)
- `addons/l10n_es/models/template_es_common.py` (134 lines)
- `addons/l10n_es/models/template_es_coop_full.py` (26 lines)
- `addons/l10n_es/models/template_es_coop_pymes.py` (26 lines)
- `addons/l10n_es/models/template_es_full.py` (36 lines)
- `addons/l10n_es/models/template_es_pymes.py` (28 lines)
- `addons/l10n_es/tests/__init__.py` (1 lines)
- `addons/l10n_es/tests/test_res_partner.py` (163 lines)
- `addons/l10n_es/upgrades/15.0.5.0/post-61-tag-split-2021.py` (76 lines)
- `addons/l10n_es/views/account_move_views.xml` (35 lines)
- `addons/l10n_es/views/account_tax_views.xml` (29 lines)
- `addons/l10n_es/views/res_config_settings_views.xml` (40 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
