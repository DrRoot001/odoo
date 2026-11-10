# Module: l10n_it

- **Module ID:** MOD-240
- **Path:** `addons/l10n_it`
- **Manifest:** `addons/l10n_it/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Piano dei conti italiano di un'impresa generica.
================================================

Italian accounting chart and localization.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
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
    "data/account_account_tag.xml",
    "data/tax_report/annual_report_sections/va.xml",
    "data/tax_report/annual_report_sections/ve.xml",
    "data/tax_report/annual_report_sections/vf.xml",
    "data/tax_report/annual_report_sections/vh.xml",
    "data/tax_report/annual_report_sections/vj.xml",
    "data/tax_report/annual_report_sections/vl.xml",
    "data/tax_report/account_annual_tax_report_data.xml",
    "data/tax_report/account_monthly_tax_report_data.xml",
    "data/tax_report/account_withholding_report_data.xml",
    "views/account_tax_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_it/__init__.py` (4 lines)
- `addons/l10n_it/__manifest__.py` (36 lines)
- `addons/l10n_it/data/account_account_tag.xml` (92 lines)
- `addons/l10n_it/data/tax_report/account_annual_tax_report_data.xml` (20 lines)
- `addons/l10n_it/data/tax_report/account_monthly_tax_report_data.xml` (326 lines)
- `addons/l10n_it/data/tax_report/account_withholding_report_data.xml` (66 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/va.xml` (147 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/ve.xml` (531 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/vf.xml` (899 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/vh.xml` (130 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/vj.xml` (142 lines)
- `addons/l10n_it/data/tax_report/annual_report_sections/vl.xml` (327 lines)
- `addons/l10n_it/data/template/account.account-it.csv` (190 lines)
- `addons/l10n_it/data/template/account.fiscal.position-it.csv` (7 lines)
- `addons/l10n_it/data/template/account.tax-it.csv` (531 lines)
- `addons/l10n_it/data/template/account.tax.group-it.csv` (15 lines)
- `addons/l10n_it/demo/__init__.py` (1 lines)
- `addons/l10n_it/demo/account_demo.py` (254 lines)
- `addons/l10n_it/demo/demo_company.xml` (43 lines)
- `addons/l10n_it/i18n/it.po` (229 lines)
- `addons/l10n_it/i18n/l10n_it.pot` (207 lines)
- `addons/l10n_it/migrations/0.10/pre-remove-report-expression.py` (10 lines)
- `addons/l10n_it/migrations/0.11/post-update_sp_taxes.py` (29 lines)
- `addons/l10n_it/migrations/0.6/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_it/migrations/0.7/post-map_carryover_to_new_report.py` (84 lines)
- `addons/l10n_it/migrations/0.9/post-migrate.py` (11 lines)
- `addons/l10n_it/migrations/15.0.0.3/post-migrate.py` (17 lines)
- `addons/l10n_it/models/__init__.py` (5 lines)
- `addons/l10n_it/models/account_move.py` (12 lines)
- `addons/l10n_it/models/account_report.py` (19 lines)
- `addons/l10n_it/models/account_tax.py` (75 lines)
- `addons/l10n_it/models/template_it.py` (45 lines)
- `addons/l10n_it/views/account_tax_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
