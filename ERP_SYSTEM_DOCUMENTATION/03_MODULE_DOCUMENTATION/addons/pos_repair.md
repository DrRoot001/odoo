# Module: pos_repair

- **Module ID:** MOD-446
- **Path:** `addons/pos_repair`
- **Manifest:** `addons/pos_repair/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and Repair

No manifest description declared.

Declared dependencies: `pos_stock`, `repair`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_stock",
    "repair"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_repair/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_repair/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_repair/__init__.py` (2 lines)
- `addons/pos_repair/__manifest__.py` (19 lines)
- `addons/pos_repair/i18n/ar.po` (58 lines)
- `addons/pos_repair/i18n/az.po` (56 lines)
- `addons/pos_repair/i18n/bg.po` (56 lines)
- `addons/pos_repair/i18n/bs.po` (58 lines)
- `addons/pos_repair/i18n/ca.po` (56 lines)
- `addons/pos_repair/i18n/cs.po` (57 lines)
- `addons/pos_repair/i18n/da.po` (56 lines)
- `addons/pos_repair/i18n/de.po` (57 lines)
- `addons/pos_repair/i18n/el.po` (56 lines)
- `addons/pos_repair/i18n/es.po` (57 lines)
- `addons/pos_repair/i18n/es_419.po` (58 lines)
- `addons/pos_repair/i18n/et.po` (56 lines)
- `addons/pos_repair/i18n/fa.po` (56 lines)
- `addons/pos_repair/i18n/fi.po` (57 lines)
- `addons/pos_repair/i18n/fr.po` (57 lines)
- `addons/pos_repair/i18n/he.po` (57 lines)
- `addons/pos_repair/i18n/hi.po` (56 lines)
- `addons/pos_repair/i18n/hr.po` (57 lines)
- `addons/pos_repair/i18n/hu.po` (56 lines)
- `addons/pos_repair/i18n/id.po` (57 lines)
- `addons/pos_repair/i18n/it.po` (57 lines)
- `addons/pos_repair/i18n/ja.po` (57 lines)
- `addons/pos_repair/i18n/kab.po` (57 lines)
- `addons/pos_repair/i18n/ko.po` (57 lines)
- `addons/pos_repair/i18n/ku.po` (56 lines)
- `addons/pos_repair/i18n/lo.po` (56 lines)
- `addons/pos_repair/i18n/lt.po` (58 lines)
- `addons/pos_repair/i18n/lv.po` (57 lines)
- `addons/pos_repair/i18n/mn.po` (56 lines)
- `addons/pos_repair/i18n/my.po` (56 lines)
- `addons/pos_repair/i18n/nb.po` (56 lines)
- `addons/pos_repair/i18n/nl.po` (58 lines)
- `addons/pos_repair/i18n/pl.po` (58 lines)
- `addons/pos_repair/i18n/pos_repair.pot` (53 lines)
- `addons/pos_repair/i18n/pt.po` (56 lines)
- `addons/pos_repair/i18n/pt_BR.po` (60 lines)
- `addons/pos_repair/i18n/ro.po` (58 lines)
- `addons/pos_repair/i18n/ru.po` (58 lines)
- `addons/pos_repair/i18n/sk.po` (56 lines)
- `addons/pos_repair/i18n/sl.po` (57 lines)
- `addons/pos_repair/i18n/sr@latin.po` (57 lines)
- `addons/pos_repair/i18n/sv.po` (57 lines)
- `addons/pos_repair/i18n/th.po` (57 lines)
- `addons/pos_repair/i18n/tr.po` (59 lines)
- `addons/pos_repair/i18n/uk.po` (57 lines)
- `addons/pos_repair/i18n/uz.po` (69 lines)
- `addons/pos_repair/i18n/vi.po` (57 lines)
- `addons/pos_repair/i18n/zh_CN.po` (57 lines)
- `addons/pos_repair/i18n/zh_TW.po` (61 lines)
- `addons/pos_repair/models/__init__.py` (3 lines)
- `addons/pos_repair/models/sale_order_line.py` (20 lines)
- `addons/pos_repair/models/stock_picking.py` (10 lines)
- `addons/pos_repair/static/src/overrides/pos_store.js` (13 lines)
- `addons/pos_repair/static/tests/tours/pos_repair_tour.js` (15 lines)
- `addons/pos_repair/tests/__init__.py` (2 lines)
- `addons/pos_repair/tests/test_frontend.py` (37 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
