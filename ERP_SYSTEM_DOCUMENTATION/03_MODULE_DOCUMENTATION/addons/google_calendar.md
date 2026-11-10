# Module: google_calendar

- **Module ID:** MOD-078
- **Path:** `addons/google_calendar`
- **Manifest:** `addons/google_calendar/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `google_account`, `calendar`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 35 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 11 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "google_account",
    "calendar"
  ],
  "data": [
    "data/google_calendar_data.xml",
    "wizard/reset_account_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_users_views.xml",
    "views/google_calendar_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "google_calendar/static/src/scss/google_calendar.scss",
      "google_calendar/static/src/views/**/*"
    ],
    "web.assets_unit_tests": [
      "google_calendar/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/google_calendar/__init__.py` (22 lines)
- `addons/google_calendar/__manifest__.py` (28 lines)
- `addons/google_calendar/controllers/__init__.py` (4 lines)
- `addons/google_calendar/controllers/google_auth.py` (9 lines)
- `addons/google_calendar/controllers/main.py` (73 lines)
- `addons/google_calendar/data/google_calendar_data.xml` (21 lines)
- `addons/google_calendar/data/neutralize.sql` (5 lines)
- `addons/google_calendar/i18n/af.po` (428 lines)
- `addons/google_calendar/i18n/ar.po` (599 lines)
- `addons/google_calendar/i18n/az.po` (543 lines)
- `addons/google_calendar/i18n/bg.po` (568 lines)
- `addons/google_calendar/i18n/bs.po` (543 lines)
- `addons/google_calendar/i18n/ca.po` (602 lines)
- `addons/google_calendar/i18n/cs.po` (607 lines)
- `addons/google_calendar/i18n/da.po` (591 lines)
- `addons/google_calendar/i18n/de.po` (622 lines)
- `addons/google_calendar/i18n/el.po` (562 lines)
- `addons/google_calendar/i18n/es.po` (607 lines)
- `addons/google_calendar/i18n/es_419.po` (582 lines)
- `addons/google_calendar/i18n/es_CL.po` (46 lines)
- `addons/google_calendar/i18n/et.po` (580 lines)
- `addons/google_calendar/i18n/eu.po` (427 lines)
- `addons/google_calendar/i18n/fa.po` (583 lines)
- `addons/google_calendar/i18n/fi.po` (609 lines)
- `addons/google_calendar/i18n/fo.po` (427 lines)
- `addons/google_calendar/i18n/fr.po` (619 lines)
- `addons/google_calendar/i18n/fr_BE.po` (32 lines)
- `addons/google_calendar/i18n/fr_CA.po` (46 lines)
- `addons/google_calendar/i18n/gl.po` (427 lines)
- `addons/google_calendar/i18n/google_calendar.pot` (529 lines)
- `addons/google_calendar/i18n/gu.po` (431 lines)
- `addons/google_calendar/i18n/he.po` (594 lines)
- `addons/google_calendar/i18n/hi.po` (574 lines)
- `addons/google_calendar/i18n/hr.po` (563 lines)
- `addons/google_calendar/i18n/hu.po` (581 lines)
- `addons/google_calendar/i18n/id.po` (605 lines)
- `addons/google_calendar/i18n/is.po` (424 lines)
- `addons/google_calendar/i18n/it.po` (622 lines)
- `addons/google_calendar/i18n/ja.po` (570 lines)
- `addons/google_calendar/i18n/ka.po` (427 lines)
- `addons/google_calendar/i18n/kab.po` (540 lines)
- `addons/google_calendar/i18n/km.po` (429 lines)
- `addons/google_calendar/i18n/ko.po` (595 lines)
- `addons/google_calendar/i18n/ku.po` (538 lines)
- `addons/google_calendar/i18n/lb.po` (429 lines)
- `addons/google_calendar/i18n/lo.po` (592 lines)
- `addons/google_calendar/i18n/lt.po` (566 lines)
- `addons/google_calendar/i18n/lv.po` (547 lines)
- `addons/google_calendar/i18n/mk.po` (427 lines)
- `addons/google_calendar/i18n/mn.po` (564 lines)
- `addons/google_calendar/i18n/my.po` (547 lines)
- `addons/google_calendar/i18n/nb.po` (561 lines)
- `addons/google_calendar/i18n/nl.po` (617 lines)
- `addons/google_calendar/i18n/pl.po` (621 lines)
- `addons/google_calendar/i18n/pt.po` (600 lines)
- `addons/google_calendar/i18n/pt_BR.po` (585 lines)
- `addons/google_calendar/i18n/ro.po` (607 lines)
- `addons/google_calendar/i18n/ru.po` (601 lines)
- `addons/google_calendar/i18n/sk.po` (596 lines)
- `addons/google_calendar/i18n/sl.po` (607 lines)
- `addons/google_calendar/i18n/sq.po` (427 lines)
- `addons/google_calendar/i18n/sr@latin.po` (545 lines)
- `addons/google_calendar/i18n/sv.po` (613 lines)
- `addons/google_calendar/i18n/th.po` (596 lines)
- `addons/google_calendar/i18n/tr.po` (619 lines)
- `addons/google_calendar/i18n/uk.po` (593 lines)
- `addons/google_calendar/i18n/uz.po` (677 lines)
- `addons/google_calendar/i18n/vi.po` (600 lines)
- `addons/google_calendar/i18n/zh_CN.po` (598 lines)
- `addons/google_calendar/i18n/zh_TW.po` (590 lines)
- `addons/google_calendar/models/__init__.py` (13 lines)
- `addons/google_calendar/models/calendar_alarm_manager.py` (15 lines)
- `addons/google_calendar/models/calendar_attendee.py` (40 lines)
- `addons/google_calendar/models/calendar_calendar.py` (256 lines)
- `addons/google_calendar/models/calendar_event.py` (492 lines)
- `addons/google_calendar/models/calendar_recurrence_rule.py` (276 lines)
- `addons/google_calendar/models/calendar_user.py` (45 lines)
- `addons/google_calendar/models/google_event_sync.py` (489 lines)
- `addons/google_calendar/models/google_sync.py` (82 lines)
- `addons/google_calendar/models/res_config_settings.py` (14 lines)
- `addons/google_calendar/models/res_users.py` (307 lines)
- `addons/google_calendar/models/res_users_settings.py` (86 lines)
- `addons/google_calendar/security/ir.access.csv` (2 lines)
- `addons/google_calendar/static/description/an_event.png` (43 lines)
- `addons/google_calendar/static/description/calendar_in_action.png` (639 lines)
- `addons/google_calendar/static/description/coworker.png` (63 lines)
- `addons/google_calendar/static/description/create_quick.png` (85 lines)
- `addons/google_calendar/static/description/email.png` (241 lines)
- `addons/google_calendar/static/description/icon.png` (4 lines)
- `addons/google_calendar/static/description/icon.svg` (1 lines)
- `addons/google_calendar/static/description/icon_hi.png` (55 lines)
- `addons/google_calendar/static/description/index.html` (116 lines)
- `addons/google_calendar/static/description/notification.png` (113 lines)
- `addons/google_calendar/static/description/recurrent.png` (229 lines)
- `addons/google_calendar/static/description/the_calendar.png` (621 lines)
- `addons/google_calendar/static/src/img/calendar_32.png` (17 lines)
- `addons/google_calendar/static/src/img/google-calendar.svg` (11 lines)
- `addons/google_calendar/static/src/scss/google_calendar.scss` (10 lines)
- `addons/google_calendar/static/src/views/google_calendar/attendee_calendar/attendee_calendar_filter_section.js` (22 lines)
- `addons/google_calendar/static/src/views/google_calendar/google_calendar_controller.js` (64 lines)
- `addons/google_calendar/static/src/views/google_calendar/google_calendar_controller.xml` (15 lines)
- `addons/google_calendar/static/src/views/google_calendar/google_calendar_model.js` (106 lines)
- `addons/google_calendar/static/tests/google_calendar.test.js` (194 lines)
- `addons/google_calendar/tests/__init__.py` (12 lines)
- `addons/google_calendar/tests/test_google_access_roles.py` (40 lines)
- `addons/google_calendar/tests/test_google_event.py` (15 lines)
- `addons/google_calendar/tests/test_multi_calendar_sync.py` (140 lines)
- `addons/google_calendar/tests/test_sync_calendars_google2odoo.py` (172 lines)
- `addons/google_calendar/tests/test_sync_calendars_odoo2google.py` (169 lines)
- `addons/google_calendar/tests/test_sync_common.py` (230 lines)
- `addons/google_calendar/tests/test_sync_google2odoo.py` (2,716 lines)
- `addons/google_calendar/tests/test_sync_odoo2google.py` (1,169 lines)
- `addons/google_calendar/tests/test_sync_odoo2google_mail.py` (159 lines)
- `addons/google_calendar/tests/test_token_access.py` (73 lines)
- `addons/google_calendar/utils/__init__.py` (6 lines)
- `addons/google_calendar/utils/google_api_resource.py` (113 lines)
- `addons/google_calendar/utils/google_calendar.py` (28 lines)
- `addons/google_calendar/utils/google_calendar_service.py` (230 lines)
- `addons/google_calendar/utils/google_event.py` (190 lines)
- `addons/google_calendar/views/google_calendar_views.xml` (57 lines)
- `addons/google_calendar/views/res_config_settings_views.xml` (36 lines)
- `addons/google_calendar/views/res_users_views.xml` (27 lines)
- `addons/google_calendar/wizard/__init__.py` (3 lines)
- `addons/google_calendar/wizard/reset_account.py` (35 lines)
- `addons/google_calendar/wizard/reset_account_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
