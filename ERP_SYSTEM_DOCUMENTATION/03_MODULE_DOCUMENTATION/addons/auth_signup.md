# Module: auth_signup

- **Module ID:** MOD-027
- **Path:** `addons/auth_signup`
- **Manifest:** `addons/auth_signup/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allow users to sign up and reset their password
===============================================
    

Declared dependencies: `base_setup`, `mail`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "mail",
    "web"
  ],
  "data": [
    "data/ir_config_parameter_data.xml",
    "data/ir_cron_data.xml",
    "data/mail_template_data.xml",
    "views/res_config_settings_views.xml",
    "views/res_users_views.xml",
    "views/auth_signup_login_templates.xml",
    "views/auth_signup_templates_email.xml",
    "views/webclient_templates.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "auth_signup/static/src/components/**/*"
    ],
    "web.assets_frontend": [
      "auth_signup/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_signup/__init__.py` (5 lines)
- `addons/auth_signup/__manifest__.py` (37 lines)
- `addons/auth_signup/controllers/__init__.py` (3 lines)
- `addons/auth_signup/controllers/main.py` (204 lines)
- `addons/auth_signup/data/ir_config_parameter_data.xml` (9 lines)
- `addons/auth_signup/data/ir_cron_data.xml` (13 lines)
- `addons/auth_signup/data/mail_template_data.xml` (133 lines)
- `addons/auth_signup/i18n/af.po` (642 lines)
- `addons/auth_signup/i18n/am.po` (638 lines)
- `addons/auth_signup/i18n/ar.po` (797 lines)
- `addons/auth_signup/i18n/auth_signup.pot` (603 lines)
- `addons/auth_signup/i18n/az.po` (652 lines)
- `addons/auth_signup/i18n/bg.po` (648 lines)
- `addons/auth_signup/i18n/bs.po` (645 lines)
- `addons/auth_signup/i18n/ca.po` (671 lines)
- `addons/auth_signup/i18n/cs.po` (810 lines)
- `addons/auth_signup/i18n/da.po` (806 lines)
- `addons/auth_signup/i18n/de.po` (899 lines)
- `addons/auth_signup/i18n/el.po` (648 lines)
- `addons/auth_signup/i18n/es.po` (817 lines)
- `addons/auth_signup/i18n/es_419.po` (890 lines)
- `addons/auth_signup/i18n/es_CL.po` (25 lines)
- `addons/auth_signup/i18n/et.po` (658 lines)
- `addons/auth_signup/i18n/eu.po` (641 lines)
- `addons/auth_signup/i18n/fa.po` (667 lines)
- `addons/auth_signup/i18n/fi.po` (819 lines)
- `addons/auth_signup/i18n/fr.po` (899 lines)
- `addons/auth_signup/i18n/fr_BE.po` (24 lines)
- `addons/auth_signup/i18n/fr_CA.po` (25 lines)
- `addons/auth_signup/i18n/gl.po` (641 lines)
- `addons/auth_signup/i18n/gu.po` (642 lines)
- `addons/auth_signup/i18n/he.po` (656 lines)
- `addons/auth_signup/i18n/hi.po` (641 lines)
- `addons/auth_signup/i18n/hr.po` (655 lines)
- `addons/auth_signup/i18n/hu.po` (661 lines)
- `addons/auth_signup/i18n/id.po` (805 lines)
- `addons/auth_signup/i18n/is.po` (638 lines)
- `addons/auth_signup/i18n/it.po` (889 lines)
- `addons/auth_signup/i18n/ja.po` (875 lines)
- `addons/auth_signup/i18n/ka.po` (641 lines)
- `addons/auth_signup/i18n/kab.po` (643 lines)
- `addons/auth_signup/i18n/km.po` (642 lines)
- `addons/auth_signup/i18n/ko.po` (759 lines)
- `addons/auth_signup/i18n/ku.po` (645 lines)
- `addons/auth_signup/i18n/lo.po` (863 lines)
- `addons/auth_signup/i18n/lt.po` (661 lines)
- `addons/auth_signup/i18n/lv.po` (648 lines)
- `addons/auth_signup/i18n/mk.po` (641 lines)
- `addons/auth_signup/i18n/mn.po` (660 lines)
- `addons/auth_signup/i18n/my.po` (642 lines)
- `addons/auth_signup/i18n/nb.po` (651 lines)
- `addons/auth_signup/i18n/nl.po` (891 lines)
- `addons/auth_signup/i18n/pl.po` (821 lines)
- `addons/auth_signup/i18n/pt.po` (742 lines)
- `addons/auth_signup/i18n/pt_BR.po` (882 lines)
- `addons/auth_signup/i18n/ro.po` (665 lines)
- `addons/auth_signup/i18n/ru.po` (664 lines)
- `addons/auth_signup/i18n/sk.po` (649 lines)
- `addons/auth_signup/i18n/sl.po` (661 lines)
- `addons/auth_signup/i18n/sq.po` (641 lines)
- `addons/auth_signup/i18n/sr@latin.po` (658 lines)
- `addons/auth_signup/i18n/sv.po` (665 lines)
- `addons/auth_signup/i18n/th.po` (757 lines)
- `addons/auth_signup/i18n/tr.po` (728 lines)
- `addons/auth_signup/i18n/uk.po` (662 lines)
- `addons/auth_signup/i18n/uz.po` (749 lines)
- `addons/auth_signup/i18n/vi.po` (800 lines)
- `addons/auth_signup/i18n/zh_CN.po` (870 lines)
- `addons/auth_signup/i18n/zh_TW.po` (699 lines)
- `addons/auth_signup/models/__init__.py` (6 lines)
- `addons/auth_signup/models/ir_http.py` (19 lines)
- `addons/auth_signup/models/res_config_settings.py` (24 lines)
- `addons/auth_signup/models/res_partner.py` (203 lines)
- `addons/auth_signup/models/res_users.py` (332 lines)
- `addons/auth_signup/static/src/components/signup.js` (36 lines)
- `addons/auth_signup/static/src/components/signup.xml` (11 lines)
- `addons/auth_signup/static/src/interactions/signup.js` (23 lines)
- `addons/auth_signup/tests/__init__.py` (6 lines)
- `addons/auth_signup/tests/test_auth_signup.py` (174 lines)
- `addons/auth_signup/tests/test_login.py` (2 lines)
- `addons/auth_signup/tests/test_reset_password.py` (98 lines)
- `addons/auth_signup/views/auth_signup_login_templates.xml` (118 lines)
- `addons/auth_signup/views/auth_signup_templates_email.xml` (16 lines)
- `addons/auth_signup/views/res_config_settings_views.xml` (25 lines)
- `addons/auth_signup/views/res_users_views.xml` (48 lines)
- `addons/auth_signup/views/webclient_templates.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
