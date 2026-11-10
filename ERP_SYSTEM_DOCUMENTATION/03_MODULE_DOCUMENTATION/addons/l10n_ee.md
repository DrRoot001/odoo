# Module: l10n_ee

- **Module ID:** MOD-170
- **Path:** `addons/l10n_ee`
- **Manifest:** `addons/l10n_ee/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Estonia in Odoo.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
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
    "data/account_tax_report_data.xml",
    "views/account_tax_form.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ee/__init__.py` (3 lines)
- `addons/l10n_ee/__manifest__.py` (26 lines)
- `addons/l10n_ee/data/account_tax_report_data.xml` (565 lines)
- `addons/l10n_ee/data/template/account.account-ee.csv` (213 lines)
- `addons/l10n_ee/data/template/account.fiscal.position-ee.csv` (11 lines)
- `addons/l10n_ee/data/template/account.tax-ee.csv` (291 lines)
- `addons/l10n_ee/data/template/account.tax.group-ee.csv` (8 lines)
- `addons/l10n_ee/demo/demo_company.xml` (43 lines)
- `addons/l10n_ee/i18n/et.po` (104 lines)
- `addons/l10n_ee/i18n/l10n_ee.pot` (99 lines)
- `addons/l10n_ee/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_ee/migrations/1.2/end-migrate_update_taxes.py` (7 lines)
- `addons/l10n_ee/migrations/1.3/end-migrate_update_data.py` (7 lines)
- `addons/l10n_ee/models/__init__.py` (4 lines)
- `addons/l10n_ee/models/account_tax.py` (17 lines)
- `addons/l10n_ee/models/res_company.py` (8 lines)
- `addons/l10n_ee/models/template_ee.py` (50 lines)
- `addons/l10n_ee/views/account_tax_form.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
