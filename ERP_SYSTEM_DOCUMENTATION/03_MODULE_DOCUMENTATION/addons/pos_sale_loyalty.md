# Module: pos_sale_loyalty

- **Module ID:** MOD-452
- **Path:** `addons/pos_sale_loyalty`
- **Manifest:** `addons/pos_sale_loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between pos_sale and pos_loyalty


This module correct some behaviors when both module are installed.


Declared dependencies: `pos_sale`, `pos_loyalty`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_sale",
    "pos_loyalty"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_sale_loyalty/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_sale_loyalty/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_sale_loyalty/__init__.py` (4 lines)
- `addons/pos_sale_loyalty/__manifest__.py` (24 lines)
- `addons/pos_sale_loyalty/i18n/ar.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/az.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/bg.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/bs.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/ca.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/cs.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/da.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/de.po` (66 lines)
- `addons/pos_sale_loyalty/i18n/el.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/es.po` (63 lines)
- `addons/pos_sale_loyalty/i18n/es_419.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/et.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/fa.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/fi.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/fr.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/he.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/hi.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/hr.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/hu.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/id.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/it.po` (63 lines)
- `addons/pos_sale_loyalty/i18n/ja.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/kab.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/ko.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/ku.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/lo.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/lt.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/lv.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/mn.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/my.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/nb.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/nl.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/pl.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/pos_sale_loyalty.pot` (55 lines)
- `addons/pos_sale_loyalty/i18n/pt.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/pt_BR.po` (67 lines)
- `addons/pos_sale_loyalty/i18n/ro.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/ru.po` (62 lines)
- `addons/pos_sale_loyalty/i18n/sk.po` (58 lines)
- `addons/pos_sale_loyalty/i18n/sl.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/sr@latin.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/sv.po` (60 lines)
- `addons/pos_sale_loyalty/i18n/th.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/tr.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/uk.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/uz.po` (69 lines)
- `addons/pos_sale_loyalty/i18n/vi.po` (59 lines)
- `addons/pos_sale_loyalty/i18n/zh_CN.po` (65 lines)
- `addons/pos_sale_loyalty/i18n/zh_TW.po` (61 lines)
- `addons/pos_sale_loyalty/models/__init__.py` (5 lines)
- `addons/pos_sale_loyalty/models/loyalty_rule.py` (11 lines)
- `addons/pos_sale_loyalty/models/sale_order.py` (13 lines)
- `addons/pos_sale_loyalty/static/src/overrides/components/control_buttons/control_buttons.js` (11 lines)
- `addons/pos_sale_loyalty/static/src/overrides/models/loyalty_rule.js` (8 lines)
- `addons/pos_sale_loyalty/static/src/overrides/models/pos_store.js` (17 lines)
- `addons/pos_sale_loyalty/static/src/overrides/pos_store.js` (13 lines)
- `addons/pos_sale_loyalty/static/tests/tours/pos_sale_loyalty_tour.js` (48 lines)
- `addons/pos_sale_loyalty/tests/__init__.py` (4 lines)
- `addons/pos_sale_loyalty/tests/test_pos_sale_loyalty.py` (160 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
