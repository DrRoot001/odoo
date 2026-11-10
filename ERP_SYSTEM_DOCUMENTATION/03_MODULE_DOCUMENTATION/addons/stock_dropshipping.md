# Module: stock_dropshipping

- **Module ID:** MOD-562
- **Path:** `addons/stock_dropshipping`
- **Manifest:** `addons/stock_dropshipping/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Drop Shipping


Manage drop shipping orders
===========================

This module adds a pre-configured Drop Shipping operation type
as well as a procurement route that allow configuring Drop
Shipping products and orders.

When drop shipping is used the goods are directly transferred
from vendors to customers (direct delivery) without
going through the retailer's warehouse. In this case no
internal transfer document is needed.



Declared dependencies: `sale_purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_purchase_stock"
  ],
  "data": [
    "data/stock_data.xml",
    "views/sale_order_views.xml",
    "views/stock_picking_views.xml",
    "views/purchase_order_views.xml"
  ],
  "demo": [
    "data/stock_dropshipping_demo.xml"
  ]
}
```

### Representative source files

- `addons/stock_dropshipping/__init__.py` (9 lines)
- `addons/stock_dropshipping/__manifest__.py` (34 lines)
- `addons/stock_dropshipping/data/stock_data.xml` (20 lines)
- `addons/stock_dropshipping/data/stock_dropshipping_demo.xml` (19 lines)
- `addons/stock_dropshipping/i18n/af.po` (165 lines)
- `addons/stock_dropshipping/i18n/ar.po` (185 lines)
- `addons/stock_dropshipping/i18n/az.po` (191 lines)
- `addons/stock_dropshipping/i18n/bg.po` (193 lines)
- `addons/stock_dropshipping/i18n/bs.po` (194 lines)
- `addons/stock_dropshipping/i18n/ca.po` (190 lines)
- `addons/stock_dropshipping/i18n/cs.po` (187 lines)
- `addons/stock_dropshipping/i18n/da.po` (187 lines)
- `addons/stock_dropshipping/i18n/de.po` (199 lines)
- `addons/stock_dropshipping/i18n/el.po` (186 lines)
- `addons/stock_dropshipping/i18n/es.po` (201 lines)
- `addons/stock_dropshipping/i18n/es_419.po` (200 lines)
- `addons/stock_dropshipping/i18n/et.po` (192 lines)
- `addons/stock_dropshipping/i18n/fa.po` (191 lines)
- `addons/stock_dropshipping/i18n/fi.po` (189 lines)
- `addons/stock_dropshipping/i18n/fr.po` (189 lines)
- `addons/stock_dropshipping/i18n/gu.po` (165 lines)
- `addons/stock_dropshipping/i18n/he.po` (189 lines)
- `addons/stock_dropshipping/i18n/hi.po` (194 lines)
- `addons/stock_dropshipping/i18n/hr.po` (195 lines)
- `addons/stock_dropshipping/i18n/hu.po` (188 lines)
- `addons/stock_dropshipping/i18n/id.po` (186 lines)
- `addons/stock_dropshipping/i18n/is.po` (161 lines)
- `addons/stock_dropshipping/i18n/it.po` (200 lines)
- `addons/stock_dropshipping/i18n/ja.po` (187 lines)
- `addons/stock_dropshipping/i18n/kab.po` (191 lines)
- `addons/stock_dropshipping/i18n/ko.po` (186 lines)
- `addons/stock_dropshipping/i18n/ku.po` (186 lines)
- `addons/stock_dropshipping/i18n/lo.po` (197 lines)
- `addons/stock_dropshipping/i18n/lt.po` (188 lines)
- `addons/stock_dropshipping/i18n/lv.po` (190 lines)
- `addons/stock_dropshipping/i18n/mk.po` (164 lines)
- `addons/stock_dropshipping/i18n/mn.po` (191 lines)
- `addons/stock_dropshipping/i18n/my.po` (191 lines)
- `addons/stock_dropshipping/i18n/nb.po` (187 lines)
- `addons/stock_dropshipping/i18n/nl.po` (187 lines)
- `addons/stock_dropshipping/i18n/pl.po` (188 lines)
- `addons/stock_dropshipping/i18n/pt.po` (194 lines)
- `addons/stock_dropshipping/i18n/pt_BR.po` (203 lines)
- `addons/stock_dropshipping/i18n/ro.po` (185 lines)
- `addons/stock_dropshipping/i18n/ru.po` (185 lines)
- `addons/stock_dropshipping/i18n/sk.po` (192 lines)
- `addons/stock_dropshipping/i18n/sl.po` (187 lines)
- `addons/stock_dropshipping/i18n/sr@latin.po` (187 lines)
- `addons/stock_dropshipping/i18n/stock_dropshipping.pot` (175 lines)
- `addons/stock_dropshipping/i18n/sv.po` (189 lines)
- `addons/stock_dropshipping/i18n/th.po` (183 lines)
- `addons/stock_dropshipping/i18n/tr.po` (190 lines)
- `addons/stock_dropshipping/i18n/uk.po` (193 lines)
- `addons/stock_dropshipping/i18n/uz.po` (202 lines)
- `addons/stock_dropshipping/i18n/vi.po` (185 lines)
- `addons/stock_dropshipping/i18n/zh_CN.po` (194 lines)
- `addons/stock_dropshipping/i18n/zh_TW.po` (185 lines)
- `addons/stock_dropshipping/models/__init__.py` (11 lines)
- `addons/stock_dropshipping/models/account_move_line.py` (12 lines)
- `addons/stock_dropshipping/models/product.py` (13 lines)
- `addons/stock_dropshipping/models/purchase.py` (93 lines)
- `addons/stock_dropshipping/models/res_company.py` (114 lines)
- `addons/stock_dropshipping/models/sale.py` (73 lines)
- `addons/stock_dropshipping/models/stock.py` (93 lines)
- `addons/stock_dropshipping/models/stock_move_line.py` (20 lines)
- `addons/stock_dropshipping/models/stock_replenish_mixin.py` (12 lines)
- `addons/stock_dropshipping/tests/__init__.py` (9 lines)
- `addons/stock_dropshipping/tests/test_dropship.py` (706 lines)
- `addons/stock_dropshipping/tests/test_dropship_variant_description.py` (64 lines)
- `addons/stock_dropshipping/tests/test_lifo_price.py` (89 lines)
- `addons/stock_dropshipping/tests/test_procurement_exception.py` (73 lines)
- `addons/stock_dropshipping/tests/test_purchase_order.py` (189 lines)
- `addons/stock_dropshipping/tests/test_stockvaluation.py` (332 lines)
- `addons/stock_dropshipping/views/purchase_order_views.xml` (19 lines)
- `addons/stock_dropshipping/views/sale_order_views.xml` (25 lines)
- `addons/stock_dropshipping/views/stock_picking_views.xml` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
