# Module: pos_restaurant_loyalty

- **Module ID:** MOD-448
- **Path:** `addons/pos_restaurant_loyalty`
- **Manifest:** `addons/pos_restaurant_loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between pos_restaurant and pos_loyalty


This module correct some behaviors when both module are installed.


Declared dependencies: `pos_restaurant`, `pos_loyalty`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_restaurant",
    "pos_loyalty"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_restaurant_loyalty/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_restaurant_loyalty/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_restaurant_loyalty/__init__.py` (1 lines)
- `addons/pos_restaurant_loyalty/__manifest__.py` (24 lines)
- `addons/pos_restaurant_loyalty/i18n/ar.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/az.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/bg.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/bs.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/ca.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/cs.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/da.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/de.po` (44 lines)
- `addons/pos_restaurant_loyalty/i18n/el.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/es.po` (40 lines)
- `addons/pos_restaurant_loyalty/i18n/es_419.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/et.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/fa.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/fi.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/fr.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/he.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/hi.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/hr.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/hu.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/id.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/it.po` (40 lines)
- `addons/pos_restaurant_loyalty/i18n/ja.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/kab.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/ko.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/ku.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/lo.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/lt.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/lv.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/mn.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/my.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/nb.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/nl.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/pl.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/pos_restaurant_loyalty.pot` (33 lines)
- `addons/pos_restaurant_loyalty/i18n/pt.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/pt_BR.po` (41 lines)
- `addons/pos_restaurant_loyalty/i18n/ro.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/ru.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/sk.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/sl.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/sr@latin.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/sv.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/th.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/tr.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/uk.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/uz.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/vi.po` (34 lines)
- `addons/pos_restaurant_loyalty/i18n/zh_CN.po` (39 lines)
- `addons/pos_restaurant_loyalty/i18n/zh_TW.po` (34 lines)
- `addons/pos_restaurant_loyalty/static/src/overrides/models/loyalty_reward.js` (16 lines)
- `addons/pos_restaurant_loyalty/static/src/overrides/models/pos_store.js` (12 lines)
- `addons/pos_restaurant_loyalty/static/tests/tours/PosRestaurantLoyaltyTour.js` (45 lines)
- `addons/pos_restaurant_loyalty/tests/__init__.py` (3 lines)
- `addons/pos_restaurant_loyalty/tests/test_pos_restaurant_loyalty.py` (64 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
