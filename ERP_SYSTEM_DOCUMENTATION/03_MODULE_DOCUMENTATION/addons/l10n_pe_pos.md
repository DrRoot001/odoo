# Module: l10n_pe_pos

- **Module ID:** MOD-291
- **Path:** `addons/l10n_pe_pos`
- **Manifest:** `addons/l10n_pe_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module brings the technical requirement for the Peruvian regulation.
Install this if you are using the Point of Sale app in Peru.
    

Declared dependencies: `l10n_pe`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_pe",
    "point_of_sale"
  ],
  "data": [
    "data/res_partner_data.xml",
    "views/templates.xml",
    "views/res_partner_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_pe_pos/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_pe_pos/__init__.py` (3 lines)
- `addons/l10n_pe_pos/__manifest__.py` (24 lines)
- `addons/l10n_pe_pos/data/res_partner_data.xml` (9 lines)
- `addons/l10n_pe_pos/i18n/es_419.po` (168 lines)
- `addons/l10n_pe_pos/i18n/l10n_pe_pos.pot` (146 lines)
- `addons/l10n_pe_pos/models/__init__.py` (6 lines)
- `addons/l10n_pe_pos/models/l10n_pe_res_city_district.py` (14 lines)
- `addons/l10n_pe_pos/models/pos_config.py` (18 lines)
- `addons/l10n_pe_pos/models/pos_session.py` (13 lines)
- `addons/l10n_pe_pos/models/res_city.py` (11 lines)
- `addons/l10n_pe_pos/models/res_partner.py` (25 lines)
- `addons/l10n_pe_pos/receipt/__init__.py` (1 lines)
- `addons/l10n_pe_pos/receipt/pos_order_receipt.py` (16 lines)
- `addons/l10n_pe_pos/static/src/app/services/pos_store.js` (22 lines)
- `addons/l10n_pe_pos/static/src/app/utils/order_payment_validation.js` (26 lines)
- `addons/l10n_pe_pos/static/src/app/utils/printer/generate_printer_data.js` (29 lines)
- `addons/l10n_pe_pos/static/src/overrides/components/paymentt_screen/payment_screen.js` (11 lines)
- `addons/l10n_pe_pos/static/src/overrides/components/ticket_screen/ticket_screen.js` (17 lines)
- `addons/l10n_pe_pos/tests/__init__.py` (3 lines)
- `addons/l10n_pe_pos/tests/test_pe_pos.py` (44 lines)
- `addons/l10n_pe_pos/views/res_partner_views.xml` (13 lines)
- `addons/l10n_pe_pos/views/templates.xml` (53 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
