# Module: l10n_be_pos_restaurant

- **Module ID:** MOD-130
- **Path:** `addons/l10n_be_pos_restaurant`
- **Manifest:** `addons/l10n_be_pos_restaurant/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `pos_restaurant`, `l10n_be`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "pos_restaurant",
    "l10n_be"
  ]
}
```

### Representative source files

- `addons/l10n_be_pos_restaurant/__init__.py` (2 lines)
- `addons/l10n_be_pos_restaurant/__manifest__.py` (9 lines)
- `addons/l10n_be_pos_restaurant/data/template/account.tax-be.csv` (5 lines)
- `addons/l10n_be_pos_restaurant/i18n/de.po` (48 lines)
- `addons/l10n_be_pos_restaurant/i18n/fr.po` (47 lines)
- `addons/l10n_be_pos_restaurant/i18n/l10n_be_pos_restaurant.pot` (43 lines)
- `addons/l10n_be_pos_restaurant/i18n/nl.po` (47 lines)
- `addons/l10n_be_pos_restaurant/models/__init__.py` (3 lines)
- `addons/l10n_be_pos_restaurant/models/pos_config.py` (60 lines)
- `addons/l10n_be_pos_restaurant/models/template_be.py` (17 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
