# Module: auth_password_policy

- **Module ID:** MOD-024
- **Path:** `addons/auth_password_policy`
- **Manifest:** `addons/auth_password_policy/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Implement basic password policy configuration & check

No manifest description declared.

Declared dependencies: `base_setup`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "web"
  ],
  "data": [
    "data/defaults.xml",
    "views/res_users.xml",
    "views/res_config_settings_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "auth_password_policy/static/src/**/*",
      [
        "remove",
        "auth_password_policy/static/src/css/password_field.css"
      ]
    ],
    "web.assets_frontend": [
      "auth_password_policy/static/src/css/password_field.css",
      "auth_password_policy/static/src/password_policy.js"
    ]
  }
}
```

### Representative source files

- `addons/auth_password_policy/__init__.py` (1 lines)
- `addons/auth_password_policy/__manifest__.py` (23 lines)
- `addons/auth_password_policy/data/defaults.xml` (8 lines)
- `addons/auth_password_policy/i18n/ar.po` (141 lines)
- `addons/auth_password_policy/i18n/auth_password_policy.pot` (124 lines)
- `addons/auth_password_policy/i18n/az.po` (131 lines)
- `addons/auth_password_policy/i18n/bg.po` (129 lines)
- `addons/auth_password_policy/i18n/bs.po` (132 lines)
- `addons/auth_password_policy/i18n/ca.po` (145 lines)
- `addons/auth_password_policy/i18n/cs.po` (143 lines)
- `addons/auth_password_policy/i18n/da.po` (142 lines)
- `addons/auth_password_policy/i18n/de.po` (145 lines)
- `addons/auth_password_policy/i18n/el.po` (132 lines)
- `addons/auth_password_policy/i18n/es.po` (144 lines)
- `addons/auth_password_policy/i18n/es_419.po` (139 lines)
- `addons/auth_password_policy/i18n/et.po` (141 lines)
- `addons/auth_password_policy/i18n/fa.po` (136 lines)
- `addons/auth_password_policy/i18n/fi.po` (142 lines)
- `addons/auth_password_policy/i18n/fr.po` (146 lines)
- `addons/auth_password_policy/i18n/gu.po` (129 lines)
- `addons/auth_password_policy/i18n/he.po` (141 lines)
- `addons/auth_password_policy/i18n/hi.po` (129 lines)
- `addons/auth_password_policy/i18n/hr.po` (142 lines)
- `addons/auth_password_policy/i18n/hu.po` (136 lines)
- `addons/auth_password_policy/i18n/id.po` (137 lines)
- `addons/auth_password_policy/i18n/it.po` (145 lines)
- `addons/auth_password_policy/i18n/ja.po` (139 lines)
- `addons/auth_password_policy/i18n/kab.po` (130 lines)
- `addons/auth_password_policy/i18n/ko.po` (142 lines)
- `addons/auth_password_policy/i18n/ku.po` (131 lines)
- `addons/auth_password_policy/i18n/lo.po` (128 lines)
- `addons/auth_password_policy/i18n/lt.po` (137 lines)
- `addons/auth_password_policy/i18n/lv.po` (131 lines)
- `addons/auth_password_policy/i18n/mn.po` (135 lines)
- `addons/auth_password_policy/i18n/my.po` (130 lines)
- `addons/auth_password_policy/i18n/nb.po` (132 lines)
- `addons/auth_password_policy/i18n/nl.po` (142 lines)
- `addons/auth_password_policy/i18n/pl.po` (144 lines)
- `addons/auth_password_policy/i18n/pt.po` (142 lines)
- `addons/auth_password_policy/i18n/pt_BR.po` (141 lines)
- `addons/auth_password_policy/i18n/ro.po` (142 lines)
- `addons/auth_password_policy/i18n/ru.po` (142 lines)
- `addons/auth_password_policy/i18n/sk.po` (133 lines)
- `addons/auth_password_policy/i18n/sl.po` (138 lines)
- `addons/auth_password_policy/i18n/sr@latin.po` (141 lines)
- `addons/auth_password_policy/i18n/sv.po` (140 lines)
- `addons/auth_password_policy/i18n/th.po` (138 lines)
- `addons/auth_password_policy/i18n/tr.po` (146 lines)
- `addons/auth_password_policy/i18n/uk.po` (143 lines)
- `addons/auth_password_policy/i18n/uz.po` (159 lines)
- `addons/auth_password_policy/i18n/vi.po` (141 lines)
- `addons/auth_password_policy/i18n/zh_CN.po` (139 lines)
- `addons/auth_password_policy/i18n/zh_TW.po` (137 lines)
- `addons/auth_password_policy/models/__init__.py` (2 lines)
- `addons/auth_password_policy/models/res_config_settings.py` (15 lines)
- `addons/auth_password_policy/models/res_users.py` (33 lines)
- `addons/auth_password_policy/static/src/css/password_field.css` (4 lines)
- `addons/auth_password_policy/static/src/css/password_field_backend.css` (13 lines)
- `addons/auth_password_policy/static/src/password_field.js` (45 lines)
- `addons/auth_password_policy/static/src/password_field.xml` (15 lines)
- `addons/auth_password_policy/static/src/password_meter.js` (45 lines)
- `addons/auth_password_policy/static/src/password_policy.js` (109 lines)
- `addons/auth_password_policy/views/res_config_settings_views.xml` (16 lines)
- `addons/auth_password_policy/views/res_users.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
