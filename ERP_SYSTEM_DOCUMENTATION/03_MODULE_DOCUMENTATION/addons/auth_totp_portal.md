# Module: auth_totp_portal

- **Module ID:** MOD-031
- **Path:** `addons/auth_totp_portal`
- **Manifest:** `addons/auth_totp_portal/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `portal`, `auth_totp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "portal",
    "auth_totp"
  ],
  "data": [
    "views/templates.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "auth_totp_portal/static/src/**/*"
    ],
    "web.assets_tests": [
      "auth_totp_portal/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/auth_totp_portal/__init__.py` (4 lines)
- `addons/auth_totp_portal/__manifest__.py` (20 lines)
- `addons/auth_totp_portal/i18n/ar.po` (133 lines)
- `addons/auth_totp_portal/i18n/auth_totp_portal.pot` (117 lines)
- `addons/auth_totp_portal/i18n/az.po` (131 lines)
- `addons/auth_totp_portal/i18n/bg.po` (133 lines)
- `addons/auth_totp_portal/i18n/bs.po` (126 lines)
- `addons/auth_totp_portal/i18n/ca.po` (134 lines)
- `addons/auth_totp_portal/i18n/cs.po` (133 lines)
- `addons/auth_totp_portal/i18n/da.po` (134 lines)
- `addons/auth_totp_portal/i18n/de.po` (137 lines)
- `addons/auth_totp_portal/i18n/el.po` (125 lines)
- `addons/auth_totp_portal/i18n/es.po` (134 lines)
- `addons/auth_totp_portal/i18n/es_419.po` (135 lines)
- `addons/auth_totp_portal/i18n/et.po` (133 lines)
- `addons/auth_totp_portal/i18n/fa.po` (132 lines)
- `addons/auth_totp_portal/i18n/fi.po` (134 lines)
- `addons/auth_totp_portal/i18n/fr.po` (135 lines)
- `addons/auth_totp_portal/i18n/he.po` (134 lines)
- `addons/auth_totp_portal/i18n/hi.po` (124 lines)
- `addons/auth_totp_portal/i18n/hr.po` (135 lines)
- `addons/auth_totp_portal/i18n/hu.po` (134 lines)
- `addons/auth_totp_portal/i18n/id.po` (134 lines)
- `addons/auth_totp_portal/i18n/it.po` (134 lines)
- `addons/auth_totp_portal/i18n/ja.po` (134 lines)
- `addons/auth_totp_portal/i18n/kab.po` (125 lines)
- `addons/auth_totp_portal/i18n/ko.po` (133 lines)
- `addons/auth_totp_portal/i18n/ku.po` (124 lines)
- `addons/auth_totp_portal/i18n/lo.po` (123 lines)
- `addons/auth_totp_portal/i18n/lt.po` (135 lines)
- `addons/auth_totp_portal/i18n/lv.po` (126 lines)
- `addons/auth_totp_portal/i18n/mn.po` (124 lines)
- `addons/auth_totp_portal/i18n/my.po` (124 lines)
- `addons/auth_totp_portal/i18n/nb.po` (124 lines)
- `addons/auth_totp_portal/i18n/nl.po` (134 lines)
- `addons/auth_totp_portal/i18n/pl.po` (134 lines)
- `addons/auth_totp_portal/i18n/pt.po` (134 lines)
- `addons/auth_totp_portal/i18n/pt_BR.po` (134 lines)
- `addons/auth_totp_portal/i18n/ro.po` (134 lines)
- `addons/auth_totp_portal/i18n/ru.po` (136 lines)
- `addons/auth_totp_portal/i18n/sk.po` (125 lines)
- `addons/auth_totp_portal/i18n/sl.po` (136 lines)
- `addons/auth_totp_portal/i18n/sr@latin.po` (127 lines)
- `addons/auth_totp_portal/i18n/sv.po` (134 lines)
- `addons/auth_totp_portal/i18n/th.po` (132 lines)
- `addons/auth_totp_portal/i18n/tr.po` (134 lines)
- `addons/auth_totp_portal/i18n/uk.po` (134 lines)
- `addons/auth_totp_portal/i18n/uz.po` (144 lines)
- `addons/auth_totp_portal/i18n/vi.po` (132 lines)
- `addons/auth_totp_portal/i18n/zh_CN.po` (133 lines)
- `addons/auth_totp_portal/i18n/zh_TW.po` (136 lines)
- `addons/auth_totp_portal/models/__init__.py` (4 lines)
- `addons/auth_totp_portal/models/res_users.py` (14 lines)
- `addons/auth_totp_portal/security/ir.access.csv` (2 lines)
- `addons/auth_totp_portal/static/src/components/totp_confirmation_dialog.js` (37 lines)
- `addons/auth_totp_portal/static/src/interactions/revoke_all_trusted_devices.js` (25 lines)
- `addons/auth_totp_portal/static/src/interactions/revoke_trusted_device.js` (24 lines)
- `addons/auth_totp_portal/static/src/interactions/totp_disable.js` (26 lines)
- `addons/auth_totp_portal/static/src/interactions/totp_enable.js` (193 lines)
- `addons/auth_totp_portal/static/src/scss/auth_totp_portal.scss` (36 lines)
- `addons/auth_totp_portal/static/tests/totp_portal.js` (129 lines)
- `addons/auth_totp_portal/tests/__init__.py` (1 lines)
- `addons/auth_totp_portal/tests/test_tour.py` (21 lines)
- `addons/auth_totp_portal/views/templates.xml` (67 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
