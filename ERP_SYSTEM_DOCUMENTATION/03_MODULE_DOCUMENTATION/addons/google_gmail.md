# Module: google_gmail

- **Module ID:** MOD-079
- **Path:** `addons/google_gmail`
- **Manifest:** `addons/google_gmail/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Gmail support for incoming / outgoing mail servers

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "views/fetchmail_server_views.xml",
    "views/ir_mail_server_views.xml",
    "views/res_config_settings_views.xml",
    "views/templates.xml"
  ]
}
```

### Representative source files

- `addons/google_gmail/__init__.py` (5 lines)
- `addons/google_gmail/__manifest__.py` (20 lines)
- `addons/google_gmail/controllers/__init__.py` (4 lines)
- `addons/google_gmail/controllers/main.py` (139 lines)
- `addons/google_gmail/i18n/ar.po` (345 lines)
- `addons/google_gmail/i18n/az.po` (316 lines)
- `addons/google_gmail/i18n/bg.po` (327 lines)
- `addons/google_gmail/i18n/bs.po` (317 lines)
- `addons/google_gmail/i18n/ca.po` (338 lines)
- `addons/google_gmail/i18n/cs.po` (329 lines)
- `addons/google_gmail/i18n/da.po` (329 lines)
- `addons/google_gmail/i18n/de.po` (347 lines)
- `addons/google_gmail/i18n/el.po` (318 lines)
- `addons/google_gmail/i18n/es.po` (347 lines)
- `addons/google_gmail/i18n/es_419.po` (344 lines)
- `addons/google_gmail/i18n/et.po` (325 lines)
- `addons/google_gmail/i18n/fa.po` (335 lines)
- `addons/google_gmail/i18n/fi.po` (347 lines)
- `addons/google_gmail/i18n/fr.po` (350 lines)
- `addons/google_gmail/i18n/google_gmail.pot` (306 lines)
- `addons/google_gmail/i18n/he.po` (317 lines)
- `addons/google_gmail/i18n/hi.po` (316 lines)
- `addons/google_gmail/i18n/hr.po` (317 lines)
- `addons/google_gmail/i18n/hu.po` (318 lines)
- `addons/google_gmail/i18n/id.po` (345 lines)
- `addons/google_gmail/i18n/it.po` (348 lines)
- `addons/google_gmail/i18n/ja.po` (344 lines)
- `addons/google_gmail/i18n/kab.po` (316 lines)
- `addons/google_gmail/i18n/ko.po` (339 lines)
- `addons/google_gmail/i18n/ku.po` (316 lines)
- `addons/google_gmail/i18n/lo.po` (340 lines)
- `addons/google_gmail/i18n/lt.po` (318 lines)
- `addons/google_gmail/i18n/lv.po` (316 lines)
- `addons/google_gmail/i18n/mn.po` (316 lines)
- `addons/google_gmail/i18n/my.po` (316 lines)
- `addons/google_gmail/i18n/nb.po` (317 lines)
- `addons/google_gmail/i18n/nl.po` (347 lines)
- `addons/google_gmail/i18n/pl.po` (346 lines)
- `addons/google_gmail/i18n/pt.po` (343 lines)
- `addons/google_gmail/i18n/pt_BR.po` (348 lines)
- `addons/google_gmail/i18n/ro.po` (349 lines)
- `addons/google_gmail/i18n/ru.po` (348 lines)
- `addons/google_gmail/i18n/sk.po` (315 lines)
- `addons/google_gmail/i18n/sl.po` (343 lines)
- `addons/google_gmail/i18n/sr@latin.po` (317 lines)
- `addons/google_gmail/i18n/sv.po` (347 lines)
- `addons/google_gmail/i18n/th.po` (339 lines)
- `addons/google_gmail/i18n/tr.po` (345 lines)
- `addons/google_gmail/i18n/uk.po` (338 lines)
- `addons/google_gmail/i18n/uz.po` (386 lines)
- `addons/google_gmail/i18n/vi.po` (346 lines)
- `addons/google_gmail/i18n/zh_CN.po` (339 lines)
- `addons/google_gmail/i18n/zh_TW.po` (337 lines)
- `addons/google_gmail/models/__init__.py` (9 lines)
- `addons/google_gmail/models/fetchmail_server.py` (59 lines)
- `addons/google_gmail/models/google_gmail_mixin.py` (276 lines)
- `addons/google_gmail/models/ir_mail_server.py` (78 lines)
- `addons/google_gmail/models/res_config_settings.py` (11 lines)
- `addons/google_gmail/models/res_users.py` (28 lines)
- `addons/google_gmail/static/description/icon.png` (12 lines)
- `addons/google_gmail/static/description/icon.svg` (1 lines)
- `addons/google_gmail/static/description/icon_hi.png` (104 lines)
- `addons/google_gmail/tests/__init__.py` (1 lines)
- `addons/google_gmail/tests/test_google_gmail.py` (74 lines)
- `addons/google_gmail/tools.py` (6 lines)
- `addons/google_gmail/views/fetchmail_server_views.xml` (32 lines)
- `addons/google_gmail/views/ir_mail_server_views.xml` (39 lines)
- `addons/google_gmail/views/res_config_settings_views.xml` (24 lines)
- `addons/google_gmail/views/templates.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
