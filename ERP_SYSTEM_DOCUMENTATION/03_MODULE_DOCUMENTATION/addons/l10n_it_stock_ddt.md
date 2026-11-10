# Module: l10n_it_stock_ddt

- **Module ID:** MOD-244
- **Path:** `addons/l10n_it_stock_ddt`
- **Manifest:** `addons/l10n_it_stock_ddt/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Documento di Trasporto (DDT)

Whenever goods are transferred between A and B, the DDT serves
as a legitimation e.g. when the police would stop you.

When you want to print an outgoing picking in an Italian company,
it will print you the DDT instead.  It is like the delivery
slip, but it also contains the value of the product,
the transportation reason, the carrier, ... which make it a DDT.

We also use a separate sequence for the DDT as the number should not
have any gaps and should only be applied at the moment the goods are sent.

When invoices are related to their sale order and the sale order with the
delivery, the system will automatically calculate the linked DDTs for every
invoice line to export in the FatturaPA XML.
    

Declared dependencies: `l10n_it_edi`, `stock_delivery`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_it_edi",
    "stock_delivery",
    "stock_account"
  ],
  "data": [
    "report/l10n_it_ddt_report.xml",
    "report/report_invoice.xml",
    "views/stock_picking_views.xml",
    "views/account_invoice_views.xml",
    "data/l10n_it_ddt_template.xml"
  ]
}
```

### Representative source files

- `addons/l10n_it_stock_ddt/__init__.py` (14 lines)
- `addons/l10n_it_stock_ddt/__manifest__.py` (35 lines)
- `addons/l10n_it_stock_ddt/data/l10n_it_ddt_template.xml` (16 lines)
- `addons/l10n_it_stock_ddt/i18n/it.po` (367 lines)
- `addons/l10n_it_stock_ddt/i18n/l10n_it_stock_ddt.pot` (340 lines)
- `addons/l10n_it_stock_ddt/models/__init__.py` (5 lines)
- `addons/l10n_it_stock_ddt/models/account_invoice.py` (110 lines)
- `addons/l10n_it_stock_ddt/models/stock_picking.py` (98 lines)
- `addons/l10n_it_stock_ddt/report/l10n_it_ddt_report.xml` (208 lines)
- `addons/l10n_it_stock_ddt/report/report_invoice.xml` (21 lines)
- `addons/l10n_it_stock_ddt/tests/__init__.py` (5 lines)
- `addons/l10n_it_stock_ddt/tests/export_xmls/deferred_invoice.xml` (143 lines)
- `addons/l10n_it_stock_ddt/tests/test_ddt.py` (198 lines)
- `addons/l10n_it_stock_ddt/tests/test_edi.py` (142 lines)
- `addons/l10n_it_stock_ddt/views/account_invoice_views.xml` (17 lines)
- `addons/l10n_it_stock_ddt/views/stock_picking_views.xml` (51 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
