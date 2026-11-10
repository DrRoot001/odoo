# Module: mail_bot_hr

- **Module ID:** MOD-353
- **Path:** `addons/mail_bot_hr`
- **Manifest:** `addons/mail_bot_hr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge module between hr and mailbot.

This module adds the OdooBot state and notifications in the user form modified by hr.

Declared dependencies: `mail_bot`, `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mail_bot",
    "hr"
  ],
  "data": [
    "views/res_users_views.xml"
  ]
}
```

### Representative source files

- `addons/mail_bot_hr/__init__.py` (0 lines)
- `addons/mail_bot_hr/__manifest__.py` (14 lines)
- `addons/mail_bot_hr/i18n/ar.po` (33 lines)
- `addons/mail_bot_hr/i18n/az.po` (33 lines)
- `addons/mail_bot_hr/i18n/bg.po` (33 lines)
- `addons/mail_bot_hr/i18n/bs.po` (33 lines)
- `addons/mail_bot_hr/i18n/ca.po` (33 lines)
- `addons/mail_bot_hr/i18n/cs.po` (33 lines)
- `addons/mail_bot_hr/i18n/da.po` (33 lines)
- `addons/mail_bot_hr/i18n/de.po` (39 lines)
- `addons/mail_bot_hr/i18n/el.po` (33 lines)
- `addons/mail_bot_hr/i18n/es.po` (39 lines)
- `addons/mail_bot_hr/i18n/es_419.po` (39 lines)
- `addons/mail_bot_hr/i18n/et.po` (33 lines)
- `addons/mail_bot_hr/i18n/fa.po` (33 lines)
- `addons/mail_bot_hr/i18n/fi.po` (39 lines)
- `addons/mail_bot_hr/i18n/fr.po` (33 lines)
- `addons/mail_bot_hr/i18n/he.po` (33 lines)
- `addons/mail_bot_hr/i18n/hi.po` (33 lines)
- `addons/mail_bot_hr/i18n/hr.po` (33 lines)
- `addons/mail_bot_hr/i18n/hu.po` (33 lines)
- `addons/mail_bot_hr/i18n/id.po` (33 lines)
- `addons/mail_bot_hr/i18n/it.po` (39 lines)
- `addons/mail_bot_hr/i18n/ja.po` (33 lines)
- `addons/mail_bot_hr/i18n/kab.po` (33 lines)
- `addons/mail_bot_hr/i18n/ko.po` (33 lines)
- `addons/mail_bot_hr/i18n/ku.po` (33 lines)
- `addons/mail_bot_hr/i18n/lo.po` (33 lines)
- `addons/mail_bot_hr/i18n/lt.po` (33 lines)
- `addons/mail_bot_hr/i18n/lv.po` (33 lines)
- `addons/mail_bot_hr/i18n/mail_bot_hr.pot` (33 lines)
- `addons/mail_bot_hr/i18n/mn.po` (33 lines)
- `addons/mail_bot_hr/i18n/my.po` (33 lines)
- `addons/mail_bot_hr/i18n/nb.po` (33 lines)
- `addons/mail_bot_hr/i18n/nl.po` (33 lines)
- `addons/mail_bot_hr/i18n/pl.po` (33 lines)
- `addons/mail_bot_hr/i18n/pt.po` (33 lines)
- `addons/mail_bot_hr/i18n/pt_BR.po` (39 lines)
- `addons/mail_bot_hr/i18n/ro.po` (33 lines)
- `addons/mail_bot_hr/i18n/ru.po` (33 lines)
- `addons/mail_bot_hr/i18n/sk.po` (33 lines)
- `addons/mail_bot_hr/i18n/sl.po` (33 lines)
- `addons/mail_bot_hr/i18n/sr@latin.po` (33 lines)
- `addons/mail_bot_hr/i18n/sv.po` (33 lines)
- `addons/mail_bot_hr/i18n/th.po` (33 lines)
- `addons/mail_bot_hr/i18n/tr.po` (33 lines)
- `addons/mail_bot_hr/i18n/uk.po` (33 lines)
- `addons/mail_bot_hr/i18n/uz.po` (33 lines)
- `addons/mail_bot_hr/i18n/vi.po` (33 lines)
- `addons/mail_bot_hr/i18n/zh_CN.po` (33 lines)
- `addons/mail_bot_hr/i18n/zh_TW.po` (33 lines)
- `addons/mail_bot_hr/views/res_users_views.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
