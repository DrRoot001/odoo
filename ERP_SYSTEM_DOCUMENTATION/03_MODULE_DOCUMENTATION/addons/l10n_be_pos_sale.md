# Module: l10n_be_pos_sale

- **Module ID:** MOD-131
- **Path:** `addons/l10n_be_pos_sale`
- **Manifest:** `addons/l10n_be_pos_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between pos_sale and l10n_be

No manifest description declared.

Declared dependencies: `pos_sale`, `l10n_be`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_sale",
    "l10n_be"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_be_pos_sale/static/src/js/**/*"
    ],
    "web.assets_tests": [
      "l10n_be_pos_sale/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_be_pos_sale/__init__.py` (3 lines)
- `addons/l10n_be_pos_sale/__manifest__.py` (21 lines)
- `addons/l10n_be_pos_sale/i18n/de.po` (64 lines)
- `addons/l10n_be_pos_sale/i18n/fr.po` (64 lines)
- `addons/l10n_be_pos_sale/i18n/l10n_be_pos_sale.pot` (56 lines)
- `addons/l10n_be_pos_sale/i18n/nl.po` (64 lines)
- `addons/l10n_be_pos_sale/models/__init__.py` (1 lines)
- `addons/l10n_be_pos_sale/models/pos_config.py` (14 lines)
- `addons/l10n_be_pos_sale/static/src/js/PaymentScreen.js` (43 lines)
- `addons/l10n_be_pos_sale/static/tests/tours/l10n_be_pos_sale_tour.js` (58 lines)
- `addons/l10n_be_pos_sale/tests/__init__.py` (3 lines)
- `addons/l10n_be_pos_sale/tests/test_l10n_be_pos_sale.py` (126 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
