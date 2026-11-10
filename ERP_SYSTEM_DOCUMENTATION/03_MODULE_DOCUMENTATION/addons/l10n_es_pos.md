# Module: l10n_es_pos

- **Module ID:** MOD-181
- **Path:** `addons/l10n_es_pos`
- **Manifest:** `addons/l10n_es_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Spanish localization for Point of Sale

No manifest description declared.

Declared dependencies: `point_of_sale`, `l10n_es`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "l10n_es"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/pos_order_views.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_es_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_es_pos/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_es_pos/__init__.py` (2 lines)
- `addons/l10n_es_pos/__manifest__.py` (22 lines)
- `addons/l10n_es_pos/i18n/es.po` (127 lines)
- `addons/l10n_es_pos/i18n/l10n_es_pos.pot` (121 lines)
- `addons/l10n_es_pos/models/__init__.py` (5 lines)
- `addons/l10n_es_pos/models/account_move.py` (17 lines)
- `addons/l10n_es_pos/models/pos_config.py` (34 lines)
- `addons/l10n_es_pos/models/pos_order.py` (37 lines)
- `addons/l10n_es_pos/models/res_company.py` (12 lines)
- `addons/l10n_es_pos/models/res_config_settings.py` (10 lines)
- `addons/l10n_es_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_es_pos/receipt/pos_order_receipt.py` (13 lines)
- `addons/l10n_es_pos/receipt/pos_order_receipt.xml` (16 lines)
- `addons/l10n_es_pos/static/src/app/models/pos_order.js` (16 lines)
- `addons/l10n_es_pos/static/src/app/services/pos_store.js` (17 lines)
- `addons/l10n_es_pos/static/src/app/utils/order_payment_validation.js` (75 lines)
- `addons/l10n_es_pos/static/src/app/utils/printer/generate_printer_data.js` (17 lines)
- `addons/l10n_es_pos/static/tests/tours/spanish_pos_tour.js` (116 lines)
- `addons/l10n_es_pos/static/tests/tours/utils/receipt_util.js` (24 lines)
- `addons/l10n_es_pos/tests/__init__.py` (6 lines)
- `addons/l10n_es_pos/tests/test_es_pos.py` (17 lines)
- `addons/l10n_es_pos/tests/test_frontend.py` (166 lines)
- `addons/l10n_es_pos/tests/test_order_receipt.py` (19 lines)
- `addons/l10n_es_pos/views/pos_order_views.xml` (24 lines)
- `addons/l10n_es_pos/views/res_config_settings_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
