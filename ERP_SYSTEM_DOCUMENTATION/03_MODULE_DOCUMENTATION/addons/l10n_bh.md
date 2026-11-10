# Module: l10n_bh

- **Module ID:** MOD-135
- **Path:** `addons/l10n_bh`
- **Manifest:** `addons/l10n_bh/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Bahrain in Odoo.
===========================================================================
Bahrain accounting basic charts and localization.

Activates:
 - Chart of Accounts
 - Taxes
 - Tax reports
 - Fiscal Positions
 - States
    

Declared dependencies: `account`, `l10n_gcc_invoice`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
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
    "l10n_gcc_invoice"
  ],
  "data": [
    "data/tax_report_full.xml",
    "data/tax_report_simplified.xml",
    "views/report_invoice_templates.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_bh/__init__.py` (1 lines)
- `addons/l10n_bh/__manifest__.py` (33 lines)
- `addons/l10n_bh/data/tax_report_full.xml` (423 lines)
- `addons/l10n_bh/data/tax_report_simplified.xml` (317 lines)
- `addons/l10n_bh/data/template/account.account-bh.csv` (167 lines)
- `addons/l10n_bh/data/template/account.fiscal.position-bh.csv` (4 lines)
- `addons/l10n_bh/data/template/account.tax-bh.csv` (57 lines)
- `addons/l10n_bh/data/template/account.tax.group-bh.csv` (5 lines)
- `addons/l10n_bh/demo/demo_company.xml` (42 lines)
- `addons/l10n_bh/i18n/ar.po` (221 lines)
- `addons/l10n_bh/i18n/l10n_bh.pot` (195 lines)
- `addons/l10n_bh/models/__init__.py` (2 lines)
- `addons/l10n_bh/models/account_move.py` (20 lines)
- `addons/l10n_bh/models/template_bh.py` (39 lines)
- `addons/l10n_bh/tests/__init__.py` (1 lines)
- `addons/l10n_bh/tests/test_account_move.py` (41 lines)
- `addons/l10n_bh/views/report_invoice_templates.xml` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
