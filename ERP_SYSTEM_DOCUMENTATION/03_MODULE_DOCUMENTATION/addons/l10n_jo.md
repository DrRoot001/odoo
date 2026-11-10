# Module: l10n_jo

- **Module ID:** MOD-245
- **Path:** `addons/l10n_jo`
- **Manifest:** `addons/l10n_jo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Jordan in Odoo.
==============================================================================

Jordan accounting basic charts and localization.

Activates:

- Chart of accounts

- Taxes

- Tax report

- Fiscal positions
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "account"
  ],
  "data": [
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml",
    "demo/demo_partner.xml"
  ]
}
```

### Representative source files

- `addons/l10n_jo/__init__.py` (1 lines)
- `addons/l10n_jo/__manifest__.py` (35 lines)
- `addons/l10n_jo/data/account_tax_report_data.xml` (678 lines)
- `addons/l10n_jo/data/template/account.account-jo_standard.csv` (170 lines)
- `addons/l10n_jo/data/template/account.fiscal.position-jo_standard.csv` (3 lines)
- `addons/l10n_jo/data/template/account.tax-jo_standard.csv` (117 lines)
- `addons/l10n_jo/data/template/account.tax.group-jo_standard.csv` (6 lines)
- `addons/l10n_jo/demo/demo_company.xml` (34 lines)
- `addons/l10n_jo/demo/demo_partner.xml` (16 lines)
- `addons/l10n_jo/i18n/ar.po` (112 lines)
- `addons/l10n_jo/i18n/l10n_jo.pot` (107 lines)
- `addons/l10n_jo/models/__init__.py` (2 lines)
- `addons/l10n_jo/models/template_jo_standard.py` (59 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
