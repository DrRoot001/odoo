# Module: mrp_subcontracting_purchase

- **Module ID:** MOD-387
- **Path:** `addons/mrp_subcontracting_purchase`
- **Manifest:** `addons/mrp_subcontracting_purchase/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This bridge module adds some smart buttons between Purchase and Subcontracting
    

Declared dependencies: `mrp_subcontracting_account`, `purchase_mrp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp_subcontracting_account",
    "purchase_mrp"
  ],
  "data": [
    "views/purchase_order_views.xml",
    "views/stock_picking_views.xml"
  ],
  "demo": [
    "data/mrp_subcontracting_purchase_demo.xml"
  ]
}
```

### Representative source files

- `addons/mrp_subcontracting_purchase/__init__.py` (5 lines)
- `addons/mrp_subcontracting_purchase/__manifest__.py` (21 lines)
- `addons/mrp_subcontracting_purchase/data/mrp_subcontracting_purchase_demo.xml` (18 lines)
- `addons/mrp_subcontracting_purchase/i18n/ar.po` (210 lines)
- `addons/mrp_subcontracting_purchase/i18n/az.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/bg.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/bs.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/ca.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/cs.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/da.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/de.po` (214 lines)
- `addons/mrp_subcontracting_purchase/i18n/el.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/es.po` (212 lines)
- `addons/mrp_subcontracting_purchase/i18n/es_419.po` (209 lines)
- `addons/mrp_subcontracting_purchase/i18n/et.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/fa.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/fi.po` (210 lines)
- `addons/mrp_subcontracting_purchase/i18n/fr.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/he.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/hi.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/hr.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/hu.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/id.po` (209 lines)
- `addons/mrp_subcontracting_purchase/i18n/it.po` (214 lines)
- `addons/mrp_subcontracting_purchase/i18n/ja.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/kab.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/ko.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/ku.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/lo.po` (211 lines)
- `addons/mrp_subcontracting_purchase/i18n/lt.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/lv.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/mn.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/mrp_subcontracting_purchase.pot` (202 lines)
- `addons/mrp_subcontracting_purchase/i18n/my.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/nb.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/nl.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/pl.po` (210 lines)
- `addons/mrp_subcontracting_purchase/i18n/pt.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/pt_BR.po` (222 lines)
- `addons/mrp_subcontracting_purchase/i18n/ro.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/ru.po` (211 lines)
- `addons/mrp_subcontracting_purchase/i18n/sk.po` (206 lines)
- `addons/mrp_subcontracting_purchase/i18n/sl.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/sr@latin.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/sv.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/th.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/tr.po` (211 lines)
- `addons/mrp_subcontracting_purchase/i18n/uk.po` (207 lines)
- `addons/mrp_subcontracting_purchase/i18n/uz.po` (235 lines)
- `addons/mrp_subcontracting_purchase/i18n/vi.po` (208 lines)
- `addons/mrp_subcontracting_purchase/i18n/zh_CN.po` (213 lines)
- `addons/mrp_subcontracting_purchase/i18n/zh_TW.po` (210 lines)
- `addons/mrp_subcontracting_purchase/models/__init__.py` (11 lines)
- `addons/mrp_subcontracting_purchase/models/account_move.py` (46 lines)
- `addons/mrp_subcontracting_purchase/models/account_move_line.py` (17 lines)
- `addons/mrp_subcontracting_purchase/models/mrp_production.py` (74 lines)
- `addons/mrp_subcontracting_purchase/models/product_product.py` (26 lines)
- `addons/mrp_subcontracting_purchase/models/purchase_order.py` (31 lines)
- `addons/mrp_subcontracting_purchase/models/stock_move.py` (42 lines)
- `addons/mrp_subcontracting_purchase/models/stock_picking.py` (50 lines)
- `addons/mrp_subcontracting_purchase/models/stock_rule.py` (61 lines)
- `addons/mrp_subcontracting_purchase/report/__init__.py` (5 lines)
- `addons/mrp_subcontracting_purchase/report/mrp_report_bom_structure.py` (24 lines)
- `addons/mrp_subcontracting_purchase/report/mrp_report_mo_overview.py` (34 lines)
- `addons/mrp_subcontracting_purchase/tests/__init__.py` (4 lines)
- `addons/mrp_subcontracting_purchase/tests/test_mrp_report_mo_overview.py` (116 lines)
- `addons/mrp_subcontracting_purchase/tests/test_mrp_subcontracting_purchase.py` (1,427 lines)
- `addons/mrp_subcontracting_purchase/views/purchase_order_views.xml` (20 lines)
- `addons/mrp_subcontracting_purchase/views/stock_picking_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
