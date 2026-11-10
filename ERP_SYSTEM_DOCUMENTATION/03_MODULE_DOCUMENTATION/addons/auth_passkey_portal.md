# Module: auth_passkey_portal

- **Module ID:** MOD-023
- **Path:** `addons/auth_passkey_portal`
- **Manifest:** `addons/auth_passkey_portal/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Passkeys for portal users


The implementation of Passkeys using the webauthn protocol.
===========================================================

Passkeys are a secure alternative to a username and a password.
When a user logs in with a Passkey, MFA will not be required.


Declared dependencies: `auth_passkey`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_passkey",
    "portal"
  ],
  "data": [
    "views/templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "auth_passkey_portal/static/src/**"
    ],
    "web.assets_tests": [
      "auth_passkey_portal/static/tests/tours/*.js"
    ]
  }
}
```

### Representative source files

- `addons/auth_passkey_portal/__init__.py` (0 lines)
- `addons/auth_passkey_portal/__manifest__.py` (27 lines)
- `addons/auth_passkey_portal/i18n/ar.po` (102 lines)
- `addons/auth_passkey_portal/i18n/auth_passkey_portal.pot` (96 lines)
- `addons/auth_passkey_portal/i18n/az.po` (100 lines)
- `addons/auth_passkey_portal/i18n/bg.po` (100 lines)
- `addons/auth_passkey_portal/i18n/bs.po` (102 lines)
- `addons/auth_passkey_portal/i18n/ca.po` (101 lines)
- `addons/auth_passkey_portal/i18n/cs.po` (101 lines)
- `addons/auth_passkey_portal/i18n/da.po` (101 lines)
- `addons/auth_passkey_portal/i18n/de.po` (108 lines)
- `addons/auth_passkey_portal/i18n/el.po` (100 lines)
- `addons/auth_passkey_portal/i18n/es.po` (108 lines)
- `addons/auth_passkey_portal/i18n/es_419.po` (109 lines)
- `addons/auth_passkey_portal/i18n/et.po` (100 lines)
- `addons/auth_passkey_portal/i18n/fa.po` (100 lines)
- `addons/auth_passkey_portal/i18n/fi.po` (108 lines)
- `addons/auth_passkey_portal/i18n/fr.po` (109 lines)
- `addons/auth_passkey_portal/i18n/he.po` (101 lines)
- `addons/auth_passkey_portal/i18n/hi.po` (100 lines)
- `addons/auth_passkey_portal/i18n/hr.po` (101 lines)
- `addons/auth_passkey_portal/i18n/hu.po` (100 lines)
- `addons/auth_passkey_portal/i18n/id.po` (100 lines)
- `addons/auth_passkey_portal/i18n/it.po` (107 lines)
- `addons/auth_passkey_portal/i18n/ja.po` (106 lines)
- `addons/auth_passkey_portal/i18n/kab.po` (101 lines)
- `addons/auth_passkey_portal/i18n/ko.po` (101 lines)
- `addons/auth_passkey_portal/i18n/ku.po` (100 lines)
- `addons/auth_passkey_portal/i18n/lo.po` (99 lines)
- `addons/auth_passkey_portal/i18n/lt.po` (102 lines)
- `addons/auth_passkey_portal/i18n/lv.po` (102 lines)
- `addons/auth_passkey_portal/i18n/mn.po` (100 lines)
- `addons/auth_passkey_portal/i18n/my.po` (100 lines)
- `addons/auth_passkey_portal/i18n/nb.po` (100 lines)
- `addons/auth_passkey_portal/i18n/nl.po` (109 lines)
- `addons/auth_passkey_portal/i18n/pl.po` (101 lines)
- `addons/auth_passkey_portal/i18n/pt.po` (100 lines)
- `addons/auth_passkey_portal/i18n/pt_BR.po` (106 lines)
- `addons/auth_passkey_portal/i18n/ro.po` (101 lines)
- `addons/auth_passkey_portal/i18n/ru.po` (102 lines)
- `addons/auth_passkey_portal/i18n/sk.po` (101 lines)
- `addons/auth_passkey_portal/i18n/sl.po` (101 lines)
- `addons/auth_passkey_portal/i18n/sr@latin.po` (101 lines)
- `addons/auth_passkey_portal/i18n/sv.po` (101 lines)
- `addons/auth_passkey_portal/i18n/th.po` (100 lines)
- `addons/auth_passkey_portal/i18n/tr.po` (102 lines)
- `addons/auth_passkey_portal/i18n/uk.po` (101 lines)
- `addons/auth_passkey_portal/i18n/uz.po` (117 lines)
- `addons/auth_passkey_portal/i18n/vi.po` (101 lines)
- `addons/auth_passkey_portal/i18n/zh_CN.po` (101 lines)
- `addons/auth_passkey_portal/i18n/zh_TW.po` (101 lines)
- `addons/auth_passkey_portal/static/src/js/passkeys_portal.js` (51 lines)
- `addons/auth_passkey_portal/static/src/js/passkeys_portal_create.js` (58 lines)
- `addons/auth_passkey_portal/static/src/xml/passkeys_portal_popups.xml` (14 lines)
- `addons/auth_passkey_portal/static/tests/tours/test_passkey_portal.js` (163 lines)
- `addons/auth_passkey_portal/tests/__init__.py` (1 lines)
- `addons/auth_passkey_portal/tests/test_passkey_portal.py` (40 lines)
- `addons/auth_passkey_portal/views/templates.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
