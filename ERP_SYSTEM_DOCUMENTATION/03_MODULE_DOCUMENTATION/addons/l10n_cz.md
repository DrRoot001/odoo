# Module: l10n_cz

- **Module ID:** MOD-156
- **Path:** `addons/l10n_cz`
- **Manifest:** `addons/l10n_cz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Czech accounting chart and localization.  With Chart of Accounts with taxes and basic fiscal positions.

Tento modul definuje:

- Českou účetní osnovu za rok 2020

- Základní sazby pro DPH z prodeje a nákupu

- Základní fiskální pozice pro českou legislativu
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
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
    "views/res_partner_views.xml",
    "data/tax_report.xml",
    "data/l10n_cz.tax_office.csv",
    "data/res_country_data.xml",
    "views/report_invoice.xml",
    "views/res_company_views.xml",
    "views/report_template.xml",
    "views/tax_office_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_cz/__init__.py` (2 lines)
- `addons/l10n_cz/__manifest__.py` (38 lines)
- `addons/l10n_cz/data/l10n_cz.tax_office.csv` (215 lines)
- `addons/l10n_cz/data/res_country_data.xml` (7 lines)
- `addons/l10n_cz/data/tax_report.xml` (995 lines)
- `addons/l10n_cz/data/template/account.account-cz.csv` (323 lines)
- `addons/l10n_cz/data/template/account.depreciation.model-cz.csv` (7 lines)
- `addons/l10n_cz/data/template/account.fiscal.position-cz.csv` (9 lines)
- `addons/l10n_cz/data/template/account.tax-cz.csv` (149 lines)
- `addons/l10n_cz/data/template/account.tax.group-cz.csv` (5 lines)
- `addons/l10n_cz/demo/demo_company.xml` (42 lines)
- `addons/l10n_cz/i18n/cs.po` (1,883 lines)
- `addons/l10n_cz/i18n/l10n_cz.pot` (1,869 lines)
- `addons/l10n_cz/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_cz/models/__init__.py` (6 lines)
- `addons/l10n_cz/models/account_move.py` (27 lines)
- `addons/l10n_cz/models/l10n_cz_tax_office.py` (18 lines)
- `addons/l10n_cz/models/res_bank.py` (67 lines)
- `addons/l10n_cz/models/res_company.py` (97 lines)
- `addons/l10n_cz/models/template_cz.py` (108 lines)
- `addons/l10n_cz/security/ir.access.csv` (3 lines)
- `addons/l10n_cz/tests/__init__.py` (2 lines)
- `addons/l10n_cz/tests/test_cz_qr.py` (97 lines)
- `addons/l10n_cz/tests/test_moves.py` (96 lines)
- `addons/l10n_cz/views/report_invoice.xml` (33 lines)
- `addons/l10n_cz/views/report_template.xml` (25 lines)
- `addons/l10n_cz/views/res_company_views.xml` (23 lines)
- `addons/l10n_cz/views/res_partner_views.xml` (39 lines)
- `addons/l10n_cz/views/tax_office_view.xml` (57 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
