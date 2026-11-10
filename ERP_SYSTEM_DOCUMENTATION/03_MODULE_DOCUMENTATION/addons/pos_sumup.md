# Module: pos_sumup

- **Module ID:** MOD-466
- **Path:** `addons/pos_sumup`
- **Manifest:** `addons/pos_sumup/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a SumUp payment terminal

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

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
      "pos_sumup/static/src/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_sumup/static/src/app/utils/payment/payment_sumup.js",
      "pos_sumup/static/src/app/models/pos_payment.js"
    ],
    "web.assets_unit_tests": [
      "pos_sumup/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_sumup/__init__.py` (1 lines)
- `addons/pos_sumup/__manifest__.py` (24 lines)
- `addons/pos_sumup/controllers/__init__.py` (1 lines)
- `addons/pos_sumup/controllers/webhook.py` (47 lines)
- `addons/pos_sumup/i18n/ar.po` (157 lines)
- `addons/pos_sumup/i18n/az.po` (157 lines)
- `addons/pos_sumup/i18n/bg.po` (157 lines)
- `addons/pos_sumup/i18n/bs.po` (157 lines)
- `addons/pos_sumup/i18n/ca.po` (157 lines)
- `addons/pos_sumup/i18n/cs.po` (157 lines)
- `addons/pos_sumup/i18n/da.po` (157 lines)
- `addons/pos_sumup/i18n/de.po` (175 lines)
- `addons/pos_sumup/i18n/el.po` (157 lines)
- `addons/pos_sumup/i18n/es.po` (161 lines)
- `addons/pos_sumup/i18n/es_419.po` (157 lines)
- `addons/pos_sumup/i18n/et.po` (157 lines)
- `addons/pos_sumup/i18n/fa.po` (157 lines)
- `addons/pos_sumup/i18n/fi.po` (161 lines)
- `addons/pos_sumup/i18n/fr.po` (157 lines)
- `addons/pos_sumup/i18n/he.po` (157 lines)
- `addons/pos_sumup/i18n/hi.po` (157 lines)
- `addons/pos_sumup/i18n/hr.po` (157 lines)
- `addons/pos_sumup/i18n/hu.po` (157 lines)
- `addons/pos_sumup/i18n/id.po` (157 lines)
- `addons/pos_sumup/i18n/it.po` (157 lines)
- `addons/pos_sumup/i18n/ja.po` (157 lines)
- `addons/pos_sumup/i18n/kab.po` (157 lines)
- `addons/pos_sumup/i18n/ko.po` (157 lines)
- `addons/pos_sumup/i18n/ku.po` (157 lines)
- `addons/pos_sumup/i18n/lo.po` (166 lines)
- `addons/pos_sumup/i18n/lt.po` (157 lines)
- `addons/pos_sumup/i18n/lv.po` (157 lines)
- `addons/pos_sumup/i18n/mn.po` (157 lines)
- `addons/pos_sumup/i18n/my.po` (157 lines)
- `addons/pos_sumup/i18n/nb.po` (157 lines)
- `addons/pos_sumup/i18n/nl.po` (170 lines)
- `addons/pos_sumup/i18n/pl.po` (157 lines)
- `addons/pos_sumup/i18n/pos_sumup.pot` (157 lines)
- `addons/pos_sumup/i18n/pt.po` (157 lines)
- `addons/pos_sumup/i18n/pt_BR.po` (173 lines)
- `addons/pos_sumup/i18n/ro.po` (157 lines)
- `addons/pos_sumup/i18n/ru.po` (157 lines)
- `addons/pos_sumup/i18n/sk.po` (157 lines)
- `addons/pos_sumup/i18n/sl.po` (157 lines)
- `addons/pos_sumup/i18n/sr@latin.po` (157 lines)
- `addons/pos_sumup/i18n/sv.po` (161 lines)
- `addons/pos_sumup/i18n/th.po` (157 lines)
- `addons/pos_sumup/i18n/tr.po` (157 lines)
- `addons/pos_sumup/i18n/uk.po` (157 lines)
- `addons/pos_sumup/i18n/uz.po` (157 lines)
- `addons/pos_sumup/i18n/vi.po` (157 lines)
- `addons/pos_sumup/i18n/zh_CN.po` (157 lines)
- `addons/pos_sumup/i18n/zh_TW.po` (157 lines)
- `addons/pos_sumup/models/__init__.py` (1 lines)
- `addons/pos_sumup/models/pos_payment_method.py` (271 lines)
- `addons/pos_sumup/static/src/app/models/pos_payment.js` (9 lines)
- `addons/pos_sumup/static/src/app/screens/payment_screen/payment_screen.js` (28 lines)
- `addons/pos_sumup/static/src/app/utils/payment/payment_sumup.js` (128 lines)
- `addons/pos_sumup/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/pos_sumup/static/tests/unit/data/pos_payment_method.data.js` (17 lines)
- `addons/pos_sumup/static/tests/unit/payment_screen.test.js` (64 lines)
- `addons/pos_sumup/static/tests/unit/payment_sumup.test.js` (267 lines)
- `addons/pos_sumup/tests/__init__.py` (3 lines)
- `addons/pos_sumup/tests/test_sumup_payment_method.py` (231 lines)
- `addons/pos_sumup/views/pos_payment_method_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
