# Module: l10n_in_sale

- **Module ID:** MOD-236
- **Path:** `addons/l10n_in_sale`
- **Manifest:** `addons/l10n_in_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

GST Sale Report

Declared dependencies: `l10n_in`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in",
    "sale"
  ],
  "data": [
    "views/sale_order_views.xml"
  ],
  "demo": [
    "data/product_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_in_sale/__init__.py` (5 lines)
- `addons/l10n_in_sale/__manifest__.py` (20 lines)
- `addons/l10n_in_sale/data/product_demo.xml` (7 lines)
- `addons/l10n_in_sale/i18n/hi.po` (64 lines)
- `addons/l10n_in_sale/i18n/l10n_in_sale.pot` (60 lines)
- `addons/l10n_in_sale/models/__init__.py` (5 lines)
- `addons/l10n_in_sale/models/sale_order.py` (79 lines)
- `addons/l10n_in_sale/models/sale_order_line.py` (15 lines)
- `addons/l10n_in_sale/tests/__init__.py` (5 lines)
- `addons/l10n_in_sale/tests/test_l10n_in_sale_fiscal_position.py` (135 lines)
- `addons/l10n_in_sale/tests/test_l10n_in_sale_qty_invoiced.py` (34 lines)
- `addons/l10n_in_sale/views/sale_order_views.xml` (19 lines)
- `addons/l10n_in_sale/wizard/__init__.py` (4 lines)
- `addons/l10n_in_sale/wizard/sale_make_invoice_advance.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
