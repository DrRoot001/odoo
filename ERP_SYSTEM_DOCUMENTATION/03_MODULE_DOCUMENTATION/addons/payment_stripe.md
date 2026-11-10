# Module: payment_stripe

- **Module ID:** MOD-412
- **Path:** `addons/payment_stripe`
- **Manifest:** `addons/payment_stripe/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An Irish-American payment provider covering the US and many others.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_provider_views.xml",
    "views/payment_stripe_templates.xml",
    "views/payment_templates.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_stripe/static/src/interactions/**/*",
      "payment_stripe/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_stripe/README.md` (75 lines)
- `addons/payment_stripe/__init__.py` (12 lines)
- `addons/payment_stripe/__manifest__.py` (28 lines)
- `addons/payment_stripe/const.py` (143 lines)
- `addons/payment_stripe/controllers/__init__.py` (3 lines)
- `addons/payment_stripe/controllers/main.py` (278 lines)
- `addons/payment_stripe/controllers/onboarding.py` (43 lines)
- `addons/payment_stripe/data/neutralize.sql` (5 lines)
- `addons/payment_stripe/data/payment_method_data.xml` (743 lines)
- `addons/payment_stripe/data/payment_provider_data.xml` (12 lines)
- `addons/payment_stripe/i18n/ar.po` (525 lines)
- `addons/payment_stripe/i18n/az.po` (501 lines)
- `addons/payment_stripe/i18n/bg.po` (496 lines)
- `addons/payment_stripe/i18n/bs.po` (500 lines)
- `addons/payment_stripe/i18n/ca.po` (515 lines)
- `addons/payment_stripe/i18n/cs.po` (504 lines)
- `addons/payment_stripe/i18n/da.po` (534 lines)
- `addons/payment_stripe/i18n/de.po` (535 lines)
- `addons/payment_stripe/i18n/el.po` (500 lines)
- `addons/payment_stripe/i18n/es.po` (527 lines)
- `addons/payment_stripe/i18n/es_419.po` (525 lines)
- `addons/payment_stripe/i18n/et.po` (505 lines)
- `addons/payment_stripe/i18n/fa.po` (524 lines)
- `addons/payment_stripe/i18n/fi.po` (528 lines)
- `addons/payment_stripe/i18n/fr.po` (526 lines)
- `addons/payment_stripe/i18n/he.po` (501 lines)
- `addons/payment_stripe/i18n/hi.po` (502 lines)
- `addons/payment_stripe/i18n/hr.po` (504 lines)
- `addons/payment_stripe/i18n/hu.po` (501 lines)
- `addons/payment_stripe/i18n/id.po` (527 lines)
- `addons/payment_stripe/i18n/is.po` (493 lines)
- `addons/payment_stripe/i18n/it.po` (532 lines)
- `addons/payment_stripe/i18n/ja.po` (526 lines)
- `addons/payment_stripe/i18n/kab.po` (496 lines)
- `addons/payment_stripe/i18n/ko.po` (522 lines)
- `addons/payment_stripe/i18n/ku.po` (496 lines)
- `addons/payment_stripe/i18n/lo.po` (508 lines)
- `addons/payment_stripe/i18n/lt.po` (507 lines)
- `addons/payment_stripe/i18n/lv.po` (495 lines)
- `addons/payment_stripe/i18n/mn.po` (499 lines)
- `addons/payment_stripe/i18n/my.po` (496 lines)
- `addons/payment_stripe/i18n/nb.po` (499 lines)
- `addons/payment_stripe/i18n/nl.po` (533 lines)
- `addons/payment_stripe/i18n/payment_stripe.pot` (492 lines)
- `addons/payment_stripe/i18n/pl.po` (529 lines)
- `addons/payment_stripe/i18n/pt.po` (518 lines)
- `addons/payment_stripe/i18n/pt_BR.po` (536 lines)
- `addons/payment_stripe/i18n/ro.po` (524 lines)
- `addons/payment_stripe/i18n/ru.po` (527 lines)
- `addons/payment_stripe/i18n/sk.po` (502 lines)
- `addons/payment_stripe/i18n/sl.po` (499 lines)
- `addons/payment_stripe/i18n/sr@latin.po` (501 lines)
- `addons/payment_stripe/i18n/sv.po` (529 lines)
- `addons/payment_stripe/i18n/th.po` (519 lines)
- `addons/payment_stripe/i18n/tr.po` (531 lines)
- `addons/payment_stripe/i18n/uk.po` (531 lines)
- `addons/payment_stripe/i18n/uz.po` (570 lines)
- `addons/payment_stripe/i18n/vi.po` (528 lines)
- `addons/payment_stripe/i18n/zh_CN.po` (517 lines)
- `addons/payment_stripe/i18n/zh_TW.po` (516 lines)
- `addons/payment_stripe/models/__init__.py` (3 lines)
- `addons/payment_stripe/models/payment_provider.py` (540 lines)
- `addons/payment_stripe/models/payment_token.py` (49 lines)
- `addons/payment_stripe/models/payment_transaction.py` (459 lines)
- `addons/payment_stripe/static/description/icon.png` (8 lines)
- `addons/payment_stripe/static/description/icon.svg` (1 lines)
- `addons/payment_stripe/static/description/icon_hi.png` (76 lines)
- `addons/payment_stripe/static/files/apple-developer-merchantid-domain-association` (1 lines)
- `addons/payment_stripe/static/src/interactions/express_checkout.js` (233 lines)
- `addons/payment_stripe/static/src/interactions/payment_form.js` (232 lines)
- `addons/payment_stripe/static/src/interactions/stripe_options.js` (18 lines)
- `addons/payment_stripe/static/src/scss/payment_stripe_templates.scss` (4 lines)
- `addons/payment_stripe/tests/__init__.py` (3 lines)
- `addons/payment_stripe/tests/common.py` (92 lines)
- `addons/payment_stripe/tests/test_processing_flows.py` (147 lines)
- `addons/payment_stripe/tests/test_refund_flows.py` (114 lines)
- `addons/payment_stripe/tests/test_stripe.py` (280 lines)
- `addons/payment_stripe/utils.py` (79 lines)
- `addons/payment_stripe/views/payment_provider_views.xml` (88 lines)
- `addons/payment_stripe/views/payment_stripe_templates.xml` (31 lines)
- `addons/payment_stripe/views/payment_templates.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
