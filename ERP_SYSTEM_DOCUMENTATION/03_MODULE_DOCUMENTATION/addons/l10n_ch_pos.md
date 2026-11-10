# Module: l10n_ch_pos

- **Module ID:** MOD-147
- **Path:** `addons/l10n_ch_pos`
- **Manifest:** `addons/l10n_ch_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Swiss POS Localization
=======================================================
    

Declared dependencies: `l10n_ch`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ch",
    "point_of_sale"
  ]
}
```

### Representative source files

- `addons/l10n_ch_pos/__init__.py` (3 lines)
- `addons/l10n_ch_pos/__manifest__.py` (13 lines)
- `addons/l10n_ch_pos/i18n/de.po` (52 lines)
- `addons/l10n_ch_pos/i18n/fr.po` (49 lines)
- `addons/l10n_ch_pos/i18n/it.po` (52 lines)
- `addons/l10n_ch_pos/i18n/l10n_ch_pos.pot` (44 lines)
- `addons/l10n_ch_pos/models/__init__.py` (3 lines)
- `addons/l10n_ch_pos/models/pos_order.py` (14 lines)
- `addons/l10n_ch_pos/tests/__init__.py` (4 lines)
- `addons/l10n_ch_pos/tests/test_ch_pos.py` (14 lines)
- `addons/l10n_ch_pos/tests/test_frontend.py` (67 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
