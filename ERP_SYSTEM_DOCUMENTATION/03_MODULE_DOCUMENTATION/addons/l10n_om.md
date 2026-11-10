# Module: l10n_om

- **Module ID:** MOD-288
- **Path:** `addons/l10n_om`
- **Manifest:** `addons/l10n_om/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Oman Accounting Module
=================================================================
Oman accounting basic charts and localization.
Activates:
- Chart of Accounts
- Taxes
- VAT Return
- Fiscal Positions
- States


Declared dependencies: `account`, `l10n_gcc_invoice`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
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
    "l10n_gcc_invoice"
  ],
  "data": [
    "data/tax_report.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_om/__init__.py` (1 lines)
- `addons/l10n_om/__manifest__.py` (29 lines)
- `addons/l10n_om/data/tax_report.xml` (363 lines)
- `addons/l10n_om/data/template/account.account-om.csv` (173 lines)
- `addons/l10n_om/data/template/account.fiscal.position-om.csv` (3 lines)
- `addons/l10n_om/data/template/account.tax-om.csv` (57 lines)
- `addons/l10n_om/data/template/account.tax.group-om.csv` (5 lines)
- `addons/l10n_om/demo/demo_company.xml` (35 lines)
- `addons/l10n_om/i18n/ar.po` (56 lines)
- `addons/l10n_om/i18n/l10n_om.pot` (51 lines)
- `addons/l10n_om/models/__init__.py` (1 lines)
- `addons/l10n_om/models/template_om.py` (48 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
