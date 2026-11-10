# Module: l10n_be_pos

- **Module ID:** MOD-129
- **Path:** `addons/l10n_be_pos`
- **Manifest:** `addons/l10n_be_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between point_of_sale and l10n_be

No manifest description declared.

Declared dependencies: `point_of_sale`, `l10n_be`, `account`.

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
    "point_of_sale",
    "l10n_be",
    "account"
  ]
}
```

### Representative source files

- `addons/l10n_be_pos/__init__.py` (4 lines)
- `addons/l10n_be_pos/__manifest__.py` (13 lines)
- `addons/l10n_be_pos/i18n/de.po` (45 lines)
- `addons/l10n_be_pos/i18n/fr.po` (45 lines)
- `addons/l10n_be_pos/i18n/l10n_be_pos.pot` (41 lines)
- `addons/l10n_be_pos/i18n/nl.po` (45 lines)
- `addons/l10n_be_pos/models/__init__.py` (3 lines)
- `addons/l10n_be_pos/models/pos_config.py` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
