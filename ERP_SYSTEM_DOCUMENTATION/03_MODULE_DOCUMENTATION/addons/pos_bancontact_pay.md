# Module: pos_bancontact_pay

- **Module ID:** MOD-424
- **Path:** `addons/pos_bancontact_pay`
- **Manifest:** `addons/pos_bancontact_pay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Accept Bancontact Pay and Wero QR code payments in POS (Payconiq).

No manifest description declared.

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 20 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 12 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

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
      "pos_bancontact_pay/static/src/app/**/*"
    ],
    "point_of_sale.customer_display_assets": [
      "pos_bancontact_pay/static/src/customer_display/**/*"
    ],
    "point_of_sale.payment_terminals": [
      "pos_bancontact_pay/static/src/app/payment_bancontact.js",
      "pos_bancontact_pay/static/src/app/pos_payment_method.js",
      "pos_bancontact_pay/static/src/app/pos_payment.js"
    ],
    "web.assets_unit_tests": [
      "pos_bancontact_pay/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_bancontact_pay/__init__.py` (3 lines)
- `addons/pos_bancontact_pay/__manifest__.py` (26 lines)
- `addons/pos_bancontact_pay/const.py` (27 lines)
- `addons/pos_bancontact_pay/controllers/__init__.py` (2 lines)
- `addons/pos_bancontact_pay/controllers/signature.py` (215 lines)
- `addons/pos_bancontact_pay/controllers/webhook.py` (139 lines)
- `addons/pos_bancontact_pay/data/neutralize.sql` (3 lines)
- `addons/pos_bancontact_pay/errors/__init__.py` (2 lines)
- `addons/pos_bancontact_pay/errors/exceptions.py` (2 lines)
- `addons/pos_bancontact_pay/errors/http.py` (46 lines)
- `addons/pos_bancontact_pay/i18n/ar.po` (391 lines)
- `addons/pos_bancontact_pay/i18n/az.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/bg.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/bs.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/ca.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/cs.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/da.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/de.po` (447 lines)
- `addons/pos_bancontact_pay/i18n/el.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/es.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/es_419.po` (435 lines)
- `addons/pos_bancontact_pay/i18n/et.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/fa.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/fi.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/fr.po` (434 lines)
- `addons/pos_bancontact_pay/i18n/he.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/hi.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/hr.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/hu.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/id.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/it.po` (431 lines)
- `addons/pos_bancontact_pay/i18n/ja.po` (427 lines)
- `addons/pos_bancontact_pay/i18n/kab.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/ko.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/ku.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/lo.po` (425 lines)
- `addons/pos_bancontact_pay/i18n/lt.po` (388 lines)
- `addons/pos_bancontact_pay/i18n/lv.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/mn.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/my.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/nb.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/nl.po` (430 lines)
- `addons/pos_bancontact_pay/i18n/pl.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/pos_bancontact_pay.pot` (378 lines)
- `addons/pos_bancontact_pay/i18n/pt.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/pt_BR.po` (436 lines)
- `addons/pos_bancontact_pay/i18n/ro.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/ru.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/sk.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/sl.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/sr@latin.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/sv.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/th.po` (390 lines)
- `addons/pos_bancontact_pay/i18n/tr.po` (390 lines)
- `addons/pos_bancontact_pay/i18n/uk.po` (387 lines)
- `addons/pos_bancontact_pay/i18n/uz.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/vi.po` (386 lines)
- `addons/pos_bancontact_pay/i18n/zh_CN.po` (410 lines)
- `addons/pos_bancontact_pay/i18n/zh_TW.po` (386 lines)
- `addons/pos_bancontact_pay/models/__init__.py` (5 lines)
- `addons/pos_bancontact_pay/models/account_journal.py` (29 lines)
- `addons/pos_bancontact_pay/models/pos_config.py` (33 lines)
- `addons/pos_bancontact_pay/models/pos_payment.py` (11 lines)
- `addons/pos_bancontact_pay/models/pos_payment_method.py` (218 lines)
- `addons/pos_bancontact_pay/models/res_company.py` (34 lines)
- `addons/pos_bancontact_pay/static/description/icon.png` (156 lines)
- `addons/pos_bancontact_pay/static/description/icon.svg` (1 lines)
- `addons/pos_bancontact_pay/static/img/frames/frame_fr.png` (569 lines)
- `addons/pos_bancontact_pay/static/img/frames/frame_fr.svg` (201 lines)
- `addons/pos_bancontact_pay/static/img/frames/frame_nl.png` (618 lines)
- `addons/pos_bancontact_pay/static/img/frames/frame_nl.svg` (188 lines)
- `addons/pos_bancontact_pay/static/img/logo/logo_colored_bg.svg` (40 lines)
- `addons/pos_bancontact_pay/static/img/logo/logo_neutral_bg.svg` (40 lines)
- `addons/pos_bancontact_pay/static/img/logo/logo_white_bg.svg` (59 lines)
- `addons/pos_bancontact_pay/static/src/app/payment_bancontact.js` (93 lines)
- `addons/pos_bancontact_pay/static/src/app/pos_payment.js` (42 lines)
- `addons/pos_bancontact_pay/static/src/app/pos_payment_method.js` (44 lines)
- `addons/pos_bancontact_pay/static/src/app/pos_store.js` (94 lines)
- `addons/pos_bancontact_pay/static/src/app/qr_code_popup/qr_code_popup.js` (6 lines)
- `addons/pos_bancontact_pay/static/src/app/qr_code_popup/qr_code_popup.xml` (23 lines)
- `addons/pos_bancontact_pay/static/src/customer_display/customer_display.xml` (21 lines)
- `addons/pos_bancontact_pay/static/tests/unit/app/payment_bancontact.test.js` (248 lines)
- `addons/pos_bancontact_pay/static/tests/unit/app/pos_payment.test.js` (67 lines)
- `addons/pos_bancontact_pay/static/tests/unit/app/pos_payment_method.test.js` (59 lines)
- `addons/pos_bancontact_pay/static/tests/unit/app/pos_store.test.js` (323 lines)
- `addons/pos_bancontact_pay/static/tests/unit/data/pos_payment_method.data.js` (82 lines)
- `addons/pos_bancontact_pay/static/tests/unit/scenario/bancontact_pay_flow.test.js` (415 lines)
- `addons/pos_bancontact_pay/static/tests/unit/ui_utils.js` (110 lines)
- `addons/pos_bancontact_pay/tests/__init__.py` (4 lines)
- `addons/pos_bancontact_pay/tests/common.py` (99 lines)
- `addons/pos_bancontact_pay/tests/test_models.py` (266 lines)
- `addons/pos_bancontact_pay/tests/test_signature.py` (578 lines)
- `addons/pos_bancontact_pay/tests/test_webhook.py` (185 lines)
- `addons/pos_bancontact_pay/views/pos_payment_method_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
