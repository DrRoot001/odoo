# Module: l10n_ma

- **Module ID:** MOD-266
- **Path:** `addons/l10n_ma`
- **Manifest:** `addons/l10n_ma/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Morocco.

This module has been built with the help of Caudigef.


Declared dependencies: `base`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
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
    "base",
    "account"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "views/portal_address_templates.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ma/__init__.py` (3 lines)
- `addons/l10n_ma/__manifest__.py` (27 lines)
- `addons/l10n_ma/controllers/__init__.py` (3 lines)
- `addons/l10n_ma/controllers/portal.py` (33 lines)
- `addons/l10n_ma/data/account_tax_report_data.xml` (1,992 lines)
- `addons/l10n_ma/data/template/account.account-ma.csv` (635 lines)
- `addons/l10n_ma/data/template/account.depreciation.model-ma.csv` (5 lines)
- `addons/l10n_ma/data/template/account.fiscal.position-ma.csv` (9 lines)
- `addons/l10n_ma/data/template/account.tax-ma.csv` (319 lines)
- `addons/l10n_ma/data/template/account.tax.group-ma.csv` (6 lines)
- `addons/l10n_ma/demo/demo_company.xml` (35 lines)
- `addons/l10n_ma/i18n/ar.po` (94 lines)
- `addons/l10n_ma/i18n/fr.po` (110 lines)
- `addons/l10n_ma/i18n/l10n_ma.pot` (82 lines)
- `addons/l10n_ma/models/__init__.py` (4 lines)
- `addons/l10n_ma/models/account_journal.py` (13 lines)
- `addons/l10n_ma/models/base_document_layout.py` (20 lines)
- `addons/l10n_ma/models/template_ma.py` (85 lines)
- `addons/l10n_ma/views/portal_address_templates.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
