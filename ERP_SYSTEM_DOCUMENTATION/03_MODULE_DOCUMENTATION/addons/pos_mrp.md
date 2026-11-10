# Module: pos_mrp

- **Module ID:** MOD-439
- **Path:** `addons/pos_mrp`
- **Manifest:** `addons/pos_mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and Mrp


This is a link module between Point of Sale and Mrp.


Declared dependencies: `pos_stock`, `mrp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_stock",
    "mrp"
  ],
  "data": [
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "pos_mrp/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_mrp/__init__.py` (4 lines)
- `addons/pos_mrp/__manifest__.py` (24 lines)
- `addons/pos_mrp/i18n/ar.po` (68 lines)
- `addons/pos_mrp/i18n/az.po` (65 lines)
- `addons/pos_mrp/i18n/bg.po` (65 lines)
- `addons/pos_mrp/i18n/bs.po` (67 lines)
- `addons/pos_mrp/i18n/ca.po` (66 lines)
- `addons/pos_mrp/i18n/cs.po` (67 lines)
- `addons/pos_mrp/i18n/da.po` (67 lines)
- `addons/pos_mrp/i18n/de.po` (69 lines)
- `addons/pos_mrp/i18n/el.po` (66 lines)
- `addons/pos_mrp/i18n/es.po` (69 lines)
- `addons/pos_mrp/i18n/es_419.po` (68 lines)
- `addons/pos_mrp/i18n/et.po` (65 lines)
- `addons/pos_mrp/i18n/fa.po` (65 lines)
- `addons/pos_mrp/i18n/fi.po` (67 lines)
- `addons/pos_mrp/i18n/fr.po` (67 lines)
- `addons/pos_mrp/i18n/he.po` (66 lines)
- `addons/pos_mrp/i18n/hi.po` (65 lines)
- `addons/pos_mrp/i18n/hr.po` (66 lines)
- `addons/pos_mrp/i18n/hu.po` (66 lines)
- `addons/pos_mrp/i18n/id.po` (68 lines)
- `addons/pos_mrp/i18n/it.po` (69 lines)
- `addons/pos_mrp/i18n/ja.po` (67 lines)
- `addons/pos_mrp/i18n/kab.po` (66 lines)
- `addons/pos_mrp/i18n/ko.po` (67 lines)
- `addons/pos_mrp/i18n/ku.po` (65 lines)
- `addons/pos_mrp/i18n/lo.po` (65 lines)
- `addons/pos_mrp/i18n/lt.po` (67 lines)
- `addons/pos_mrp/i18n/lv.po` (66 lines)
- `addons/pos_mrp/i18n/mn.po` (65 lines)
- `addons/pos_mrp/i18n/my.po` (65 lines)
- `addons/pos_mrp/i18n/nb.po` (66 lines)
- `addons/pos_mrp/i18n/nl.po` (67 lines)
- `addons/pos_mrp/i18n/pl.po` (68 lines)
- `addons/pos_mrp/i18n/pos_mrp.pot` (62 lines)
- `addons/pos_mrp/i18n/pt.po` (67 lines)
- `addons/pos_mrp/i18n/pt_BR.po` (70 lines)
- `addons/pos_mrp/i18n/ro.po` (67 lines)
- `addons/pos_mrp/i18n/ru.po` (69 lines)
- `addons/pos_mrp/i18n/sk.po` (65 lines)
- `addons/pos_mrp/i18n/sl.po` (67 lines)
- `addons/pos_mrp/i18n/sr@latin.po` (66 lines)
- `addons/pos_mrp/i18n/sv.po` (67 lines)
- `addons/pos_mrp/i18n/th.po` (67 lines)
- `addons/pos_mrp/i18n/tr.po` (67 lines)
- `addons/pos_mrp/i18n/uk.po` (66 lines)
- `addons/pos_mrp/i18n/uz.po` (75 lines)
- `addons/pos_mrp/i18n/vi.po` (66 lines)
- `addons/pos_mrp/i18n/zh_CN.po` (69 lines)
- `addons/pos_mrp/i18n/zh_TW.po` (69 lines)
- `addons/pos_mrp/models/__init__.py` (6 lines)
- `addons/pos_mrp/models/pos_order.py` (21 lines)
- `addons/pos_mrp/models/pos_order_line.py` (18 lines)
- `addons/pos_mrp/models/stock_picking.py` (12 lines)
- `addons/pos_mrp/security/ir.access.csv` (3 lines)
- `addons/pos_mrp/static/tests/tours/pos_mrp_tour.js` (31 lines)
- `addons/pos_mrp/tests/__init__.py` (6 lines)
- `addons/pos_mrp/tests/common.py` (125 lines)
- `addons/pos_mrp/tests/test_frontend.py` (82 lines)
- `addons/pos_mrp/tests/test_pos_mrp_flow.py` (642 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
