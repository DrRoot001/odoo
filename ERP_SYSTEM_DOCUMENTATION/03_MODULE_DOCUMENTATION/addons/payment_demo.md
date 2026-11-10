# Module: payment_demo

- **Module ID:** MOD-399
- **Path:** `addons/payment_demo`
- **Manifest:** `addons/payment_demo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider for running fake payment flows for demo purposes.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_demo_templates.xml",
    "views/payment_provider_views.xml",
    "views/payment_token_views.xml",
    "views/payment_transaction_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_demo/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/payment_demo/README.md` (35 lines)
- `addons/payment_demo/__init__.py` (12 lines)
- `addons/payment_demo/__manifest__.py` (24 lines)
- `addons/payment_demo/const.py` (4 lines)
- `addons/payment_demo/controllers/__init__.py` (3 lines)
- `addons/payment_demo/controllers/main.py` (17 lines)
- `addons/payment_demo/controllers/portal.py` (36 lines)
- `addons/payment_demo/data/payment_method_data.xml` (28 lines)
- `addons/payment_demo/data/payment_provider_data.xml` (14 lines)
- `addons/payment_demo/i18n/ar.po` (320 lines)
- `addons/payment_demo/i18n/az.po` (328 lines)
- `addons/payment_demo/i18n/bg.po` (329 lines)
- `addons/payment_demo/i18n/bs.po` (330 lines)
- `addons/payment_demo/i18n/ca.po` (322 lines)
- `addons/payment_demo/i18n/cs.po` (319 lines)
- `addons/payment_demo/i18n/da.po` (314 lines)
- `addons/payment_demo/i18n/de.po` (332 lines)
- `addons/payment_demo/i18n/el.po` (318 lines)
- `addons/payment_demo/i18n/es.po` (327 lines)
- `addons/payment_demo/i18n/es_419.po` (326 lines)
- `addons/payment_demo/i18n/et.po` (347 lines)
- `addons/payment_demo/i18n/fa.po` (359 lines)
- `addons/payment_demo/i18n/fi.po` (319 lines)
- `addons/payment_demo/i18n/fr.po` (325 lines)
- `addons/payment_demo/i18n/he.po` (339 lines)
- `addons/payment_demo/i18n/hi.po` (336 lines)
- `addons/payment_demo/i18n/hr.po` (333 lines)
- `addons/payment_demo/i18n/hu.po` (320 lines)
- `addons/payment_demo/i18n/id.po` (327 lines)
- `addons/payment_demo/i18n/it.po` (327 lines)
- `addons/payment_demo/i18n/ja.po` (317 lines)
- `addons/payment_demo/i18n/kab.po` (320 lines)
- `addons/payment_demo/i18n/ko.po` (317 lines)
- `addons/payment_demo/i18n/ku.po` (322 lines)
- `addons/payment_demo/i18n/lo.po` (315 lines)
- `addons/payment_demo/i18n/lt.po` (332 lines)
- `addons/payment_demo/i18n/lv.po` (334 lines)
- `addons/payment_demo/i18n/mn.po` (329 lines)
- `addons/payment_demo/i18n/my.po` (326 lines)
- `addons/payment_demo/i18n/nb.po` (318 lines)
- `addons/payment_demo/i18n/nl.po` (325 lines)
- `addons/payment_demo/i18n/payment_demo.pot` (306 lines)
- `addons/payment_demo/i18n/pl.po` (329 lines)
- `addons/payment_demo/i18n/pt.po` (327 lines)
- `addons/payment_demo/i18n/pt_BR.po` (329 lines)
- `addons/payment_demo/i18n/ro.po` (324 lines)
- `addons/payment_demo/i18n/ru.po` (333 lines)
- `addons/payment_demo/i18n/sk.po` (358 lines)
- `addons/payment_demo/i18n/sl.po` (320 lines)
- `addons/payment_demo/i18n/sr@latin.po` (328 lines)
- `addons/payment_demo/i18n/sv.po` (330 lines)
- `addons/payment_demo/i18n/th.po` (322 lines)
- `addons/payment_demo/i18n/tr.po` (327 lines)
- `addons/payment_demo/i18n/uk.po` (362 lines)
- `addons/payment_demo/i18n/uz.po` (376 lines)
- `addons/payment_demo/i18n/vi.po` (329 lines)
- `addons/payment_demo/i18n/zh_CN.po` (321 lines)
- `addons/payment_demo/i18n/zh_TW.po` (322 lines)
- `addons/payment_demo/models/__init__.py` (3 lines)
- `addons/payment_demo/models/payment_provider.py` (40 lines)
- `addons/payment_demo/models/payment_token.py` (33 lines)
- `addons/payment_demo/models/payment_transaction.py` (165 lines)
- `addons/payment_demo/static/description/icon.png` (8 lines)
- `addons/payment_demo/static/description/icon.svg` (1 lines)
- `addons/payment_demo/static/description/icon_hi.png` (22 lines)
- `addons/payment_demo/static/img/demo.png` (13 lines)
- `addons/payment_demo/static/src/interactions/express_checkout.js` (82 lines)
- `addons/payment_demo/static/src/interactions/payment_demo_mixin.js` (34 lines)
- `addons/payment_demo/static/src/interactions/payment_form.js` (53 lines)
- `addons/payment_demo/tests/__init__.py` (3 lines)
- `addons/payment_demo/tests/common.py` (17 lines)
- `addons/payment_demo/tests/test_payment_transaction.py` (89 lines)
- `addons/payment_demo/tests/test_processing_flows.py` (22 lines)
- `addons/payment_demo/views/payment_demo_templates.xml` (217 lines)
- `addons/payment_demo/views/payment_provider_views.xml` (15 lines)
- `addons/payment_demo/views/payment_token_views.xml` (19 lines)
- `addons/payment_demo/views/payment_transaction_views.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
