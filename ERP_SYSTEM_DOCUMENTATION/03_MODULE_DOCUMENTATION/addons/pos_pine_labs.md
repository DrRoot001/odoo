# Module: pos_pine_labs

- **Module ID:** MOD-443
- **Path:** `addons/pos_pine_labs`
- **Manifest:** `addons/pos_pine_labs/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with Pine Labs payment terminals


Allow Pine Labs POS payments
==============================

This module is available only for companies that use INR currency.
It enables customers to pay for their orders using debit/credit cards and UPI through Pine Labs POS terminals.
A Pine Labs merchant account is required to process transactions.
Features include:

* Quick payments by swiping, scanning, or tapping your credit/debit card or UPI QR code at the payment terminal.
* Supported cards: Visa, MasterCard, RuPay.
    

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
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
    "views/pos_payment_views.xml",
    "views/pos_payment_method_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_pine_labs/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_pine_labs/__init__.py` (1 lines)
- `addons/pos_pine_labs/__manifest__.py` (30 lines)
- `addons/pos_pine_labs/data/neutralize.sql` (4 lines)
- `addons/pos_pine_labs/i18n/ar.po` (232 lines)
- `addons/pos_pine_labs/i18n/az.po` (225 lines)
- `addons/pos_pine_labs/i18n/bg.po` (225 lines)
- `addons/pos_pine_labs/i18n/bs.po` (227 lines)
- `addons/pos_pine_labs/i18n/ca.po` (228 lines)
- `addons/pos_pine_labs/i18n/cs.po` (226 lines)
- `addons/pos_pine_labs/i18n/da.po` (234 lines)
- `addons/pos_pine_labs/i18n/de.po` (253 lines)
- `addons/pos_pine_labs/i18n/el.po` (226 lines)
- `addons/pos_pine_labs/i18n/es.po` (252 lines)
- `addons/pos_pine_labs/i18n/es_419.po` (250 lines)
- `addons/pos_pine_labs/i18n/et.po` (225 lines)
- `addons/pos_pine_labs/i18n/fa.po` (225 lines)
- `addons/pos_pine_labs/i18n/fi.po` (245 lines)
- `addons/pos_pine_labs/i18n/fr.po` (237 lines)
- `addons/pos_pine_labs/i18n/he.po` (226 lines)
- `addons/pos_pine_labs/i18n/hi.po` (225 lines)
- `addons/pos_pine_labs/i18n/hr.po` (226 lines)
- `addons/pos_pine_labs/i18n/hu.po` (226 lines)
- `addons/pos_pine_labs/i18n/id.po` (233 lines)
- `addons/pos_pine_labs/i18n/it.po` (249 lines)
- `addons/pos_pine_labs/i18n/ja.po` (231 lines)
- `addons/pos_pine_labs/i18n/kab.po` (226 lines)
- `addons/pos_pine_labs/i18n/ko.po` (231 lines)
- `addons/pos_pine_labs/i18n/ku.po` (225 lines)
- `addons/pos_pine_labs/i18n/lo.po` (243 lines)
- `addons/pos_pine_labs/i18n/lt.po` (227 lines)
- `addons/pos_pine_labs/i18n/lv.po` (226 lines)
- `addons/pos_pine_labs/i18n/mn.po` (225 lines)
- `addons/pos_pine_labs/i18n/my.po` (226 lines)
- `addons/pos_pine_labs/i18n/nb.po` (226 lines)
- `addons/pos_pine_labs/i18n/nl.po` (241 lines)
- `addons/pos_pine_labs/i18n/pl.po` (236 lines)
- `addons/pos_pine_labs/i18n/pos_pine_labs.pot` (220 lines)
- `addons/pos_pine_labs/i18n/pt.po` (237 lines)
- `addons/pos_pine_labs/i18n/pt_BR.po` (252 lines)
- `addons/pos_pine_labs/i18n/ro.po` (234 lines)
- `addons/pos_pine_labs/i18n/ru.po` (230 lines)
- `addons/pos_pine_labs/i18n/sk.po` (225 lines)
- `addons/pos_pine_labs/i18n/sl.po` (227 lines)
- `addons/pos_pine_labs/i18n/sr@latin.po` (226 lines)
- `addons/pos_pine_labs/i18n/sv.po` (228 lines)
- `addons/pos_pine_labs/i18n/th.po` (227 lines)
- `addons/pos_pine_labs/i18n/tr.po` (233 lines)
- `addons/pos_pine_labs/i18n/uk.po` (226 lines)
- `addons/pos_pine_labs/i18n/uz.po` (276 lines)
- `addons/pos_pine_labs/i18n/vi.po` (228 lines)
- `addons/pos_pine_labs/i18n/zh_CN.po` (241 lines)
- `addons/pos_pine_labs/i18n/zh_TW.po` (232 lines)
- `addons/pos_pine_labs/models/__init__.py` (2 lines)
- `addons/pos_pine_labs/models/pine_labs_pos_request.py` (75 lines)
- `addons/pos_pine_labs/models/pos_payment.py` (8 lines)
- `addons/pos_pine_labs/models/pos_payment_method.py` (98 lines)
- `addons/pos_pine_labs/static/src/app/screens/payment_screen/payment_screen.js` (29 lines)
- `addons/pos_pine_labs/static/src/app/utils/payment/payment_pine_labs.js` (269 lines)
- `addons/pos_pine_labs/views/pos_payment_method_views.xml` (24 lines)
- `addons/pos_pine_labs/views/pos_payment_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
