# Module: l10n_hn

- **Module ID:** MOD-215
- **Path:** `addons/l10n_hn`
- **Manifest:** `addons/l10n_hn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Honduras.
====================================================================

Agrega una nomenclatura contable para Honduras. También incluye impuestos y la
moneda Lempira. -- Adds accounting chart for Honduras. It also includes taxes
and the Lempira currency.

Declared dependencies: `base`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
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
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_hn/__init__.py` (2 lines)
- `addons/l10n_hn/__manifest__.py` (26 lines)
- `addons/l10n_hn/data/template/account.account-hn.csv` (35 lines)
- `addons/l10n_hn/data/template/account.tax-hn.csv` (9 lines)
- `addons/l10n_hn/data/template/account.tax.group-hn.csv` (2 lines)
- `addons/l10n_hn/demo/demo_company.xml` (36 lines)
- `addons/l10n_hn/i18n/es_419.po` (62 lines)
- `addons/l10n_hn/i18n/l10n_hn.pot` (48 lines)
- `addons/l10n_hn/models/__init__.py` (2 lines)
- `addons/l10n_hn/models/template_hn.py` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
