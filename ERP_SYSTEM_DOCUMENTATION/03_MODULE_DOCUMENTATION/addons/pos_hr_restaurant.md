# Module: pos_hr_restaurant

- **Module ID:** MOD-434
- **Path:** `addons/pos_hr_restaurant`
- **Manifest:** `addons/pos_hr_restaurant/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between pos_hr and pos_restaurant


This module adapts the behavior of the PoS when the pos_hr and pos_restaurant are installed.


Declared dependencies: `pos_hr`, `pos_restaurant`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_hr",
    "pos_restaurant"
  ],
  "assets": {
    "web.assets_tests": [
      "pos_hr_restaurant/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_hr_restaurant/__init__.py` (2 lines)
- `addons/pos_hr_restaurant/__manifest__.py` (20 lines)
- `addons/pos_hr_restaurant/i18n/ar.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/az.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/bg.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/bs.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/ca.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/cs.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/da.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/de.po` (40 lines)
- `addons/pos_hr_restaurant/i18n/el.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/es.po` (40 lines)
- `addons/pos_hr_restaurant/i18n/es_419.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/et.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/fa.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/fi.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/fr.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/he.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/hi.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/hr.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/hu.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/id.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/it.po` (40 lines)
- `addons/pos_hr_restaurant/i18n/ja.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/kab.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/ko.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/ku.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/lo.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/lt.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/lv.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/mn.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/my.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/nb.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/nl.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/pl.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/pos_hr_restaurant.pot` (33 lines)
- `addons/pos_hr_restaurant/i18n/pt.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/pt_BR.po` (41 lines)
- `addons/pos_hr_restaurant/i18n/ro.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/ru.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/sk.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/sl.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/sr@latin.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/sv.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/th.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/tr.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/uk.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/uz.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/vi.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/zh_CN.po` (33 lines)
- `addons/pos_hr_restaurant/i18n/zh_TW.po` (33 lines)
- `addons/pos_hr_restaurant/static/tests/tours/pos_hr_restaurant_tour.js` (49 lines)
- `addons/pos_hr_restaurant/tests/__init__.py` (3 lines)
- `addons/pos_hr_restaurant/tests/test_frontend.py` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
