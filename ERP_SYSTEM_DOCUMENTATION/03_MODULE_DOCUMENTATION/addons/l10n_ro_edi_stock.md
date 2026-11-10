# Module: l10n_ro_edi_stock

- **Module ID:** MOD-306
- **Path:** `addons/l10n_ro_edi_stock`
- **Manifest:** `addons/l10n_ro_edi_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


E-Transport implementation for Romania
    

Declared dependencies: `stock_delivery`, `l10n_ro_edi`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 13 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock_delivery",
    "l10n_ro_edi"
  ],
  "data": [
    "data/template_etransport.xml",
    "views/res_config_settings_views.xml",
    "views/stock_picking_batch_views.xml",
    "views/stock_picking_views.xml",
    "views/delivery_carrier_views.xml",
    "report/report_deliveryslip.xml",
    "report/report_picking_batch.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_ro_edi_stock/static/src/components/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ro_edi_stock/__init__.py` (1 lines)
- `addons/l10n_ro_edi_stock/__manifest__.py` (26 lines)
- `addons/l10n_ro_edi_stock/data/template_etransport.xml` (88 lines)
- `addons/l10n_ro_edi_stock/i18n/l10n_ro_edi_stock.pot` (1,865 lines)
- `addons/l10n_ro_edi_stock/i18n/ro.po` (1,886 lines)
- `addons/l10n_ro_edi_stock/models/__init__.py` (5 lines)
- `addons/l10n_ro_edi_stock/models/delivery_carrier.py` (7 lines)
- `addons/l10n_ro_edi_stock/models/etransport_api.py` (80 lines)
- `addons/l10n_ro_edi_stock/models/l10n_ro_edi_stock_document.py` (20 lines)
- `addons/l10n_ro_edi_stock/models/stock_picking.py` (967 lines)
- `addons/l10n_ro_edi_stock/models/stock_picking_batch.py` (439 lines)
- `addons/l10n_ro_edi_stock/report/report_deliveryslip.xml` (11 lines)
- `addons/l10n_ro_edi_stock/report/report_picking_batch.xml` (11 lines)
- `addons/l10n_ro_edi_stock/static/src/components/document_state/document_state_field.js` (24 lines)
- `addons/l10n_ro_edi_stock/tests/__init__.py` (4 lines)
- `addons/l10n_ro_edi_stock/tests/common.py` (82 lines)
- `addons/l10n_ro_edi_stock/tests/test_batch_stock_etransport.py` (122 lines)
- `addons/l10n_ro_edi_stock/tests/test_etransport_dropship_flows.py` (216 lines)
- `addons/l10n_ro_edi_stock/tests/test_etransport_flows.py` (212 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_dropship_domestic_vendor_b2c_1.xml` (14 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_dropship_foreign_vendor_b2c_1.xml` (12 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_export_1.xml` (12 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_intra_community_purchase_1.xml` (12 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_send_and_amend_etransport_1.xml` (14 lines)
- `addons/l10n_ro_edi_stock/tests/test_files/test_send_and_amend_etransport_2.xml` (14 lines)
- `addons/l10n_ro_edi_stock/views/delivery_carrier_views.xml` (13 lines)
- `addons/l10n_ro_edi_stock/views/res_config_settings_views.xml` (14 lines)
- `addons/l10n_ro_edi_stock/views/stock_picking_batch_views.xml` (141 lines)
- `addons/l10n_ro_edi_stock/views/stock_picking_views.xml` (142 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
