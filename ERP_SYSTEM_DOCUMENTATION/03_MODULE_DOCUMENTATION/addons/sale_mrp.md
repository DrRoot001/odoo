# Module: sale_mrp

- **Module ID:** MOD-520
- **Path:** `addons/sale_mrp`
- **Manifest:** `addons/sale_mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module provides facility to the user to install mrp and sales modulesat a time.
====================================================================================

It is basically used when we want to keep track of production orders generated
from sales order. It adds sales name and sales Reference on production order.
    

Declared dependencies: `mrp`, `sale_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 20 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp",
    "sale_stock"
  ],
  "data": [
    "views/mrp_production_views.xml",
    "views/sale_order_views.xml",
    "views/sale_portal_templates.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/sale_mrp/__init__.py` (4 lines)
- `addons/sale_mrp/__manifest__.py` (24 lines)
- `addons/sale_mrp/controllers/__init__.py` (3 lines)
- `addons/sale_mrp/controllers/portal.py` (18 lines)
- `addons/sale_mrp/i18n/am.po` (168 lines)
- `addons/sale_mrp/i18n/ar.po` (196 lines)
- `addons/sale_mrp/i18n/az.po` (181 lines)
- `addons/sale_mrp/i18n/bg.po` (181 lines)
- `addons/sale_mrp/i18n/bs.po` (174 lines)
- `addons/sale_mrp/i18n/ca.po` (200 lines)
- `addons/sale_mrp/i18n/cs.po` (197 lines)
- `addons/sale_mrp/i18n/da.po` (195 lines)
- `addons/sale_mrp/i18n/de.po` (206 lines)
- `addons/sale_mrp/i18n/el.po` (195 lines)
- `addons/sale_mrp/i18n/es.po` (205 lines)
- `addons/sale_mrp/i18n/es_419.po` (202 lines)
- `addons/sale_mrp/i18n/es_CL.po` (25 lines)
- `addons/sale_mrp/i18n/et.po` (199 lines)
- `addons/sale_mrp/i18n/eu.po` (170 lines)
- `addons/sale_mrp/i18n/fa.po` (183 lines)
- `addons/sale_mrp/i18n/fi.po` (208 lines)
- `addons/sale_mrp/i18n/fo.po` (170 lines)
- `addons/sale_mrp/i18n/fr.po` (196 lines)
- `addons/sale_mrp/i18n/fr_BE.po` (24 lines)
- `addons/sale_mrp/i18n/gl.po` (170 lines)
- `addons/sale_mrp/i18n/gu.po` (172 lines)
- `addons/sale_mrp/i18n/he.po` (195 lines)
- `addons/sale_mrp/i18n/hi.po` (172 lines)
- `addons/sale_mrp/i18n/hr.po` (183 lines)
- `addons/sale_mrp/i18n/hu.po` (195 lines)
- `addons/sale_mrp/i18n/id.po` (196 lines)
- `addons/sale_mrp/i18n/is.po` (168 lines)
- `addons/sale_mrp/i18n/it.po` (204 lines)
- `addons/sale_mrp/i18n/ja.po` (194 lines)
- `addons/sale_mrp/i18n/ka.po` (174 lines)
- `addons/sale_mrp/i18n/kab.po` (172 lines)
- `addons/sale_mrp/i18n/ko.po` (194 lines)
- `addons/sale_mrp/i18n/ku.po` (171 lines)
- `addons/sale_mrp/i18n/lo.po` (172 lines)
- `addons/sale_mrp/i18n/lt.po` (187 lines)
- `addons/sale_mrp/i18n/lv.po` (177 lines)
- `addons/sale_mrp/i18n/mk.po` (171 lines)
- `addons/sale_mrp/i18n/mn.po` (184 lines)
- `addons/sale_mrp/i18n/my.po` (171 lines)
- `addons/sale_mrp/i18n/nb.po` (194 lines)
- `addons/sale_mrp/i18n/nl.po` (206 lines)
- `addons/sale_mrp/i18n/pl.po` (199 lines)
- `addons/sale_mrp/i18n/pt.po` (199 lines)
- `addons/sale_mrp/i18n/pt_BR.po` (207 lines)
- `addons/sale_mrp/i18n/ro.po` (186 lines)
- `addons/sale_mrp/i18n/ru.po` (194 lines)
- `addons/sale_mrp/i18n/sale_mrp.pot` (164 lines)
- `addons/sale_mrp/i18n/sk.po` (181 lines)
- `addons/sale_mrp/i18n/sl.po` (180 lines)
- `addons/sale_mrp/i18n/sr@latin.po` (179 lines)
- `addons/sale_mrp/i18n/sv.po` (197 lines)
- `addons/sale_mrp/i18n/th.po` (195 lines)
- `addons/sale_mrp/i18n/tr.po` (204 lines)
- `addons/sale_mrp/i18n/uk.po` (183 lines)
- `addons/sale_mrp/i18n/uz.po` (206 lines)
- `addons/sale_mrp/i18n/vi.po` (196 lines)
- `addons/sale_mrp/i18n/zh_CN.po` (201 lines)
- `addons/sale_mrp/i18n/zh_TW.po` (193 lines)
- `addons/sale_mrp/models/__init__.py` (9 lines)
- `addons/sale_mrp/models/mrp_bom.py` (49 lines)
- `addons/sale_mrp/models/mrp_production.py` (53 lines)
- `addons/sale_mrp/models/sale_order.py` (47 lines)
- `addons/sale_mrp/models/sale_order_line.py` (149 lines)
- `addons/sale_mrp/models/stock_move.py` (24 lines)
- `addons/sale_mrp/models/stock_orderpoint.py` (21 lines)
- `addons/sale_mrp/models/stock_rule.py` (11 lines)
- `addons/sale_mrp/security/ir.access.csv` (7 lines)
- `addons/sale_mrp/tests/__init__.py` (9 lines)
- `addons/sale_mrp/tests/test_multistep_manufacturing.py` (294 lines)
- `addons/sale_mrp/tests/test_sale_mrp_anglo_saxon_valuation.py` (887 lines)
- `addons/sale_mrp/tests/test_sale_mrp_flow.py` (3,059 lines)
- `addons/sale_mrp/tests/test_sale_mrp_kit_bom.py` (912 lines)
- `addons/sale_mrp/tests/test_sale_mrp_lead_time.py` (180 lines)
- `addons/sale_mrp/tests/test_sale_mrp_procurement.py` (416 lines)
- `addons/sale_mrp/tests/test_sale_mrp_report.py` (167 lines)
- `addons/sale_mrp/views/mrp_production_views.xml` (19 lines)
- `addons/sale_mrp/views/sale_order_views.xml` (23 lines)
- `addons/sale_mrp/views/sale_portal_templates.xml` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
