# Module: pos_dpopay

- **Module ID:** MOD-428
- **Path:** `addons/pos_dpopay`
- **Manifest:** `addons/pos_dpopay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Integrate your POS with DPO payment terminal.


Allow DPO POS payments
==============================

It supports all currencies supported by the terminal device — primarily for use in the **African region**.
It enables customers to pay for their orders using debit/credit cards and Mobile Money through DPO POS terminals.
A DPO merchant account is required to process transactions.
Features include:

* Quick payments by swiping, scanning, or tapping your credit/debit card or Mobile Money (Airtel Money / M-Pesa) at the payment terminal.
* Supported cards: Visa, MasterCard, American Express etc.
    

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
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
    "views/pos_payment_method_views.xml",
    "views/pos_payment_views.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_dpopay/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_dpopay/__init__.py` (3 lines)
- `addons/pos_dpopay/__manifest__.py` (32 lines)
- `addons/pos_dpopay/i18n/ar.po` (305 lines)
- `addons/pos_dpopay/i18n/az.po` (297 lines)
- `addons/pos_dpopay/i18n/bg.po` (297 lines)
- `addons/pos_dpopay/i18n/bs.po` (298 lines)
- `addons/pos_dpopay/i18n/ca.po` (297 lines)
- `addons/pos_dpopay/i18n/cs.po` (297 lines)
- `addons/pos_dpopay/i18n/da.po` (297 lines)
- `addons/pos_dpopay/i18n/de.po` (343 lines)
- `addons/pos_dpopay/i18n/el.po` (297 lines)
- `addons/pos_dpopay/i18n/es.po` (343 lines)
- `addons/pos_dpopay/i18n/es_419.po` (344 lines)
- `addons/pos_dpopay/i18n/et.po` (297 lines)
- `addons/pos_dpopay/i18n/fa.po` (297 lines)
- `addons/pos_dpopay/i18n/fi.po` (331 lines)
- `addons/pos_dpopay/i18n/fr.po` (322 lines)
- `addons/pos_dpopay/i18n/he.po` (298 lines)
- `addons/pos_dpopay/i18n/hi.po` (297 lines)
- `addons/pos_dpopay/i18n/hr.po` (298 lines)
- `addons/pos_dpopay/i18n/hu.po` (297 lines)
- `addons/pos_dpopay/i18n/id.po` (321 lines)
- `addons/pos_dpopay/i18n/it.po` (336 lines)
- `addons/pos_dpopay/i18n/ja.po` (316 lines)
- `addons/pos_dpopay/i18n/kab.po` (297 lines)
- `addons/pos_dpopay/i18n/ko.po` (299 lines)
- `addons/pos_dpopay/i18n/ku.po` (297 lines)
- `addons/pos_dpopay/i18n/lo.po` (321 lines)
- `addons/pos_dpopay/i18n/lt.po` (299 lines)
- `addons/pos_dpopay/i18n/lv.po` (298 lines)
- `addons/pos_dpopay/i18n/mn.po` (297 lines)
- `addons/pos_dpopay/i18n/my.po` (297 lines)
- `addons/pos_dpopay/i18n/nb.po` (297 lines)
- `addons/pos_dpopay/i18n/nl.po` (323 lines)
- `addons/pos_dpopay/i18n/pl.po` (324 lines)
- `addons/pos_dpopay/i18n/pos_dpopay.pot` (291 lines)
- `addons/pos_dpopay/i18n/pt.po` (297 lines)
- `addons/pos_dpopay/i18n/pt_BR.po` (338 lines)
- `addons/pos_dpopay/i18n/ro.po` (298 lines)
- `addons/pos_dpopay/i18n/ru.po` (316 lines)
- `addons/pos_dpopay/i18n/sk.po` (297 lines)
- `addons/pos_dpopay/i18n/sl.po` (298 lines)
- `addons/pos_dpopay/i18n/sr@latin.po` (298 lines)
- `addons/pos_dpopay/i18n/sv.po` (298 lines)
- `addons/pos_dpopay/i18n/th.po` (302 lines)
- `addons/pos_dpopay/i18n/tr.po` (297 lines)
- `addons/pos_dpopay/i18n/uk.po` (298 lines)
- `addons/pos_dpopay/i18n/uz.po` (297 lines)
- `addons/pos_dpopay/i18n/vi.po` (297 lines)
- `addons/pos_dpopay/i18n/zh_CN.po` (320 lines)
- `addons/pos_dpopay/i18n/zh_TW.po` (298 lines)
- `addons/pos_dpopay/models/__init__.py` (4 lines)
- `addons/pos_dpopay/models/pos_payment.py` (11 lines)
- `addons/pos_dpopay/models/pos_payment_method.py` (122 lines)
- `addons/pos_dpopay/static/src/app/screens/payment_screen/payment_screen.js` (29 lines)
- `addons/pos_dpopay/static/src/app/utils/payment/payment_dpopay.js` (329 lines)
- `addons/pos_dpopay/tests/__init__.py` (3 lines)
- `addons/pos_dpopay/tests/test_payment_method.py` (45 lines)
- `addons/pos_dpopay/views/pos_payment_method_views.xml` (29 lines)
- `addons/pos_dpopay/views/pos_payment_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
