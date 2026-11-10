# Module: l10n_ar_stock

- **Module ID:** MOD-122
- **Path:** `addons/l10n_ar_stock`
- **Manifest:** `addons/l10n_ar_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Argentinean - Stock

Declared dependencies: `l10n_ar`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ar",
    "stock_account"
  ],
  "data": [
    "data/ir_actions_server_data.xml",
    "data/ir_cron_data.xml",
    "data/mail_template_data.xml",
    "views/stock_picking_type_views.xml",
    "views/stock_picking_views.xml",
    "views/stock_picking_batch_views.xml",
    "views/report_delivery_guide.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ar_stock/__init__.py` (1 lines)
- `addons/l10n_ar_stock/__manifest__.py` (21 lines)
- `addons/l10n_ar_stock/data/ir_actions_server_data.xml` (35 lines)
- `addons/l10n_ar_stock/data/ir_cron_data.xml` (13 lines)
- `addons/l10n_ar_stock/data/mail_template_data.xml` (42 lines)
- `addons/l10n_ar_stock/i18n/es_419.po` (562 lines)
- `addons/l10n_ar_stock/i18n/l10n_ar_stock.pot` (459 lines)
- `addons/l10n_ar_stock/models/__init__.py` (3 lines)
- `addons/l10n_ar_stock/models/stock_picking.py` (272 lines)
- `addons/l10n_ar_stock/models/stock_picking_batch.py` (34 lines)
- `addons/l10n_ar_stock/models/stock_picking_type.py` (110 lines)
- `addons/l10n_ar_stock/tests/__init__.py` (3 lines)
- `addons/l10n_ar_stock/tests/test_l10n_ar_delivery_guide.py` (114 lines)
- `addons/l10n_ar_stock/tests/test_l10n_ar_delivery_guide_batch.py` (193 lines)
- `addons/l10n_ar_stock/tests/test_l10n_ar_stock_batch.py` (76 lines)
- `addons/l10n_ar_stock/views/report_delivery_guide.xml` (94 lines)
- `addons/l10n_ar_stock/views/stock_picking_batch_views.xml` (21 lines)
- `addons/l10n_ar_stock/views/stock_picking_type_views.xml` (28 lines)
- `addons/l10n_ar_stock/views/stock_picking_views.xml` (29 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
