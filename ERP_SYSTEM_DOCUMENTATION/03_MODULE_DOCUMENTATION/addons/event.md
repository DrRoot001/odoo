# Module: event

- **Module ID:** MOD-064
- **Path:** `addons/event`
- **Manifest:** `addons/event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Trainings, Conferences, Meetings, Exhibitions, Registrations


Organization and management of Events.
======================================

The event module allows you to efficiently organize events and all related tasks: planning, registration tracking,
attendances, etc.

Key Features
------------
* Manage your Events and Registrations
* Use emails to automatically confirm and send acknowledgments for any event registration


Declared dependencies: `barcodes`, `base_setup`, `digest`, `mail`, `phone_validation`, `portal`, `utm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 20 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 40 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 16 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "barcodes",
    "base_setup",
    "digest",
    "mail",
    "phone_validation",
    "portal",
    "utm"
  ],
  "data": [
    "security/event_security.xml",
    "views/digest_views.xml",
    "views/event_menu_views.xml",
    "views/event_ticket_views.xml",
    "views/event_mail_views.xml",
    "views/event_registration_views.xml",
    "views/event_slot_views.xml",
    "views/event_type_views.xml",
    "views/event_event_views.xml",
    "views/event_stage_views.xml",
    "report/event_event_templates.xml",
    "report/event_event_reports.xml",
    "report/event_registration_report.xml",
    "data/digest_data.xml",
    "data/ir_cron_data.xml",
    "data/mail_template_data.xml",
    "data/portal_entry_data.xml",
    "data/event_data.xml",
    "data/event_tour.xml",
    "views/res_config_settings_views.xml",
    "views/event_templates.xml",
    "views/res_partner_views.xml",
    "views/event_tag_views.xml",
    "views/event_question_views.xml",
    "views/event_registration_answer_views.xml",
    "views/portal_templates.xml",
    "data/event_question_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_users_demo.xml",
    "data/res_partner_demo.xml",
    "data/event_demo_misc.xml",
    "data/event_demo.xml",
    "data/event_registration_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "event/static/src/client_action/**/*",
      "event/static/src/scss/event.scss",
      "event/static/src/event_state_selection_field/*",
      "event/static/src/icon_selection_field/icon_selection_field.js",
      "event/static/src/icon_selection_field/icon_selection_field.xml",
      "event/static/src/template_reference_field/*",
      "event/static/src/js/tours/**/*",
      "event/static/src/views/**/*"
    ],
    "web.assets_frontend": [
      "event/static/src/js/tours/**/*"
    ],
    "web.report_assets_common": [
      "/event/static/src/scss/event_badge_report.scss",
      "/event/static/src/scss/event_full_page_ticket_report.scss",
      "/event/static/src/scss/event_full_page_ticket_responsive_html_report.scss"
    ],
    "web.report_assets_pdf": [
      "/event/static/src/scss/event_full_page_ticket_report_pdf.scss"
    ]
  }
}
```

### Representative source files

- `addons/event/__init__.py` (6 lines)
- `addons/event/__manifest__.py` (82 lines)
- `addons/event/controllers/__init__.py` (5 lines)
- `addons/event/controllers/main.py` (105 lines)
- `addons/event/controllers/portal.py` (97 lines)
- `addons/event/data/digest_data.xml` (8 lines)
- `addons/event/data/event_data.xml` (28 lines)
- `addons/event/data/event_demo.xml` (313 lines)
- `addons/event/data/event_demo_misc.xml` (93 lines)
- `addons/event/data/event_question_data.xml` (25 lines)
- `addons/event/data/event_registration_demo.xml` (166 lines)
- `addons/event/data/event_tour.xml` (8 lines)
- `addons/event/data/ir_cron_data.xml` (14 lines)
- `addons/event/data/mail_template_data.xml` (822 lines)
- `addons/event/data/portal_entry_data.xml` (12 lines)
- `addons/event/data/res_partner_demo.xml` (67 lines)
- `addons/event/data/res_users_demo.xml` (6 lines)
- `addons/event/i18n/af.po` (5,397 lines)
- `addons/event/i18n/am.po` (5,393 lines)
- `addons/event/i18n/ar.po` (8,891 lines)
- `addons/event/i18n/az.po` (5,429 lines)
- `addons/event/i18n/bg.po` (5,470 lines)
- `addons/event/i18n/bs.po` (5,413 lines)
- `addons/event/i18n/ca.po` (7,247 lines)
- `addons/event/i18n/cs.po` (5,644 lines)
- `addons/event/i18n/da.po` (5,629 lines)
- `addons/event/i18n/de.po` (12,281 lines)
- `addons/event/i18n/el.po` (5,432 lines)
- `addons/event/i18n/es.po` (9,779 lines)
- `addons/event/i18n/es_419.po` (12,251 lines)
- `addons/event/i18n/es_CL.po` (199 lines)
- `addons/event/i18n/et.po` (5,579 lines)
- `addons/event/i18n/eu.po` (5,396 lines)
- `addons/event/i18n/event.pot` (4,931 lines)
- `addons/event/i18n/fa.po` (5,432 lines)
- `addons/event/i18n/fi.po` (12,210 lines)
- `addons/event/i18n/fo.po` (5,396 lines)
- `addons/event/i18n/fr.po` (9,836 lines)
- `addons/event/i18n/fr_BE.po` (269 lines)
- `addons/event/i18n/fr_CA.po` (182 lines)
- `addons/event/i18n/gl.po` (5,396 lines)
- `addons/event/i18n/gu.po` (5,407 lines)
- `addons/event/i18n/he.po` (5,508 lines)
- `addons/event/i18n/hi.po` (5,432 lines)
- `addons/event/i18n/hr.po` (5,466 lines)
- `addons/event/i18n/hu.po` (5,445 lines)
- `addons/event/i18n/id.po` (12,169 lines)
- `addons/event/i18n/is.po` (5,393 lines)
- `addons/event/i18n/it.po` (12,233 lines)
- `addons/event/i18n/ja.po` (8,052 lines)
- `addons/event/i18n/ka.po` (5,396 lines)
- `addons/event/i18n/kab.po` (5,408 lines)
- `addons/event/i18n/km.po` (5,400 lines)
- `addons/event/i18n/ko.po` (8,003 lines)
- `addons/event/i18n/ku.po` (5,420 lines)
- `addons/event/i18n/lb.po` (5,398 lines)
- `addons/event/i18n/lo.po` (8,006 lines)
- `addons/event/i18n/lt.po` (5,481 lines)
- `addons/event/i18n/lv.po` (5,425 lines)
- `addons/event/i18n/mk.po` (5,396 lines)
- `addons/event/i18n/mn.po` (5,444 lines)
- `addons/event/i18n/my.po` (5,414 lines)
- `addons/event/i18n/nb.po` (5,430 lines)
- `addons/event/i18n/nl.po` (12,246 lines)
- `addons/event/i18n/pl.po` (10,575 lines)
- `addons/event/i18n/pt.po` (8,075 lines)
- `addons/event/i18n/pt_BR.po` (12,140 lines)
- `addons/event/i18n/ro.po` (5,668 lines)
- `addons/event/i18n/ru.po` (8,930 lines)
- `addons/event/i18n/sk.po` (5,453 lines)
- `addons/event/i18n/sl.po` (5,595 lines)
- `addons/event/i18n/sq.po` (5,396 lines)
- `addons/event/i18n/sr@latin.po` (5,580 lines)
- `addons/event/i18n/sv.po` (9,761 lines)
- `addons/event/i18n/th.po` (12,053 lines)
- `addons/event/i18n/tr.po` (9,007 lines)
- `addons/event/i18n/uk.po` (5,573 lines)
- `addons/event/i18n/uz.po` (6,282 lines)
- `addons/event/i18n/vi.po` (8,043 lines)
- `addons/event/i18n/zh_CN.po` (9,635 lines)
- `addons/event/i18n/zh_TW.po` (7,179 lines)
- `addons/event/models/__init__.py` (24 lines)
- `addons/event/models/digest.py` (22 lines)
- `addons/event/models/event_event.py` (914 lines)
- `addons/event/models/event_mail.py` (488 lines)
- `addons/event/models/event_mail_registration.py` (56 lines)
- `addons/event/models/event_mail_slot.py` (31 lines)
- `addons/event/models/event_question.py` (102 lines)
- `addons/event/models/event_question_answer.py` (21 lines)
- `addons/event/models/event_registration.py` (522 lines)
- `addons/event/models/event_registration_answer.py` (32 lines)
- `addons/event/models/event_slot.py` (145 lines)
- `addons/event/models/event_stage.py` (18 lines)
- `addons/event/models/event_tag.py` (41 lines)
- `addons/event/models/event_ticket.py` (205 lines)
- `addons/event/models/event_type.py` (62 lines)
- `addons/event/models/event_type_mail.py` (44 lines)
- `addons/event/models/event_type_ticket.py` (36 lines)
- `addons/event/models/mail_template.py` (28 lines)
- `addons/event/models/res_config_settings.py` (76 lines)
- `addons/event/models/res_partner.py` (87 lines)
- `addons/event/report/__init__.py` (2 lines)
- `addons/event/report/event_event_reports.xml` (100 lines)
- `addons/event/report/event_event_templates.xml` (426 lines)
- `addons/event/report/event_registration_report.xml` (78 lines)
- `addons/event/security/event_security.xml` (32 lines)
- `addons/event/security/ir.access.csv` (40 lines)
- `addons/event/static/description/icon.png` (21 lines)
- `addons/event/static/description/icon.svg` (1 lines)
- `addons/event/static/description/icon_hi.png` (132 lines)
- `addons/event/static/src/client_action/event_barcode.js` (143 lines)
- `addons/event/static/src/client_action/event_barcode.scss` (67 lines)
- `addons/event/static/src/client_action/event_barcode.xml` (28 lines)
- `addons/event/static/src/client_action/event_registration_summary_dialog.js` (111 lines)
- `addons/event/static/src/client_action/event_registration_summary_dialog.xml` (79 lines)
- `addons/event/static/src/event_state_selection_field/event_state_selection_field.js` (69 lines)
- `addons/event/static/src/event_state_selection_field/event_state_selection_field.scss` (12 lines)
- `addons/event/static/src/event_state_selection_field/event_state_selection_field.xml` (24 lines)
- `addons/event/static/src/icon_selection_field/icon_selection_field.js` (38 lines)
- `addons/event/static/src/icon_selection_field/icon_selection_field.xml` (8 lines)
- `addons/event/static/src/img/apple-calendar-128.png` (26 lines)
- `addons/event/static/src/img/apple-calendar.svg` (48 lines)
- `addons/event/static/src/img/event_ticket.svg` (56 lines)
- `addons/event/static/src/img/google-calendar-128.png` (7 lines)
- `addons/event/static/src/img/google-calendar.svg` (11 lines)
- `addons/event/static/src/img/how_to_fold_1.png` (50 lines)
- `addons/event/static/src/img/how_to_fold_2.png` (46 lines)
- `addons/event/static/src/img/how_to_fold_3.png` (49 lines)
- `addons/event/static/src/img/how_to_fold_4.png` (352 lines)
- `addons/event/static/src/img/outlook-calendar-128.png` (15 lines)
- `addons/event/static/src/img/outlook-calendar.svg` (20 lines)
- `addons/event/static/src/img/partner_bloem.png` (76 lines)
- `addons/event/static/src/img/partner_pterocarpus.png` (23 lines)
- `addons/event/static/src/img/partner_tree_dealers.png` (86 lines)
- `addons/event/static/src/js/tours/event_steps.js` (9 lines)
- `addons/event/static/src/js/tours/event_tour.js` (104 lines)
- `addons/event/static/src/scss/event.scss` (24 lines)
- `addons/event/static/src/scss/event_badge_report.scss` (75 lines)
- `addons/event/static/src/scss/event_full_page_ticket_report.scss` (84 lines)
- `addons/event/static/src/scss/event_full_page_ticket_report_pdf.scss` (6 lines)
- `addons/event/static/src/scss/event_full_page_ticket_responsive_html_report.scss` (45 lines)
- `addons/event/static/src/template_reference_field/field_event_mail_template_reference.js` (38 lines)
- `addons/event/static/src/template_reference_field/field_event_mail_template_reference.scss` (5 lines)
- `addons/event/static/src/template_reference_field/field_event_mail_template_reference.xml` (14 lines)
- `addons/event/static/src/views/event_registration_kanban_controller.js` (43 lines)
- `addons/event/static/src/views/event_registration_list_controller.js` (43 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_common_renderer.xml` (11 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_controller.js` (140 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_controller.xml` (10 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_model.js` (90 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_renderer.js` (49 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_calendar_view.js` (14 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_multi_selection_buttons.js` (12 lines)
- `addons/event/static/src/views/event_slot/calendar/event_slot_multi_selection_buttons.xml` (10 lines)
- `addons/event/static/src/views/event_slot/list/event_slot_list_controller.js` (29 lines)
- `addons/event/static/src/views/event_slot/list/event_slot_list_view.js` (10 lines)
- `addons/event/tests/__init__.py` (7 lines)
- `addons/event/tests/common.py` (228 lines)
- `addons/event/tests/test_event_internals.py` (1,286 lines)
- `addons/event/tests/test_event_mail_schedule.py` (1,175 lines)

Additional files not expanded here: 18. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
