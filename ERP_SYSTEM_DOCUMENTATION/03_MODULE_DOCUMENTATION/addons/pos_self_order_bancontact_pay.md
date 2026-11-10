# Module: pos_self_order_bancontact_pay

- **Module ID:** MOD-456
- **Path:** `addons/pos_self_order_bancontact_pay`
- **Manifest:** `addons/pos_self_order_bancontact_pay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Accept Bancontact Pay and Wero QR code payments in a kiosk (Payconiq).

No manifest description declared.

Declared dependencies: `pos_self_order`, `pos_bancontact_pay`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_self_order",
    "pos_bancontact_pay"
  ],
  "assets": {
    "point_of_sale.payment_terminals": [
      "pos_self_order_bancontact_pay/static/src/app/bancontact_pay/**/*"
    ],
    "pos_self_order.assets": [
      "pos_self_order_bancontact_pay/static/src/app/self_order/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_self_order_bancontact_pay/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_bancontact_pay/__init__.py` (2 lines)
- `addons/pos_self_order_bancontact_pay/__manifest__.py` (21 lines)
- `addons/pos_self_order_bancontact_pay/controllers/__init__.py` (2 lines)
- `addons/pos_self_order_bancontact_pay/controllers/kiosk.py` (24 lines)
- `addons/pos_self_order_bancontact_pay/controllers/webhook.py` (24 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ar.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/az.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/bg.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/bs.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ca.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/cs.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/da.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/de.po` (99 lines)
- `addons/pos_self_order_bancontact_pay/i18n/el.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/es.po` (96 lines)
- `addons/pos_self_order_bancontact_pay/i18n/es_419.po` (96 lines)
- `addons/pos_self_order_bancontact_pay/i18n/et.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/fa.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/fi.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/fr.po` (97 lines)
- `addons/pos_self_order_bancontact_pay/i18n/he.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/hi.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/hr.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/hu.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/id.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/it.po` (96 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ja.po` (96 lines)
- `addons/pos_self_order_bancontact_pay/i18n/kab.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ko.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ku.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/lo.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/lt.po` (92 lines)
- `addons/pos_self_order_bancontact_pay/i18n/lv.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/mn.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/my.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/nb.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/nl.po` (96 lines)
- `addons/pos_self_order_bancontact_pay/i18n/pl.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/pos_self_order_bancontact_pay.pot` (87 lines)
- `addons/pos_self_order_bancontact_pay/i18n/pt.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/pt_BR.po` (100 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ro.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/ru.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/sk.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/sl.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/sr@latin.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/sv.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/th.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/tr.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/uk.po` (91 lines)
- `addons/pos_self_order_bancontact_pay/i18n/uz.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/vi.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/i18n/zh_CN.po` (97 lines)
- `addons/pos_self_order_bancontact_pay/i18n/zh_TW.po` (90 lines)
- `addons/pos_self_order_bancontact_pay/models/__init__.py` (2 lines)
- `addons/pos_self_order_bancontact_pay/models/pos_config.py` (12 lines)
- `addons/pos_self_order_bancontact_pay/models/pos_payment_method.py` (12 lines)
- `addons/pos_self_order_bancontact_pay/static/src/app/bancontact_pay/payment_bancontact.js` (40 lines)
- `addons/pos_self_order_bancontact_pay/static/src/app/self_order/payment_page/payment_page.js` (42 lines)
- `addons/pos_self_order_bancontact_pay/static/src/app/self_order/payment_page/payment_page.xml` (17 lines)
- `addons/pos_self_order_bancontact_pay/static/src/app/self_order/services/self_order_service.js` (46 lines)
- `addons/pos_self_order_bancontact_pay/static/tests/unit/app/payment_bancontact.test.js` (98 lines)
- `addons/pos_self_order_bancontact_pay/static/tests/unit/scenario/kiosk_bancontact_pay_flow.test.js` (92 lines)
- `addons/pos_self_order_bancontact_pay/static/tests/unit/ui_utils.js` (78 lines)
- `addons/pos_self_order_bancontact_pay/tests/__init__.py` (2 lines)
- `addons/pos_self_order_bancontact_pay/tests/test_models.py` (26 lines)
- `addons/pos_self_order_bancontact_pay/tests/test_webhook.py` (61 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
