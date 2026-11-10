# Module: delivery

- **Module ID:** MOD-062
- **Path:** `addons/delivery`
- **Manifest:** `addons/delivery/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows you to add delivery methods in sale orders.
==================================================
You can define your own carrier for prices.
The system is able to add and compute the shipping line.


Declared dependencies: `sale`, `payment_custom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 22 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "payment_custom"
  ],
  "data": [
    "report/ir_actions_report_templates.xml",
    "report/ir_actions_report.xml",
    "data/delivery_data.xml",
    "data/ir_sequence_data.xml",
    "data/mail_template_data.xml",
    "data/payment_provider_data.xml",
    "data/payment_method_data.xml",
    "security/ir.access.csv",
    "views/delivery_carrier_views.xml",
    "views/delivery_price_rule_views.xml",
    "views/delivery_zip_prefix_views.xml",
    "views/ir_module_module_views.xml",
    "views/payment_form_templates.xml",
    "views/payment_provider_views.xml",
    "views/portal_templates.xml",
    "views/res_partner_views.xml",
    "views/sale_order_views.xml",
    "wizard/res_config_settings_views.xml",
    "wizard/choose_delivery_carrier_views.xml",
    "wizard/delivery_note_line_views.xml",
    "wizard/delivery_note_views.xml"
  ],
  "demo": [
    "data/delivery_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "delivery/static/src/**/*",
      [
        "remove",
        "delivery/static/src/backend/**/*"
      ]
    ],
    "web.assets_backend": [
      "delivery/static/src/backend/**/*"
    ],
    "web.assets_tests": [
      "delivery/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/delivery/__init__.py` (12 lines)
- `addons/delivery/__manifest__.py` (49 lines)
- `addons/delivery/const.py` (4 lines)
- `addons/delivery/data/delivery_data.xml` (25 lines)
- `addons/delivery/data/delivery_demo.xml` (64 lines)
- `addons/delivery/data/ir_sequence_data.xml` (12 lines)
- `addons/delivery/data/mail_template_data.xml` (41 lines)
- `addons/delivery/data/neutralize.sql` (7 lines)
- `addons/delivery/data/payment_method_data.xml` (14 lines)
- `addons/delivery/data/payment_provider_data.xml` (19 lines)
- `addons/delivery/i18n/af.po` (1,274 lines)
- `addons/delivery/i18n/am.po` (1,270 lines)
- `addons/delivery/i18n/ar.po` (1,376 lines)
- `addons/delivery/i18n/az.po` (1,336 lines)
- `addons/delivery/i18n/bg.po` (1,389 lines)
- `addons/delivery/i18n/bs.po` (1,340 lines)
- `addons/delivery/i18n/ca.po` (1,436 lines)
- `addons/delivery/i18n/cs.po` (1,391 lines)
- `addons/delivery/i18n/da.po` (1,346 lines)
- `addons/delivery/i18n/de.po` (1,503 lines)
- `addons/delivery/i18n/delivery.pot` (1,318 lines)
- `addons/delivery/i18n/el.po` (1,351 lines)
- `addons/delivery/i18n/es.po` (1,453 lines)
- `addons/delivery/i18n/es_419.po` (1,495 lines)
- `addons/delivery/i18n/es_CL.po` (129 lines)
- `addons/delivery/i18n/et.po` (1,395 lines)
- `addons/delivery/i18n/eu.po` (1,273 lines)
- `addons/delivery/i18n/fa.po` (1,375 lines)
- `addons/delivery/i18n/fi.po` (1,462 lines)
- `addons/delivery/i18n/fo.po` (1,273 lines)
- `addons/delivery/i18n/fr.po` (1,503 lines)
- `addons/delivery/i18n/fr_CA.po` (104 lines)
- `addons/delivery/i18n/gl.po` (1,273 lines)
- `addons/delivery/i18n/gu.po` (1,274 lines)
- `addons/delivery/i18n/he.po` (1,365 lines)
- `addons/delivery/i18n/hi.po` (1,367 lines)
- `addons/delivery/i18n/hr.po` (1,364 lines)
- `addons/delivery/i18n/hu.po` (1,350 lines)
- `addons/delivery/i18n/id.po` (1,474 lines)
- `addons/delivery/i18n/is.po` (1,270 lines)
- `addons/delivery/i18n/it.po` (1,500 lines)
- `addons/delivery/i18n/ja.po` (1,468 lines)
- `addons/delivery/i18n/ka.po` (1,273 lines)
- `addons/delivery/i18n/kab.po` (1,334 lines)
- `addons/delivery/i18n/km.po` (1,276 lines)
- `addons/delivery/i18n/ko.po` (1,373 lines)
- `addons/delivery/i18n/ku.po` (1,332 lines)
- `addons/delivery/i18n/lo.po` (1,445 lines)
- `addons/delivery/i18n/lt.po` (1,357 lines)
- `addons/delivery/i18n/lv.po` (1,341 lines)
- `addons/delivery/i18n/mk.po` (1,273 lines)
- `addons/delivery/i18n/mn.po` (1,481 lines)
- `addons/delivery/i18n/my.po` (1,333 lines)
- `addons/delivery/i18n/nb.po` (1,359 lines)
- `addons/delivery/i18n/nl.po` (1,496 lines)
- `addons/delivery/i18n/pl.po` (1,402 lines)
- `addons/delivery/i18n/pt.po` (1,437 lines)
- `addons/delivery/i18n/pt_BR.po` (1,496 lines)
- `addons/delivery/i18n/ro.po` (1,390 lines)
- `addons/delivery/i18n/ru.po` (1,448 lines)
- `addons/delivery/i18n/sk.po` (1,342 lines)
- `addons/delivery/i18n/sl.po` (1,384 lines)
- `addons/delivery/i18n/sq.po` (1,273 lines)
- `addons/delivery/i18n/sr@latin.po` (1,337 lines)
- `addons/delivery/i18n/sv.po` (1,388 lines)
- `addons/delivery/i18n/th.po` (1,443 lines)
- `addons/delivery/i18n/tr.po` (1,397 lines)
- `addons/delivery/i18n/uk.po` (1,371 lines)
- `addons/delivery/i18n/uz.po` (1,541 lines)
- `addons/delivery/i18n/vi.po` (1,387 lines)
- `addons/delivery/i18n/zh_CN.po` (1,450 lines)
- `addons/delivery/i18n/zh_TW.po` (1,365 lines)
- `addons/delivery/models/__init__.py` (16 lines)
- `addons/delivery/models/delivery_carrier.py` (674 lines)
- `addons/delivery/models/delivery_price_rule.py` (99 lines)
- `addons/delivery/models/delivery_zip_prefix.py` (28 lines)
- `addons/delivery/models/ir_http.py` (12 lines)
- `addons/delivery/models/ir_module_module.py` (20 lines)
- `addons/delivery/models/payment_method.py` (12 lines)
- `addons/delivery/models/payment_provider.py` (84 lines)
- `addons/delivery/models/payment_transaction.py` (35 lines)
- `addons/delivery/models/product_category.py` (21 lines)
- `addons/delivery/models/res_partner.py` (14 lines)
- `addons/delivery/models/sale_order.py` (220 lines)
- `addons/delivery/models/sale_order_line.py` (70 lines)
- `addons/delivery/report/ir_actions_report.xml` (16 lines)
- `addons/delivery/report/ir_actions_report_templates.xml` (130 lines)
- `addons/delivery/security/ir.access.csv` (12 lines)
- `addons/delivery/static/src/backend/widgets/carrier_rates_loader.js` (81 lines)
- `addons/delivery/static/src/backend/widgets/carrier_rates_loader.xml` (20 lines)
- `addons/delivery/static/src/img/payment_method_cash_on_delivery.png` (21 lines)
- `addons/delivery/static/src/img/payment_provider_cash_on_delivery.png` (20 lines)
- `addons/delivery/static/src/interactions/payment_form.js` (19 lines)
- `addons/delivery/static/tests/tours/tour_test_get_all_rates.js` (62 lines)
- `addons/delivery/tests/__init__.py` (9 lines)
- `addons/delivery/tests/cash_on_delivery_common.py` (39 lines)
- `addons/delivery/tests/common.py` (39 lines)
- `addons/delivery/tests/test_choose_delivery_carrier.py` (50 lines)
- `addons/delivery/tests/test_delivery_availability.py` (284 lines)
- `addons/delivery/tests/test_delivery_cost.py` (684 lines)
- `addons/delivery/tests/test_payment_provider.py` (75 lines)
- `addons/delivery/tests/test_payment_transaction.py` (37 lines)
- `addons/delivery/views/delivery_carrier_views.xml` (249 lines)
- `addons/delivery/views/delivery_price_rule_views.xml` (45 lines)
- `addons/delivery/views/delivery_zip_prefix_views.xml` (19 lines)
- `addons/delivery/views/ir_module_module_views.xml` (46 lines)
- `addons/delivery/views/payment_form_templates.xml` (10 lines)
- `addons/delivery/views/payment_provider_views.xml` (18 lines)
- `addons/delivery/views/portal_templates.xml` (12 lines)
- `addons/delivery/views/res_partner_views.xml` (15 lines)
- `addons/delivery/views/sale_order_views.xml` (60 lines)
- `addons/delivery/wizard/__init__.py` (3 lines)
- `addons/delivery/wizard/choose_delivery_carrier.py` (163 lines)
- `addons/delivery/wizard/choose_delivery_carrier_views.xml` (76 lines)
- `addons/delivery/wizard/delivery_note.py` (72 lines)
- `addons/delivery/wizard/delivery_note_line.py` (35 lines)
- `addons/delivery/wizard/delivery_note_line_views.xml` (27 lines)
- `addons/delivery/wizard/delivery_note_views.xml` (31 lines)
- `addons/delivery/wizard/res_config_settings.py` (10 lines)
- `addons/delivery/wizard/res_config_settings_views.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
