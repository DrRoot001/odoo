# Module: l10n_vn_edi_viettel_stock

- **Module ID:** MOD-344
- **Path:** `addons/l10n_vn_edi_viettel_stock`
- **Manifest:** `addons/l10n_vn_edi_viettel_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Delivery E-invoicing using SInvoice by Viettel


Vietnam - Delivery E-invoicing
==============================
Using SInvoice by Viettel
    

Declared dependencies: `l10n_vn_edi_viettel`, `stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
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
    "l10n_vn_edi_viettel",
    "stock"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/stock_warehouse_views.xml",
    "views/stock_picking_views.xml",
    "wizard/wizard_send_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_vn_edi_viettel_stock/__init__.py` (4 lines)
- `addons/l10n_vn_edi_viettel_stock/__manifest__.py` (28 lines)
- `addons/l10n_vn_edi_viettel_stock/i18n/l10n_vn_edi_viettel_stock.pot` (365 lines)
- `addons/l10n_vn_edi_viettel_stock/i18n/vi.po` (368 lines)
- `addons/l10n_vn_edi_viettel_stock/models/__init__.py` (7 lines)
- `addons/l10n_vn_edi_viettel_stock/models/res_company.py` (17 lines)
- `addons/l10n_vn_edi_viettel_stock/models/res_config_settings.py` (17 lines)
- `addons/l10n_vn_edi_viettel_stock/models/stock_move.py` (30 lines)
- `addons/l10n_vn_edi_viettel_stock/models/stock_picking.py` (416 lines)
- `addons/l10n_vn_edi_viettel_stock/models/stock_warehouse.py` (17 lines)
- `addons/l10n_vn_edi_viettel_stock/security/ir.access.csv` (4 lines)
- `addons/l10n_vn_edi_viettel_stock/tests/__init__.py` (2 lines)
- `addons/l10n_vn_edi_viettel_stock/tests/test_stock_edi.py` (352 lines)
- `addons/l10n_vn_edi_viettel_stock/views/res_config_settings_views.xml` (23 lines)
- `addons/l10n_vn_edi_viettel_stock/views/stock_picking_views.xml` (52 lines)
- `addons/l10n_vn_edi_viettel_stock/views/stock_warehouse_views.xml` (15 lines)
- `addons/l10n_vn_edi_viettel_stock/wizard/__init__.py` (4 lines)
- `addons/l10n_vn_edi_viettel_stock/wizard/l10n_vn_edi_send_wizard.py` (58 lines)
- `addons/l10n_vn_edi_viettel_stock/wizard/l10n_vn_edi_template_field_line.py` (37 lines)
- `addons/l10n_vn_edi_viettel_stock/wizard/wizard_send_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
