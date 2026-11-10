# Module: auth_totp

- **Module ID:** MOD-029
- **Path:** `addons/auth_totp`
- **Manifest:** `addons/auth_totp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Two-Factor Authentication (TOTP)
================================
Allows users to configure two-factor authentication on their user account
for extra security, using time-based one-time passwords (TOTP).

Once enabled, the user will need to enter a 6-digit code as provided
by their authenticator app before being granted access to the system.
All popular authenticator apps are supported.

Note: logically, two-factor prevents password-based RPC access for users
where it is enabled. In order to be able to execute RPC scripts, the user
can setup API keys to replace their main password.
    

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "data/ir_action_data.xml",
    "views/res_users_views.xml",
    "views/templates.xml",
    "wizard/auth_totp_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_tests": [
      "auth_totp/static/tests/**/*"
    ],
    "web.assets_backend": [
      "auth_totp/static/src/scss/**/*",
      "auth_totp/static/src/services/check_identity/*"
    ],
    "web.assets_frontend": [
      "auth_totp/static/src/services/check_identity/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_totp/__init__.py` (4 lines)
- `addons/auth_totp/__manifest__.py` (41 lines)
- `addons/auth_totp/controllers/__init__.py` (2 lines)
- `addons/auth_totp/controllers/home.py` (93 lines)
- `addons/auth_totp/data/ir_action_data.xml` (14 lines)
- `addons/auth_totp/i18n/ar.po` (451 lines)
- `addons/auth_totp/i18n/auth_totp.pot` (421 lines)
- `addons/auth_totp/i18n/az.po` (428 lines)
- `addons/auth_totp/i18n/bg.po` (431 lines)
- `addons/auth_totp/i18n/bs.po` (427 lines)
- `addons/auth_totp/i18n/ca.po` (444 lines)
- `addons/auth_totp/i18n/cs.po` (444 lines)
- `addons/auth_totp/i18n/da.po` (454 lines)
- `addons/auth_totp/i18n/de.po` (487 lines)
- `addons/auth_totp/i18n/el.po` (426 lines)
- `addons/auth_totp/i18n/es.po` (472 lines)
- `addons/auth_totp/i18n/es_419.po` (482 lines)
- `addons/auth_totp/i18n/et.po` (444 lines)
- `addons/auth_totp/i18n/fa.po` (442 lines)
- `addons/auth_totp/i18n/fi.po` (479 lines)
- `addons/auth_totp/i18n/fr.po` (487 lines)
- `addons/auth_totp/i18n/he.po` (429 lines)
- `addons/auth_totp/i18n/hi.po` (425 lines)
- `addons/auth_totp/i18n/hr.po` (432 lines)
- `addons/auth_totp/i18n/hu.po` (443 lines)
- `addons/auth_totp/i18n/id.po` (460 lines)
- `addons/auth_totp/i18n/it.po` (478 lines)
- `addons/auth_totp/i18n/ja.po` (476 lines)
- `addons/auth_totp/i18n/kab.po` (426 lines)
- `addons/auth_totp/i18n/ko.po` (445 lines)
- `addons/auth_totp/i18n/ku.po` (428 lines)
- `addons/auth_totp/i18n/lo.po` (456 lines)
- `addons/auth_totp/i18n/lt.po` (430 lines)
- `addons/auth_totp/i18n/lv.po` (430 lines)
- `addons/auth_totp/i18n/mn.po` (425 lines)
- `addons/auth_totp/i18n/my.po` (429 lines)
- `addons/auth_totp/i18n/nb.po` (426 lines)
- `addons/auth_totp/i18n/nl.po` (480 lines)
- `addons/auth_totp/i18n/pl.po` (462 lines)
- `addons/auth_totp/i18n/pt.po` (451 lines)
- `addons/auth_totp/i18n/pt_BR.po` (482 lines)
- `addons/auth_totp/i18n/ro.po` (447 lines)
- `addons/auth_totp/i18n/ru.po` (481 lines)
- `addons/auth_totp/i18n/sk.po` (429 lines)
- `addons/auth_totp/i18n/sl.po` (445 lines)
- `addons/auth_totp/i18n/sr@latin.po` (429 lines)
- `addons/auth_totp/i18n/sv.po` (459 lines)
- `addons/auth_totp/i18n/th.po` (444 lines)
- `addons/auth_totp/i18n/tr.po` (463 lines)
- `addons/auth_totp/i18n/uk.po` (444 lines)
- `addons/auth_totp/i18n/uz.po` (516 lines)
- `addons/auth_totp/i18n/vi.po` (445 lines)
- `addons/auth_totp/i18n/zh_CN.po` (470 lines)
- `addons/auth_totp/i18n/zh_TW.po` (452 lines)
- `addons/auth_totp/models/__init__.py` (8 lines)
- `addons/auth_totp/models/auth_totp.py` (32 lines)
- `addons/auth_totp/models/auth_totp_rate_limit_log.py` (15 lines)
- `addons/auth_totp/models/ir_http.py` (16 lines)
- `addons/auth_totp/models/res_users.py` (242 lines)
- `addons/auth_totp/models/totp.py` (56 lines)
- `addons/auth_totp/security/ir.access.csv` (6 lines)
- `addons/auth_totp/static/src/scss/res_users_view_form.scss` (3 lines)
- `addons/auth_totp/static/src/services/check_identity/check_identity.js` (15 lines)
- `addons/auth_totp/static/src/services/check_identity/check_identity.xml` (22 lines)
- `addons/auth_totp/static/tests/apikeys_flow.js` (111 lines)
- `addons/auth_totp/static/tests/totp_flow.js` (438 lines)
- `addons/auth_totp/tests/__init__.py` (2 lines)
- `addons/auth_totp/tests/test_apikeys.py` (58 lines)
- `addons/auth_totp/tests/test_totp.py` (195 lines)
- `addons/auth_totp/views/res_users_views.xml` (82 lines)
- `addons/auth_totp/views/templates.xml` (47 lines)
- `addons/auth_totp/wizard/__init__.py` (4 lines)
- `addons/auth_totp/wizard/auth_totp_wizard.py` (74 lines)
- `addons/auth_totp/wizard/auth_totp_wizard_views.xml` (44 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
