# Module: website_payment

- **Module ID:** MOD-631
- **Path:** `addons/website_payment`
- **Manifest:** `addons/website_payment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Payment integration with website


This is a bridge module that adds multi-website support for payment providers.
    

Declared dependencies: `website`, `account_payment`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "account_payment",
    "portal"
  ],
  "data": [
    "views/payment_provider.xml",
    "views/res_config_settings_views.xml",
    "views/snippets/snippets.xml",
    "views/snippets/s_supported_payment_methods.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_payment/static/src/snippets/**/*.js",
      [
        "remove",
        "website_payment/static/src/snippets/**/*.edit.js"
      ]
    ],
    "website.assets_inside_builder_iframe": [
      "website_payment/static/src/**/*.edit.js"
    ],
    "website.website_builder_assets": [
      "website_payment/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_payment/__init__.py` (5 lines)
- `addons/website_payment/__manifest__.py` (35 lines)
- `addons/website_payment/controllers/__init__.py` (5 lines)
- `addons/website_payment/controllers/payment.py` (18 lines)
- `addons/website_payment/controllers/portal.py` (70 lines)
- `addons/website_payment/i18n/af.po` (198 lines)
- `addons/website_payment/i18n/ar.po` (412 lines)
- `addons/website_payment/i18n/az.po` (221 lines)
- `addons/website_payment/i18n/bg.po` (229 lines)
- `addons/website_payment/i18n/bs.po` (189 lines)
- `addons/website_payment/i18n/ca.po` (385 lines)
- `addons/website_payment/i18n/cs.po` (376 lines)
- `addons/website_payment/i18n/da.po` (418 lines)
- `addons/website_payment/i18n/de.po` (476 lines)
- `addons/website_payment/i18n/el.po` (225 lines)
- `addons/website_payment/i18n/es.po` (422 lines)
- `addons/website_payment/i18n/es_419.po` (465 lines)
- `addons/website_payment/i18n/es_CL.po` (27 lines)
- `addons/website_payment/i18n/et.po` (391 lines)
- `addons/website_payment/i18n/eu.po` (187 lines)
- `addons/website_payment/i18n/fa.po` (376 lines)
- `addons/website_payment/i18n/fi.po` (445 lines)
- `addons/website_payment/i18n/fr.po` (474 lines)
- `addons/website_payment/i18n/fr_CA.po` (22 lines)
- `addons/website_payment/i18n/gl.po` (187 lines)
- `addons/website_payment/i18n/gu.po` (197 lines)
- `addons/website_payment/i18n/he.po` (314 lines)
- `addons/website_payment/i18n/hi.po` (225 lines)
- `addons/website_payment/i18n/hr.po` (424 lines)
- `addons/website_payment/i18n/hu.po` (261 lines)
- `addons/website_payment/i18n/id.po` (420 lines)
- `addons/website_payment/i18n/is.po` (182 lines)
- `addons/website_payment/i18n/it.po` (475 lines)
- `addons/website_payment/i18n/ja.po` (466 lines)
- `addons/website_payment/i18n/ka.po` (187 lines)
- `addons/website_payment/i18n/kab.po` (189 lines)
- `addons/website_payment/i18n/kk.po` (184 lines)
- `addons/website_payment/i18n/km.po` (185 lines)
- `addons/website_payment/i18n/ko.po` (423 lines)
- `addons/website_payment/i18n/ku.po` (210 lines)
- `addons/website_payment/i18n/lo.po` (194 lines)
- `addons/website_payment/i18n/lt.po` (304 lines)
- `addons/website_payment/i18n/lv.po` (332 lines)
- `addons/website_payment/i18n/mk.po` (189 lines)
- `addons/website_payment/i18n/mn.po` (236 lines)
- `addons/website_payment/i18n/my.po` (216 lines)
- `addons/website_payment/i18n/nb.po` (237 lines)
- `addons/website_payment/i18n/nl.po` (472 lines)
- `addons/website_payment/i18n/pl.po` (429 lines)
- `addons/website_payment/i18n/pt.po` (379 lines)
- `addons/website_payment/i18n/pt_BR.po` (478 lines)
- `addons/website_payment/i18n/ro.po` (396 lines)
- `addons/website_payment/i18n/ru.po` (400 lines)
- `addons/website_payment/i18n/sk.po` (238 lines)
- `addons/website_payment/i18n/sl.po` (377 lines)
- `addons/website_payment/i18n/sq.po` (187 lines)
- `addons/website_payment/i18n/sr@latin.po` (374 lines)
- `addons/website_payment/i18n/sv.po` (405 lines)
- `addons/website_payment/i18n/th.po` (387 lines)
- `addons/website_payment/i18n/tr.po` (451 lines)
- `addons/website_payment/i18n/uk.po` (376 lines)
- `addons/website_payment/i18n/uz.po` (524 lines)
- `addons/website_payment/i18n/vi.po` (396 lines)
- `addons/website_payment/i18n/website_payment.pot` (180 lines)
- `addons/website_payment/i18n/zh_CN.po` (426 lines)
- `addons/website_payment/i18n/zh_TW.po` (450 lines)
- `addons/website_payment/models/__init__.py` (3 lines)
- `addons/website_payment/models/payment_provider.py` (67 lines)
- `addons/website_payment/models/res_config_settings.py` (29 lines)
- `addons/website_payment/static/description/icon.png` (34 lines)
- `addons/website_payment/static/description/icon.svg` (1 lines)
- `addons/website_payment/static/description/icon_hi.png` (102 lines)
- `addons/website_payment/static/img/s_supported_payment_methods.svg` (4 lines)
- `addons/website_payment/static/src/snippets/s_supported_payment_methods/000.edit.xml` (28 lines)
- `addons/website_payment/static/src/snippets/s_supported_payment_methods/000.xml` (20 lines)
- `addons/website_payment/static/src/snippets/s_supported_payment_methods/supported_payment_methods.edit.js` (31 lines)
- `addons/website_payment/static/src/snippets/s_supported_payment_methods/supported_payment_methods.js` (51 lines)
- `addons/website_payment/static/src/website_builder/supported_payment_methods_option.xml` (56 lines)
- `addons/website_payment/static/src/website_builder/supported_payment_methods_option_plugin.js` (64 lines)
- `addons/website_payment/tests/__init__.py` (1 lines)
- `addons/website_payment/tests/test_website_payment_technical_page.py` (11 lines)
- `addons/website_payment/views/payment_provider.xml` (22 lines)
- `addons/website_payment/views/res_config_settings_views.xml` (125 lines)
- `addons/website_payment/views/snippets/s_supported_payment_methods.xml` (29 lines)
- `addons/website_payment/views/snippets/snippets.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
