# Module: hr_presence

- **Module ID:** MOD-093
- **Path:** `addons/hr_presence`
- **Manifest:** `addons/hr_presence/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Control Employees Presence
==========================

Based on:
    * The IP Address
    * The User's Session
    * The Sent Emails

Allows to contact directly the employee in case of unjustified absence.
    

Declared dependencies: `hr`, `hr_holidays`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "hr_holidays",
    "sms"
  ],
  "data": [
    "views/hr_employee_views.xml",
    "data/mail_template_data.xml",
    "data/sms_data.xml",
    "data/ir_cron.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_presence/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_presence/__init__.py` (3 lines)
- `addons/hr_presence/__manifest__.py` (32 lines)
- `addons/hr_presence/data/ir_cron.xml` (15 lines)
- `addons/hr_presence/data/mail_template_data.xml` (24 lines)
- `addons/hr_presence/data/sms_data.xml` (10 lines)
- `addons/hr_presence/i18n/ar.po` (284 lines)
- `addons/hr_presence/i18n/az.po` (236 lines)
- `addons/hr_presence/i18n/bg.po` (236 lines)
- `addons/hr_presence/i18n/bs.po` (238 lines)
- `addons/hr_presence/i18n/ca.po` (272 lines)
- `addons/hr_presence/i18n/cs.po` (276 lines)
- `addons/hr_presence/i18n/da.po` (241 lines)
- `addons/hr_presence/i18n/de.po` (305 lines)
- `addons/hr_presence/i18n/el.po` (237 lines)
- `addons/hr_presence/i18n/es.po` (301 lines)
- `addons/hr_presence/i18n/es_419.po` (295 lines)
- `addons/hr_presence/i18n/et.po` (236 lines)
- `addons/hr_presence/i18n/fa.po` (236 lines)
- `addons/hr_presence/i18n/fi.po` (292 lines)
- `addons/hr_presence/i18n/fr.po` (291 lines)
- `addons/hr_presence/i18n/he.po` (244 lines)
- `addons/hr_presence/i18n/hi.po` (236 lines)
- `addons/hr_presence/i18n/hr.po` (246 lines)
- `addons/hr_presence/i18n/hr_presence.pot` (222 lines)
- `addons/hr_presence/i18n/hu.po` (244 lines)
- `addons/hr_presence/i18n/id.po` (284 lines)
- `addons/hr_presence/i18n/it.po` (297 lines)
- `addons/hr_presence/i18n/ja.po` (276 lines)
- `addons/hr_presence/i18n/kab.po` (237 lines)
- `addons/hr_presence/i18n/ko.po` (279 lines)
- `addons/hr_presence/i18n/ku.po` (236 lines)
- `addons/hr_presence/i18n/lo.po` (285 lines)
- `addons/hr_presence/i18n/lt.po` (243 lines)
- `addons/hr_presence/i18n/lv.po` (237 lines)
- `addons/hr_presence/i18n/mn.po` (244 lines)
- `addons/hr_presence/i18n/my.po` (236 lines)
- `addons/hr_presence/i18n/nb.po` (240 lines)
- `addons/hr_presence/i18n/nl.po` (288 lines)
- `addons/hr_presence/i18n/pl.po` (292 lines)
- `addons/hr_presence/i18n/pt.po` (279 lines)
- `addons/hr_presence/i18n/pt_BR.po` (302 lines)
- `addons/hr_presence/i18n/ro.po` (244 lines)
- `addons/hr_presence/i18n/ru.po` (288 lines)
- `addons/hr_presence/i18n/sk.po` (236 lines)
- `addons/hr_presence/i18n/sl.po` (250 lines)
- `addons/hr_presence/i18n/sr@latin.po` (237 lines)
- `addons/hr_presence/i18n/sv.po` (252 lines)
- `addons/hr_presence/i18n/th.po` (275 lines)
- `addons/hr_presence/i18n/tr.po` (293 lines)
- `addons/hr_presence/i18n/uk.po` (245 lines)
- `addons/hr_presence/i18n/uz.po` (316 lines)
- `addons/hr_presence/i18n/vi.po` (284 lines)
- `addons/hr_presence/i18n/zh_CN.po` (288 lines)
- `addons/hr_presence/i18n/zh_TW.po` (275 lines)
- `addons/hr_presence/models/__init__.py` (8 lines)
- `addons/hr_presence/models/hr_employee.py` (161 lines)
- `addons/hr_presence/models/hr_employee_public.py` (12 lines)
- `addons/hr_presence/models/ir_websocket.py` (31 lines)
- `addons/hr_presence/models/res_company.py` (10 lines)
- `addons/hr_presence/models/res_config_settings.py` (12 lines)
- `addons/hr_presence/models/res_users_log.py` (9 lines)
- `addons/hr_presence/security/ir.access.csv` (3 lines)
- `addons/hr_presence/static/src/presence_cog_menu/presence_cog_menu.js` (69 lines)
- `addons/hr_presence/static/src/presence_cog_menu/presence_cog_menu.xml` (25 lines)
- `addons/hr_presence/static/src/search/hr_presence_action_menus/hr_presence_action_menus.js` (26 lines)
- `addons/hr_presence/static/src/search/hr_presence_action_menus/hr_presence_action_menus.xml` (10 lines)
- `addons/hr_presence/static/src/views/hooks.js` (34 lines)
- `addons/hr_presence/views/hr_employee_views.xml` (73 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
