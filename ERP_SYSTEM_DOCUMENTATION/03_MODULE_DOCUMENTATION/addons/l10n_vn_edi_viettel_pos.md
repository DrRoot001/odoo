# Module: l10n_vn_edi_viettel_pos

- **Module ID:** MOD-343
- **Path:** `addons/l10n_vn_edi_viettel_pos`
- **Manifest:** `addons/l10n_vn_edi_viettel_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

POS E-invoicing using SInvoice by Viettel


Vietnam - POS E-invoicing
=========================
Using SInvoice by Viettel
    

Declared dependencies: `l10n_vn_edi_viettel`, `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_vn_edi_viettel",
    "point_of_sale"
  ],
  "data": [
    "data/res_partner_data.xml",
    "views/res_config_settings_views.xml",
    "views/account_move_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "l10n_vn_edi_viettel_pos/static/src/**/*"
    ],
    "web.assets_tests": [
      "l10n_vn_edi_viettel_pos/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_vn_edi_viettel_pos/__init__.py` (3 lines)
- `addons/l10n_vn_edi_viettel_pos/__manifest__.py` (35 lines)
- `addons/l10n_vn_edi_viettel_pos/data/res_partner_data.xml` (8 lines)
- `addons/l10n_vn_edi_viettel_pos/i18n/l10n_vn_edi_viettel_pos.pot` (214 lines)
- `addons/l10n_vn_edi_viettel_pos/i18n/vi.po` (215 lines)
- `addons/l10n_vn_edi_viettel_pos/models/__init__.py` (9 lines)
- `addons/l10n_vn_edi_viettel_pos/models/account_move.py` (31 lines)
- `addons/l10n_vn_edi_viettel_pos/models/pos_config.py` (32 lines)
- `addons/l10n_vn_edi_viettel_pos/models/pos_order.py` (49 lines)
- `addons/l10n_vn_edi_viettel_pos/models/pos_session.py` (15 lines)
- `addons/l10n_vn_edi_viettel_pos/models/res_company.py` (12 lines)
- `addons/l10n_vn_edi_viettel_pos/models/res_config_settings.py` (22 lines)
- `addons/l10n_vn_edi_viettel_pos/models/res_partner.py` (31 lines)
- `addons/l10n_vn_edi_viettel_pos/security/ir.access.csv` (3 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/components/invoice_button/invoice_button.js` (33 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/components/payment_screen/payment_screen.js` (36 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/components/payment_screen/payment_screen.xml` (8 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/components/ticket_screen/ticket_screen.js` (13 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/models/pos_order.js` (21 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/models/pos_store.js` (10 lines)
- `addons/l10n_vn_edi_viettel_pos/static/src/overrides/utils/order_payment_validation.js` (54 lines)
- `addons/l10n_vn_edi_viettel_pos/static/tests/tours/l10n_vn_edi_viettel_pos_tour.js` (63 lines)
- `addons/l10n_vn_edi_viettel_pos/tests/__init__.py` (4 lines)
- `addons/l10n_vn_edi_viettel_pos/tests/test_l10n_vn_edi_pos.py` (220 lines)
- `addons/l10n_vn_edi_viettel_pos/tests/test_l10n_vn_edi_pos_tour.py` (67 lines)
- `addons/l10n_vn_edi_viettel_pos/views/account_move_views.xml` (13 lines)
- `addons/l10n_vn_edi_viettel_pos/views/res_config_settings_views.xml` (37 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
