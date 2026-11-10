# Module: pos_razorpay

- **Module ID:** MOD-445
- **Path:** `addons/pos_razorpay`
- **Manifest:** `addons/pos_razorpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with a Razorpay payment terminal


Allow Razorpay POS payments
==============================

This module allows customers to pay for their orders with debit/credit
cards and UPI. The transactions are processed by Razorpay POS. A Razorpay merchant account is necessary. It allows the
following:

* Fast payment by just swiping/scanning a credit/debit card or a QR code while on the payment screen
* Supported cards: Visa, MasterCard, Rupay, UPI
    

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

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
      "pos_razorpay/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_razorpay/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_razorpay/__init__.py` (1 lines)
- `addons/pos_razorpay/__manifest__.py` (32 lines)
- `addons/pos_razorpay/data/neutralize.sql` (3 lines)
- `addons/pos_razorpay/i18n/ar.po` (320 lines)
- `addons/pos_razorpay/i18n/az.po` (292 lines)
- `addons/pos_razorpay/i18n/bg.po` (292 lines)
- `addons/pos_razorpay/i18n/bs.po` (294 lines)
- `addons/pos_razorpay/i18n/ca.po` (300 lines)
- `addons/pos_razorpay/i18n/cs.po` (295 lines)
- `addons/pos_razorpay/i18n/da.po` (323 lines)
- `addons/pos_razorpay/i18n/de.po` (336 lines)
- `addons/pos_razorpay/i18n/el.po` (293 lines)
- `addons/pos_razorpay/i18n/es.po` (336 lines)
- `addons/pos_razorpay/i18n/es_419.po` (335 lines)
- `addons/pos_razorpay/i18n/et.po` (292 lines)
- `addons/pos_razorpay/i18n/fa.po` (292 lines)
- `addons/pos_razorpay/i18n/fi.po` (313 lines)
- `addons/pos_razorpay/i18n/fr.po` (324 lines)
- `addons/pos_razorpay/i18n/he.po` (293 lines)
- `addons/pos_razorpay/i18n/hi.po` (292 lines)
- `addons/pos_razorpay/i18n/hr.po` (293 lines)
- `addons/pos_razorpay/i18n/hu.po` (293 lines)
- `addons/pos_razorpay/i18n/id.po` (320 lines)
- `addons/pos_razorpay/i18n/it.po` (337 lines)
- `addons/pos_razorpay/i18n/ja.po` (310 lines)
- `addons/pos_razorpay/i18n/kab.po` (293 lines)
- `addons/pos_razorpay/i18n/ko.po` (307 lines)
- `addons/pos_razorpay/i18n/ku.po` (292 lines)
- `addons/pos_razorpay/i18n/lo.po` (292 lines)
- `addons/pos_razorpay/i18n/lt.po` (294 lines)
- `addons/pos_razorpay/i18n/lv.po` (293 lines)
- `addons/pos_razorpay/i18n/mn.po` (292 lines)
- `addons/pos_razorpay/i18n/my.po` (292 lines)
- `addons/pos_razorpay/i18n/nb.po` (293 lines)
- `addons/pos_razorpay/i18n/nl.po` (322 lines)
- `addons/pos_razorpay/i18n/pl.po` (322 lines)
- `addons/pos_razorpay/i18n/pos_razorpay.pot` (287 lines)
- `addons/pos_razorpay/i18n/pt.po` (322 lines)
- `addons/pos_razorpay/i18n/pt_BR.po` (336 lines)
- `addons/pos_razorpay/i18n/ro.po` (322 lines)
- `addons/pos_razorpay/i18n/ru.po` (319 lines)
- `addons/pos_razorpay/i18n/sk.po` (292 lines)
- `addons/pos_razorpay/i18n/sl.po` (294 lines)
- `addons/pos_razorpay/i18n/sr@latin.po` (293 lines)
- `addons/pos_razorpay/i18n/sv.po` (311 lines)
- `addons/pos_razorpay/i18n/th.po` (305 lines)
- `addons/pos_razorpay/i18n/tr.po` (318 lines)
- `addons/pos_razorpay/i18n/uk.po` (293 lines)
- `addons/pos_razorpay/i18n/uz.po` (353 lines)
- `addons/pos_razorpay/i18n/vi.po` (317 lines)
- `addons/pos_razorpay/i18n/zh_CN.po` (313 lines)
- `addons/pos_razorpay/i18n/zh_TW.po` (305 lines)
- `addons/pos_razorpay/models/__init__.py` (2 lines)
- `addons/pos_razorpay/models/pos_payment.py` (8 lines)
- `addons/pos_razorpay/models/pos_payment_method.py` (123 lines)
- `addons/pos_razorpay/models/razorpay_pos_request.py` (64 lines)
- `addons/pos_razorpay/static/src/app/screens/payment_screen/payment_screen.js` (66 lines)
- `addons/pos_razorpay/static/src/app/services/pos_store.js` (62 lines)
- `addons/pos_razorpay/static/src/app/utls/payment/payment_razorpay.js` (314 lines)
- `addons/pos_razorpay/static/src/overrides/models/pos_payment.js` (21 lines)
- `addons/pos_razorpay/static/tests/tours/razorpay_tour.js` (59 lines)
- `addons/pos_razorpay/tests/__init__.py` (1 lines)
- `addons/pos_razorpay/tests/test_basic.py` (158 lines)
- `addons/pos_razorpay/views/pos_payment_method_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
