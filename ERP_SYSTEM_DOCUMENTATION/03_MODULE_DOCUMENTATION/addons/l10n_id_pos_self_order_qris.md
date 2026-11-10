# Module: l10n_id_pos_self_order_qris

- **Module ID:** MOD-224
- **Path:** `addons/l10n_id_pos_self_order_qris`
- **Manifest:** `addons/l10n_id_pos_self_order_qris/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Accept QRIS QR code payments in a kiosk.

No manifest description declared.

Declared dependencies: `pos_self_order`, `l10n_id_pos`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "pos_self_order",
    "l10n_id_pos"
  ],
  "assets": {
    "pos_self_order.assets": [
      "point_of_sale/static/lib/qrcode.js",
      "l10n_id_pos_self_order_qris/static/src/payment/payment_qris.js",
      "l10n_id_pos_self_order_qris/static/src/payment/payment_page.js",
      "l10n_id_pos_self_order_qris/static/src/payment/payment_page.xml"
    ]
  }
}
```

### Representative source files

- `addons/l10n_id_pos_self_order_qris/__init__.py` (3 lines)
- `addons/l10n_id_pos_self_order_qris/__manifest__.py` (20 lines)
- `addons/l10n_id_pos_self_order_qris/i18n/id.po` (85 lines)
- `addons/l10n_id_pos_self_order_qris/i18n/l10n_id_pos_self_order_qris.pot` (79 lines)
- `addons/l10n_id_pos_self_order_qris/models/__init__.py` (3 lines)
- `addons/l10n_id_pos_self_order_qris/models/pos_payment_method.py` (224 lines)
- `addons/l10n_id_pos_self_order_qris/static/src/payment/payment_page.js` (114 lines)
- `addons/l10n_id_pos_self_order_qris/static/src/payment/payment_page.xml` (18 lines)
- `addons/l10n_id_pos_self_order_qris/static/src/payment/payment_qris.js` (126 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
