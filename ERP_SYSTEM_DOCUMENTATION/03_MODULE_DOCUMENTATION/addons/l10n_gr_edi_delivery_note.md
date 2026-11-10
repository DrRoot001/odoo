# Module: l10n_gr_edi_delivery_note

- **Module ID:** MOD-209
- **Path:** `addons/l10n_gr_edi_delivery_note`
- **Manifest:** `addons/l10n_gr_edi_delivery_note/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Transmit Greece myDATA EDI for Delivery Notes


        This module allows transmitting electronic Delivery Notes
        to Greece's tax authority myDATA platform.
    

Declared dependencies: `l10n_gr_edi`, `stock`, `sale`, `sale_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_gr_edi",
    "stock",
    "sale",
    "sale_stock"
  ],
  "data": [
    "views/res_company_views.xml",
    "views/res_partner_views.xml",
    "views/stock_picking_views.xml",
    "views/report_deliveryslip.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_gr_edi_delivery_note/__init__.py` (1 lines)
- `addons/l10n_gr_edi_delivery_note/__manifest__.py` (22 lines)
- `addons/l10n_gr_edi_delivery_note/i18n/el.po` (482 lines)
- `addons/l10n_gr_edi_delivery_note/i18n/l10n_gr_edi_delivery_note.pot` (482 lines)
- `addons/l10n_gr_edi_delivery_note/models/__init__.py` (4 lines)
- `addons/l10n_gr_edi_delivery_note/models/account_move.py` (34 lines)
- `addons/l10n_gr_edi_delivery_note/models/l10n_gr_edi_document.py` (39 lines)
- `addons/l10n_gr_edi_delivery_note/models/stock_move.py` (50 lines)
- `addons/l10n_gr_edi_delivery_note/models/stock_picking.py` (431 lines)
- `addons/l10n_gr_edi_delivery_note/security/ir.access.csv` (4 lines)
- `addons/l10n_gr_edi_delivery_note/tests/__init__.py` (1 lines)
- `addons/l10n_gr_edi_delivery_note/tests/test_mydata_delivery_note.py` (154 lines)
- `addons/l10n_gr_edi_delivery_note/views/report_deliveryslip.xml` (20 lines)
- `addons/l10n_gr_edi_delivery_note/views/res_company_views.xml` (28 lines)
- `addons/l10n_gr_edi_delivery_note/views/res_partner_views.xml` (28 lines)
- `addons/l10n_gr_edi_delivery_note/views/stock_picking_views.xml` (129 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
