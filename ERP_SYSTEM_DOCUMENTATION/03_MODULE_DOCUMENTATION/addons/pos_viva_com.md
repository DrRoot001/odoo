# Module: pos_viva_com

- **Module ID:** MOD-467
- **Path:** `addons/pos_viva_com`
- **Manifest:** `addons/pos_viva_com/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your PoS with a Viva.com payment terminal

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_viva_com/static/src/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_viva_com/static/src/app/utils/error_messages.js",
      "pos_viva_com/static/src/app/payment_viva_com.js",
      "pos_viva_com/static/src/overrides/models/pos_payment.js"
    ],
    "web.assets_tests": [
      "pos_viva_com/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_viva_com/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_viva_com/__init__.py` (5 lines)
- `addons/pos_viva_com/__manifest__.py` (28 lines)
- `addons/pos_viva_com/controllers/__init__.py` (2 lines)
- `addons/pos_viva_com/controllers/main.py` (141 lines)
- `addons/pos_viva_com/data/neutralize.sql` (2 lines)
- `addons/pos_viva_com/i18n/ar.po` (388 lines)
- `addons/pos_viva_com/i18n/az.po` (379 lines)
- `addons/pos_viva_com/i18n/bg.po` (381 lines)
- `addons/pos_viva_com/i18n/bs.po` (384 lines)
- `addons/pos_viva_com/i18n/ca.po` (386 lines)
- `addons/pos_viva_com/i18n/cs.po` (383 lines)
- `addons/pos_viva_com/i18n/da.po` (393 lines)
- `addons/pos_viva_com/i18n/de.po` (428 lines)
- `addons/pos_viva_com/i18n/el.po` (379 lines)
- `addons/pos_viva_com/i18n/es.po` (400 lines)
- `addons/pos_viva_com/i18n/es_419.po` (401 lines)
- `addons/pos_viva_com/i18n/et.po` (381 lines)
- `addons/pos_viva_com/i18n/fa.po` (379 lines)
- `addons/pos_viva_com/i18n/fi.po` (399 lines)
- `addons/pos_viva_com/i18n/fr.po` (411 lines)
- `addons/pos_viva_com/i18n/he.po` (381 lines)
- `addons/pos_viva_com/i18n/hi.po` (381 lines)
- `addons/pos_viva_com/i18n/hr.po` (381 lines)
- `addons/pos_viva_com/i18n/hu.po` (379 lines)
- `addons/pos_viva_com/i18n/id.po` (399 lines)
- `addons/pos_viva_com/i18n/it.po` (409 lines)
- `addons/pos_viva_com/i18n/ja.po` (392 lines)
- `addons/pos_viva_com/i18n/kab.po` (382 lines)
- `addons/pos_viva_com/i18n/ko.po` (385 lines)
- `addons/pos_viva_com/i18n/ku.po` (378 lines)
- `addons/pos_viva_com/i18n/lo.po` (387 lines)
- `addons/pos_viva_com/i18n/lt.po` (381 lines)
- `addons/pos_viva_com/i18n/lv.po` (384 lines)
- `addons/pos_viva_com/i18n/mn.po` (379 lines)
- `addons/pos_viva_com/i18n/my.po` (379 lines)
- `addons/pos_viva_com/i18n/nb.po` (380 lines)
- `addons/pos_viva_com/i18n/nl.po` (407 lines)
- `addons/pos_viva_com/i18n/pl.po` (411 lines)
- `addons/pos_viva_com/i18n/pos_viva_com.pot` (374 lines)
- `addons/pos_viva_com/i18n/pt.po` (406 lines)
- `addons/pos_viva_com/i18n/pt_BR.po` (423 lines)
- `addons/pos_viva_com/i18n/ro.po` (390 lines)
- `addons/pos_viva_com/i18n/ru.po` (393 lines)
- `addons/pos_viva_com/i18n/sk.po` (385 lines)
- `addons/pos_viva_com/i18n/sl.po` (383 lines)
- `addons/pos_viva_com/i18n/sr@latin.po` (380 lines)
- `addons/pos_viva_com/i18n/sv.po` (388 lines)
- `addons/pos_viva_com/i18n/th.po` (383 lines)
- `addons/pos_viva_com/i18n/tr.po` (396 lines)
- `addons/pos_viva_com/i18n/uk.po` (384 lines)
- `addons/pos_viva_com/i18n/uz.po` (445 lines)
- `addons/pos_viva_com/i18n/vi.po` (389 lines)
- `addons/pos_viva_com/i18n/zh_CN.po` (387 lines)
- `addons/pos_viva_com/i18n/zh_TW.po` (387 lines)
- `addons/pos_viva_com/models/__init__.py` (5 lines)
- `addons/pos_viva_com/models/pos_payment.py` (65 lines)
- `addons/pos_viva_com/models/pos_payment_method.py` (338 lines)
- `addons/pos_viva_com/static/src/app/hooks/use_viva_app.js` (198 lines)
- `addons/pos_viva_com/static/src/app/payment_viva_com.js` (250 lines)
- `addons/pos_viva_com/static/src/app/screens/payment_screen/payment_lines/payment_lines.js` (52 lines)
- `addons/pos_viva_com/static/src/app/screens/payment_screen/payment_screen.js` (115 lines)
- `addons/pos_viva_com/static/src/app/utils/error_messages.js` (21 lines)
- `addons/pos_viva_com/static/src/overrides/models/pos_payment.js` (17 lines)
- `addons/pos_viva_com/static/tests/tours/utils/payment_screen_viva_com_util.js` (20 lines)
- `addons/pos_viva_com/static/tests/tours/viva_com_tour.js` (77 lines)
- `addons/pos_viva_com/static/tests/unit/app/payment_lines.test.js` (119 lines)
- `addons/pos_viva_com/static/tests/unit/app/payment_screen.test.js` (33 lines)
- `addons/pos_viva_com/static/tests/unit/data/pos_payment_method.data.js` (8 lines)
- `addons/pos_viva_com/tests/__init__.py` (2 lines)
- `addons/pos_viva_com/tests/test_frontend.py` (97 lines)
- `addons/pos_viva_com/tests/test_pos_payment_method.py` (50 lines)
- `addons/pos_viva_com/views/pos_payment_method_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
