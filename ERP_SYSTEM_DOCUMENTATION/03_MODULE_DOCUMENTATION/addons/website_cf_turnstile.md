# Module: website_cf_turnstile

- **Module ID:** MOD-599
- **Path:** `addons/website_cf_turnstile`
- **Manifest:** `addons/website_cf_turnstile/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements Cloudflare Turnstile so that you can prevent bot spam on your forms.
    

Declared dependencies: `website`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 7 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website"
  ],
  "data": [
    "views/res_config_settings_view.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_cf_turnstile/static/src/interactions/**/*.js",
      "website_cf_turnstile/static/src/interactions/**/*.xml"
    ],
    "web.assets_unit_tests": [
      "website_cf_turnstile/static/tests/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_cf_turnstile/static/src/interactions/**/*.js",
      "website_cf_turnstile/static/src/interactions/**/*.xml"
    ]
  }
}
```

### Representative source files

- `addons/website_cf_turnstile/__init__.py` (4 lines)
- `addons/website_cf_turnstile/__manifest__.py` (28 lines)
- `addons/website_cf_turnstile/data/neutralize.sql` (4 lines)
- `addons/website_cf_turnstile/i18n/ar.po` (134 lines)
- `addons/website_cf_turnstile/i18n/az.po` (127 lines)
- `addons/website_cf_turnstile/i18n/bg.po` (127 lines)
- `addons/website_cf_turnstile/i18n/bs.po` (129 lines)
- `addons/website_cf_turnstile/i18n/ca.po` (131 lines)
- `addons/website_cf_turnstile/i18n/cs.po` (128 lines)
- `addons/website_cf_turnstile/i18n/da.po` (136 lines)
- `addons/website_cf_turnstile/i18n/de.po` (142 lines)
- `addons/website_cf_turnstile/i18n/el.po` (128 lines)
- `addons/website_cf_turnstile/i18n/es.po` (140 lines)
- `addons/website_cf_turnstile/i18n/es_419.po` (135 lines)
- `addons/website_cf_turnstile/i18n/et.po` (127 lines)
- `addons/website_cf_turnstile/i18n/fa.po` (127 lines)
- `addons/website_cf_turnstile/i18n/fi.po` (135 lines)
- `addons/website_cf_turnstile/i18n/fr.po` (137 lines)
- `addons/website_cf_turnstile/i18n/he.po` (128 lines)
- `addons/website_cf_turnstile/i18n/hi.po` (127 lines)
- `addons/website_cf_turnstile/i18n/hr.po` (128 lines)
- `addons/website_cf_turnstile/i18n/hu.po` (128 lines)
- `addons/website_cf_turnstile/i18n/id.po` (134 lines)
- `addons/website_cf_turnstile/i18n/it.po` (140 lines)
- `addons/website_cf_turnstile/i18n/ja.po` (135 lines)
- `addons/website_cf_turnstile/i18n/kab.po` (128 lines)
- `addons/website_cf_turnstile/i18n/ko.po` (133 lines)
- `addons/website_cf_turnstile/i18n/ku.po` (127 lines)
- `addons/website_cf_turnstile/i18n/lo.po` (127 lines)
- `addons/website_cf_turnstile/i18n/lt.po` (129 lines)
- `addons/website_cf_turnstile/i18n/lv.po` (128 lines)
- `addons/website_cf_turnstile/i18n/mn.po` (127 lines)
- `addons/website_cf_turnstile/i18n/my.po` (127 lines)
- `addons/website_cf_turnstile/i18n/nb.po` (128 lines)
- `addons/website_cf_turnstile/i18n/nl.po` (135 lines)
- `addons/website_cf_turnstile/i18n/pl.po` (137 lines)
- `addons/website_cf_turnstile/i18n/pt.po` (136 lines)
- `addons/website_cf_turnstile/i18n/pt_BR.po` (139 lines)
- `addons/website_cf_turnstile/i18n/ro.po` (136 lines)
- `addons/website_cf_turnstile/i18n/ru.po` (140 lines)
- `addons/website_cf_turnstile/i18n/sk.po` (127 lines)
- `addons/website_cf_turnstile/i18n/sl.po` (129 lines)
- `addons/website_cf_turnstile/i18n/sr@latin.po` (128 lines)
- `addons/website_cf_turnstile/i18n/sv.po` (136 lines)
- `addons/website_cf_turnstile/i18n/th.po` (131 lines)
- `addons/website_cf_turnstile/i18n/tr.po` (140 lines)
- `addons/website_cf_turnstile/i18n/uk.po` (128 lines)
- `addons/website_cf_turnstile/i18n/uz.po` (155 lines)
- `addons/website_cf_turnstile/i18n/vi.po` (131 lines)
- `addons/website_cf_turnstile/i18n/website_cf_turnstile.pot` (123 lines)
- `addons/website_cf_turnstile/i18n/zh_CN.po` (133 lines)
- `addons/website_cf_turnstile/i18n/zh_TW.po` (138 lines)
- `addons/website_cf_turnstile/models/__init__.py` (5 lines)
- `addons/website_cf_turnstile/models/ir_http.py` (104 lines)
- `addons/website_cf_turnstile/models/res_config_settings.py` (10 lines)
- `addons/website_cf_turnstile/static/src/interactions/error_handler.js` (23 lines)
- `addons/website_cf_turnstile/static/src/interactions/form.js` (39 lines)
- `addons/website_cf_turnstile/static/src/interactions/turnstile.js` (122 lines)
- `addons/website_cf_turnstile/static/src/interactions/turnstile.xml` (19 lines)
- `addons/website_cf_turnstile/static/src/interactions/turnstile_captcha.js` (40 lines)
- `addons/website_cf_turnstile/static/tests/helpers.js` (8 lines)
- `addons/website_cf_turnstile/static/tests/interactions/form.test.js` (27 lines)
- `addons/website_cf_turnstile/static/tests/interactions/turnstile_captcha.test.js` (26 lines)
- `addons/website_cf_turnstile/views/res_config_settings_view.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
