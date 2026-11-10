# Module: auth_password_policy_signup

- **Module ID:** MOD-026
- **Path:** `addons/auth_password_policy_signup`
- **Manifest:** `addons/auth_password_policy_signup/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `auth_password_policy`, `auth_signup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 1 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_password_policy",
    "auth_signup"
  ],
  "data": [
    "views/signup_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "auth_password_policy_signup/static/src/public/**/*",
      "auth_password_policy/static/src/password_meter.js",
      "auth_password_policy/static/src/password_policy.js"
    ]
  }
}
```

### Representative source files

- `addons/auth_password_policy_signup/__init__.py` (3 lines)
- `addons/auth_password_policy_signup/__manifest__.py` (18 lines)
- `addons/auth_password_policy_signup/controllers.py` (10 lines)
- `addons/auth_password_policy_signup/i18n/ar.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/auth_password_policy_signup.pot` (36 lines)
- `addons/auth_password_policy_signup/i18n/az.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/bg.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/bs.po` (42 lines)
- `addons/auth_password_policy_signup/i18n/ca.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/cs.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/da.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/de.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/el.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/es.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/es_419.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/et.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/fa.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/fi.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/fr.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/he.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/hi.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/hr.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/hu.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/id.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/it.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/ja.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/kab.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/ko.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/ku.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/lo.po` (39 lines)
- `addons/auth_password_policy_signup/i18n/lt.po` (42 lines)
- `addons/auth_password_policy_signup/i18n/lv.po` (42 lines)
- `addons/auth_password_policy_signup/i18n/mn.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/my.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/nb.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/nl.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/pl.po` (42 lines)
- `addons/auth_password_policy_signup/i18n/pt.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/pt_BR.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/ro.po` (42 lines)
- `addons/auth_password_policy_signup/i18n/ru.po` (43 lines)
- `addons/auth_password_policy_signup/i18n/sk.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/sl.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/sr@latin.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/sv.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/th.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/tr.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/uk.po` (41 lines)
- `addons/auth_password_policy_signup/i18n/uz.po` (50 lines)
- `addons/auth_password_policy_signup/i18n/vi.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/zh_CN.po` (40 lines)
- `addons/auth_password_policy_signup/i18n/zh_TW.po` (42 lines)
- `addons/auth_password_policy_signup/models/__init__.py` (1 lines)
- `addons/auth_password_policy_signup/models/ir_http.py` (11 lines)
- `addons/auth_password_policy_signup/static/src/public/components/password_meter/password_meter.js` (30 lines)
- `addons/auth_password_policy_signup/static/src/public/components/password_meter/password_meter.xml` (9 lines)
- `addons/auth_password_policy_signup/views/signup_templates.xml` (11 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
