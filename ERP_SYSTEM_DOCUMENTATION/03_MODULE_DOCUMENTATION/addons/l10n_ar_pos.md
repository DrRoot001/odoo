# Module: l10n_ar_pos

- **Module ID:** MOD-121
- **Path:** `addons/l10n_ar_pos`
- **Manifest:** `addons/l10n_ar_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module brings the technical requirement for the Argentinean regulation.
Install this if you are using the Point of Sale app in Argentina.
    

Declared dependencies: `l10n_ar`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ar",
    "point_of_sale"
  ],
  "data": [
    "views/res_partner_views.xml",
    "views/templates.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_ar_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_ar_pos/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ar_pos/__init__.py` (2 lines)
- `addons/l10n_ar_pos/__manifest__.py` (28 lines)
- `addons/l10n_ar_pos/i18n/es_419.po` (109 lines)
- `addons/l10n_ar_pos/i18n/l10n_ar_pos.pot` (96 lines)
- `addons/l10n_ar_pos/models/__init__.py` (5 lines)
- `addons/l10n_ar_pos/models/l10n_ar_afip_responsibility_type.py` (12 lines)
- `addons/l10n_ar_pos/models/pos_config.py` (18 lines)
- `addons/l10n_ar_pos/models/pos_session.py` (13 lines)
- `addons/l10n_ar_pos/models/res_partner.py` (21 lines)
- `addons/l10n_ar_pos/static/src/app/models/pos_order.js` (8 lines)
- `addons/l10n_ar_pos/static/src/app/screens/payment_screen/payment_screen.js` (11 lines)
- `addons/l10n_ar_pos/static/src/app/screens/product_screen/product_screen.js` (15 lines)
- `addons/l10n_ar_pos/static/src/app/screens/ticket_screen/ticket_screen.js` (19 lines)
- `addons/l10n_ar_pos/static/src/app/services/pos_store.js` (23 lines)
- `addons/l10n_ar_pos/static/tests/tours/l10n_ar_tour.js` (21 lines)
- `addons/l10n_ar_pos/tests/__init__.py` (3 lines)
- `addons/l10n_ar_pos/tests/test_ar_pos.py` (15 lines)
- `addons/l10n_ar_pos/tests/test_pos_ar.py` (59 lines)
- `addons/l10n_ar_pos/views/res_partner_views.xml` (13 lines)
- `addons/l10n_ar_pos/views/templates.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
