# Module: payment_razorpay

- **Module ID:** MOD-410
- **Path:** `addons/payment_razorpay`
- **Manifest:** `addons/payment_razorpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering India.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_provider_views.xml",
    "views/payment_razorpay_templates.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_razorpay/static/src/interactions/payment_form.js"
    ]
  }
}
```

### Representative source files

- `addons/payment_razorpay/README.md` (49 lines)
- `addons/payment_razorpay/__init__.py` (12 lines)
- `addons/payment_razorpay/__manifest__.py` (21 lines)
- `addons/payment_razorpay/const.py` (141 lines)
- `addons/payment_razorpay/controllers/__init__.py` (3 lines)
- `addons/payment_razorpay/controllers/main.py` (84 lines)
- `addons/payment_razorpay/controllers/onboarding.py` (83 lines)
- `addons/payment_razorpay/data/neutralize.sql` (10 lines)
- `addons/payment_razorpay/data/payment_method_data.xml` (163 lines)
- `addons/payment_razorpay/data/payment_provider_data.xml` (9 lines)
- `addons/payment_razorpay/i18n/ar.po` (389 lines)
- `addons/payment_razorpay/i18n/az.po` (379 lines)
- `addons/payment_razorpay/i18n/bg.po` (379 lines)
- `addons/payment_razorpay/i18n/bs.po` (380 lines)
- `addons/payment_razorpay/i18n/ca.po` (380 lines)
- `addons/payment_razorpay/i18n/cs.po` (380 lines)
- `addons/payment_razorpay/i18n/da.po` (381 lines)
- `addons/payment_razorpay/i18n/de.po` (403 lines)
- `addons/payment_razorpay/i18n/el.po` (380 lines)
- `addons/payment_razorpay/i18n/es.po` (394 lines)
- `addons/payment_razorpay/i18n/es_419.po` (393 lines)
- `addons/payment_razorpay/i18n/et.po` (379 lines)
- `addons/payment_razorpay/i18n/fa.po` (379 lines)
- `addons/payment_razorpay/i18n/fi.po` (387 lines)
- `addons/payment_razorpay/i18n/fr.po` (399 lines)
- `addons/payment_razorpay/i18n/he.po` (380 lines)
- `addons/payment_razorpay/i18n/hi.po` (379 lines)
- `addons/payment_razorpay/i18n/hr.po` (380 lines)
- `addons/payment_razorpay/i18n/hu.po` (380 lines)
- `addons/payment_razorpay/i18n/id.po` (390 lines)
- `addons/payment_razorpay/i18n/it.po` (401 lines)
- `addons/payment_razorpay/i18n/ja.po` (395 lines)
- `addons/payment_razorpay/i18n/kab.po` (379 lines)
- `addons/payment_razorpay/i18n/ko.po` (383 lines)
- `addons/payment_razorpay/i18n/ku.po` (379 lines)
- `addons/payment_razorpay/i18n/lo.po` (391 lines)
- `addons/payment_razorpay/i18n/lt.po` (381 lines)
- `addons/payment_razorpay/i18n/lv.po` (379 lines)
- `addons/payment_razorpay/i18n/mn.po` (379 lines)
- `addons/payment_razorpay/i18n/my.po` (379 lines)
- `addons/payment_razorpay/i18n/nb.po` (380 lines)
- `addons/payment_razorpay/i18n/nl.po` (400 lines)
- `addons/payment_razorpay/i18n/payment_razorpay.pot` (373 lines)
- `addons/payment_razorpay/i18n/pl.po` (397 lines)
- `addons/payment_razorpay/i18n/pt.po` (386 lines)
- `addons/payment_razorpay/i18n/pt_BR.po` (398 lines)
- `addons/payment_razorpay/i18n/ro.po` (382 lines)
- `addons/payment_razorpay/i18n/ru.po` (393 lines)
- `addons/payment_razorpay/i18n/sk.po` (378 lines)
- `addons/payment_razorpay/i18n/sl.po` (381 lines)
- `addons/payment_razorpay/i18n/sr@latin.po` (380 lines)
- `addons/payment_razorpay/i18n/sv.po` (385 lines)
- `addons/payment_razorpay/i18n/th.po` (383 lines)
- `addons/payment_razorpay/i18n/tr.po` (389 lines)
- `addons/payment_razorpay/i18n/uk.po` (382 lines)
- `addons/payment_razorpay/i18n/uz.po` (437 lines)
- `addons/payment_razorpay/i18n/vi.po` (389 lines)
- `addons/payment_razorpay/i18n/zh_CN.po` (386 lines)
- `addons/payment_razorpay/i18n/zh_TW.po` (383 lines)
- `addons/payment_razorpay/models/__init__.py` (3 lines)
- `addons/payment_razorpay/models/payment_provider.py` (302 lines)
- `addons/payment_razorpay/models/payment_token.py` (50 lines)
- `addons/payment_razorpay/models/payment_transaction.py` (487 lines)
- `addons/payment_razorpay/static/description/icon.png` (13 lines)
- `addons/payment_razorpay/static/description/icon.svg` (1 lines)
- `addons/payment_razorpay/static/description/icon_hi.png` (84 lines)
- `addons/payment_razorpay/static/src/interactions/payment_form.js` (85 lines)
- `addons/payment_razorpay/tests/__init__.py` (3 lines)
- `addons/payment_razorpay/tests/common.py` (69 lines)
- `addons/payment_razorpay/tests/test_payment_provider.py` (28 lines)
- `addons/payment_razorpay/tests/test_payment_transaction.py` (168 lines)
- `addons/payment_razorpay/tests/test_processing_flows.py` (97 lines)
- `addons/payment_razorpay/views/payment_provider_views.xml` (103 lines)
- `addons/payment_razorpay/views/payment_razorpay_templates.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
