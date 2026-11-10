# Module: l10n_id_pos

- **Module ID:** MOD-223
- **Path:** `addons/l10n_id_pos`
- **Manifest:** `addons/l10n_id_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Indonesian Point of Sale

Declared dependencies: `l10n_id`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_id",
    "point_of_sale"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_id_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_id_pos/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_id_pos/__init__.py` (2 lines)
- `addons/l10n_id_pos/__manifest__.py` (22 lines)
- `addons/l10n_id_pos/i18n/id.po` (107 lines)
- `addons/l10n_id_pos/i18n/l10n_id_pos.pot` (102 lines)
- `addons/l10n_id_pos/models/__init__.py` (4 lines)
- `addons/l10n_id_pos/models/pos_order.py` (10 lines)
- `addons/l10n_id_pos/models/pos_payment_method.py` (21 lines)
- `addons/l10n_id_pos/models/qris_transaction.py` (15 lines)
- `addons/l10n_id_pos/static/src/app/components/popups/qr_code_popup.js` (67 lines)
- `addons/l10n_id_pos/static/src/app/models/pos_payment.js` (20 lines)
- `addons/l10n_id_pos/static/src/app/services/pos_store.js` (11 lines)
- `addons/l10n_id_pos/static/tests/test_pos_qris_payment.tour.js` (87 lines)
- `addons/l10n_id_pos/tests/__init__.py` (1 lines)
- `addons/l10n_id_pos/tests/test_qris_pos.py` (261 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
