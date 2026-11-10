# Module: l10n_ae_pos

- **Module ID:** MOD-118
- **Path:** `addons/l10n_ae_pos`
- **Manifest:** `addons/l10n_ae_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


United Arab Emirates POS Localization
===========================================================
    

Declared dependencies: `l10n_gcc_pos`, `l10n_ae`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_gcc_pos",
    "l10n_ae"
  ],
  "data": [
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_ae_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ae_pos/__init__.py` (1 lines)
- `addons/l10n_ae_pos/__manifest__.py` (23 lines)
- `addons/l10n_ae_pos/i18n/ar.po` (49 lines)
- `addons/l10n_ae_pos/i18n/l10n_ae_pos.pot` (44 lines)
- `addons/l10n_ae_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_ae_pos/receipt/pos_order_receipt.py` (12 lines)
- `addons/l10n_ae_pos/receipt/pos_order_receipt.xml` (15 lines)
- `addons/l10n_ae_pos/static/src/overrides/models/pos_order.js` (8 lines)
- `addons/l10n_ae_pos/static/src/overrides/utils/printer/generate_printer_data.js` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
