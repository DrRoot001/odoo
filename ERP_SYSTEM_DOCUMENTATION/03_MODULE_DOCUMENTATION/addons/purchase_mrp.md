# Module: purchase_mrp

- **Module ID:** MOD-498
- **Path:** `addons/purchase_mrp`
- **Manifest:** `addons/purchase_mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module provides facility to the user to install mrp and purchase modules at a time.
========================================================================================

It is basically used when we want to keep track of production orders generated
from purchase order.
    

Declared dependencies: `mrp`, `purchase_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp",
    "purchase_stock"
  ],
  "data": [
    "views/mrp_bom_views.xml",
    "views/purchase_order_views.xml",
    "views/mrp_production_views.xml",
    "views/stock_orderpoint_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/purchase_mrp_demo.xml"
  ]
}
```

### Representative source files

- `addons/purchase_mrp/__init__.py` (5 lines)
- `addons/purchase_mrp/__manifest__.py` (28 lines)
- `addons/purchase_mrp/data/purchase_mrp_demo.xml` (5 lines)
- `addons/purchase_mrp/i18n/ar.po` (171 lines)
- `addons/purchase_mrp/i18n/az.po` (174 lines)
- `addons/purchase_mrp/i18n/bg.po` (177 lines)
- `addons/purchase_mrp/i18n/bs.po` (174 lines)
- `addons/purchase_mrp/i18n/ca.po` (178 lines)
- `addons/purchase_mrp/i18n/cs.po` (173 lines)
- `addons/purchase_mrp/i18n/da.po` (174 lines)
- `addons/purchase_mrp/i18n/de.po` (180 lines)
- `addons/purchase_mrp/i18n/el.po` (171 lines)
- `addons/purchase_mrp/i18n/es.po` (182 lines)
- `addons/purchase_mrp/i18n/es_419.po` (171 lines)
- `addons/purchase_mrp/i18n/et.po` (181 lines)
- `addons/purchase_mrp/i18n/fa.po` (175 lines)
- `addons/purchase_mrp/i18n/fi.po` (177 lines)
- `addons/purchase_mrp/i18n/fr.po` (174 lines)
- `addons/purchase_mrp/i18n/gu.po` (161 lines)
- `addons/purchase_mrp/i18n/he.po` (188 lines)
- `addons/purchase_mrp/i18n/hi.po` (179 lines)
- `addons/purchase_mrp/i18n/hr.po` (182 lines)
- `addons/purchase_mrp/i18n/hu.po` (173 lines)
- `addons/purchase_mrp/i18n/id.po` (172 lines)
- `addons/purchase_mrp/i18n/is.po` (161 lines)
- `addons/purchase_mrp/i18n/it.po` (183 lines)
- `addons/purchase_mrp/i18n/ja.po` (171 lines)
- `addons/purchase_mrp/i18n/kab.po` (172 lines)
- `addons/purchase_mrp/i18n/ko.po` (170 lines)
- `addons/purchase_mrp/i18n/ku.po` (168 lines)
- `addons/purchase_mrp/i18n/lo.po` (174 lines)
- `addons/purchase_mrp/i18n/lt.po` (174 lines)
- `addons/purchase_mrp/i18n/lv.po` (175 lines)
- `addons/purchase_mrp/i18n/mn.po` (191 lines)
- `addons/purchase_mrp/i18n/my.po` (172 lines)
- `addons/purchase_mrp/i18n/nb.po` (169 lines)
- `addons/purchase_mrp/i18n/nl.po` (183 lines)
- `addons/purchase_mrp/i18n/pl.po` (175 lines)
- `addons/purchase_mrp/i18n/pt.po` (180 lines)
- `addons/purchase_mrp/i18n/pt_BR.po` (183 lines)
- `addons/purchase_mrp/i18n/purchase_mrp.pot` (159 lines)
- `addons/purchase_mrp/i18n/ro.po` (187 lines)
- `addons/purchase_mrp/i18n/ru.po` (172 lines)
- `addons/purchase_mrp/i18n/sk.po` (187 lines)
- `addons/purchase_mrp/i18n/sl.po` (173 lines)
- `addons/purchase_mrp/i18n/sr@latin.po` (173 lines)
- `addons/purchase_mrp/i18n/sv.po` (174 lines)
- `addons/purchase_mrp/i18n/th.po` (170 lines)
- `addons/purchase_mrp/i18n/tr.po` (175 lines)
- `addons/purchase_mrp/i18n/uk.po` (182 lines)
- `addons/purchase_mrp/i18n/uz.po` (195 lines)
- `addons/purchase_mrp/i18n/vi.po` (171 lines)
- `addons/purchase_mrp/i18n/zh_CN.po` (171 lines)
- `addons/purchase_mrp/i18n/zh_TW.po` (168 lines)
- `addons/purchase_mrp/models/__init__.py` (8 lines)
- `addons/purchase_mrp/models/mrp_bom.py` (76 lines)
- `addons/purchase_mrp/models/mrp_production.py` (63 lines)
- `addons/purchase_mrp/models/purchase.py` (124 lines)
- `addons/purchase_mrp/models/stock_move.py` (68 lines)
- `addons/purchase_mrp/models/stock_rule.py` (14 lines)
- `addons/purchase_mrp/report/__init__.py` (5 lines)
- `addons/purchase_mrp/report/mrp_report_bom_structure.py` (48 lines)
- `addons/purchase_mrp/report/mrp_report_mo_overview.py` (98 lines)
- `addons/purchase_mrp/security/ir.access.csv` (3 lines)
- `addons/purchase_mrp/tests/__init__.py` (6 lines)
- `addons/purchase_mrp/tests/test_anglo_saxon_valuation.py` (1,018 lines)
- `addons/purchase_mrp/tests/test_purchase_mrp_flow.py` (1,496 lines)
- `addons/purchase_mrp/tests/test_replenishment.py` (209 lines)
- `addons/purchase_mrp/views/mrp_bom_views.xml` (24 lines)
- `addons/purchase_mrp/views/mrp_production_views.xml` (19 lines)
- `addons/purchase_mrp/views/purchase_order_views.xml` (18 lines)
- `addons/purchase_mrp/views/stock_orderpoint_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
