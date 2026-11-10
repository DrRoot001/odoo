# Module: l10n_pt

- **Module ID:** MOD-301
- **Path:** `addons/l10n_pt`
- **Manifest:** `addons/l10n_pt/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Portugal - Accounting

Declared dependencies: `base`, `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/account_tax_report.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_pt/static/src/helpers/*.js"
    ],
    "web.assets_frontend": [
      "l10n_pt/static/src/helpers/*.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_pt/__init__.py` (1 lines)
- `addons/l10n_pt/__manifest__.py` (31 lines)
- `addons/l10n_pt/data/account_tax_report.xml` (615 lines)
- `addons/l10n_pt/data/template/account.account-pt.csv` (643 lines)
- `addons/l10n_pt/data/template/account.fiscal.position-pt.csv` (5 lines)
- `addons/l10n_pt/data/template/account.tax-pt.csv` (209 lines)
- `addons/l10n_pt/data/template/account.tax.group-pt.csv` (11 lines)
- `addons/l10n_pt/demo/demo_company.xml` (44 lines)
- `addons/l10n_pt/i18n/l10n_pt.pot` (56 lines)
- `addons/l10n_pt/i18n/pt.po` (60 lines)
- `addons/l10n_pt/models/__init__.py` (3 lines)
- `addons/l10n_pt/models/account_account.py` (7 lines)
- `addons/l10n_pt/models/account_tax.py` (21 lines)
- `addons/l10n_pt/models/template_pt.py` (55 lines)
- `addons/l10n_pt/static/src/helpers/account_tax.js` (27 lines)
- `addons/l10n_pt/tests/__init__.py` (1 lines)
- `addons/l10n_pt/tests/test_taxes_tax_totals_summary.py` (788 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
