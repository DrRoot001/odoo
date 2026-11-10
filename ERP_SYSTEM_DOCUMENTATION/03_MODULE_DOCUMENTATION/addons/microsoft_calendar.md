# Module: microsoft_calendar

- **Module ID:** MOD-375
- **Path:** `addons/microsoft_calendar`
- **Manifest:** `addons/microsoft_calendar/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `microsoft_account`, `calendar`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "microsoft_account",
    "calendar"
  ],
  "data": [
    "data/microsoft_calendar_data.xml",
    "wizard/reset_account_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_users_views.xml",
    "views/microsoft_calendar_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "microsoft_calendar/static/src/scss/microsoft_calendar.scss",
      "microsoft_calendar/static/src/views/**/*"
    ],
    "web.assets_unit_tests": [
      "microsoft_calendar/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/microsoft_calendar/__init__.py` (17 lines)
- `addons/microsoft_calendar/__manifest__.py` (27 lines)
- `addons/microsoft_calendar/controllers/__init__.py` (4 lines)
- `addons/microsoft_calendar/controllers/main.py` (67 lines)
- `addons/microsoft_calendar/controllers/microsoft_auth.py` (9 lines)
- `addons/microsoft_calendar/data/microsoft_calendar_data.xml` (16 lines)
- `addons/microsoft_calendar/data/neutralize.sql` (11 lines)
- `addons/microsoft_calendar/i18n/ar.po` (511 lines)
- `addons/microsoft_calendar/i18n/az.po` (460 lines)
- `addons/microsoft_calendar/i18n/bg.po` (463 lines)
- `addons/microsoft_calendar/i18n/bs.po` (453 lines)
- `addons/microsoft_calendar/i18n/ca.po` (507 lines)
- `addons/microsoft_calendar/i18n/cs.po` (492 lines)
- `addons/microsoft_calendar/i18n/da.po` (500 lines)
- `addons/microsoft_calendar/i18n/de.po` (523 lines)
- `addons/microsoft_calendar/i18n/el.po` (463 lines)
- `addons/microsoft_calendar/i18n/es.po` (520 lines)
- `addons/microsoft_calendar/i18n/es_419.po` (520 lines)
- `addons/microsoft_calendar/i18n/et.po` (486 lines)
- `addons/microsoft_calendar/i18n/fa.po` (481 lines)
- `addons/microsoft_calendar/i18n/fi.po` (520 lines)
- `addons/microsoft_calendar/i18n/fr.po` (526 lines)
- `addons/microsoft_calendar/i18n/he.po` (482 lines)
- `addons/microsoft_calendar/i18n/hi.po` (481 lines)
- `addons/microsoft_calendar/i18n/hr.po` (473 lines)
- `addons/microsoft_calendar/i18n/hu.po` (479 lines)
- `addons/microsoft_calendar/i18n/id.po` (520 lines)
- `addons/microsoft_calendar/i18n/it.po` (522 lines)
- `addons/microsoft_calendar/i18n/ja.po` (512 lines)
- `addons/microsoft_calendar/i18n/kab.po` (452 lines)
- `addons/microsoft_calendar/i18n/ko.po` (509 lines)
- `addons/microsoft_calendar/i18n/ku.po` (455 lines)
- `addons/microsoft_calendar/i18n/lo.po` (475 lines)
- `addons/microsoft_calendar/i18n/lt.po` (462 lines)
- `addons/microsoft_calendar/i18n/lv.po` (452 lines)
- `addons/microsoft_calendar/i18n/microsoft_calendar.pot` (443 lines)
- `addons/microsoft_calendar/i18n/mn.po` (463 lines)
- `addons/microsoft_calendar/i18n/my.po` (462 lines)
- `addons/microsoft_calendar/i18n/nb.po` (468 lines)
- `addons/microsoft_calendar/i18n/nl.po` (521 lines)
- `addons/microsoft_calendar/i18n/pl.po` (523 lines)
- `addons/microsoft_calendar/i18n/pt.po` (520 lines)
- `addons/microsoft_calendar/i18n/pt_BR.po` (522 lines)
- `addons/microsoft_calendar/i18n/ro.po` (520 lines)
- `addons/microsoft_calendar/i18n/ru.po` (522 lines)
- `addons/microsoft_calendar/i18n/sk.po` (451 lines)
- `addons/microsoft_calendar/i18n/sl.po` (483 lines)
- `addons/microsoft_calendar/i18n/sr@latin.po` (461 lines)
- `addons/microsoft_calendar/i18n/sv.po` (519 lines)
- `addons/microsoft_calendar/i18n/th.po` (509 lines)
- `addons/microsoft_calendar/i18n/tr.po` (522 lines)
- `addons/microsoft_calendar/i18n/uk.po` (517 lines)
- `addons/microsoft_calendar/i18n/uz.po` (593 lines)
- `addons/microsoft_calendar/i18n/vi.po` (515 lines)
- `addons/microsoft_calendar/i18n/zh_CN.po` (499 lines)
- `addons/microsoft_calendar/i18n/zh_TW.po` (501 lines)
- `addons/microsoft_calendar/models/__init__.py` (10 lines)
- `addons/microsoft_calendar/models/calendar_alarm_manager.py` (15 lines)
- `addons/microsoft_calendar/models/calendar_attendee.py` (37 lines)
- `addons/microsoft_calendar/models/calendar_event.py` (749 lines)
- `addons/microsoft_calendar/models/calendar_recurrence_rule.py` (215 lines)
- `addons/microsoft_calendar/models/microsoft_sync.py` (578 lines)
- `addons/microsoft_calendar/models/res_config_settings.py` (12 lines)
- `addons/microsoft_calendar/models/res_users.py` (230 lines)
- `addons/microsoft_calendar/models/res_users_settings.py` (23 lines)
- `addons/microsoft_calendar/security/ir.access.csv` (2 lines)
- `addons/microsoft_calendar/static/description/icon.png` (13 lines)
- `addons/microsoft_calendar/static/description/icon.svg` (1 lines)
- `addons/microsoft_calendar/static/description/icon_hi.png` (71 lines)
- `addons/microsoft_calendar/static/src/img/calendar_outlook_32.png` (6 lines)
- `addons/microsoft_calendar/static/src/img/outlook-calendar.svg` (20 lines)
- `addons/microsoft_calendar/static/src/scss/microsoft_calendar.scss` (10 lines)
- `addons/microsoft_calendar/static/src/views/microsoft_calendar/microsoft_calendar_controller.js` (63 lines)
- `addons/microsoft_calendar/static/src/views/microsoft_calendar/microsoft_calendar_controller.xml` (14 lines)
- `addons/microsoft_calendar/static/src/views/microsoft_calendar/microsoft_calendar_model.js` (86 lines)
- `addons/microsoft_calendar/static/tests/microsoft_calendar.test.js` (128 lines)
- `addons/microsoft_calendar/tests/__init__.py` (11 lines)
- `addons/microsoft_calendar/tests/common.py` (544 lines)
- `addons/microsoft_calendar/tests/test_answer_events.py` (212 lines)
- `addons/microsoft_calendar/tests/test_create_events.py` (857 lines)
- `addons/microsoft_calendar/tests/test_delete_events.py` (363 lines)
- `addons/microsoft_calendar/tests/test_microsoft_event.py` (591 lines)
- `addons/microsoft_calendar/tests/test_microsoft_service.py` (526 lines)
- `addons/microsoft_calendar/tests/test_multicalendar.py` (99 lines)
- `addons/microsoft_calendar/tests/test_sync_odoo2microsoft_mail.py` (112 lines)
- `addons/microsoft_calendar/tests/test_update_events.py` (1,697 lines)
- `addons/microsoft_calendar/utils/__init__.py` (4 lines)
- `addons/microsoft_calendar/utils/microsoft_calendar.py` (219 lines)
- `addons/microsoft_calendar/utils/microsoft_event.py` (268 lines)
- `addons/microsoft_calendar/views/microsoft_calendar_views.xml` (59 lines)
- `addons/microsoft_calendar/views/res_config_settings_views.xml` (26 lines)
- `addons/microsoft_calendar/views/res_users_views.xml` (28 lines)
- `addons/microsoft_calendar/wizard/__init__.py` (3 lines)
- `addons/microsoft_calendar/wizard/reset_account.py` (26 lines)
- `addons/microsoft_calendar/wizard/reset_account_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
