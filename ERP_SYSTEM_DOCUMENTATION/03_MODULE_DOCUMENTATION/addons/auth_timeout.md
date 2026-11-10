# Module: auth_timeout

- **Module ID:** MOD-028
- **Path:** `addons/auth_timeout`
- **Manifest:** `addons/auth_timeout/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Ask for authentication after user inactivity

No manifest description declared.

Declared dependencies: `auth_totp`, `auth_totp_mail`, `auth_passkey`, `bus`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_totp",
    "auth_totp_mail",
    "auth_passkey",
    "bus"
  ],
  "data": [
    "views/res_groups_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "auth_timeout/static/src/services/check_identity/*"
    ],
    "web.assets_frontend": [
      "auth_timeout/static/src/services/check_identity/*"
    ],
    "web.assets_tests": [
      "auth_timeout/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_timeout/__init__.py` (1 lines)
- `addons/auth_timeout/__manifest__.py` (22 lines)
- `addons/auth_timeout/i18n/ar.po` (257 lines)
- `addons/auth_timeout/i18n/auth_timeout.pot` (245 lines)
- `addons/auth_timeout/i18n/az.po` (252 lines)
- `addons/auth_timeout/i18n/bg.po` (252 lines)
- `addons/auth_timeout/i18n/bs.po` (254 lines)
- `addons/auth_timeout/i18n/ca.po` (253 lines)
- `addons/auth_timeout/i18n/cs.po` (252 lines)
- `addons/auth_timeout/i18n/da.po` (260 lines)
- `addons/auth_timeout/i18n/de.po` (271 lines)
- `addons/auth_timeout/i18n/el.po` (252 lines)
- `addons/auth_timeout/i18n/es.po` (267 lines)
- `addons/auth_timeout/i18n/es_419.po` (273 lines)
- `addons/auth_timeout/i18n/et.po` (252 lines)
- `addons/auth_timeout/i18n/fa.po` (252 lines)
- `addons/auth_timeout/i18n/fi.po` (267 lines)
- `addons/auth_timeout/i18n/fr.po` (273 lines)
- `addons/auth_timeout/i18n/he.po` (253 lines)
- `addons/auth_timeout/i18n/hi.po` (249 lines)
- `addons/auth_timeout/i18n/hr.po` (253 lines)
- `addons/auth_timeout/i18n/hu.po` (252 lines)
- `addons/auth_timeout/i18n/id.po` (257 lines)
- `addons/auth_timeout/i18n/it.po` (269 lines)
- `addons/auth_timeout/i18n/ja.po` (257 lines)
- `addons/auth_timeout/i18n/kab.po` (253 lines)
- `addons/auth_timeout/i18n/ko.po` (255 lines)
- `addons/auth_timeout/i18n/ku.po` (249 lines)
- `addons/auth_timeout/i18n/lo.po` (253 lines)
- `addons/auth_timeout/i18n/lt.po` (254 lines)
- `addons/auth_timeout/i18n/lv.po` (254 lines)
- `addons/auth_timeout/i18n/mn.po` (252 lines)
- `addons/auth_timeout/i18n/my.po` (252 lines)
- `addons/auth_timeout/i18n/nb.po` (252 lines)
- `addons/auth_timeout/i18n/nl.po` (268 lines)
- `addons/auth_timeout/i18n/pl.po` (263 lines)
- `addons/auth_timeout/i18n/pt.po` (253 lines)
- `addons/auth_timeout/i18n/pt_BR.po` (267 lines)
- `addons/auth_timeout/i18n/ro.po` (265 lines)
- `addons/auth_timeout/i18n/ru.po` (264 lines)
- `addons/auth_timeout/i18n/sk.po` (253 lines)
- `addons/auth_timeout/i18n/sl.po` (253 lines)
- `addons/auth_timeout/i18n/sr@latin.po` (250 lines)
- `addons/auth_timeout/i18n/sv.po` (264 lines)
- `addons/auth_timeout/i18n/th.po` (253 lines)
- `addons/auth_timeout/i18n/tr.po` (268 lines)
- `addons/auth_timeout/i18n/uk.po` (253 lines)
- `addons/auth_timeout/i18n/uz.po` (308 lines)
- `addons/auth_timeout/i18n/vi.po` (253 lines)
- `addons/auth_timeout/i18n/zh_CN.po` (256 lines)
- `addons/auth_timeout/i18n/zh_TW.po` (252 lines)
- `addons/auth_timeout/models/__init__.py` (5 lines)
- `addons/auth_timeout/models/auth_totp_device.py` (14 lines)
- `addons/auth_timeout/models/ir_http.py` (152 lines)
- `addons/auth_timeout/models/ir_websocket.py` (44 lines)
- `addons/auth_timeout/models/res_groups.py` (235 lines)
- `addons/auth_timeout/models/res_users.py` (32 lines)
- `addons/auth_timeout/static/src/services/check_identity/check_identity.js` (79 lines)
- `addons/auth_timeout/static/tests/tours/auth_timeout_tour.js` (212 lines)
- `addons/auth_timeout/tests/__init__.py` (1 lines)
- `addons/auth_timeout/tests/test_auth_timeout.py` (560 lines)
- `addons/auth_timeout/views/res_groups_views.xml` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
