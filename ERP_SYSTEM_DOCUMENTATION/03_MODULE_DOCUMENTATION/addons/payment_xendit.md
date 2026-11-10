# Module: payment_xendit

- **Module ID:** MOD-415
- **Path:** `addons/payment_xendit`
- **Manifest:** `addons/payment_xendit/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider for Indonesian and the Philippines.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
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
    "views/payment_xendit_templates.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_xendit/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_xendit/README.md` (46 lines)
- `addons/payment_xendit/__init__.py` (12 lines)
- `addons/payment_xendit/__manifest__.py` (22 lines)
- `addons/payment_xendit/const.py` (118 lines)
- `addons/payment_xendit/controllers/__init__.py` (3 lines)
- `addons/payment_xendit/controllers/main.py` (83 lines)
- `addons/payment_xendit/data/neutralize.sql` (3 lines)
- `addons/payment_xendit/data/payment_method_data.xml` (497 lines)
- `addons/payment_xendit/data/payment_provider_data.xml` (9 lines)
- `addons/payment_xendit/i18n/ar.po` (400 lines)
- `addons/payment_xendit/i18n/az.po` (359 lines)
- `addons/payment_xendit/i18n/bg.po` (359 lines)
- `addons/payment_xendit/i18n/bs.po` (348 lines)
- `addons/payment_xendit/i18n/ca.po` (384 lines)
- `addons/payment_xendit/i18n/cs.po` (378 lines)
- `addons/payment_xendit/i18n/da.po` (373 lines)
- `addons/payment_xendit/i18n/de.po` (406 lines)
- `addons/payment_xendit/i18n/el.po` (354 lines)
- `addons/payment_xendit/i18n/es.po` (403 lines)
- `addons/payment_xendit/i18n/es_419.po` (402 lines)
- `addons/payment_xendit/i18n/et.po` (374 lines)
- `addons/payment_xendit/i18n/fa.po` (362 lines)
- `addons/payment_xendit/i18n/fi.po` (403 lines)
- `addons/payment_xendit/i18n/fr.po` (403 lines)
- `addons/payment_xendit/i18n/he.po` (372 lines)
- `addons/payment_xendit/i18n/hi.po` (359 lines)
- `addons/payment_xendit/i18n/hr.po` (363 lines)
- `addons/payment_xendit/i18n/hu.po` (360 lines)
- `addons/payment_xendit/i18n/id.po` (403 lines)
- `addons/payment_xendit/i18n/it.po` (403 lines)
- `addons/payment_xendit/i18n/ja.po` (402 lines)
- `addons/payment_xendit/i18n/kab.po` (347 lines)
- `addons/payment_xendit/i18n/ko.po` (399 lines)
- `addons/payment_xendit/i18n/ku.po` (353 lines)
- `addons/payment_xendit/i18n/lo.po` (349 lines)
- `addons/payment_xendit/i18n/lt.po` (361 lines)
- `addons/payment_xendit/i18n/lv.po` (347 lines)
- `addons/payment_xendit/i18n/mn.po` (359 lines)
- `addons/payment_xendit/i18n/my.po` (353 lines)
- `addons/payment_xendit/i18n/nb.po` (360 lines)
- `addons/payment_xendit/i18n/nl.po` (402 lines)
- `addons/payment_xendit/i18n/payment_xendit.pot` (343 lines)
- `addons/payment_xendit/i18n/pl.po` (407 lines)
- `addons/payment_xendit/i18n/pt.po` (400 lines)
- `addons/payment_xendit/i18n/pt_BR.po` (409 lines)
- `addons/payment_xendit/i18n/ro.po` (399 lines)
- `addons/payment_xendit/i18n/ru.po` (406 lines)
- `addons/payment_xendit/i18n/sk.po` (346 lines)
- `addons/payment_xendit/i18n/sl.po` (367 lines)
- `addons/payment_xendit/i18n/sr@latin.po` (357 lines)
- `addons/payment_xendit/i18n/sv.po` (403 lines)
- `addons/payment_xendit/i18n/th.po` (379 lines)
- `addons/payment_xendit/i18n/tr.po` (400 lines)
- `addons/payment_xendit/i18n/uk.po` (375 lines)
- `addons/payment_xendit/i18n/uz.po` (434 lines)
- `addons/payment_xendit/i18n/vi.po` (400 lines)
- `addons/payment_xendit/i18n/zh_CN.po` (401 lines)
- `addons/payment_xendit/i18n/zh_TW.po` (401 lines)
- `addons/payment_xendit/models/__init__.py` (3 lines)
- `addons/payment_xendit/models/payment_provider.py` (120 lines)
- `addons/payment_xendit/models/payment_transaction.py` (512 lines)
- `addons/payment_xendit/static/description/icon.png` (30 lines)
- `addons/payment_xendit/static/description/icon.svg` (1 lines)
- `addons/payment_xendit/static/description/icon_hi.png` (66 lines)
- `addons/payment_xendit/static/src/interactions/payment_form.js` (40 lines)
- `addons/payment_xendit/tests/__init__.py` (3 lines)
- `addons/payment_xendit/tests/common.py` (102 lines)
- `addons/payment_xendit/tests/test_payment_provider.py` (26 lines)
- `addons/payment_xendit/tests/test_payment_transaction.py` (616 lines)
- `addons/payment_xendit/tests/test_processing_flows.py` (224 lines)
- `addons/payment_xendit/views/payment_provider_views.xml` (28 lines)
- `addons/payment_xendit/views/payment_xendit_templates.xml` (11 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
