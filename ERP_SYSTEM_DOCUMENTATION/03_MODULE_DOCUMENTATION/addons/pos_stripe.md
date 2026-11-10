# Module: pos_stripe

- **Module ID:** MOD-465
- **Path:** `addons/pos_stripe`
- **Manifest:** `addons/pos_stripe/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a Stripe payment terminal

No manifest description declared.

Declared dependencies: `point_of_sale`, `payment_stripe`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "payment_stripe"
  ],
  "data": [
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_stripe/static/src/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_stripe/static/src/app/payment_stripe.js",
      "pos_stripe/static/src/overrides/models/pos_payment.js"
    ],
    "web.assets_unit_tests": [
      "pos_stripe/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_stripe/__init__.py` (4 lines)
- `addons/pos_stripe/__manifest__.py` (25 lines)
- `addons/pos_stripe/i18n/ar.po` (191 lines)
- `addons/pos_stripe/i18n/az.po` (187 lines)
- `addons/pos_stripe/i18n/bg.po` (187 lines)
- `addons/pos_stripe/i18n/bs.po` (188 lines)
- `addons/pos_stripe/i18n/ca.po` (194 lines)
- `addons/pos_stripe/i18n/cs.po` (188 lines)
- `addons/pos_stripe/i18n/da.po` (190 lines)
- `addons/pos_stripe/i18n/de.po` (193 lines)
- `addons/pos_stripe/i18n/el.po` (188 lines)
- `addons/pos_stripe/i18n/es.po` (194 lines)
- `addons/pos_stripe/i18n/es_419.po` (196 lines)
- `addons/pos_stripe/i18n/et.po` (189 lines)
- `addons/pos_stripe/i18n/fa.po` (187 lines)
- `addons/pos_stripe/i18n/fi.po` (191 lines)
- `addons/pos_stripe/i18n/fr.po` (193 lines)
- `addons/pos_stripe/i18n/he.po` (188 lines)
- `addons/pos_stripe/i18n/hi.po` (187 lines)
- `addons/pos_stripe/i18n/hr.po` (188 lines)
- `addons/pos_stripe/i18n/hu.po` (188 lines)
- `addons/pos_stripe/i18n/id.po` (192 lines)
- `addons/pos_stripe/i18n/it.po` (195 lines)
- `addons/pos_stripe/i18n/ja.po` (188 lines)
- `addons/pos_stripe/i18n/kab.po` (187 lines)
- `addons/pos_stripe/i18n/ko.po` (189 lines)
- `addons/pos_stripe/i18n/ku.po` (187 lines)
- `addons/pos_stripe/i18n/lo.po` (187 lines)
- `addons/pos_stripe/i18n/lt.po` (189 lines)
- `addons/pos_stripe/i18n/lv.po` (187 lines)
- `addons/pos_stripe/i18n/mn.po` (187 lines)
- `addons/pos_stripe/i18n/my.po` (187 lines)
- `addons/pos_stripe/i18n/nb.po` (189 lines)
- `addons/pos_stripe/i18n/nl.po` (191 lines)
- `addons/pos_stripe/i18n/pl.po` (193 lines)
- `addons/pos_stripe/i18n/pos_stripe.pot` (183 lines)
- `addons/pos_stripe/i18n/pt.po` (192 lines)
- `addons/pos_stripe/i18n/pt_BR.po` (193 lines)
- `addons/pos_stripe/i18n/ro.po` (192 lines)
- `addons/pos_stripe/i18n/ru.po` (195 lines)
- `addons/pos_stripe/i18n/sk.po` (186 lines)
- `addons/pos_stripe/i18n/sl.po` (188 lines)
- `addons/pos_stripe/i18n/sr@latin.po` (188 lines)
- `addons/pos_stripe/i18n/sv.po` (191 lines)
- `addons/pos_stripe/i18n/th.po` (187 lines)
- `addons/pos_stripe/i18n/tr.po` (192 lines)
- `addons/pos_stripe/i18n/uk.po` (192 lines)
- `addons/pos_stripe/i18n/uz.po` (214 lines)
- `addons/pos_stripe/i18n/vi.po` (191 lines)
- `addons/pos_stripe/i18n/zh_CN.po` (189 lines)
- `addons/pos_stripe/i18n/zh_TW.po` (190 lines)
- `addons/pos_stripe/models/__init__.py` (4 lines)
- `addons/pos_stripe/models/pos_payment_method.py` (140 lines)
- `addons/pos_stripe/static/src/app/payment_stripe.js` (459 lines)
- `addons/pos_stripe/static/src/overrides/models/pos_payment.js` (19 lines)
- `addons/pos_stripe/static/src/overrides/screens/payment_screen.js` (28 lines)
- `addons/pos_stripe/static/src/overrides/screens/tip_screen.js` (17 lines)
- `addons/pos_stripe/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/pos_stripe/static/tests/unit/data/pos_payment_method.data.js` (23 lines)
- `addons/pos_stripe/static/tests/unit/payment_stripe.test.js` (205 lines)
- `addons/pos_stripe/tests/__init__.py` (1 lines)
- `addons/pos_stripe/tests/test_pos_payment_method.py` (129 lines)
- `addons/pos_stripe/views/pos_payment_method_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
