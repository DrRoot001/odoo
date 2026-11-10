# Module: l10n_fr_pdp_pos

- **Module ID:** MOD-196
- **Path:** `addons/l10n_fr_pdp_pos`
- **Manifest:** `addons/l10n_fr_pdp_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Flux 10 e-reporting for POS

No manifest description declared.

Declared dependencies: `l10n_fr_pdp`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_fr_pdp",
    "point_of_sale"
  ]
}
```

### Representative source files

- `addons/l10n_fr_pdp_pos/__init__.py` (1 lines)
- `addons/l10n_fr_pdp_pos/__manifest__.py` (9 lines)
- `addons/l10n_fr_pdp_pos/i18n/fr.po` (52 lines)
- `addons/l10n_fr_pdp_pos/i18n/l10n_fr_pdp_pos.pot` (48 lines)
- `addons/l10n_fr_pdp_pos/models/__init__.py` (2 lines)
- `addons/l10n_fr_pdp_pos/models/account_move.py` (24 lines)
- `addons/l10n_fr_pdp_pos/models/res_company.py` (28 lines)
- `addons/l10n_fr_pdp_pos/tests/__init__.py` (1 lines)
- `addons/l10n_fr_pdp_pos/tests/test_pos_flow_lifecycle.py` (358 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
