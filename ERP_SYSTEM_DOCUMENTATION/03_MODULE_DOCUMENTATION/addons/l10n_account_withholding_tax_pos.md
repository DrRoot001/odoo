# Module: l10n_account_withholding_tax_pos

- **Module ID:** MOD-116
- **Path:** `addons/l10n_account_withholding_tax_pos`
- **Manifest:** `addons/l10n_account_withholding_tax_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Add support for the withholding tax module in the PoS.

Declared dependencies: `l10n_account_withholding_tax`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_account_withholding_tax",
    "point_of_sale"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_account_withholding_tax/static/src/helpers/*.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_account_withholding_tax_pos/__init__.py` (3 lines)
- `addons/l10n_account_withholding_tax_pos/__manifest__.py` (15 lines)
- `addons/l10n_account_withholding_tax_pos/models/__init__.py` (3 lines)
- `addons/l10n_account_withholding_tax_pos/models/account_tax.py` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
