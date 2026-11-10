# Module: pos_adyen

- **Module ID:** MOD-423
- **Path:** `addons/pos_adyen`
- **Manifest:** `addons/pos_adyen/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with an Adyen payment terminal

No manifest description declared.

Declared dependencies: `point_of_sale`, `payment_adyen`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "payment_adyen"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_adyen/static/src/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_adyen/static/src/app/utils/payment/payment_adyen.js",
      "pos_adyen/static/src/app/models/pos_payment.js"
    ],
    "web.assets_tests": [
      "pos_adyen/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_adyen/static/tests/unit/data/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_adyen/__init__.py` (5 lines)
- `addons/pos_adyen/__manifest__.py` (29 lines)
- `addons/pos_adyen/controllers/__init__.py` (2 lines)
- `addons/pos_adyen/controllers/main.py` (81 lines)
- `addons/pos_adyen/controllers/payment_adyen.py` (16 lines)
- `addons/pos_adyen/data/neutralize.sql` (3 lines)
- `addons/pos_adyen/i18n/ar.po` (240 lines)
- `addons/pos_adyen/i18n/az.po` (229 lines)
- `addons/pos_adyen/i18n/bg.po` (246 lines)
- `addons/pos_adyen/i18n/bs.po` (230 lines)
- `addons/pos_adyen/i18n/ca.po` (244 lines)
- `addons/pos_adyen/i18n/cs.po` (251 lines)
- `addons/pos_adyen/i18n/da.po` (249 lines)
- `addons/pos_adyen/i18n/de.po` (247 lines)
- `addons/pos_adyen/i18n/el.po` (229 lines)
- `addons/pos_adyen/i18n/es.po` (245 lines)
- `addons/pos_adyen/i18n/es_419.po` (240 lines)
- `addons/pos_adyen/i18n/et.po` (256 lines)
- `addons/pos_adyen/i18n/fa.po` (229 lines)
- `addons/pos_adyen/i18n/fi.po` (234 lines)
- `addons/pos_adyen/i18n/fr.po` (247 lines)
- `addons/pos_adyen/i18n/he.po` (234 lines)
- `addons/pos_adyen/i18n/hi.po` (229 lines)
- `addons/pos_adyen/i18n/hr.po` (233 lines)
- `addons/pos_adyen/i18n/hu.po` (232 lines)
- `addons/pos_adyen/i18n/id.po` (239 lines)
- `addons/pos_adyen/i18n/it.po` (242 lines)
- `addons/pos_adyen/i18n/ja.po` (232 lines)
- `addons/pos_adyen/i18n/kab.po` (229 lines)
- `addons/pos_adyen/i18n/ko.po` (234 lines)
- `addons/pos_adyen/i18n/ku.po` (225 lines)
- `addons/pos_adyen/i18n/lo.po` (234 lines)
- `addons/pos_adyen/i18n/lt.po` (233 lines)
- `addons/pos_adyen/i18n/lv.po` (230 lines)
- `addons/pos_adyen/i18n/mn.po` (232 lines)
- `addons/pos_adyen/i18n/my.po` (226 lines)
- `addons/pos_adyen/i18n/nb.po` (237 lines)
- `addons/pos_adyen/i18n/nl.po` (243 lines)
- `addons/pos_adyen/i18n/pl.po` (248 lines)
- `addons/pos_adyen/i18n/pos_adyen.pot` (220 lines)
- `addons/pos_adyen/i18n/pt.po` (248 lines)
- `addons/pos_adyen/i18n/pt_BR.po` (247 lines)
- `addons/pos_adyen/i18n/ro.po` (268 lines)
- `addons/pos_adyen/i18n/ru.po` (245 lines)
- `addons/pos_adyen/i18n/sk.po` (229 lines)
- `addons/pos_adyen/i18n/sl.po` (228 lines)
- `addons/pos_adyen/i18n/sr@latin.po` (229 lines)
- `addons/pos_adyen/i18n/sv.po` (240 lines)
- `addons/pos_adyen/i18n/th.po` (235 lines)
- `addons/pos_adyen/i18n/tr.po` (245 lines)
- `addons/pos_adyen/i18n/uk.po` (253 lines)
- `addons/pos_adyen/i18n/uz.po` (271 lines)
- `addons/pos_adyen/i18n/vi.po` (252 lines)
- `addons/pos_adyen/i18n/zh_CN.po` (234 lines)
- `addons/pos_adyen/i18n/zh_TW.po` (238 lines)
- `addons/pos_adyen/models/__init__.py` (7 lines)
- `addons/pos_adyen/models/pos_config.py` (20 lines)
- `addons/pos_adyen/models/pos_order.py` (15 lines)
- `addons/pos_adyen/models/pos_payment.py` (19 lines)
- `addons/pos_adyen/models/pos_payment_method.py` (304 lines)
- `addons/pos_adyen/models/res_config_settings.py` (19 lines)
- `addons/pos_adyen/static/src/app/models/pos_payment.js` (27 lines)
- `addons/pos_adyen/static/src/app/screens/payment_screen/payment_screen.js` (47 lines)
- `addons/pos_adyen/static/src/app/utils/payment/payment_adyen.js` (402 lines)
- `addons/pos_adyen/static/tests/tours/adyen_tour.js` (141 lines)
- `addons/pos_adyen/static/tests/unit/data/pos_payment_method.data.js` (12 lines)
- `addons/pos_adyen/tests/__init__.py` (3 lines)
- `addons/pos_adyen/tests/test_basic.py` (86 lines)
- `addons/pos_adyen/views/pos_payment_method_views.xml` (23 lines)
- `addons/pos_adyen/views/res_config_settings_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
