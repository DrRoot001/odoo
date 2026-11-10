# Module: pos_self_order_razorpay

- **Module ID:** MOD-460
- **Path:** `addons/pos_self_order_razorpay`
- **Manifest:** `addons/pos_self_order_razorpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Addon for the Self Order App that allows customers to pay by Razorpay POS Terminal.

No manifest description declared.

Declared dependencies: `pos_razorpay`, `pos_self_order`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_razorpay",
    "pos_self_order"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_self_order_razorpay/static/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_razorpay/__init__.py` (2 lines)
- `addons/pos_self_order_razorpay/__manifest__.py` (14 lines)
- `addons/pos_self_order_razorpay/controllers/__init__.py` (1 lines)
- `addons/pos_self_order_razorpay/controllers/orders.py` (72 lines)
- `addons/pos_self_order_razorpay/i18n/ar.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/az.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/bg.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/bs.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/ca.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/cs.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/da.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/de.po` (49 lines)
- `addons/pos_self_order_razorpay/i18n/el.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/es.po` (49 lines)
- `addons/pos_self_order_razorpay/i18n/es_419.po` (50 lines)
- `addons/pos_self_order_razorpay/i18n/et.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/fa.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/fi.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/fr.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/he.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/hi.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/hr.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/hu.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/id.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/it.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/ja.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/kab.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/ko.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/ku.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/lo.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/lt.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/lv.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/mn.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/my.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/nb.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/nl.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/pl.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/pos_self_order_razorpay.pot` (43 lines)
- `addons/pos_self_order_razorpay/i18n/pt.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/pt_BR.po` (50 lines)
- `addons/pos_self_order_razorpay/i18n/ro.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/ru.po` (48 lines)
- `addons/pos_self_order_razorpay/i18n/sk.po` (46 lines)
- `addons/pos_self_order_razorpay/i18n/sl.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/sr@latin.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/sv.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/th.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/tr.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/uk.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/uz.po` (56 lines)
- `addons/pos_self_order_razorpay/i18n/vi.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/zh_CN.po` (47 lines)
- `addons/pos_self_order_razorpay/i18n/zh_TW.po` (47 lines)
- `addons/pos_self_order_razorpay/models/__init__.py` (1 lines)
- `addons/pos_self_order_razorpay/models/pos_payment_method.py` (37 lines)
- `addons/pos_self_order_razorpay/static/src/app/pages/payment_page/payment_page.js` (17 lines)
- `addons/pos_self_order_razorpay/static/src/app/razorpay.js` (154 lines)
- `addons/pos_self_order_razorpay/static/src/app/services/self_order_service.js` (40 lines)
- `addons/pos_self_order_razorpay/tests/__init__.py` (3 lines)
- `addons/pos_self_order_razorpay/tests/test_razorpay_payment_status.py` (153 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
