# Module: l10n_fi_sale

- **Module ID:** MOD-188
- **Path:** `addons/l10n_fi_sale`
- **Manifest:** `addons/l10n_fi_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Finland Sale

Declared dependencies: `l10n_fi`, `sale`.

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
    "l10n_fi",
    "sale"
  ]
}
```

### Representative source files

- `addons/l10n_fi_sale/__init__.py` (4 lines)
- `addons/l10n_fi_sale/__manifest__.py` (14 lines)
- `addons/l10n_fi_sale/i18n/fi.po` (52 lines)
- `addons/l10n_fi_sale/i18n/l10n_fi_sale.pot` (47 lines)
- `addons/l10n_fi_sale/models/__init__.py` (4 lines)
- `addons/l10n_fi_sale/models/sale.py` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
