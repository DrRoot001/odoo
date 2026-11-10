# Module: l10n_sa_pos

- **Module ID:** MOD-313
- **Path:** `addons/l10n_sa_pos`
- **Manifest:** `addons/l10n_sa_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Saudi Arabia POS Localization
===========================================================
    

Declared dependencies: `l10n_gcc_pos`, `l10n_sa`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_gcc_pos",
    "l10n_sa"
  ],
  "data": [
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "web/static/lib/zxing-library/zxing-library.js",
      "l10n_sa_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_sa_pos/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "web/static/lib/zxing-library/zxing-library.js",
      "l10n_sa_pos/static/src/app/utils/qr.js",
      "l10n_sa_pos/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_sa_pos/__init__.py` (5 lines)
- `addons/l10n_sa_pos/__manifest__.py` (33 lines)
- `addons/l10n_sa_pos/i18n/ar.po` (153 lines)
- `addons/l10n_sa_pos/i18n/l10n_sa_pos.pot` (146 lines)
- `addons/l10n_sa_pos/models/__init__.py` (4 lines)
- `addons/l10n_sa_pos/models/pos_config.py` (28 lines)
- `addons/l10n_sa_pos/models/pos_order.py` (40 lines)
- `addons/l10n_sa_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_sa_pos/receipt/pos_order_receipt.py` (55 lines)
- `addons/l10n_sa_pos/receipt/pos_order_receipt.xml` (32 lines)
- `addons/l10n_sa_pos/static/src/app/add_zatca_refund_reason_popup/add_zatca_refund_reason_popup.js` (26 lines)
- `addons/l10n_sa_pos/static/src/app/add_zatca_refund_reason_popup/add_zatca_refund_reason_popup.xml` (23 lines)
- `addons/l10n_sa_pos/static/src/app/utils/printer/generate_printer_data.js` (16 lines)
- `addons/l10n_sa_pos/static/src/app/utils/qr.js` (58 lines)
- `addons/l10n_sa_pos/static/src/overrides/components/ticket_screen/ticket_screen.js` (19 lines)
- `addons/l10n_sa_pos/static/src/overrides/models/pos_order.js` (41 lines)
- `addons/l10n_sa_pos/static/tests/tours/sa_pos_tour.js` (22 lines)
- `addons/l10n_sa_pos/static/tests/unit/sa_pos_unit.test.js` (76 lines)
- `addons/l10n_sa_pos/tests/__init__.py` (4 lines)
- `addons/l10n_sa_pos/tests/test_order_receipt.py` (35 lines)
- `addons/l10n_sa_pos/tests/test_sa_pos.py` (109 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
