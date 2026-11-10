# Module: l10n_in_boe

- **Module ID:** MOD-228
- **Path:** `addons/l10n_in_boe`
- **Manifest:** `addons/l10n_in_boe/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


- Adds Bill of Entry (BOE) support for the Indian localization.
- This Allows users to record import BOE details, link stock receipts, create BOE journal entries, and account for custom duties using landed costs.


Declared dependencies: `l10n_in`, `stock_landed_costs`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in",
    "stock_landed_costs"
  ],
  "data": [
    "views/account_move_views.xml",
    "wizard/l10n_in_boe_wizard.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_in_boe/__init__.py` (2 lines)
- `addons/l10n_in_boe/__manifest__.py` (20 lines)
- `addons/l10n_in_boe/i18n/hi.po` (295 lines)
- `addons/l10n_in_boe/i18n/l10n_in_boe.pot` (295 lines)
- `addons/l10n_in_boe/models/__init__.py` (1 lines)
- `addons/l10n_in_boe/models/account_move.py` (21 lines)
- `addons/l10n_in_boe/security/ir.access.csv` (3 lines)
- `addons/l10n_in_boe/tests/__init__.py` (1 lines)
- `addons/l10n_in_boe/tests/test_l10n_in_boe_flow.py` (112 lines)
- `addons/l10n_in_boe/views/account_move_views.xml` (29 lines)
- `addons/l10n_in_boe/wizard/__init__.py` (1 lines)
- `addons/l10n_in_boe/wizard/l10n_in_boe_wizard.py` (309 lines)
- `addons/l10n_in_boe/wizard/l10n_in_boe_wizard.xml` (71 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
