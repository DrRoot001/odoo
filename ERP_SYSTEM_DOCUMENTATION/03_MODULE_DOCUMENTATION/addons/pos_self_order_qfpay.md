# Module: pos_self_order_qfpay

- **Module ID:** MOD-459
- **Path:** `addons/pos_self_order_qfpay`
- **Manifest:** `addons/pos_self_order_qfpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Addon for the Self Order App that allows customers to pay by QFPay.

No manifest description declared.

Declared dependencies: `pos_qfpay`, `pos_self_order`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_qfpay",
    "pos_self_order"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_qfpay/static/src/app/qfpay.js",
      "pos_self_order_qfpay/static/src/**/*"
    ],
    "pos_self_order.assets_tests": [
      "pos_qfpay/static/src/app/qfpay.js",
      "pos_qfpay/static/tests/tours/utils/common.js",
      "pos_self_order_qfpay/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_qfpay/__init__.py` (1 lines)
- `addons/pos_self_order_qfpay/__manifest__.py` (21 lines)
- `addons/pos_self_order_qfpay/i18n/ar.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/az.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/bg.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/bs.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/ca.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/cs.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/da.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/de.po` (47 lines)
- `addons/pos_self_order_qfpay/i18n/el.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/es.po` (47 lines)
- `addons/pos_self_order_qfpay/i18n/es_419.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/et.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/fa.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/fi.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/fr.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/he.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/hi.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/hr.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/hu.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/id.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/it.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/ja.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/kab.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/ko.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/ku.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/lo.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/lt.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/lv.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/mn.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/my.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/nb.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/nl.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/pl.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/pos_self_order_qfpay.pot` (41 lines)
- `addons/pos_self_order_qfpay/i18n/pt.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/pt_BR.po` (48 lines)
- `addons/pos_self_order_qfpay/i18n/ro.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/ru.po` (46 lines)
- `addons/pos_self_order_qfpay/i18n/sk.po` (44 lines)
- `addons/pos_self_order_qfpay/i18n/sl.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/sr@latin.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/sv.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/th.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/tr.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/uk.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/uz.po` (54 lines)
- `addons/pos_self_order_qfpay/i18n/vi.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/zh_CN.po` (45 lines)
- `addons/pos_self_order_qfpay/i18n/zh_TW.po` (45 lines)
- `addons/pos_self_order_qfpay/models/__init__.py` (1 lines)
- `addons/pos_self_order_qfpay/models/pos_payment_method.py` (31 lines)
- `addons/pos_self_order_qfpay/static/src/app/pages/payment_page/payment_page.js` (27 lines)
- `addons/pos_self_order_qfpay/static/src/app/services/self_order_service.js` (34 lines)
- `addons/pos_self_order_qfpay/static/tests/tours/qfpay_self_tour.js` (52 lines)
- `addons/pos_self_order_qfpay/tests/__init__.py` (1 lines)
- `addons/pos_self_order_qfpay/tests/test_basic.py` (60 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
