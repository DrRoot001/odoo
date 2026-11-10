# Module: payment

- **Module ID:** MOD-392
- **Path:** `addons/payment`
- **Manifest:** `addons/payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

The payment engine used by payment provider modules.

No manifest description declared.

Declared dependencies: `onboarding`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 14 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 7 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "onboarding",
    "portal"
  ],
  "data": [
    "data/ir_actions_server_data.xml",
    "data/ir_cron_data.xml",
    "data/payment_provider_data.xml",
    "data/portal_entry_data.xml",
    "security/ir.access.csv",
    "views/express_checkout_templates.xml",
    "views/payment_form_templates.xml",
    "views/portal_templates.xml",
    "views/payment_data_views.xml",
    "views/payment_provider_views.xml",
    "views/payment_method_views.xml",
    "views/payment_transaction_views.xml",
    "views/payment_token_views.xml",
    "views/res_partner_views.xml",
    "wizards/payment_capture_wizard_views.xml",
    "wizards/payment_link_wizard_views.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment/static/src/interactions/*",
      "payment/static/src/scss/*",
      "payment/static/src/xml/*"
    ],
    "web.assets_backend": [
      "payment/static/src/scss/payment_provider.scss",
      "payment/static/src/js/payment_wizard_copy_clipboard_field.js",
      "payment/static/src/components/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "payment/static/src/interactions/express_checkout.js",
      "payment/static/src/interactions/payment_button.js",
      "payment/static/src/interactions/payment_form.js"
    ],
    "web.assets_unit_tests": [
      "payment/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/payment/__init__.py` (11 lines)
- `addons/payment/__manifest__.py` (52 lines)
- `addons/payment/const.py` (551 lines)
- `addons/payment/controllers/__init__.py` (3 lines)
- `addons/payment/controllers/payment_status.py` (104 lines)
- `addons/payment/controllers/portal.py` (592 lines)
- `addons/payment/data/ir_actions_server_data.xml` (31 lines)
- `addons/payment/data/ir_cron_data.xml` (28 lines)
- `addons/payment/data/neutralize.sql` (3 lines)
- `addons/payment/data/payment_provider_data.xml` (172 lines)
- `addons/payment/data/portal_entry_data.xml` (12 lines)
- `addons/payment/i18n/af.po` (2,469 lines)
- `addons/payment/i18n/am.po` (2,465 lines)
- `addons/payment/i18n/ar.po` (2,575 lines)
- `addons/payment/i18n/az.po` (2,509 lines)
- `addons/payment/i18n/bg.po` (2,523 lines)
- `addons/payment/i18n/bs.po` (2,501 lines)
- `addons/payment/i18n/ca.po` (2,567 lines)
- `addons/payment/i18n/cs.po` (2,575 lines)
- `addons/payment/i18n/da.po` (2,515 lines)
- `addons/payment/i18n/de.po` (2,676 lines)
- `addons/payment/i18n/el.po` (2,536 lines)
- `addons/payment/i18n/es.po` (2,653 lines)
- `addons/payment/i18n/es_419.po` (2,640 lines)
- `addons/payment/i18n/es_CL.po` (147 lines)
- `addons/payment/i18n/et.po` (2,516 lines)
- `addons/payment/i18n/eu.po` (2,468 lines)
- `addons/payment/i18n/fa.po` (2,525 lines)
- `addons/payment/i18n/fi.po` (2,618 lines)
- `addons/payment/i18n/fo.po` (2,468 lines)
- `addons/payment/i18n/fr.po` (2,642 lines)
- `addons/payment/i18n/fr_BE.po` (160 lines)
- `addons/payment/i18n/fr_CA.po` (135 lines)
- `addons/payment/i18n/gl.po` (2,468 lines)
- `addons/payment/i18n/gu.po` (2,475 lines)
- `addons/payment/i18n/he.po` (2,514 lines)
- `addons/payment/i18n/hi.po` (2,491 lines)
- `addons/payment/i18n/hr.po` (2,557 lines)
- `addons/payment/i18n/hu.po` (2,554 lines)
- `addons/payment/i18n/hy.po` (2,467 lines)
- `addons/payment/i18n/id.po` (2,610 lines)
- `addons/payment/i18n/is.po` (2,475 lines)
- `addons/payment/i18n/it.po` (2,661 lines)
- `addons/payment/i18n/ja.po` (2,591 lines)
- `addons/payment/i18n/ka.po` (2,468 lines)
- `addons/payment/i18n/kab.po` (2,492 lines)
- `addons/payment/i18n/kk.po` (2,467 lines)
- `addons/payment/i18n/km.po` (2,474 lines)
- `addons/payment/i18n/ko.po` (2,572 lines)
- `addons/payment/i18n/ku.po` (2,490 lines)
- `addons/payment/i18n/lb.po` (2,470 lines)
- `addons/payment/i18n/lo.po` (2,575 lines)
- `addons/payment/i18n/lt.po` (2,543 lines)
- `addons/payment/i18n/lv.po` (2,512 lines)
- `addons/payment/i18n/mk.po` (2,468 lines)
- `addons/payment/i18n/mn.po` (2,648 lines)
- `addons/payment/i18n/my.po` (2,492 lines)
- `addons/payment/i18n/nb.po` (2,501 lines)
- `addons/payment/i18n/nl.po` (2,668 lines)
- `addons/payment/i18n/payment.pot` (2,475 lines)
- `addons/payment/i18n/pl.po` (2,654 lines)
- `addons/payment/i18n/pt.po` (2,552 lines)
- `addons/payment/i18n/pt_BR.po` (2,701 lines)
- `addons/payment/i18n/ro.po` (2,610 lines)
- `addons/payment/i18n/ru.po` (2,610 lines)
- `addons/payment/i18n/sk.po` (2,523 lines)
- `addons/payment/i18n/sl.po` (2,563 lines)
- `addons/payment/i18n/sq.po` (2,469 lines)
- `addons/payment/i18n/sr@latin.po` (2,517 lines)
- `addons/payment/i18n/sv.po` (2,615 lines)
- `addons/payment/i18n/ta.po` (2,469 lines)
- `addons/payment/i18n/th.po` (2,555 lines)
- `addons/payment/i18n/tr.po` (2,610 lines)
- `addons/payment/i18n/uk.po` (2,528 lines)
- `addons/payment/i18n/uz.po` (3,896 lines)
- `addons/payment/i18n/vi.po` (2,601 lines)
- `addons/payment/i18n/zh_CN.po` (2,568 lines)
- `addons/payment/i18n/zh_TW.po` (2,550 lines)
- `addons/payment/logging.py` (90 lines)
- `addons/payment/models/__init__.py` (15 lines)
- `addons/payment/models/ir_http.py` (12 lines)
- `addons/payment/models/ir_websocket.py` (76 lines)
- `addons/payment/models/payment_data.py` (121 lines)
- `addons/payment/models/payment_method.py` (273 lines)
- `addons/payment/models/payment_provider.py` (1,273 lines)
- `addons/payment/models/payment_token.py` (185 lines)
- `addons/payment/models/payment_transaction.py` (1,585 lines)
- `addons/payment/models/portal_entry.py` (35 lines)
- `addons/payment/models/res_company.py` (101 lines)
- `addons/payment/models/res_country.py` (30 lines)
- `addons/payment/models/res_partner.py` (38 lines)
- `addons/payment/security/ir.access.csv` (13 lines)
- `addons/payment/static/description/icon.png` (5 lines)
- `addons/payment/static/description/icon.svg` (1 lines)
- `addons/payment/static/description/icon_hi.png` (12 lines)
- `addons/payment/static/img/7eleven.png` (18 lines)
- `addons/payment/static/img/abitab.png` (51 lines)
- `addons/payment/static/img/ach_direct_debit.png` (27 lines)
- `addons/payment/static/img/affirm.png` (40 lines)
- `addons/payment/static/img/afterpay.png` (23 lines)
- `addons/payment/static/img/afterpay_riverty.png` (50 lines)
- `addons/payment/static/img/akulaku.png` (68 lines)
- `addons/payment/static/img/alipay.png` (17 lines)
- `addons/payment/static/img/alipay_hk.png` (26 lines)
- `addons/payment/static/img/alipay_plus.png` (9 lines)
- `addons/payment/static/img/alma.png` (22 lines)
- `addons/payment/static/img/aman.png` (20 lines)
- `addons/payment/static/img/amazon_pay.png` (54 lines)
- `addons/payment/static/img/amex.png` (22 lines)
- `addons/payment/static/img/apple_pay.png` (42 lines)
- `addons/payment/static/img/appota.png` (79 lines)
- `addons/payment/static/img/argencard.png` (13 lines)
- `addons/payment/static/img/atome.png` (65 lines)
- `addons/payment/static/img/bacs_direct_debit.png` (101 lines)
- `addons/payment/static/img/bancnet.png` (27 lines)
- `addons/payment/static/img/banco_de_bogota.png` (47 lines)
- `addons/payment/static/img/banco_guayaquil.png` (48 lines)
- `addons/payment/static/img/banco_pichincha.png` (64 lines)
- `addons/payment/static/img/bancolombia.png` (24 lines)
- `addons/payment/static/img/bancontact.png` (66 lines)
- `addons/payment/static/img/bank.png` (11 lines)
- `addons/payment/static/img/bank_bca.png` (54 lines)
- `addons/payment/static/img/bank_permata.png` (30 lines)
- `addons/payment/static/img/becs_direct_debit.png` (24 lines)
- `addons/payment/static/img/belfius.png` (10 lines)
- `addons/payment/static/img/benefit.png` (67 lines)
- `addons/payment/static/img/bharatqr.png` (40 lines)
- `addons/payment/static/img/billease.png` (23 lines)
- `addons/payment/static/img/billink.png` (59 lines)
- `addons/payment/static/img/bizum.png` (20 lines)
- `addons/payment/static/img/blik.png` (43 lines)
- `addons/payment/static/img/bni.png` (14 lines)
- `addons/payment/static/img/boleto.png` (25 lines)
- `addons/payment/static/img/boost.png` (38 lines)
- `addons/payment/static/img/bri.png` (49 lines)
- `addons/payment/static/img/bsi.png` (21 lines)
- `addons/payment/static/img/cabal.png` (15 lines)
- `addons/payment/static/img/caixa.png` (30 lines)
- `addons/payment/static/img/card.png` (17 lines)
- `addons/payment/static/img/cash_app_pay.png` (46 lines)
- `addons/payment/static/img/cashalo.png` (78 lines)
- `addons/payment/static/img/cebuana.png` (107 lines)
- `addons/payment/static/img/cencosud.png` (48 lines)
- `addons/payment/static/img/cetelem.png` (39 lines)
- `addons/payment/static/img/cimb_niaga.png` (25 lines)
- `addons/payment/static/img/cirrus.png` (21 lines)
- `addons/payment/static/img/clearpay.png` (25 lines)
- `addons/payment/static/img/codensa.png` (27 lines)
- `addons/payment/static/img/cofidis.png` (61 lines)
- `addons/payment/static/img/contact.png` (29 lines)
- `addons/payment/static/img/cordial.png` (26 lines)
- `addons/payment/static/img/cordobesa.png` (52 lines)
- `addons/payment/static/img/cvs.png` (16 lines)
- `addons/payment/static/img/dana.png` (50 lines)
- `addons/payment/static/img/dankort.png` (62 lines)
- `addons/payment/static/img/davivienda.png` (56 lines)
- `addons/payment/static/img/diners.png` (222 lines)
- `addons/payment/static/img/discover.png` (57 lines)
- `addons/payment/static/img/duitnow.png` (100 lines)
- `addons/payment/static/img/elo.png` (54 lines)

Additional files not expanded here: 178. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
