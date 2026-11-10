# Module: l10n_gt

- **Module ID:** MOD-212
- **Path:** `addons/l10n_gt`
- **Manifest:** `addons/l10n_gt/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Guatemala.
=====================================================================

Agrega una nomenclatura contable para Guatemala. También icluye impuestos y
la moneda del Quetzal. -- Adds accounting chart for Guatemala. It also includes
taxes and the Quetzal currency.

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "account"
  ],
  "data": [
    "data/res.city.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_gt/__init__.py` (3 lines)
- `addons/l10n_gt/__manifest__.py` (26 lines)
- `addons/l10n_gt/data/res.city.csv` (332 lines)
- `addons/l10n_gt/data/template/account.account-gt.csv` (90 lines)
- `addons/l10n_gt/data/template/account.depreciation.model-gt.csv` (6 lines)
- `addons/l10n_gt/data/template/account.tax-gt.csv` (17 lines)
- `addons/l10n_gt/data/template/account.tax.group-gt.csv` (4 lines)
- `addons/l10n_gt/demo/demo_company.xml` (36 lines)
- `addons/l10n_gt/i18n/es_419.po` (84 lines)
- `addons/l10n_gt/i18n/l10n_gt.pot` (72 lines)
- `addons/l10n_gt/models/__init__.py` (3 lines)
- `addons/l10n_gt/models/res_partner.py` (19 lines)
- `addons/l10n_gt/models/template_gt.py` (58 lines)
- `addons/l10n_gt/tools/__init__.py` (2 lines)
- `addons/l10n_gt/tools/partner_identifiers.py` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
