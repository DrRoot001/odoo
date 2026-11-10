# Module: payment_paypal

- **Module ID:** MOD-408
- **Path:** `addons/payment_paypal`
- **Manifest:** `addons/payment_paypal/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An American payment provider for online payments all over the world.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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
    "views/payment_form_templates.xml",
    "views/payment_paypal_templates.xml",
    "views/payment_provider_views.xml",
    "views/payment_transaction_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_paypal/static/src/interactions/**/*",
      "payment_paypal/static/src/scss/payment_paypal.scss"
    ],
    "web.assets_backend": [
      "payment_paypal/static/src/onboarding/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_paypal/README.md` (42 lines)
- `addons/payment_paypal/__init__.py` (12 lines)
- `addons/payment_paypal/__manifest__.py` (30 lines)
- `addons/payment_paypal/const.py` (86 lines)
- `addons/payment_paypal/controllers/__init__.py` (3 lines)
- `addons/payment_paypal/controllers/main.py` (334 lines)
- `addons/payment_paypal/controllers/onboarding.py` (110 lines)
- `addons/payment_paypal/data/neutralize.sql` (12 lines)
- `addons/payment_paypal/data/payment_method_data.xml` (284 lines)
- `addons/payment_paypal/data/payment_provider_data.xml` (11 lines)
- `addons/payment_paypal/i18n/ar.po` (419 lines)
- `addons/payment_paypal/i18n/az.po` (400 lines)
- `addons/payment_paypal/i18n/bg.po` (403 lines)
- `addons/payment_paypal/i18n/bs.po` (402 lines)
- `addons/payment_paypal/i18n/ca.po` (418 lines)
- `addons/payment_paypal/i18n/cs.po` (407 lines)
- `addons/payment_paypal/i18n/da.po` (408 lines)
- `addons/payment_paypal/i18n/de.po` (442 lines)
- `addons/payment_paypal/i18n/el.po` (407 lines)
- `addons/payment_paypal/i18n/es.po` (423 lines)
- `addons/payment_paypal/i18n/es_419.po` (422 lines)
- `addons/payment_paypal/i18n/et.po` (407 lines)
- `addons/payment_paypal/i18n/fa.po` (403 lines)
- `addons/payment_paypal/i18n/fi.po` (426 lines)
- `addons/payment_paypal/i18n/fr.po` (422 lines)
- `addons/payment_paypal/i18n/he.po` (409 lines)
- `addons/payment_paypal/i18n/hi.po` (400 lines)
- `addons/payment_paypal/i18n/hr.po` (409 lines)
- `addons/payment_paypal/i18n/hu.po` (408 lines)
- `addons/payment_paypal/i18n/id.po` (420 lines)
- `addons/payment_paypal/i18n/it.po` (435 lines)
- `addons/payment_paypal/i18n/ja.po` (421 lines)
- `addons/payment_paypal/i18n/kab.po` (399 lines)
- `addons/payment_paypal/i18n/ko.po` (417 lines)
- `addons/payment_paypal/i18n/ku.po` (400 lines)
- `addons/payment_paypal/i18n/lo.po` (411 lines)
- `addons/payment_paypal/i18n/lt.po` (410 lines)
- `addons/payment_paypal/i18n/lv.po` (399 lines)
- `addons/payment_paypal/i18n/mn.po` (406 lines)
- `addons/payment_paypal/i18n/my.po` (400 lines)
- `addons/payment_paypal/i18n/nb.po` (406 lines)
- `addons/payment_paypal/i18n/nl.po` (440 lines)
- `addons/payment_paypal/i18n/payment_paypal.pot` (393 lines)
- `addons/payment_paypal/i18n/pl.po` (428 lines)
- `addons/payment_paypal/i18n/pt.po` (410 lines)
- `addons/payment_paypal/i18n/pt_BR.po` (438 lines)
- `addons/payment_paypal/i18n/ro.po` (420 lines)
- `addons/payment_paypal/i18n/ru.po` (423 lines)
- `addons/payment_paypal/i18n/sk.po` (408 lines)
- `addons/payment_paypal/i18n/sl.po` (404 lines)
- `addons/payment_paypal/i18n/sr@latin.po` (401 lines)
- `addons/payment_paypal/i18n/sv.po` (418 lines)
- `addons/payment_paypal/i18n/th.po` (411 lines)
- `addons/payment_paypal/i18n/tr.po` (427 lines)
- `addons/payment_paypal/i18n/uk.po` (415 lines)
- `addons/payment_paypal/i18n/uz.po` (456 lines)
- `addons/payment_paypal/i18n/vi.po` (418 lines)
- `addons/payment_paypal/i18n/zh_CN.po` (431 lines)
- `addons/payment_paypal/i18n/zh_TW.po` (415 lines)
- `addons/payment_paypal/models/__init__.py` (3 lines)
- `addons/payment_paypal/models/payment_provider.py` (365 lines)
- `addons/payment_paypal/models/payment_token.py` (18 lines)
- `addons/payment_paypal/models/payment_transaction.py` (461 lines)
- `addons/payment_paypal/static/description/icon.png` (7 lines)
- `addons/payment_paypal/static/description/icon.svg` (1 lines)
- `addons/payment_paypal/static/description/icon_hi.png` (86 lines)
- `addons/payment_paypal/static/src/interactions/payment_button.js` (76 lines)
- `addons/payment_paypal/static/src/interactions/payment_form.js` (381 lines)
- `addons/payment_paypal/static/src/onboarding/paypal_onboarding.js` (59 lines)
- `addons/payment_paypal/static/src/onboarding/paypal_onboarding.scss` (6 lines)
- `addons/payment_paypal/static/src/scss/payment_paypal.scss` (7 lines)
- `addons/payment_paypal/tests/__init__.py` (3 lines)
- `addons/payment_paypal/tests/common.py` (111 lines)
- `addons/payment_paypal/tests/test_paypal.py` (366 lines)
- `addons/payment_paypal/utils.py` (119 lines)
- `addons/payment_paypal/views/payment_form_templates.xml` (26 lines)
- `addons/payment_paypal/views/payment_paypal_templates.xml` (36 lines)
- `addons/payment_paypal/views/payment_provider_views.xml` (123 lines)
- `addons/payment_paypal/views/payment_transaction_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
