# Module: l10n_test_pos_qr_payment

- **Module ID:** MOD-322
- **Path:** `addons/l10n_test_pos_qr_payment`
- **Manifest:** `addons/l10n_test_pos_qr_payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


        This module contains tests related to point of sale QR code payment.
        It tests all the supported qr codes: SEPA, Swiss QR and EMV QR (using the hk and br implementation)
    

Declared dependencies: `point_of_sale`, `account_qr_code_sepa`, `l10n_be`, `l10n_ch`, `l10n_hk`, `l10n_br`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "account_qr_code_sepa",
    "l10n_be",
    "l10n_ch",
    "l10n_hk",
    "l10n_br"
  ],
  "assets": {
    "web.assets_tests": [
      "l10n_test_pos_qr_payment/static/tests/tours/*"
    ],
    "web.assets_unit_tests": [
      "l10n_test_pos_qr_payment/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_test_pos_qr_payment/__init__.py` (0 lines)
- `addons/l10n_test_pos_qr_payment/__manifest__.py` (29 lines)
- `addons/l10n_test_pos_qr_payment/static/tests/tours/test_pos_payment_tour.js` (102 lines)
- `addons/l10n_test_pos_qr_payment/static/tests/unit/data/pos_config.data.js` (8 lines)
- `addons/l10n_test_pos_qr_payment/static/tests/unit/data/pos_payment_method.data.js` (14 lines)
- `addons/l10n_test_pos_qr_payment/static/tests/unit/service/pos_store.test.js` (19 lines)
- `addons/l10n_test_pos_qr_payment/tests/__init__.py` (3 lines)
- `addons/l10n_test_pos_qr_payment/tests/common.py` (57 lines)
- `addons/l10n_test_pos_qr_payment/tests/test_pos_qr_payment.py` (262 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
