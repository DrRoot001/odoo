# Module: mail_bot

- **Module ID:** MOD-352
- **Path:** `addons/mail_bot`
- **Manifest:** `addons/mail_bot/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add OdooBot in discussions

No manifest description declared.

Declared dependencies: `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail"
  ],
  "data": [
    "views/res_users_views.xml",
    "data/mailbot_data.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "mail_bot/static/src/scss/odoobot_style.scss"
    ]
  }
}
```

### Representative source files

- `addons/mail_bot/__init__.py` (4 lines)
- `addons/mail_bot/__manifest__.py` (22 lines)
- `addons/mail_bot/controllers/__init__.py` (3 lines)
- `addons/mail_bot/controllers/thread.py` (12 lines)
- `addons/mail_bot/data/mailbot_data.xml` (8 lines)
- `addons/mail_bot/i18n/ar.po` (338 lines)
- `addons/mail_bot/i18n/az.po` (327 lines)
- `addons/mail_bot/i18n/bg.po` (323 lines)
- `addons/mail_bot/i18n/bs.po` (328 lines)
- `addons/mail_bot/i18n/ca.po` (336 lines)
- `addons/mail_bot/i18n/cs.po` (330 lines)
- `addons/mail_bot/i18n/da.po` (330 lines)
- `addons/mail_bot/i18n/de.po` (382 lines)
- `addons/mail_bot/i18n/el.po` (327 lines)
- `addons/mail_bot/i18n/es.po` (343 lines)
- `addons/mail_bot/i18n/es_419.po` (337 lines)
- `addons/mail_bot/i18n/et.po` (331 lines)
- `addons/mail_bot/i18n/fa.po` (330 lines)
- `addons/mail_bot/i18n/fi.po` (340 lines)
- `addons/mail_bot/i18n/fr.po` (345 lines)
- `addons/mail_bot/i18n/gu.po` (325 lines)
- `addons/mail_bot/i18n/he.po` (334 lines)
- `addons/mail_bot/i18n/hi.po` (323 lines)
- `addons/mail_bot/i18n/hr.po` (330 lines)
- `addons/mail_bot/i18n/hu.po` (329 lines)
- `addons/mail_bot/i18n/id.po` (339 lines)
- `addons/mail_bot/i18n/is.po` (320 lines)
- `addons/mail_bot/i18n/it.po` (342 lines)
- `addons/mail_bot/i18n/ja.po` (340 lines)
- `addons/mail_bot/i18n/kab.po` (324 lines)
- `addons/mail_bot/i18n/ko.po` (338 lines)
- `addons/mail_bot/i18n/ku.po` (323 lines)
- `addons/mail_bot/i18n/lo.po` (361 lines)
- `addons/mail_bot/i18n/lt.po` (330 lines)
- `addons/mail_bot/i18n/lv.po` (324 lines)
- `addons/mail_bot/i18n/mail_bot.pot` (320 lines)
- `addons/mail_bot/i18n/mn.po` (330 lines)
- `addons/mail_bot/i18n/my.po` (323 lines)
- `addons/mail_bot/i18n/nb.po` (327 lines)
- `addons/mail_bot/i18n/nl.po` (378 lines)
- `addons/mail_bot/i18n/pl.po` (336 lines)
- `addons/mail_bot/i18n/pt.po` (333 lines)
- `addons/mail_bot/i18n/pt_BR.po` (380 lines)
- `addons/mail_bot/i18n/ro.po` (333 lines)
- `addons/mail_bot/i18n/ru.po` (338 lines)
- `addons/mail_bot/i18n/sk.po` (327 lines)
- `addons/mail_bot/i18n/sl.po` (338 lines)
- `addons/mail_bot/i18n/sr@latin.po` (328 lines)
- `addons/mail_bot/i18n/sv.po` (337 lines)
- `addons/mail_bot/i18n/th.po` (337 lines)
- `addons/mail_bot/i18n/tr.po` (345 lines)
- `addons/mail_bot/i18n/uk.po` (332 lines)
- `addons/mail_bot/i18n/uz.po` (373 lines)
- `addons/mail_bot/i18n/vi.po` (342 lines)
- `addons/mail_bot/i18n/zh_CN.po` (361 lines)
- `addons/mail_bot/i18n/zh_TW.po` (337 lines)
- `addons/mail_bot/models/__init__.py` (5 lines)
- `addons/mail_bot/models/discuss_channel.py` (15 lines)
- `addons/mail_bot/models/mail_bot.py` (334 lines)
- `addons/mail_bot/models/res_users.py` (46 lines)
- `addons/mail_bot/static/description/icon.png` (40 lines)
- `addons/mail_bot/static/description/icon.svg` (1 lines)
- `addons/mail_bot/static/description/icon_hi.png` (137 lines)
- `addons/mail_bot/static/src/scss/odoobot_style.scss` (8 lines)
- `addons/mail_bot/views/res_users_views.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
