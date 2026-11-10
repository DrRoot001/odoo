# Module: loyalty

- **Module ID:** MOD-349
- **Path:** `addons/loyalty`
- **Manifest:** `addons/loyalty/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Use discounts, gift cards, eWallets and loyalty programs in your sales channels

No manifest description declared.

Declared dependencies: `product`, `portal`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 17 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "product",
    "portal",
    "account"
  ],
  "data": [
    "report/loyalty_report_templates.xml",
    "report/loyalty_report.xml",
    "data/mail_template_data.xml",
    "data/loyalty_data.xml",
    "wizard/loyalty_card_update_balance_views.xml",
    "wizard/loyalty_generate_wizard_views.xml",
    "views/loyalty_card_views.xml",
    "views/loyalty_history_views.xml",
    "views/loyalty_mail_views.xml",
    "views/loyalty_program_views.xml",
    "views/loyalty_reward_views.xml",
    "views/loyalty_rule_views.xml",
    "views/portal_templates.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/loyalty_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "loyalty/static/src/js/**/*.js",
      "loyalty/static/src/scss/*.scss",
      "loyalty/static/src/xml/*.xml",
      [
        "remove",
        "loyalty/static/src/js/portal/**/*"
      ],
      [
        "remove",
        "loyalty/static/src/scss/*.dark.scss"
      ]
    ],
    "web.assets_web_dark": [
      "loyalty/static/src/scss/*.dark.scss"
    ],
    "web.assets_frontend": [
      "loyalty/static/src/js/portal/**/*",
      "loyalty/static/src/interactions/*"
    ]
  }
}
```

### Representative source files

- `addons/loyalty/__init__.py` (3 lines)
- `addons/loyalty/__manifest__.py` (43 lines)
- `addons/loyalty/controllers/__init__.py` (1 lines)
- `addons/loyalty/controllers/portal.py` (149 lines)
- `addons/loyalty/data/loyalty_data.xml` (53 lines)
- `addons/loyalty/data/loyalty_demo.xml` (75 lines)
- `addons/loyalty/data/mail_template_data.xml` (132 lines)
- `addons/loyalty/i18n/ar.po` (2,535 lines)
- `addons/loyalty/i18n/az.po` (2,344 lines)
- `addons/loyalty/i18n/bg.po` (2,350 lines)
- `addons/loyalty/i18n/bs.po` (2,346 lines)
- `addons/loyalty/i18n/ca.po` (2,418 lines)
- `addons/loyalty/i18n/cs.po` (2,400 lines)
- `addons/loyalty/i18n/da.po` (2,357 lines)
- `addons/loyalty/i18n/de.po` (2,895 lines)
- `addons/loyalty/i18n/el.po` (2,351 lines)
- `addons/loyalty/i18n/es.po` (2,553 lines)
- `addons/loyalty/i18n/es_419.po` (2,902 lines)
- `addons/loyalty/i18n/et.po` (2,755 lines)
- `addons/loyalty/i18n/fa.po` (2,344 lines)
- `addons/loyalty/i18n/fi.po` (2,874 lines)
- `addons/loyalty/i18n/fr.po` (2,701 lines)
- `addons/loyalty/i18n/he.po` (2,345 lines)
- `addons/loyalty/i18n/hi.po` (2,344 lines)
- `addons/loyalty/i18n/hr.po` (2,345 lines)
- `addons/loyalty/i18n/hu.po` (2,349 lines)
- `addons/loyalty/i18n/id.po` (2,666 lines)
- `addons/loyalty/i18n/it.po` (2,690 lines)
- `addons/loyalty/i18n/ja.po` (2,667 lines)
- `addons/loyalty/i18n/kab.po` (2,345 lines)
- `addons/loyalty/i18n/ko.po` (2,653 lines)
- `addons/loyalty/i18n/ku.po` (2,344 lines)
- `addons/loyalty/i18n/lo.po` (2,724 lines)
- `addons/loyalty/i18n/loyalty.pot` (2,272 lines)
- `addons/loyalty/i18n/lt.po` (2,346 lines)
- `addons/loyalty/i18n/lv.po` (2,345 lines)
- `addons/loyalty/i18n/mn.po` (2,344 lines)
- `addons/loyalty/i18n/my.po` (2,345 lines)
- `addons/loyalty/i18n/nb.po` (2,351 lines)
- `addons/loyalty/i18n/nl.po` (2,885 lines)
- `addons/loyalty/i18n/pl.po` (2,675 lines)
- `addons/loyalty/i18n/pt.po` (2,738 lines)
- `addons/loyalty/i18n/pt_BR.po` (2,880 lines)
- `addons/loyalty/i18n/ro.po` (2,500 lines)
- `addons/loyalty/i18n/ru.po` (2,558 lines)
- `addons/loyalty/i18n/sk.po` (2,344 lines)
- `addons/loyalty/i18n/sl.po` (2,414 lines)
- `addons/loyalty/i18n/sr@latin.po` (2,346 lines)
- `addons/loyalty/i18n/sv.po` (2,424 lines)
- `addons/loyalty/i18n/th.po` (2,630 lines)
- `addons/loyalty/i18n/tr.po` (2,676 lines)
- `addons/loyalty/i18n/uk.po` (2,345 lines)
- `addons/loyalty/i18n/uz.po` (2,881 lines)
- `addons/loyalty/i18n/vi.po` (2,673 lines)
- `addons/loyalty/i18n/zh_CN.po` (2,723 lines)
- `addons/loyalty/i18n/zh_TW.po` (2,638 lines)
- `addons/loyalty/models/__init__.py` (14 lines)
- `addons/loyalty/models/loyalty_card.py` (309 lines)
- `addons/loyalty/models/loyalty_history.py` (313 lines)
- `addons/loyalty/models/loyalty_mail.py` (29 lines)
- `addons/loyalty/models/loyalty_program.py` (762 lines)
- `addons/loyalty/models/loyalty_reward.py` (404 lines)
- `addons/loyalty/models/loyalty_rule.py` (169 lines)
- `addons/loyalty/models/product_pricelist.py` (25 lines)
- `addons/loyalty/models/product_product.py` (49 lines)
- `addons/loyalty/models/product_template.py` (33 lines)
- `addons/loyalty/models/res_partner.py` (48 lines)
- `addons/loyalty/report/loyalty_report.xml` (22 lines)
- `addons/loyalty/report/loyalty_report_templates.xml` (133 lines)
- `addons/loyalty/security/ir.access.csv` (6 lines)
- `addons/loyalty/static/img/2_plus_1.svg` (32 lines)
- `addons/loyalty/static/img/coupons.svg` (56 lines)
- `addons/loyalty/static/img/discount_placeholder_thumbnail.png` (31 lines)
- `addons/loyalty/static/img/ewallet.svg` (15 lines)
- `addons/loyalty/static/img/fidelity_cards.svg` (13 lines)
- `addons/loyalty/static/img/gift_card.png` (22 lines)
- `addons/loyalty/static/img/gift_card.svg` (22 lines)
- `addons/loyalty/static/img/loyalty_cards.svg` (9 lines)
- `addons/loyalty/static/img/loyalty_cards_2.svg` (1 lines)
- `addons/loyalty/static/img/portal-loyalty.svg` (14 lines)
- `addons/loyalty/static/img/promo_code.svg` (10 lines)
- `addons/loyalty/static/img/promotional_program.svg` (13 lines)
- `addons/loyalty/static/src/img/ewallet.svg` (15 lines)
- `addons/loyalty/static/src/img/loyalty.svg` (14 lines)
- `addons/loyalty/static/src/interactions/loyalty_card.js` (21 lines)
- `addons/loyalty/static/src/js/loyalty_card_list_view.js` (9 lines)
- `addons/loyalty/static/src/js/loyalty_control_panel_widget.js` (13 lines)
- `addons/loyalty/static/src/js/loyalty_list_view.js` (55 lines)
- `addons/loyalty/static/src/js/portal/loyalty_card_dialog/loyalty_card_dialog.js` (38 lines)
- `addons/loyalty/static/src/js/portal/loyalty_card_dialog/loyalty_card_dialog.xml` (66 lines)
- `addons/loyalty/static/src/scss/loyalty.dark.scss` (7 lines)
- `addons/loyalty/static/src/scss/loyalty.scss` (64 lines)
- `addons/loyalty/static/src/xml/loyalty_templates.xml` (56 lines)
- `addons/loyalty/tests/__init__.py` (3 lines)
- `addons/loyalty/tests/test_loyalty.py` (397 lines)
- `addons/loyalty/views/loyalty_card_views.xml` (105 lines)
- `addons/loyalty/views/loyalty_history_views.xml` (28 lines)
- `addons/loyalty/views/loyalty_mail_views.xml` (16 lines)
- `addons/loyalty/views/loyalty_program_views.xml` (314 lines)
- `addons/loyalty/views/loyalty_reward_views.xml` (145 lines)
- `addons/loyalty/views/loyalty_rule_views.xml` (111 lines)
- `addons/loyalty/views/portal_templates.xml` (106 lines)
- `addons/loyalty/views/res_partner_views.xml` (23 lines)
- `addons/loyalty/wizard/__init__.py` (3 lines)
- `addons/loyalty/wizard/base_partner_merge.py` (41 lines)
- `addons/loyalty/wizard/loyalty_card_update_balance.py` (22 lines)
- `addons/loyalty/wizard/loyalty_card_update_balance_views.xml` (33 lines)
- `addons/loyalty/wizard/loyalty_generate_wizard.py` (116 lines)
- `addons/loyalty/wizard/loyalty_generate_wizard_views.xml` (66 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
