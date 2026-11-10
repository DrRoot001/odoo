# Module: pos_online_payment

- **Module ID:** MOD-440
- **Path:** `addons/pos_online_payment`
- **Manifest:** `addons/pos_online_payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `point_of_sale`, `account_payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "account_payment"
  ],
  "data": [
    "security/ir.access.csv",
    "views/res_config_settings_views.xml",
    "views/payment_transaction_views.xml",
    "views/pos_payment_views.xml",
    "views/pos_payment_method_views.xml",
    "views/payment_portal_templates.xml",
    "views/account_payment_views.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "pos_online_payment/static/src/portal/**/*"
    ],
    "point_of_sale.assets_prod": [
      "pos_online_payment/static/src/app/**/*",
      "pos_online_payment/static/src/overrides/pos_overrides/**/*"
    ],
    "web.assets_tests": [
      "pos_online_payment/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_online_payment/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_online_payment/__init__.py` (9 lines)
- `addons/pos_online_payment/__manifest__.py` (35 lines)
- `addons/pos_online_payment/controllers/__init__.py` (2 lines)
- `addons/pos_online_payment/controllers/payment_portal.py` (337 lines)
- `addons/pos_online_payment/controllers/payment_status.py` (28 lines)
- `addons/pos_online_payment/i18n/ar.po` (593 lines)
- `addons/pos_online_payment/i18n/az.po` (572 lines)
- `addons/pos_online_payment/i18n/bg.po` (572 lines)
- `addons/pos_online_payment/i18n/bs.po` (574 lines)
- `addons/pos_online_payment/i18n/ca.po` (601 lines)
- `addons/pos_online_payment/i18n/cs.po` (578 lines)
- `addons/pos_online_payment/i18n/da.po` (597 lines)
- `addons/pos_online_payment/i18n/de.po` (620 lines)
- `addons/pos_online_payment/i18n/el.po` (573 lines)
- `addons/pos_online_payment/i18n/es.po` (603 lines)
- `addons/pos_online_payment/i18n/es_419.po` (603 lines)
- `addons/pos_online_payment/i18n/et.po` (573 lines)
- `addons/pos_online_payment/i18n/fa.po` (572 lines)
- `addons/pos_online_payment/i18n/fi.po` (595 lines)
- `addons/pos_online_payment/i18n/fr.po` (610 lines)
- `addons/pos_online_payment/i18n/he.po` (573 lines)
- `addons/pos_online_payment/i18n/hi.po` (572 lines)
- `addons/pos_online_payment/i18n/hr.po` (573 lines)
- `addons/pos_online_payment/i18n/hu.po` (573 lines)
- `addons/pos_online_payment/i18n/id.po` (597 lines)
- `addons/pos_online_payment/i18n/it.po` (605 lines)
- `addons/pos_online_payment/i18n/ja.po` (590 lines)
- `addons/pos_online_payment/i18n/kab.po` (573 lines)
- `addons/pos_online_payment/i18n/ko.po` (587 lines)
- `addons/pos_online_payment/i18n/ku.po` (572 lines)
- `addons/pos_online_payment/i18n/lo.po` (597 lines)
- `addons/pos_online_payment/i18n/lt.po` (574 lines)
- `addons/pos_online_payment/i18n/lv.po` (573 lines)
- `addons/pos_online_payment/i18n/mn.po` (572 lines)
- `addons/pos_online_payment/i18n/my.po` (572 lines)
- `addons/pos_online_payment/i18n/nb.po` (573 lines)
- `addons/pos_online_payment/i18n/nl.po` (606 lines)
- `addons/pos_online_payment/i18n/pl.po` (603 lines)
- `addons/pos_online_payment/i18n/pos_online_payment.pot` (569 lines)
- `addons/pos_online_payment/i18n/pt.po` (600 lines)
- `addons/pos_online_payment/i18n/pt_BR.po` (615 lines)
- `addons/pos_online_payment/i18n/ro.po` (598 lines)
- `addons/pos_online_payment/i18n/ru.po` (601 lines)
- `addons/pos_online_payment/i18n/sk.po` (572 lines)
- `addons/pos_online_payment/i18n/sl.po` (574 lines)
- `addons/pos_online_payment/i18n/sr@latin.po` (573 lines)
- `addons/pos_online_payment/i18n/sv.po` (602 lines)
- `addons/pos_online_payment/i18n/th.po` (588 lines)
- `addons/pos_online_payment/i18n/tr.po` (596 lines)
- `addons/pos_online_payment/i18n/uk.po` (573 lines)
- `addons/pos_online_payment/i18n/uz.po` (678 lines)
- `addons/pos_online_payment/i18n/vi.po` (597 lines)
- `addons/pos_online_payment/i18n/zh_CN.po` (585 lines)
- `addons/pos_online_payment/i18n/zh_TW.po` (584 lines)
- `addons/pos_online_payment/models/__init__.py` (9 lines)
- `addons/pos_online_payment/models/account_payment.py` (25 lines)
- `addons/pos_online_payment/models/payment_transaction.py` (84 lines)
- `addons/pos_online_payment/models/pos_config.py` (45 lines)
- `addons/pos_online_payment/models/pos_order.py` (80 lines)
- `addons/pos_online_payment/models/pos_payment.py` (56 lines)
- `addons/pos_online_payment/models/pos_payment_method.py` (199 lines)
- `addons/pos_online_payment/security/ir.access.csv` (2 lines)
- `addons/pos_online_payment/static/src/app/models/pos_order.js` (31 lines)
- `addons/pos_online_payment/static/src/app/models/pos_payment.js` (20 lines)
- `addons/pos_online_payment/static/src/app/screens/payment_screen/payment_lines/payment_lines.xml` (9 lines)
- `addons/pos_online_payment/static/src/app/screens/payment_screen/payment_screen.js` (22 lines)
- `addons/pos_online_payment/static/src/app/services/pos_store.js` (139 lines)
- `addons/pos_online_payment/static/src/app/utils/order_payment_validation.js` (245 lines)
- `addons/pos_online_payment/static/src/overrides/pos_overrides/services/customer_display_plugin.js` (11 lines)
- `addons/pos_online_payment/static/src/overrides/pos_overrides/services/pos_store.js` (22 lines)
- `addons/pos_online_payment/static/src/portal/js/payment_status_dwell.js` (20 lines)
- `addons/pos_online_payment/static/src/portal/scss/payment_portal_template.scss` (176 lines)
- `addons/pos_online_payment/static/tests/tours/online_payment_tour.js` (99 lines)
- `addons/pos_online_payment/static/tests/unit/components/payment_lines.test.js` (59 lines)
- `addons/pos_online_payment/static/tests/unit/customer_display/customer_display.test.js` (42 lines)
- `addons/pos_online_payment/tests/__init__.py` (4 lines)
- `addons/pos_online_payment/tests/online_payment_common.py` (58 lines)
- `addons/pos_online_payment/tests/test_frontend.py` (481 lines)
- `addons/pos_online_payment/views/account_payment_views.xml` (20 lines)
- `addons/pos_online_payment/views/payment_portal_templates.xml` (234 lines)
- `addons/pos_online_payment/views/payment_transaction_views.xml` (18 lines)
- `addons/pos_online_payment/views/pos_payment_method_views.xml` (48 lines)
- `addons/pos_online_payment/views/pos_payment_views.xml` (13 lines)
- `addons/pos_online_payment/views/res_config_settings_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
