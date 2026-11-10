# Module: l10n_lu

- **Module ID:** MOD-264
- **Path:** `addons/l10n_lu`
- **Manifest:** `addons/l10n_lu/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Luxembourg.
======================================================================

    * the Luxembourg Official Chart of Accounts (law of June 2009 + 2015 chart and Taxes),
    * the Tax Code Chart for Luxembourg
    * the main taxes used in Luxembourg
    * default fiscal position for local, intracom, extracom

Notes:
    * the 2015 chart of taxes is implemented to a large extent,
      see the first sheet of tax.xls for details of coverage
    * to update the chart of tax template, update tax.xls and run tax2csv.py


Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/account.account.tag.csv",
    "data/l10n_lu_chart_data.xml",
    "data/tax_report/section_1.xml",
    "data/tax_report/section_2.xml",
    "data/tax_report/sections_34.xml",
    "data/tax_report/tax_report.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_lu/__init__.py` (11 lines)
- `addons/l10n_lu/__manifest__.py` (42 lines)
- `addons/l10n_lu/data/account.account.tag.csv` (61 lines)
- `addons/l10n_lu/data/l10n_lu_chart_data.xml` (5 lines)
- `addons/l10n_lu/data/tax_report/section_1.xml` (321 lines)
- `addons/l10n_lu/data/tax_report/section_2.xml` (1,755 lines)
- `addons/l10n_lu/data/tax_report/sections_34.xml` (240 lines)
- `addons/l10n_lu/data/tax_report/tax_report.xml` (19 lines)
- `addons/l10n_lu/data/template/account.account-lu.csv` (747 lines)
- `addons/l10n_lu/data/template/account.fiscal.position-lu.csv` (6 lines)
- `addons/l10n_lu/data/template/account.tax-lu.csv` (1,007 lines)
- `addons/l10n_lu/data/template/account.tax.group-lu.csv` (13 lines)
- `addons/l10n_lu/demo/demo_company.xml` (43 lines)
- `addons/l10n_lu/i18n/de.po` (428 lines)
- `addons/l10n_lu/i18n/fr.po` (401 lines)
- `addons/l10n_lu/i18n/l10n_lu.pot` (375 lines)
- `addons/l10n_lu/i18n/lb.po` (393 lines)
- `addons/l10n_lu/migrations/2.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_lu/migrations/2.2/end-migrate_update_taxes.py` (7 lines)
- `addons/l10n_lu/models/__init__.py` (2 lines)
- `addons/l10n_lu/models/template_lu.py` (70 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
