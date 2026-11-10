# Module: l10n_hr

- **Module ID:** MOD-216
- **Path:** `addons/l10n_hr`
- **Manifest:** `addons/l10n_hr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Croatian Chart of Accounts updated (RRIF ver.2021)

Sources:
https://www.rrif.hr/dok/preuzimanje/Bilanca-2016.pdf
https://www.rrif.hr/dok/preuzimanje/RRIF-RP2021.PDF
https://www.rrif.hr/dok/preuzimanje/RRIF-RP2021-ENG.PDF
    

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
    "data/l10n_hr_chart_data.xml",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_hr/__init__.py` (2 lines)
- `addons/l10n_hr/__manifest__.py` (30 lines)
- `addons/l10n_hr/data/account_tax_report_data.xml` (848 lines)
- `addons/l10n_hr/data/l10n_hr_chart_data.xml` (7 lines)
- `addons/l10n_hr/data/template/account.account-hr.csv` (555 lines)
- `addons/l10n_hr/data/template/account.fiscal.position-hr.csv` (6 lines)
- `addons/l10n_hr/data/template/account.tax-hr.csv` (143 lines)
- `addons/l10n_hr/data/template/account.tax.group-hr.csv` (5 lines)
- `addons/l10n_hr/demo/demo_company.xml` (54 lines)
- `addons/l10n_hr/i18n/hr.po` (58 lines)
- `addons/l10n_hr/i18n/l10n_hr.pot` (53 lines)
- `addons/l10n_hr/models/__init__.py` (2 lines)
- `addons/l10n_hr/models/template_hr.py` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
