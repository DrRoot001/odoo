# Module: auth_oauth

- **Module ID:** MOD-021
- **Path:** `addons/auth_oauth`
- **Manifest:** `addons/auth_oauth/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allow users to login through OAuth2 Provider.
=============================================


Declared dependencies: `base`, `web`, `base_setup`, `auth_signup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web",
    "base_setup",
    "auth_signup"
  ],
  "data": [
    "data/auth_oauth_data.xml",
    "views/auth_oauth_views.xml",
    "views/res_config_settings_views.xml",
    "views/auth_oauth_templates.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "auth_oauth/static/**/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_oauth/__init__.py` (5 lines)
- `addons/auth_oauth/__manifest__.py` (25 lines)
- `addons/auth_oauth/controllers/__init__.py` (4 lines)
- `addons/auth_oauth/controllers/main.py` (180 lines)
- `addons/auth_oauth/data/auth_oauth_data.xml` (39 lines)
- `addons/auth_oauth/data/neutralize.sql` (3 lines)
- `addons/auth_oauth/i18n/af.po` (271 lines)
- `addons/auth_oauth/i18n/am.po` (267 lines)
- `addons/auth_oauth/i18n/ar.po` (278 lines)
- `addons/auth_oauth/i18n/auth_oauth.pot` (267 lines)
- `addons/auth_oauth/i18n/az.po` (274 lines)
- `addons/auth_oauth/i18n/bg.po` (280 lines)
- `addons/auth_oauth/i18n/bs.po` (280 lines)
- `addons/auth_oauth/i18n/ca.po` (285 lines)
- `addons/auth_oauth/i18n/cs.po` (280 lines)
- `addons/auth_oauth/i18n/da.po` (278 lines)
- `addons/auth_oauth/i18n/de.po` (283 lines)
- `addons/auth_oauth/i18n/el.po` (279 lines)
- `addons/auth_oauth/i18n/es.po` (282 lines)
- `addons/auth_oauth/i18n/es_419.po` (277 lines)
- `addons/auth_oauth/i18n/es_CL.po` (61 lines)
- `addons/auth_oauth/i18n/et.po` (282 lines)
- `addons/auth_oauth/i18n/eu.po` (270 lines)
- `addons/auth_oauth/i18n/fa.po` (279 lines)
- `addons/auth_oauth/i18n/fi.po` (286 lines)
- `addons/auth_oauth/i18n/fo.po` (270 lines)
- `addons/auth_oauth/i18n/fr.po` (283 lines)
- `addons/auth_oauth/i18n/fr_BE.po` (53 lines)
- `addons/auth_oauth/i18n/fr_CA.po` (61 lines)
- `addons/auth_oauth/i18n/gl.po` (270 lines)
- `addons/auth_oauth/i18n/gu.po` (271 lines)
- `addons/auth_oauth/i18n/he.po` (301 lines)
- `addons/auth_oauth/i18n/hi.po` (271 lines)
- `addons/auth_oauth/i18n/hr.po` (280 lines)
- `addons/auth_oauth/i18n/hu.po` (284 lines)
- `addons/auth_oauth/i18n/id.po` (278 lines)
- `addons/auth_oauth/i18n/is.po` (267 lines)
- `addons/auth_oauth/i18n/it.po` (283 lines)
- `addons/auth_oauth/i18n/ja.po` (280 lines)
- `addons/auth_oauth/i18n/ka.po` (270 lines)
- `addons/auth_oauth/i18n/kab.po` (276 lines)
- `addons/auth_oauth/i18n/km.po` (271 lines)
- `addons/auth_oauth/i18n/ko.po` (276 lines)
- `addons/auth_oauth/i18n/ku.po` (271 lines)
- `addons/auth_oauth/i18n/lo.po` (277 lines)
- `addons/auth_oauth/i18n/lt.po` (288 lines)
- `addons/auth_oauth/i18n/lv.po` (281 lines)
- `addons/auth_oauth/i18n/mk.po` (270 lines)
- `addons/auth_oauth/i18n/mn.po` (279 lines)
- `addons/auth_oauth/i18n/my.po` (272 lines)
- `addons/auth_oauth/i18n/nb.po` (275 lines)
- `addons/auth_oauth/i18n/nl.po` (281 lines)
- `addons/auth_oauth/i18n/pl.po` (285 lines)
- `addons/auth_oauth/i18n/pt.po` (283 lines)
- `addons/auth_oauth/i18n/pt_BR.po` (281 lines)
- `addons/auth_oauth/i18n/ro.po` (280 lines)
- `addons/auth_oauth/i18n/ru.po` (279 lines)
- `addons/auth_oauth/i18n/sk.po` (277 lines)
- `addons/auth_oauth/i18n/sl.po` (280 lines)
- `addons/auth_oauth/i18n/sq.po` (270 lines)
- `addons/auth_oauth/i18n/sr@latin.po` (278 lines)
- `addons/auth_oauth/i18n/sv.po` (289 lines)
- `addons/auth_oauth/i18n/ta.po` (271 lines)
- `addons/auth_oauth/i18n/th.po` (277 lines)
- `addons/auth_oauth/i18n/tr.po` (287 lines)
- `addons/auth_oauth/i18n/uk.po` (281 lines)
- `addons/auth_oauth/i18n/uz.po` (324 lines)
- `addons/auth_oauth/i18n/vi.po` (278 lines)
- `addons/auth_oauth/i18n/zh_CN.po` (276 lines)
- `addons/auth_oauth/i18n/zh_TW.po` (277 lines)
- `addons/auth_oauth/models/__init__.py` (7 lines)
- `addons/auth_oauth/models/auth_oauth.py` (23 lines)
- `addons/auth_oauth/models/ir_config_parameter.py` (17 lines)
- `addons/auth_oauth/models/res_config_settings.py` (36 lines)
- `addons/auth_oauth/models/res_users.py` (170 lines)
- `addons/auth_oauth/security/ir.access.csv` (2 lines)
- `addons/auth_oauth/static/src/scss/auth_oauth.scss` (28 lines)
- `addons/auth_oauth/views/auth_oauth_templates.xml` (8 lines)
- `addons/auth_oauth/views/auth_oauth_views.xml` (47 lines)
- `addons/auth_oauth/views/res_config_settings_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
