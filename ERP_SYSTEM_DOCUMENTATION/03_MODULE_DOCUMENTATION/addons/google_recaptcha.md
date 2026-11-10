# Module: google_recaptcha

- **Module ID:** MOD-080
- **Path:** `addons/google_recaptcha`
- **Manifest:** `addons/google_recaptcha/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module implements reCaptchaV3 so that you can prevent bot spam on your public modules.
    

Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup"
  ],
  "data": [
    "views/res_config_settings_view.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "google_recaptcha/static/src/scss/recaptcha.scss",
      "google_recaptcha/static/src/js/recaptcha.js",
      "google_recaptcha/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/google_recaptcha/__init__.py` (4 lines)
- `addons/google_recaptcha/__manifest__.py` (22 lines)
- `addons/google_recaptcha/data/neutralize.sql` (4 lines)
- `addons/google_recaptcha/i18n/ar.po` (170 lines)
- `addons/google_recaptcha/i18n/az.po` (161 lines)
- `addons/google_recaptcha/i18n/bg.po` (161 lines)
- `addons/google_recaptcha/i18n/bs.po` (163 lines)
- `addons/google_recaptcha/i18n/ca.po` (164 lines)
- `addons/google_recaptcha/i18n/cs.po` (163 lines)
- `addons/google_recaptcha/i18n/da.po` (163 lines)
- `addons/google_recaptcha/i18n/de.po` (174 lines)
- `addons/google_recaptcha/i18n/el.po` (162 lines)
- `addons/google_recaptcha/i18n/es.po` (174 lines)
- `addons/google_recaptcha/i18n/es_419.po` (174 lines)
- `addons/google_recaptcha/i18n/et.po` (161 lines)
- `addons/google_recaptcha/i18n/fa.po` (161 lines)
- `addons/google_recaptcha/i18n/fi.po` (173 lines)
- `addons/google_recaptcha/i18n/fr.po` (174 lines)
- `addons/google_recaptcha/i18n/google_recaptcha.pot` (157 lines)
- `addons/google_recaptcha/i18n/he.po` (162 lines)
- `addons/google_recaptcha/i18n/hi.po` (161 lines)
- `addons/google_recaptcha/i18n/hr.po` (162 lines)
- `addons/google_recaptcha/i18n/hu.po` (162 lines)
- `addons/google_recaptcha/i18n/id.po` (170 lines)
- `addons/google_recaptcha/i18n/it.po` (174 lines)
- `addons/google_recaptcha/i18n/ja.po` (169 lines)
- `addons/google_recaptcha/i18n/kab.po` (162 lines)
- `addons/google_recaptcha/i18n/ko.po` (166 lines)
- `addons/google_recaptcha/i18n/ku.po` (161 lines)
- `addons/google_recaptcha/i18n/lo.po` (169 lines)
- `addons/google_recaptcha/i18n/lt.po` (163 lines)
- `addons/google_recaptcha/i18n/lv.po` (162 lines)
- `addons/google_recaptcha/i18n/mn.po` (161 lines)
- `addons/google_recaptcha/i18n/my.po` (161 lines)
- `addons/google_recaptcha/i18n/nb.po` (162 lines)
- `addons/google_recaptcha/i18n/nl.po` (170 lines)
- `addons/google_recaptcha/i18n/pl.po` (172 lines)
- `addons/google_recaptcha/i18n/pt.po` (164 lines)
- `addons/google_recaptcha/i18n/pt_BR.po` (173 lines)
- `addons/google_recaptcha/i18n/ro.po` (169 lines)
- `addons/google_recaptcha/i18n/ru.po` (174 lines)
- `addons/google_recaptcha/i18n/sk.po` (161 lines)
- `addons/google_recaptcha/i18n/sl.po` (165 lines)
- `addons/google_recaptcha/i18n/sr@latin.po` (162 lines)
- `addons/google_recaptcha/i18n/sv.po` (168 lines)
- `addons/google_recaptcha/i18n/th.po` (164 lines)
- `addons/google_recaptcha/i18n/tr.po` (173 lines)
- `addons/google_recaptcha/i18n/uk.po` (162 lines)
- `addons/google_recaptcha/i18n/uz.po` (194 lines)
- `addons/google_recaptcha/i18n/vi.po` (167 lines)
- `addons/google_recaptcha/i18n/zh_CN.po` (169 lines)
- `addons/google_recaptcha/i18n/zh_TW.po` (169 lines)
- `addons/google_recaptcha/models/__init__.py` (5 lines)
- `addons/google_recaptcha/models/ir_http.py` (120 lines)
- `addons/google_recaptcha/models/res_config_settings.py` (18 lines)
- `addons/google_recaptcha/static/src/interactions/recaptcha_form.js` (54 lines)
- `addons/google_recaptcha/static/src/js/recaptcha.js` (55 lines)
- `addons/google_recaptcha/static/src/scss/recaptcha.scss` (5 lines)
- `addons/google_recaptcha/static/src/xml/recaptcha.xml` (14 lines)
- `addons/google_recaptcha/views/res_config_settings_view.xml` (35 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
