# Module: calendar

- **Module ID:** MOD-046
- **Path:** `addons/calendar`
- **Manifest:** `addons/calendar/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Schedule employees' meetings


This is a full-featured calendar system.
========================================

It supports:
------------
    - Calendar of events
    - Recurring events

If you need to manage your meetings, you should install the CRM module.
    

Declared dependencies: `base`, `mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 47 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 19 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 39 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 59 | Client behavior/assets. |
| Tests | 20 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 10 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "mail"
  ],
  "data": [
    "data/calendar_cron.xml",
    "data/mail_templates_chatter.xml",
    "data/mail_template_data.xml",
    "data/calendar_data.xml",
    "data/mail_activity_type_data.xml",
    "data/mail_message_subtype_data.xml",
    "views/mail_activity_views.xml",
    "views/calendar_calendar_views.xml",
    "views/calendar_templates.xml",
    "views/calendar_user_views.xml",
    "views/calendar_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/res_users_views.xml",
    "wizard/calendar_event_archive_or_unlink_wizard.xml",
    "wizard/calendar_event_multi_archive_or_unlink_wizard.xml",
    "wizard/mail_activity_schedule_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/calendar_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "calendar/static/src/core/common/**/*",
      "calendar/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "calendar/static/tests/**/*.js",
      [
        "remove",
        "calendar/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "calendar/static/tests/tours/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      "calendar/static/tests/mock_server/**/*"
    ],
    "mail.assets_public": [
      "calendar/static/src/core/common/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "calendar/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "calendar/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/calendar/__init__.py` (27 lines)
- `addons/calendar/__manifest__.py` (74 lines)
- `addons/calendar/controllers/__init__.py` (3 lines)
- `addons/calendar/controllers/main.py` (133 lines)
- `addons/calendar/data/calendar_cron.xml` (16 lines)
- `addons/calendar/data/calendar_data.xml` (61 lines)
- `addons/calendar/data/calendar_demo.xml` (125 lines)
- `addons/calendar/data/mail_activity_type_data.xml` (8 lines)
- `addons/calendar/data/mail_message_subtype_data.xml` (19 lines)
- `addons/calendar/data/mail_template_data.xml` (621 lines)
- `addons/calendar/data/mail_templates_chatter.xml` (27 lines)
- `addons/calendar/i18n/af.po` (3,614 lines)
- `addons/calendar/i18n/am.po` (3,610 lines)
- `addons/calendar/i18n/ar.po` (4,145 lines)
- `addons/calendar/i18n/az.po` (4,090 lines)
- `addons/calendar/i18n/bg.po` (4,100 lines)
- `addons/calendar/i18n/bn.po` (3,612 lines)
- `addons/calendar/i18n/bs.po` (4,098 lines)
- `addons/calendar/i18n/ca.po` (5,882 lines)
- `addons/calendar/i18n/calendar.pot` (3,650 lines)
- `addons/calendar/i18n/cs.po` (4,188 lines)
- `addons/calendar/i18n/da.po` (4,192 lines)
- `addons/calendar/i18n/de.po` (6,038 lines)
- `addons/calendar/i18n/el.po` (4,103 lines)
- `addons/calendar/i18n/es.po` (7,487 lines)
- `addons/calendar/i18n/es_419.po` (6,016 lines)
- `addons/calendar/i18n/es_CL.po` (124 lines)
- `addons/calendar/i18n/et.po` (4,175 lines)
- `addons/calendar/i18n/eu.po` (3,613 lines)
- `addons/calendar/i18n/fa.po` (4,147 lines)
- `addons/calendar/i18n/fi.po` (5,956 lines)
- `addons/calendar/i18n/fo.po` (3,613 lines)
- `addons/calendar/i18n/fr.po` (6,013 lines)
- `addons/calendar/i18n/fr_BE.po` (606 lines)
- `addons/calendar/i18n/fr_CA.po` (124 lines)
- `addons/calendar/i18n/gl.po` (3,613 lines)
- `addons/calendar/i18n/gu.po` (3,614 lines)
- `addons/calendar/i18n/he.po` (4,138 lines)
- `addons/calendar/i18n/hi.po` (4,161 lines)
- `addons/calendar/i18n/hr.po` (4,210 lines)
- `addons/calendar/i18n/hu.po` (4,089 lines)
- `addons/calendar/i18n/id.po` (6,003 lines)
- `addons/calendar/i18n/is.po` (3,610 lines)
- `addons/calendar/i18n/it.po` (6,000 lines)
- `addons/calendar/i18n/ja.po` (4,655 lines)
- `addons/calendar/i18n/ka.po` (3,613 lines)
- `addons/calendar/i18n/kab.po` (4,045 lines)
- `addons/calendar/i18n/km.po` (3,615 lines)
- `addons/calendar/i18n/ko.po` (4,164 lines)
- `addons/calendar/i18n/ku.po` (4,015 lines)
- `addons/calendar/i18n/lo.po` (5,842 lines)
- `addons/calendar/i18n/lt.po` (4,103 lines)
- `addons/calendar/i18n/lv.po` (4,206 lines)
- `addons/calendar/i18n/mk.po` (3,613 lines)
- `addons/calendar/i18n/mn.po` (5,902 lines)
- `addons/calendar/i18n/my.po` (4,016 lines)
- `addons/calendar/i18n/nb.po` (4,083 lines)
- `addons/calendar/i18n/nl.po` (6,006 lines)
- `addons/calendar/i18n/pl.po` (4,194 lines)
- `addons/calendar/i18n/pt.po` (5,954 lines)
- `addons/calendar/i18n/pt_BR.po` (6,017 lines)
- `addons/calendar/i18n/ro.po` (4,192 lines)
- `addons/calendar/i18n/ru.po` (6,386 lines)
- `addons/calendar/i18n/sk.po` (4,112 lines)
- `addons/calendar/i18n/sl.po` (4,180 lines)
- `addons/calendar/i18n/sq.po` (3,613 lines)
- `addons/calendar/i18n/sr@latin.po` (4,156 lines)
- `addons/calendar/i18n/sv.po` (4,183 lines)
- `addons/calendar/i18n/th.po` (5,761 lines)
- `addons/calendar/i18n/tr.po` (4,615 lines)
- `addons/calendar/i18n/uk.po` (4,175 lines)
- `addons/calendar/i18n/uz.po` (4,703 lines)
- `addons/calendar/i18n/vi.po` (4,624 lines)
- `addons/calendar/i18n/zh_CN.po` (6,744 lines)
- `addons/calendar/i18n/zh_TW.po` (4,332 lines)
- `addons/calendar/models/__init__.py` (20 lines)
- `addons/calendar/models/calendar_alarm.py` (77 lines)
- `addons/calendar/models/calendar_alarm_manager.py` (267 lines)
- `addons/calendar/models/calendar_attendee.py` (242 lines)
- `addons/calendar/models/calendar_calendar.py` (147 lines)
- `addons/calendar/models/calendar_event.py` (2,201 lines)
- `addons/calendar/models/calendar_event_type.py` (22 lines)
- `addons/calendar/models/calendar_filter.py` (65 lines)
- `addons/calendar/models/calendar_recurrence.py` (653 lines)
- `addons/calendar/models/calendar_user.py` (50 lines)
- `addons/calendar/models/discuss_channel.py` (93 lines)
- `addons/calendar/models/ir_http.py` (29 lines)
- `addons/calendar/models/mail_activity.py` (99 lines)
- `addons/calendar/models/mail_activity_mixin.py` (19 lines)
- `addons/calendar/models/mail_activity_type.py` (9 lines)
- `addons/calendar/models/res_partner.py` (155 lines)
- `addons/calendar/models/res_users.py` (210 lines)
- `addons/calendar/models/res_users_settings.py` (9 lines)
- `addons/calendar/models/utils.py` (11 lines)
- `addons/calendar/security/ir.access.csv` (19 lines)
- `addons/calendar/static/description/icon.png` (26 lines)
- `addons/calendar/static/description/icon.svg` (1 lines)
- `addons/calendar/static/description/icon_hi.png` (110 lines)
- `addons/calendar/static/src/core/common/@types/models.d.ts` (13 lines)
- `addons/calendar/static/src/core/common/calendar_event_model.js` (17 lines)
- `addons/calendar/static/src/core/web/@types/models.d.ts` (5 lines)
- `addons/calendar/static/src/core/web/activity_list_popover_item_patch.js` (14 lines)
- `addons/calendar/static/src/core/web/activity_list_popover_item_patch.xml` (10 lines)
- `addons/calendar/static/src/core/web/activity_menu_patch.js` (43 lines)
- `addons/calendar/static/src/core/web/activity_menu_patch.xml` (21 lines)
- `addons/calendar/static/src/core/web/activity_model_patch.js` (23 lines)
- `addons/calendar/static/src/core/web/activity_patch.js` (44 lines)
- `addons/calendar/static/src/core/web/activity_patch.xml` (45 lines)
- `addons/calendar/static/src/core/web/messaging_menu_model_patch.js` (33 lines)
- `addons/calendar/static/src/core/web/schedule_meeting.js` (19 lines)
- `addons/calendar/static/src/core/web/store_service_patch.js` (26 lines)
- `addons/calendar/static/src/img/apple-calendar-128.png` (26 lines)
- `addons/calendar/static/src/img/bell.png` (7 lines)
- `addons/calendar/static/src/img/check-circle.png` (9 lines)
- `addons/calendar/static/src/img/google-calendar-128.png` (7 lines)
- `addons/calendar/static/src/img/outlook-calendar-128.png` (15 lines)
- `addons/calendar/static/src/img/state_accepted.png` (4 lines)
- `addons/calendar/static/src/img/state_declined.png` (4 lines)
- `addons/calendar/static/src/img/state_needsAction.png` (5 lines)
- `addons/calendar/static/src/img/state_tentative.png` (4 lines)
- `addons/calendar/static/src/img/sync.png` (5 lines)
- `addons/calendar/static/src/img/times-circle.png` (8 lines)
- `addons/calendar/static/src/js/services/calendar_notification_service.js` (95 lines)
- `addons/calendar/static/src/scss/calendar.scss` (146 lines)
- `addons/calendar/static/src/scss/calendar_event_views.scss` (64 lines)
- `addons/calendar/static/src/scss/res_partner.scss` (5 lines)
- `addons/calendar/static/src/views/ask_recurrence_update_policy_dialog.js` (46 lines)
- `addons/calendar/static/src/views/ask_recurrence_update_policy_dialog.xml` (20 lines)
- `addons/calendar/static/src/views/ask_recurrence_update_policy_hook.js` (17 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_common_renderer.js` (137 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_common_renderer.xml` (9 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_list_popover.js` (89 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_list_popover.xml` (35 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_list_popover_item.js` (128 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_list_popover_item.xml` (63 lines)
- `addons/calendar/static/src/views/attendee_calendar/activity/attendee_calendar_activity_model.js` (121 lines)
- `addons/calendar/static/src/views/attendee_calendar/attendee_calendar_controller.js` (113 lines)
- `addons/calendar/static/src/views/attendee_calendar/attendee_calendar_controller.xml` (74 lines)
- `addons/calendar/static/src/views/attendee_calendar/attendee_calendar_model.js` (384 lines)
- `addons/calendar/static/src/views/attendee_calendar/attendee_calendar_renderer.js` (13 lines)
- `addons/calendar/static/src/views/attendee_calendar/attendee_calendar_view.js` (14 lines)
- `addons/calendar/static/src/views/attendee_calendar/common/attendee_calendar_common_popover.js` (113 lines)
- `addons/calendar/static/src/views/attendee_calendar/common/attendee_calendar_common_popover.xml` (20 lines)
- `addons/calendar/static/src/views/attendee_calendar/common/attendee_calendar_common_renderer.js` (115 lines)
- `addons/calendar/static/src/views/attendee_calendar/common/attendee_calendar_common_renderer.xml` (18 lines)
- `addons/calendar/static/src/views/attendee_calendar/filter_section/attendee_calendar_calendar_filter_section.js` (158 lines)
- `addons/calendar/static/src/views/attendee_calendar/filter_section/attendee_calendar_calendar_filter_section.xml` (39 lines)
- `addons/calendar/static/src/views/attendee_calendar/filter_section/attendee_calendar_filter_section.js` (72 lines)
- `addons/calendar/static/src/views/attendee_calendar/filter_section/attendee_calendar_filter_section.scss` (12 lines)
- `addons/calendar/static/src/views/attendee_calendar/filter_section/attendee_calendar_filter_section.xml` (21 lines)
- `addons/calendar/static/src/views/attendee_calendar/side_panel/attendee_calendar_side_panel.js` (19 lines)
- `addons/calendar/static/src/views/attendee_calendar/side_panel/attendee_calendar_side_panel.xml` (16 lines)
- `addons/calendar/static/src/views/attendee_calendar/year/attendee_calendar_year_popover.js` (17 lines)
- `addons/calendar/static/src/views/attendee_calendar/year/attendee_calendar_year_popover.xml` (9 lines)
- `addons/calendar/static/src/views/attendee_calendar/year/attendee_calendar_year_renderer.js` (9 lines)
- `addons/calendar/static/src/views/calendar_form/calendar_event_form_controller.js` (91 lines)
- `addons/calendar/static/src/views/calendar_form/calendar_event_form_model.js` (37 lines)
- `addons/calendar/static/src/views/calendar_form/calendar_event_form_view.js` (13 lines)
- `addons/calendar/static/src/views/calendar_form/calendar_event_quick_create.js` (99 lines)
- `addons/calendar/static/src/views/calendar_form/calendar_event_quick_create.xml` (12 lines)

Additional files not expanded here: 70. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
