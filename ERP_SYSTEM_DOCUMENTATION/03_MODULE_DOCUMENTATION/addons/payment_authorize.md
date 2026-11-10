# Module: payment_authorize

- **Module ID:** MOD-396
- **Path:** `addons/payment_authorize`
- **Manifest:** `addons/payment_authorize/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An payment provider covering the US, Australia, and Canada.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_authorize_templates.xml",
    "views/payment_provider_views.xml",
    "views/payment_token_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_authorize/static/src/interactions/payment_form.js",
      "payment_authorize/static/src/scss/payment_authorize.scss"
    ]
  }
}
```

### Representative source files

- `addons/payment_authorize/README.md` (70 lines)
- `addons/payment_authorize/__init__.py` (12 lines)
- `addons/payment_authorize/__manifest__.py` (28 lines)
- `addons/payment_authorize/const.py` (37 lines)
- `addons/payment_authorize/controllers/__init__.py` (3 lines)
- `addons/payment_authorize/controllers/main.py` (90 lines)
- `addons/payment_authorize/data/neutralize.sql` (6 lines)
- `addons/payment_authorize/data/payment_method_data.xml` (83 lines)
- `addons/payment_authorize/data/payment_provider_data.xml` (10 lines)
- `addons/payment_authorize/i18n/ar.po` (377 lines)
- `addons/payment_authorize/i18n/az.po` (353 lines)
- `addons/payment_authorize/i18n/bg.po` (353 lines)
- `addons/payment_authorize/i18n/bs.po` (356 lines)
- `addons/payment_authorize/i18n/ca.po` (372 lines)
- `addons/payment_authorize/i18n/cs.po` (362 lines)
- `addons/payment_authorize/i18n/da.po` (361 lines)
- `addons/payment_authorize/i18n/de.po` (381 lines)
- `addons/payment_authorize/i18n/el.po` (360 lines)
- `addons/payment_authorize/i18n/es.po` (380 lines)
- `addons/payment_authorize/i18n/es_419.po` (376 lines)
- `addons/payment_authorize/i18n/et.po` (358 lines)
- `addons/payment_authorize/i18n/fa.po` (356 lines)
- `addons/payment_authorize/i18n/fi.po` (384 lines)
- `addons/payment_authorize/i18n/fr.po` (381 lines)
- `addons/payment_authorize/i18n/he.po` (360 lines)
- `addons/payment_authorize/i18n/hi.po` (353 lines)
- `addons/payment_authorize/i18n/hr.po` (360 lines)
- `addons/payment_authorize/i18n/hu.po` (358 lines)
- `addons/payment_authorize/i18n/id.po` (376 lines)
- `addons/payment_authorize/i18n/it.po` (380 lines)
- `addons/payment_authorize/i18n/ja.po` (378 lines)
- `addons/payment_authorize/i18n/kab.po` (353 lines)
- `addons/payment_authorize/i18n/ko.po` (375 lines)
- `addons/payment_authorize/i18n/ku.po` (353 lines)
- `addons/payment_authorize/i18n/lo.po` (364 lines)
- `addons/payment_authorize/i18n/lt.po` (365 lines)
- `addons/payment_authorize/i18n/lv.po` (353 lines)
- `addons/payment_authorize/i18n/mn.po` (357 lines)
- `addons/payment_authorize/i18n/my.po` (353 lines)
- `addons/payment_authorize/i18n/nb.po` (360 lines)
- `addons/payment_authorize/i18n/nl.po` (383 lines)
- `addons/payment_authorize/i18n/payment_authorize.pot` (349 lines)
- `addons/payment_authorize/i18n/pl.po` (381 lines)
- `addons/payment_authorize/i18n/pt.po` (369 lines)
- `addons/payment_authorize/i18n/pt_BR.po` (383 lines)
- `addons/payment_authorize/i18n/ro.po` (375 lines)
- `addons/payment_authorize/i18n/ru.po` (378 lines)
- `addons/payment_authorize/i18n/sk.po` (358 lines)
- `addons/payment_authorize/i18n/sl.po` (355 lines)
- `addons/payment_authorize/i18n/sr@latin.po` (354 lines)
- `addons/payment_authorize/i18n/sv.po` (377 lines)
- `addons/payment_authorize/i18n/th.po` (372 lines)
- `addons/payment_authorize/i18n/tr.po` (383 lines)
- `addons/payment_authorize/i18n/uk.po` (363 lines)
- `addons/payment_authorize/i18n/uz.po` (414 lines)
- `addons/payment_authorize/i18n/vi.po` (375 lines)
- `addons/payment_authorize/i18n/zh_CN.po` (374 lines)
- `addons/payment_authorize/i18n/zh_TW.po` (369 lines)
- `addons/payment_authorize/models/__init__.py` (3 lines)
- `addons/payment_authorize/models/authorize_request.py` (377 lines)
- `addons/payment_authorize/models/payment_provider.py` (200 lines)
- `addons/payment_authorize/models/payment_token.py` (16 lines)
- `addons/payment_authorize/models/payment_transaction.py` (295 lines)
- `addons/payment_authorize/static/description/icon.png` (11 lines)
- `addons/payment_authorize/static/description/icon.svg` (1 lines)
- `addons/payment_authorize/static/description/icon_hi.png` (96 lines)
- `addons/payment_authorize/static/src/interactions/payment_form.js` (225 lines)
- `addons/payment_authorize/static/src/scss/payment_authorize.scss` (16 lines)
- `addons/payment_authorize/tests/__init__.py` (9 lines)
- `addons/payment_authorize/tests/common.py` (47 lines)
- `addons/payment_authorize/tests/test_authorize.py` (169 lines)
- `addons/payment_authorize/tests/test_payment_transaction.py` (16 lines)
- `addons/payment_authorize/tests/test_processing_flows.py` (45 lines)
- `addons/payment_authorize/tests/test_refund_flows.py` (103 lines)
- `addons/payment_authorize/views/payment_authorize_templates.xml` (57 lines)
- `addons/payment_authorize/views/payment_provider_views.xml` (85 lines)
- `addons/payment_authorize/views/payment_token_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
