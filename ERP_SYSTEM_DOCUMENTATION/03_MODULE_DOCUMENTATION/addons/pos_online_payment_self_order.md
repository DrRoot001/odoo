# Module: pos_online_payment_self_order

- **Module ID:** MOD-441
- **Path:** `addons/pos_online_payment_self_order`
- **Manifest:** `addons/pos_online_payment_self_order/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Support online payment in self-order

No manifest description declared.

Declared dependencies: `pos_online_payment`, `pos_self_order`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 10 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_online_payment",
    "pos_self_order"
  ],
  "data": [
    "views/res_config_settings_views.xml"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_online_payment_self_order/static/src/app/**/*",
      "point_of_sale/static/lib/qrcode.js"
    ],
    "web.assets_frontend": [
      "pos_online_payment_self_order/static/src/portal/**/*"
    ],
    "web.assets_tests": [
      "pos_online_payment_self_order/static/tests/tours/pos_online_payment_multi_table_order.js"
    ],
    "pos_self_order.assets_tests": [
      "pos_online_payment_self_order/static/tests/tours/pos_self_order_mobile_online_payment_tour.js"
    ],
    "web.assets_unit_tests": [
      "pos_online_payment_self_order/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_online_payment_self_order/__init__.py` (5 lines)
- `addons/pos_online_payment_self_order/__manifest__.py` (33 lines)
- `addons/pos_online_payment_self_order/controllers/__init__.py` (5 lines)
- `addons/pos_online_payment_self_order/controllers/payment_portal.py` (24 lines)
- `addons/pos_online_payment_self_order/controllers/payment_status.py` (10 lines)
- `addons/pos_online_payment_self_order/i18n/ar.po` (172 lines)
- `addons/pos_online_payment_self_order/i18n/az.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/bg.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/bs.po` (165 lines)
- `addons/pos_online_payment_self_order/i18n/ca.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/cs.po` (165 lines)
- `addons/pos_online_payment_self_order/i18n/da.po` (172 lines)
- `addons/pos_online_payment_self_order/i18n/de.po` (173 lines)
- `addons/pos_online_payment_self_order/i18n/el.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/es.po` (171 lines)
- `addons/pos_online_payment_self_order/i18n/es_419.po` (171 lines)
- `addons/pos_online_payment_self_order/i18n/et.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/fa.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/fi.po` (170 lines)
- `addons/pos_online_payment_self_order/i18n/fr.po` (172 lines)
- `addons/pos_online_payment_self_order/i18n/he.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/hi.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/hr.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/hu.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/id.po` (171 lines)
- `addons/pos_online_payment_self_order/i18n/it.po` (171 lines)
- `addons/pos_online_payment_self_order/i18n/ja.po` (167 lines)
- `addons/pos_online_payment_self_order/i18n/kab.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/ko.po` (167 lines)
- `addons/pos_online_payment_self_order/i18n/ku.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/lo.po` (167 lines)
- `addons/pos_online_payment_self_order/i18n/lt.po` (165 lines)
- `addons/pos_online_payment_self_order/i18n/lv.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/mn.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/my.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/nb.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/nl.po` (170 lines)
- `addons/pos_online_payment_self_order/i18n/pl.po` (174 lines)
- `addons/pos_online_payment_self_order/i18n/pos_online_payment_self_order.pot` (160 lines)
- `addons/pos_online_payment_self_order/i18n/pt.po` (169 lines)
- `addons/pos_online_payment_self_order/i18n/pt_BR.po` (172 lines)
- `addons/pos_online_payment_self_order/i18n/ro.po` (170 lines)
- `addons/pos_online_payment_self_order/i18n/ru.po` (173 lines)
- `addons/pos_online_payment_self_order/i18n/sk.po` (163 lines)
- `addons/pos_online_payment_self_order/i18n/sl.po` (165 lines)
- `addons/pos_online_payment_self_order/i18n/sr@latin.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/sv.po` (170 lines)
- `addons/pos_online_payment_self_order/i18n/th.po` (167 lines)
- `addons/pos_online_payment_self_order/i18n/tr.po` (171 lines)
- `addons/pos_online_payment_self_order/i18n/uk.po` (164 lines)
- `addons/pos_online_payment_self_order/i18n/uz.po` (195 lines)
- `addons/pos_online_payment_self_order/i18n/vi.po` (172 lines)
- `addons/pos_online_payment_self_order/i18n/zh_CN.po` (168 lines)
- `addons/pos_online_payment_self_order/i18n/zh_TW.po` (170 lines)
- `addons/pos_online_payment_self_order/models/__init__.py` (9 lines)
- `addons/pos_online_payment_self_order/models/ir_http.py` (10 lines)
- `addons/pos_online_payment_self_order/models/payment_transaction.py` (19 lines)
- `addons/pos_online_payment_self_order/models/pos_config.py` (33 lines)
- `addons/pos_online_payment_self_order/models/pos_order.py` (94 lines)
- `addons/pos_online_payment_self_order/models/pos_payment_method.py` (25 lines)
- `addons/pos_online_payment_self_order/models/res_config_settings.py` (9 lines)
- `addons/pos_online_payment_self_order/static/src/app/components/order_widget/order_widget.js` (58 lines)
- `addons/pos_online_payment_self_order/static/src/app/pages/payment_page/payment_page.js` (58 lines)
- `addons/pos_online_payment_self_order/static/src/app/pages/payment_page/payment_page.xml` (12 lines)
- `addons/pos_online_payment_self_order/static/src/app/services/self_order_service.js` (85 lines)
- `addons/pos_online_payment_self_order/static/src/portal/pos_self_order_payment_form_patch.js` (44 lines)
- `addons/pos_online_payment_self_order/static/tests/tours/pos_online_payment_multi_table_order.js` (51 lines)
- `addons/pos_online_payment_self_order/static/tests/tours/pos_self_order_mobile_online_payment_tour.js` (157 lines)
- `addons/pos_online_payment_self_order/static/tests/unit/data/pos_config.data.js` (6 lines)
- `addons/pos_online_payment_self_order/static/tests/unit/data/pos_payment_method.data.js` (25 lines)
- `addons/pos_online_payment_self_order/static/tests/unit/scenario/pos_self_order_flow.test.js` (37 lines)
- `addons/pos_online_payment_self_order/static/tests/unit/services/self_order_service.test.js` (82 lines)
- `addons/pos_online_payment_self_order/tests/__init__.py` (6 lines)
- `addons/pos_online_payment_self_order/tests/test_self_order_fake_payment.py` (146 lines)
- `addons/pos_online_payment_self_order/tests/test_self_order_frontend.py` (124 lines)
- `addons/pos_online_payment_self_order/tests/test_self_order_mobile.py` (210 lines)
- `addons/pos_online_payment_self_order/tests/test_self_order_payment_method.py` (62 lines)
- `addons/pos_online_payment_self_order/views/res_config_settings_views.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
