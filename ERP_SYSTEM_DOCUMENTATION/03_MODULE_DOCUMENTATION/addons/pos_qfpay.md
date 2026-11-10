# Module: pos_qfpay

- **Module ID:** MOD-444
- **Path:** `addons/pos_qfpay`
- **Manifest:** `addons/pos_qfpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with the QFPay terminal in Hong Kong

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
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
      "pos_qfpay/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_qfpay/static/src/app/qfpay.js",
      "pos_qfpay/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_qfpay/__init__.py` (3 lines)
- `addons/pos_qfpay/__manifest__.py` (22 lines)
- `addons/pos_qfpay/controllers/__init__.py` (2 lines)
- `addons/pos_qfpay/controllers/main.py` (49 lines)
- `addons/pos_qfpay/data/neutralize.sql` (3 lines)
- `addons/pos_qfpay/i18n/ar.po` (191 lines)
- `addons/pos_qfpay/i18n/az.po` (184 lines)
- `addons/pos_qfpay/i18n/bg.po` (184 lines)
- `addons/pos_qfpay/i18n/bs.po` (186 lines)
- `addons/pos_qfpay/i18n/ca.po` (185 lines)
- `addons/pos_qfpay/i18n/cs.po` (185 lines)
- `addons/pos_qfpay/i18n/da.po` (184 lines)
- `addons/pos_qfpay/i18n/de.po` (198 lines)
- `addons/pos_qfpay/i18n/el.po` (184 lines)
- `addons/pos_qfpay/i18n/es.po` (195 lines)
- `addons/pos_qfpay/i18n/es_419.po` (197 lines)
- `addons/pos_qfpay/i18n/et.po` (184 lines)
- `addons/pos_qfpay/i18n/fa.po` (184 lines)
- `addons/pos_qfpay/i18n/fi.po` (190 lines)
- `addons/pos_qfpay/i18n/fr.po` (199 lines)
- `addons/pos_qfpay/i18n/he.po` (185 lines)
- `addons/pos_qfpay/i18n/hi.po` (184 lines)
- `addons/pos_qfpay/i18n/hr.po` (185 lines)
- `addons/pos_qfpay/i18n/hu.po` (184 lines)
- `addons/pos_qfpay/i18n/id.po` (192 lines)
- `addons/pos_qfpay/i18n/it.po` (198 lines)
- `addons/pos_qfpay/i18n/ja.po` (193 lines)
- `addons/pos_qfpay/i18n/kab.po` (185 lines)
- `addons/pos_qfpay/i18n/ko.po` (185 lines)
- `addons/pos_qfpay/i18n/ku.po` (184 lines)
- `addons/pos_qfpay/i18n/lo.po` (184 lines)
- `addons/pos_qfpay/i18n/lt.po` (186 lines)
- `addons/pos_qfpay/i18n/lv.po` (185 lines)
- `addons/pos_qfpay/i18n/mn.po` (184 lines)
- `addons/pos_qfpay/i18n/my.po` (185 lines)
- `addons/pos_qfpay/i18n/nb.po` (184 lines)
- `addons/pos_qfpay/i18n/nl.po` (198 lines)
- `addons/pos_qfpay/i18n/pl.po` (198 lines)
- `addons/pos_qfpay/i18n/pos_qfpay.pot` (181 lines)
- `addons/pos_qfpay/i18n/pt.po` (184 lines)
- `addons/pos_qfpay/i18n/pt_BR.po` (196 lines)
- `addons/pos_qfpay/i18n/ro.po` (196 lines)
- `addons/pos_qfpay/i18n/ru.po` (191 lines)
- `addons/pos_qfpay/i18n/sk.po` (184 lines)
- `addons/pos_qfpay/i18n/sl.po` (185 lines)
- `addons/pos_qfpay/i18n/sr@latin.po` (185 lines)
- `addons/pos_qfpay/i18n/sv.po` (185 lines)
- `addons/pos_qfpay/i18n/th.po` (185 lines)
- `addons/pos_qfpay/i18n/tr.po` (197 lines)
- `addons/pos_qfpay/i18n/uk.po` (185 lines)
- `addons/pos_qfpay/i18n/uz.po` (225 lines)
- `addons/pos_qfpay/i18n/vi.po` (190 lines)
- `addons/pos_qfpay/i18n/zh_CN.po` (188 lines)
- `addons/pos_qfpay/i18n/zh_TW.po` (188 lines)
- `addons/pos_qfpay/models/__init__.py` (2 lines)
- `addons/pos_qfpay/models/pos_payment_method.py` (83 lines)
- `addons/pos_qfpay/static/src/app/payment_qfpay.js` (166 lines)
- `addons/pos_qfpay/static/src/app/qfpay.js` (64 lines)
- `addons/pos_qfpay/static/src/app/services/pos_store.js` (14 lines)
- `addons/pos_qfpay/static/tests/tours/qfpay_tour.js` (99 lines)
- `addons/pos_qfpay/static/tests/tours/utils/common.js` (73 lines)
- `addons/pos_qfpay/tests/__init__.py` (3 lines)
- `addons/pos_qfpay/tests/test_basic.py` (33 lines)
- `addons/pos_qfpay/views/pos_payment_method_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
