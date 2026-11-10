# Module: pos_sale_stock

- **Module ID:** MOD-454
- **Path:** `addons/pos_sale_stock`
- **Manifest:** `addons/pos_sale_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between PoS Stock and Sales

No manifest description declared.

Declared dependencies: `pos_stock`, `pos_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_stock",
    "pos_sale"
  ],
  "data": [
    "views/stock_template.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_sale_stock/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_sale_stock/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_sale_stock/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_sale_stock/__init__.py` (2 lines)
- `addons/pos_sale_stock/__manifest__.py` (23 lines)
- `addons/pos_sale_stock/i18n/ar.po` (103 lines)
- `addons/pos_sale_stock/i18n/az.po` (102 lines)
- `addons/pos_sale_stock/i18n/bg.po` (102 lines)
- `addons/pos_sale_stock/i18n/bs.po` (103 lines)
- `addons/pos_sale_stock/i18n/ca.po` (102 lines)
- `addons/pos_sale_stock/i18n/cs.po` (102 lines)
- `addons/pos_sale_stock/i18n/da.po` (102 lines)
- `addons/pos_sale_stock/i18n/de.po` (104 lines)
- `addons/pos_sale_stock/i18n/el.po` (102 lines)
- `addons/pos_sale_stock/i18n/es.po` (103 lines)
- `addons/pos_sale_stock/i18n/es_419.po` (104 lines)
- `addons/pos_sale_stock/i18n/et.po` (102 lines)
- `addons/pos_sale_stock/i18n/fa.po` (102 lines)
- `addons/pos_sale_stock/i18n/fi.po` (103 lines)
- `addons/pos_sale_stock/i18n/fr.po` (105 lines)
- `addons/pos_sale_stock/i18n/he.po` (103 lines)
- `addons/pos_sale_stock/i18n/hi.po` (102 lines)
- `addons/pos_sale_stock/i18n/hr.po` (103 lines)
- `addons/pos_sale_stock/i18n/hu.po` (102 lines)
- `addons/pos_sale_stock/i18n/id.po` (102 lines)
- `addons/pos_sale_stock/i18n/it.po` (103 lines)
- `addons/pos_sale_stock/i18n/ja.po` (104 lines)
- `addons/pos_sale_stock/i18n/kab.po` (102 lines)
- `addons/pos_sale_stock/i18n/ko.po` (102 lines)
- `addons/pos_sale_stock/i18n/ku.po` (102 lines)
- `addons/pos_sale_stock/i18n/lo.po` (102 lines)
- `addons/pos_sale_stock/i18n/lt.po` (104 lines)
- `addons/pos_sale_stock/i18n/lv.po` (103 lines)
- `addons/pos_sale_stock/i18n/mn.po` (102 lines)
- `addons/pos_sale_stock/i18n/my.po` (102 lines)
- `addons/pos_sale_stock/i18n/nb.po` (102 lines)
- `addons/pos_sale_stock/i18n/nl.po` (104 lines)
- `addons/pos_sale_stock/i18n/pl.po` (103 lines)
- `addons/pos_sale_stock/i18n/pos_sale_stock.pot` (99 lines)
- `addons/pos_sale_stock/i18n/pt.po` (102 lines)
- `addons/pos_sale_stock/i18n/pt_BR.po` (104 lines)
- `addons/pos_sale_stock/i18n/ro.po` (103 lines)
- `addons/pos_sale_stock/i18n/ru.po` (103 lines)
- `addons/pos_sale_stock/i18n/sk.po` (102 lines)
- `addons/pos_sale_stock/i18n/sl.po` (103 lines)
- `addons/pos_sale_stock/i18n/sr@latin.po` (104 lines)
- `addons/pos_sale_stock/i18n/sv.po` (103 lines)
- `addons/pos_sale_stock/i18n/th.po` (103 lines)
- `addons/pos_sale_stock/i18n/tr.po` (102 lines)
- `addons/pos_sale_stock/i18n/uk.po` (103 lines)
- `addons/pos_sale_stock/i18n/uz.po` (102 lines)
- `addons/pos_sale_stock/i18n/vi.po` (102 lines)
- `addons/pos_sale_stock/i18n/zh_CN.po` (104 lines)
- `addons/pos_sale_stock/i18n/zh_TW.po` (103 lines)
- `addons/pos_sale_stock/models/__init__.py` (4 lines)
- `addons/pos_sale_stock/models/pos_order.py` (63 lines)
- `addons/pos_sale_stock/models/pos_order_line.py` (55 lines)
- `addons/pos_sale_stock/models/sale_order.py` (81 lines)
- `addons/pos_sale_stock/models/stock_picking.py` (18 lines)
- `addons/pos_sale_stock/report/__init__.py` (1 lines)
- `addons/pos_sale_stock/report/sale_report.py` (19 lines)
- `addons/pos_sale_stock/static/src/app/models/pos_order_line.js` (15 lines)
- `addons/pos_sale_stock/static/src/app/services/pos_store.js` (94 lines)
- `addons/pos_sale_stock/static/tests/tours/pos_sale_stock_tour.js` (21 lines)
- `addons/pos_sale_stock/static/tests/unit/data/sale_order.data.js` (81 lines)
- `addons/pos_sale_stock/static/tests/unit/data/sale_order_line.data.js` (100 lines)
- `addons/pos_sale_stock/static/tests/unit/scenarios/pos_sale_stock_flow.test.js` (106 lines)
- `addons/pos_sale_stock/tests/__init__.py` (3 lines)
- `addons/pos_sale_stock/tests/test_pos_sale_flow.py` (1,042 lines)
- `addons/pos_sale_stock/tests/test_pos_sale_lot.py` (135 lines)
- `addons/pos_sale_stock/tests/test_pos_sale_report.py` (80 lines)
- `addons/pos_sale_stock/views/stock_template.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
