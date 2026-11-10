# Module: pos_discount

- **Module ID:** MOD-427
- **Path:** `addons/pos_discount`
- **Manifest:** `addons/pos_discount/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Simple Discounts in the Point of Sale 



This module allows the cashier to quickly give percentage-based
discount to a customer.



Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 17 | Client behavior/assets. |
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
    "data/pos_discount_data.xml",
    "views/res_config_settings_views.xml",
    "views/pos_config_views.xml",
    "views/pos_session_sales_details.xml",
    "receipt/pos_order_receipt.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_discount/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_discount/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_discount/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_discount/__init__.py` (8 lines)
- `addons/pos_discount/__manifest__.py` (37 lines)
- `addons/pos_discount/data/pos_discount_data.xml` (18 lines)
- `addons/pos_discount/i18n/af.po` (173 lines)
- `addons/pos_discount/i18n/ar.po` (192 lines)
- `addons/pos_discount/i18n/az.po` (176 lines)
- `addons/pos_discount/i18n/bg.po` (184 lines)
- `addons/pos_discount/i18n/bs.po` (176 lines)
- `addons/pos_discount/i18n/ca.po` (197 lines)
- `addons/pos_discount/i18n/cs.po` (193 lines)
- `addons/pos_discount/i18n/da.po` (191 lines)
- `addons/pos_discount/i18n/de.po` (201 lines)
- `addons/pos_discount/i18n/el.po` (186 lines)
- `addons/pos_discount/i18n/es.po` (202 lines)
- `addons/pos_discount/i18n/es_419.po` (197 lines)
- `addons/pos_discount/i18n/es_CL.po` (26 lines)
- `addons/pos_discount/i18n/et.po` (193 lines)
- `addons/pos_discount/i18n/eu.po` (175 lines)
- `addons/pos_discount/i18n/fa.po` (185 lines)
- `addons/pos_discount/i18n/fi.po` (194 lines)
- `addons/pos_discount/i18n/fo.po` (175 lines)
- `addons/pos_discount/i18n/fr.po` (195 lines)
- `addons/pos_discount/i18n/gu.po` (177 lines)
- `addons/pos_discount/i18n/he.po` (187 lines)
- `addons/pos_discount/i18n/hi.po` (173 lines)
- `addons/pos_discount/i18n/hr.po` (186 lines)
- `addons/pos_discount/i18n/hu.po` (185 lines)
- `addons/pos_discount/i18n/id.po` (199 lines)
- `addons/pos_discount/i18n/is.po` (173 lines)
- `addons/pos_discount/i18n/it.po` (199 lines)
- `addons/pos_discount/i18n/ja.po` (191 lines)
- `addons/pos_discount/i18n/ka.po` (175 lines)
- `addons/pos_discount/i18n/kab.po` (177 lines)
- `addons/pos_discount/i18n/km.po` (176 lines)
- `addons/pos_discount/i18n/ko.po` (191 lines)
- `addons/pos_discount/i18n/ku.po` (173 lines)
- `addons/pos_discount/i18n/lo.po` (183 lines)
- `addons/pos_discount/i18n/lt.po` (188 lines)
- `addons/pos_discount/i18n/lv.po` (182 lines)
- `addons/pos_discount/i18n/mk.po` (177 lines)
- `addons/pos_discount/i18n/mn.po` (187 lines)
- `addons/pos_discount/i18n/my.po` (173 lines)
- `addons/pos_discount/i18n/nb.po` (185 lines)
- `addons/pos_discount/i18n/nl.po` (192 lines)
- `addons/pos_discount/i18n/pl.po` (199 lines)
- `addons/pos_discount/i18n/pos_discount.pot` (170 lines)
- `addons/pos_discount/i18n/pt.po` (192 lines)
- `addons/pos_discount/i18n/pt_BR.po` (199 lines)
- `addons/pos_discount/i18n/ro.po` (186 lines)
- `addons/pos_discount/i18n/ru.po` (190 lines)
- `addons/pos_discount/i18n/sk.po` (186 lines)
- `addons/pos_discount/i18n/sl.po` (189 lines)
- `addons/pos_discount/i18n/sr@latin.po` (177 lines)
- `addons/pos_discount/i18n/sv.po` (194 lines)
- `addons/pos_discount/i18n/th.po` (192 lines)
- `addons/pos_discount/i18n/tr.po` (202 lines)
- `addons/pos_discount/i18n/uk.po` (193 lines)
- `addons/pos_discount/i18n/uz.po` (213 lines)
- `addons/pos_discount/i18n/vi.po` (192 lines)
- `addons/pos_discount/i18n/zh_CN.po` (193 lines)
- `addons/pos_discount/i18n/zh_TW.po` (187 lines)
- `addons/pos_discount/models/__init__.py` (8 lines)
- `addons/pos_discount/models/account_move_line.py` (18 lines)
- `addons/pos_discount/models/pos_config.py` (32 lines)
- `addons/pos_discount/models/product_template.py` (20 lines)
- `addons/pos_discount/models/report_sale_details.py` (16 lines)
- `addons/pos_discount/models/res_config_settings.py` (22 lines)
- `addons/pos_discount/receipt/pos_order_receipt.xml` (10 lines)
- `addons/pos_discount/static/src/app/models/pos_order_line.js` (45 lines)
- `addons/pos_discount/static/src/app/screens/product_screen/control_buttons/control_buttons.js` (52 lines)
- `addons/pos_discount/static/src/app/screens/product_screen/control_buttons/control_buttons.xml` (13 lines)
- `addons/pos_discount/static/src/app/screens/product_screen/product_screen.js` (18 lines)
- `addons/pos_discount/static/src/app/screens/ticket_screen/ticket_screen.js` (48 lines)
- `addons/pos_discount/static/src/app/services/pos_store.js` (153 lines)
- `addons/pos_discount/static/tests/tours/test_pos_global_discount_flow.js` (82 lines)
- `addons/pos_discount/static/tests/tours/test_taxes_global_discount.js` (432 lines)
- `addons/pos_discount/static/tests/unit/components/control_buttons.test.js` (35 lines)
- `addons/pos_discount/static/tests/unit/components/product_screen.test.js` (71 lines)
- `addons/pos_discount/static/tests/unit/components/ticket_screen.test.js` (35 lines)
- `addons/pos_discount/static/tests/unit/data/pos_config.data.js` (7 lines)
- `addons/pos_discount/static/tests/unit/data/product_product.data.js` (17 lines)
- `addons/pos_discount/static/tests/unit/data/product_template.data.js` (19 lines)
- `addons/pos_discount/static/tests/unit/models/pos_order_line.test.js` (39 lines)
- `addons/pos_discount/static/tests/unit/scenario/pos_discount_flow.test.js` (156 lines)
- `addons/pos_discount/static/tests/unit/services/pos_service.test.js` (74 lines)
- `addons/pos_discount/static/tests/unit/ui_utils.js` (11 lines)
- `addons/pos_discount/tests/__init__.py` (1 lines)
- `addons/pos_discount/tests/test_taxes_global_discount.py` (132 lines)
- `addons/pos_discount/views/pos_config_views.xml` (6 lines)
- `addons/pos_discount/views/pos_session_sales_details.xml` (19 lines)
- `addons/pos_discount/views/res_config_settings_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
