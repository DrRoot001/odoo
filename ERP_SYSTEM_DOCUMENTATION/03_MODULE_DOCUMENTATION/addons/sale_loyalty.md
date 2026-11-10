# Module: sale_loyalty

- **Module ID:** MOD-516
- **Path:** `addons/sale_loyalty`
- **Manifest:** `addons/sale_loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Use discounts and loyalty programs in sales orders

Integrate discount and loyalty programs mechanisms in sales orders.

Declared dependencies: `sale`, `loyalty`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 31 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 10 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 14 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "loyalty"
  ],
  "data": [
    "data/sale_loyalty_data.xml",
    "wizard/sale_loyalty_coupon_wizard_views.xml",
    "wizard/sale_loyalty_reward_wizard_views.xml",
    "views/loyalty_card_views.xml",
    "views/loyalty_program_views.xml",
    "views/sale_order_views.xml",
    "views/sale_portal_templates.xml",
    "views/res_partner_views.xml",
    "views/sale_loyalty_menus.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "sale_loyalty/static/src/interactions/gift_card.js",
      "sale_loyalty/static/src/scss/gift_card.scss"
    ],
    "web.assets_backend": [
      "sale_loyalty/static/src/xml/discount_menu_widget.xml",
      "sale_loyalty/static/src/sale_order_form_view/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_loyalty/__init__.py` (8 lines)
- `addons/sale_loyalty/__manifest__.py` (35 lines)
- `addons/sale_loyalty/controllers/__init__.py` (3 lines)
- `addons/sale_loyalty/controllers/gift_card.py` (39 lines)
- `addons/sale_loyalty/controllers/portal.py` (12 lines)
- `addons/sale_loyalty/data/sale_loyalty_data.xml` (11 lines)
- `addons/sale_loyalty/i18n/ar.po` (673 lines)
- `addons/sale_loyalty/i18n/az.po` (659 lines)
- `addons/sale_loyalty/i18n/bg.po` (659 lines)
- `addons/sale_loyalty/i18n/bs.po` (661 lines)
- `addons/sale_loyalty/i18n/ca.po` (675 lines)
- `addons/sale_loyalty/i18n/cs.po` (663 lines)
- `addons/sale_loyalty/i18n/da.po` (689 lines)
- `addons/sale_loyalty/i18n/de.po` (696 lines)
- `addons/sale_loyalty/i18n/el.po` (660 lines)
- `addons/sale_loyalty/i18n/es.po` (682 lines)
- `addons/sale_loyalty/i18n/es_419.po` (684 lines)
- `addons/sale_loyalty/i18n/et.po` (683 lines)
- `addons/sale_loyalty/i18n/fa.po` (659 lines)
- `addons/sale_loyalty/i18n/fi.po` (683 lines)
- `addons/sale_loyalty/i18n/fr.po` (691 lines)
- `addons/sale_loyalty/i18n/he.po` (665 lines)
- `addons/sale_loyalty/i18n/hi.po` (665 lines)
- `addons/sale_loyalty/i18n/hr.po` (666 lines)
- `addons/sale_loyalty/i18n/hu.po` (677 lines)
- `addons/sale_loyalty/i18n/id.po` (677 lines)
- `addons/sale_loyalty/i18n/it.po` (681 lines)
- `addons/sale_loyalty/i18n/ja.po` (678 lines)
- `addons/sale_loyalty/i18n/kab.po` (660 lines)
- `addons/sale_loyalty/i18n/ko.po` (676 lines)
- `addons/sale_loyalty/i18n/ku.po` (659 lines)
- `addons/sale_loyalty/i18n/lo.po` (675 lines)
- `addons/sale_loyalty/i18n/lt.po` (661 lines)
- `addons/sale_loyalty/i18n/lv.po` (660 lines)
- `addons/sale_loyalty/i18n/mn.po` (678 lines)
- `addons/sale_loyalty/i18n/my.po` (660 lines)
- `addons/sale_loyalty/i18n/nb.po` (663 lines)
- `addons/sale_loyalty/i18n/nl.po` (689 lines)
- `addons/sale_loyalty/i18n/pl.po` (680 lines)
- `addons/sale_loyalty/i18n/pt.po` (680 lines)
- `addons/sale_loyalty/i18n/pt_BR.po` (693 lines)
- `addons/sale_loyalty/i18n/ro.po` (697 lines)
- `addons/sale_loyalty/i18n/ru.po` (686 lines)
- `addons/sale_loyalty/i18n/sale_loyalty.pot` (655 lines)
- `addons/sale_loyalty/i18n/sk.po` (666 lines)
- `addons/sale_loyalty/i18n/sl.po` (671 lines)
- `addons/sale_loyalty/i18n/sr@latin.po` (661 lines)
- `addons/sale_loyalty/i18n/sv.po` (677 lines)
- `addons/sale_loyalty/i18n/th.po` (669 lines)
- `addons/sale_loyalty/i18n/tr.po` (680 lines)
- `addons/sale_loyalty/i18n/uk.po` (666 lines)
- `addons/sale_loyalty/i18n/uz.po` (786 lines)
- `addons/sale_loyalty/i18n/vi.po` (679 lines)
- `addons/sale_loyalty/i18n/zh_CN.po` (677 lines)
- `addons/sale_loyalty/i18n/zh_TW.po` (671 lines)
- `addons/sale_loyalty/models/__init__.py` (12 lines)
- `addons/sale_loyalty/models/account_move_line.py` (14 lines)
- `addons/sale_loyalty/models/loyalty_card.py` (60 lines)
- `addons/sale_loyalty/models/loyalty_history.py` (12 lines)
- `addons/sale_loyalty/models/loyalty_program.py` (27 lines)
- `addons/sale_loyalty/models/loyalty_reward.py` (20 lines)
- `addons/sale_loyalty/models/sale_order.py` (1,853 lines)
- `addons/sale_loyalty/models/sale_order_coupon_points.py` (18 lines)
- `addons/sale_loyalty/models/sale_order_line.py` (178 lines)
- `addons/sale_loyalty/security/ir.access.csv` (18 lines)
- `addons/sale_loyalty/static/src/interactions/gift_card.js` (59 lines)
- `addons/sale_loyalty/static/src/sale_order_form_view/sale_order_static_list.js` (8 lines)
- `addons/sale_loyalty/static/src/scss/gift_card.scss` (9 lines)
- `addons/sale_loyalty/static/src/xml/discount_menu_widget.xml` (15 lines)
- `addons/sale_loyalty/tests/__init__.py` (16 lines)
- `addons/sale_loyalty/tests/common.py` (376 lines)
- `addons/sale_loyalty/tests/test_buy_gift_card.py` (76 lines)
- `addons/sale_loyalty/tests/test_loyalty.py` (1,464 lines)
- `addons/sale_loyalty/tests/test_loyalty_history.py` (210 lines)
- `addons/sale_loyalty/tests/test_pay_with_gift_card.py` (245 lines)
- `addons/sale_loyalty/tests/test_program_multi_company.py` (140 lines)
- `addons/sale_loyalty/tests/test_program_numbers.py` (2,486 lines)
- `addons/sale_loyalty/tests/test_program_rules.py` (547 lines)
- `addons/sale_loyalty/tests/test_program_with_code_operations.py` (693 lines)
- `addons/sale_loyalty/tests/test_program_without_code_operations.py` (101 lines)
- `addons/sale_loyalty/tests/test_sale_auto_invoice.py` (95 lines)
- `addons/sale_loyalty/tests/test_sale_invoicing.py` (128 lines)
- `addons/sale_loyalty/tests/test_unlink_reward.py` (77 lines)
- `addons/sale_loyalty/views/loyalty_card_views.xml` (15 lines)
- `addons/sale_loyalty/views/loyalty_program_views.xml` (24 lines)
- `addons/sale_loyalty/views/res_partner_views.xml` (15 lines)
- `addons/sale_loyalty/views/sale_loyalty_menus.xml` (23 lines)
- `addons/sale_loyalty/views/sale_order_views.xml` (73 lines)
- `addons/sale_loyalty/views/sale_portal_templates.xml` (134 lines)
- `addons/sale_loyalty/wizard/__init__.py` (3 lines)
- `addons/sale_loyalty/wizard/sale_loyalty_coupon_wizard.py` (31 lines)
- `addons/sale_loyalty/wizard/sale_loyalty_coupon_wizard_views.xml` (29 lines)
- `addons/sale_loyalty/wizard/sale_loyalty_reward_wizard.py` (83 lines)
- `addons/sale_loyalty/wizard/sale_loyalty_reward_wizard_views.xml` (66 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
