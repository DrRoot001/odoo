# Module: auth_totp_mail

- **Module ID:** MOD-030
- **Path:** `addons/auth_totp_mail`
- **Manifest:** `addons/auth_totp_mail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


2FA Invite mail
===============
Allow the users to invite another user to use Two-Factor authentication
by sending an email to the target user. This email redirects them to:
- the users security settings if the user is internal.
- the portal security settings page if the user is not internal.
    

Declared dependencies: `auth_totp`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_totp",
    "mail"
  ],
  "data": [
    "data/ir_action_data.xml",
    "data/mail_template_data.xml",
    "data/security_notifications_template.xml",
    "views/res_config_settings_views.xml",
    "views/res_users_views.xml",
    "views/templates.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "auth_totp_mail/static/tests/**/*"
    ],
    "web.assets_backend": [
      "auth_totp_mail/static/src/services/check_identity/*"
    ],
    "web.assets_frontend": [
      "auth_totp_mail/static/src/services/check_identity/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_totp_mail/__init__.py` (4 lines)
- `addons/auth_totp_mail/__manifest__.py` (35 lines)
- `addons/auth_totp_mail/controllers/__init__.py` (4 lines)
- `addons/auth_totp_mail/controllers/home.py` (32 lines)
- `addons/auth_totp_mail/controllers/main.py` (9 lines)
- `addons/auth_totp_mail/data/ir_action_data.xml` (27 lines)
- `addons/auth_totp_mail/data/mail_template_data.xml` (81 lines)
- `addons/auth_totp_mail/data/security_notifications_template.xml` (16 lines)
- `addons/auth_totp_mail/i18n/ar.po` (537 lines)
- `addons/auth_totp_mail/i18n/auth_totp_mail.pot` (348 lines)
- `addons/auth_totp_mail/i18n/az.po` (370 lines)
- `addons/auth_totp_mail/i18n/bg.po` (370 lines)
- `addons/auth_totp_mail/i18n/bs.po` (369 lines)
- `addons/auth_totp_mail/i18n/ca.po` (545 lines)
- `addons/auth_totp_mail/i18n/cs.po` (397 lines)
- `addons/auth_totp_mail/i18n/da.po` (529 lines)
- `addons/auth_totp_mail/i18n/de.po` (655 lines)
- `addons/auth_totp_mail/i18n/el.po` (368 lines)
- `addons/auth_totp_mail/i18n/es.po` (652 lines)
- `addons/auth_totp_mail/i18n/es_419.po` (645 lines)
- `addons/auth_totp_mail/i18n/et.po` (395 lines)
- `addons/auth_totp_mail/i18n/fa.po` (395 lines)
- `addons/auth_totp_mail/i18n/fi.po` (549 lines)
- `addons/auth_totp_mail/i18n/fr.po` (655 lines)
- `addons/auth_totp_mail/i18n/he.po` (371 lines)
- `addons/auth_totp_mail/i18n/hi.po` (369 lines)
- `addons/auth_totp_mail/i18n/hr.po` (374 lines)
- `addons/auth_totp_mail/i18n/hu.po` (371 lines)
- `addons/auth_totp_mail/i18n/id.po` (545 lines)
- `addons/auth_totp_mail/i18n/it.po` (644 lines)
- `addons/auth_totp_mail/i18n/ja.po` (633 lines)
- `addons/auth_totp_mail/i18n/kab.po` (368 lines)
- `addons/auth_totp_mail/i18n/ko.po` (534 lines)
- `addons/auth_totp_mail/i18n/ku.po` (370 lines)
- `addons/auth_totp_mail/i18n/lo.po` (517 lines)
- `addons/auth_totp_mail/i18n/lt.po` (374 lines)
- `addons/auth_totp_mail/i18n/lv.po` (372 lines)
- `addons/auth_totp_mail/i18n/mn.po` (367 lines)
- `addons/auth_totp_mail/i18n/my.po` (370 lines)
- `addons/auth_totp_mail/i18n/nb.po` (368 lines)
- `addons/auth_totp_mail/i18n/nl.po` (634 lines)
- `addons/auth_totp_mail/i18n/pl.po` (549 lines)
- `addons/auth_totp_mail/i18n/pt.po` (632 lines)
- `addons/auth_totp_mail/i18n/pt_BR.po` (646 lines)
- `addons/auth_totp_mail/i18n/ro.po` (400 lines)
- `addons/auth_totp_mail/i18n/ru.po` (552 lines)
- `addons/auth_totp_mail/i18n/sk.po` (371 lines)
- `addons/auth_totp_mail/i18n/sl.po` (495 lines)
- `addons/auth_totp_mail/i18n/sr@latin.po` (371 lines)
- `addons/auth_totp_mail/i18n/sv.po` (544 lines)
- `addons/auth_totp_mail/i18n/th.po` (529 lines)
- `addons/auth_totp_mail/i18n/tr.po` (535 lines)
- `addons/auth_totp_mail/i18n/uk.po` (400 lines)
- `addons/auth_totp_mail/i18n/uz.po` (552 lines)
- `addons/auth_totp_mail/i18n/vi.po` (538 lines)
- `addons/auth_totp_mail/i18n/zh_CN.po` (618 lines)
- `addons/auth_totp_mail/i18n/zh_TW.po` (538 lines)
- `addons/auth_totp_mail/models/__init__.py` (6 lines)
- `addons/auth_totp_mail/models/auth_totp_device.py` (29 lines)
- `addons/auth_totp_mail/models/ir_http.py` (16 lines)
- `addons/auth_totp_mail/models/res_config_settings.py` (31 lines)
- `addons/auth_totp_mail/models/res_users.py` (214 lines)
- `addons/auth_totp_mail/static/src/services/check_identity/check_identity.js` (30 lines)
- `addons/auth_totp_mail/static/src/services/check_identity/check_identity.scss` (4 lines)
- `addons/auth_totp_mail/static/src/services/check_identity/check_identity.xml` (25 lines)
- `addons/auth_totp_mail/static/tests/totp_flow.js` (64 lines)
- `addons/auth_totp_mail/tests/__init__.py` (5 lines)
- `addons/auth_totp_mail/tests/test_auth_signup.py` (83 lines)
- `addons/auth_totp_mail/tests/test_notify_security_update_totp.py` (55 lines)
- `addons/auth_totp_mail/tests/test_totp.py` (59 lines)
- `addons/auth_totp_mail/views/res_config_settings_views.xml` (23 lines)
- `addons/auth_totp_mail/views/res_users_views.xml` (49 lines)
- `addons/auth_totp_mail/views/templates.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
