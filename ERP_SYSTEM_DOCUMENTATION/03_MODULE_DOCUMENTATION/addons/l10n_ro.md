# Module: l10n_ro

- **Module ID:** MOD-304
- **Path:** `addons/l10n_ro`
- **Manifest:** `addons/l10n_ro/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the Accounting Chart, VAT structure, Fiscal Position and Tax Mapping.
It also adds the Registration Number for Romania in Odoo.
================================================================================================================

Romanian accounting chart and localization.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
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
    "views/res_partner_view.xml",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ro/__init__.py` (11 lines)
- `addons/l10n_ro/__manifest__.py` (30 lines)
- `addons/l10n_ro/data/account_tax_report_data.xml` (964 lines)
- `addons/l10n_ro/data/template/account.account-ro.csv` (580 lines)
- `addons/l10n_ro/data/template/account.fiscal.position-ro.csv` (10 lines)
- `addons/l10n_ro/data/template/account.tax-ro.csv` (341 lines)
- `addons/l10n_ro/data/template/account.tax.group-ro.csv` (19 lines)
- `addons/l10n_ro/demo/demo_company.xml` (43 lines)
- `addons/l10n_ro/i18n/l10n_ro.pot` (76 lines)
- `addons/l10n_ro/i18n/ro.po` (82 lines)
- `addons/l10n_ro/migrations/1.1/pre-migrate.py` (20 lines)
- `addons/l10n_ro/models/__init__.py` (3 lines)
- `addons/l10n_ro/models/res_partner.py` (20 lines)
- `addons/l10n_ro/models/template_ro.py` (128 lines)
- `addons/l10n_ro/views/res_partner_view.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
