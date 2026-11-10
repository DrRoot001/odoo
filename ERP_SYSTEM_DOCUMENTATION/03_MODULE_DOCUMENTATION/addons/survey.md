# Module: survey

- **Module ID:** MOD-567
- **Path:** `addons/survey`
- **Manifest:** `addons/survey/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Send your surveys or share them live.


Create beautiful surveys and visualize answers
==============================================

It depends on the answers or reviews of some questions by different users. A
survey may have multiple pages. Each page may contain multiple questions and
each question may have multiple answers. Different users may give different
answers of question and according to that survey is done. Partners are also
sent mails with personal token for the invitation of the survey.
    

Declared dependencies: `auth_signup`, `http_routing`, `mail`, `web_tour`, `gamification`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 37 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 39 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 46 | Client behavior/assets. |
| Tests | 18 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 23 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_signup",
    "http_routing",
    "mail",
    "web_tour",
    "gamification",
    "digest"
  ],
  "data": [
    "report/survey_templates.xml",
    "report/survey_reports.xml",
    "data/digest_data.xml",
    "data/ir_actions_server_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_template_data.xml",
    "data/survey_tour.xml",
    "security/survey_security.xml",
    "views/digest_views.xml",
    "views/survey_menus.xml",
    "views/survey_survey_views.xml",
    "views/survey_user_views.xml",
    "views/survey_question_views.xml",
    "views/survey_templates.xml",
    "views/survey_templates_management.xml",
    "views/survey_templates_print.xml",
    "views/survey_templates_statistics.xml",
    "views/survey_templates_user_input_session.xml",
    "views/gamification_badge_views.xml",
    "wizard/survey_invite_views.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/gamification_badge_demo.xml",
    "data/res_users_demo.xml",
    "data/survey_demo_feedback.xml",
    "data/survey_demo_feedback_user_input.xml",
    "data/survey_demo_feedback_user_input_line.xml",
    "data/survey_demo_certification.xml",
    "data/survey_demo_certification_user_input.xml",
    "data/survey_demo_certification_user_input_line.xml",
    "data/survey_demo_conditional.xml"
  ],
  "assets": {
    "survey.survey_assets": [
      [
        "include",
        "web.chartjs_lib"
      ],
      "survey/static/src/utils.js",
      "/survey/static/src/interactions/survey_image_zoomer_templates.xml",
      "survey/static/src/js/survey_preload_image_mixin.js",
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_frontend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      "survey/static/src/scss/survey_templates_form.scss",
      "survey/static/src/scss/survey_templates_results.scss",
      "survey/static/src/interactions/survey_breadcrumb_templates.xml",
      "survey/static/src/xml/survey_paginated_results_rows_template.xml",
      "survey/static/src/interactions/*"
    ],
    "survey.survey_user_input_session_assets": [
      "survey/static/src/interactions/utils.js",
      "survey/static/src/interactions/survey_session_chart.js",
      "survey/static/src/interactions/survey_session_text_answers.js",
      "survey/static/src/interactions/survey_session_leaderboard.js",
      "survey/static/src/interactions/survey_session_manage.js",
      "survey/static/src/xml/survey_session_text_answer_template.xml"
    ],
    "web.report_assets_common": [
      "survey/static/src/scss/survey_reports.scss"
    ],
    "web.assets_backend": [
      "survey/static/src/question_page/*",
      "survey/static/src/views/**/*.js",
      "survey/static/src/views/**/*.xml",
      "survey/static/src/scss/survey_survey_views.scss",
      "survey/static/src/scss/survey_question_views.scss",
      "survey/static/src/js/tours/survey_tour.js"
    ],
    "web.assets_web_dark": [
      "survey/static/src/scss/*.dark.scss"
    ],
    "web.assets_tests": [
      "survey/static/tests/tours/*.js"
    ],
    "web.assets_unit_tests": [
      "survey/static/tests/components/*.test.js",
      "survey/static/tests/fields/*.test.js"
    ],
    "web.assets_frontend": [
      "survey/static/src/js/tours/survey_tour.js"
    ]
  }
}
```

### Representative source files

- `addons/survey/__init__.py` (7 lines)
- `addons/survey/__manifest__.py` (116 lines)
- `addons/survey/controllers/__init__.py` (5 lines)
- `addons/survey/controllers/main.py` (950 lines)
- `addons/survey/controllers/survey_session_manage.py` (272 lines)
- `addons/survey/data/digest_data.xml` (9 lines)
- `addons/survey/data/gamification_badge_demo.xml` (11 lines)
- `addons/survey/data/ir_actions_server_data.xml` (14 lines)
- `addons/survey/data/mail_message_subtype_data.xml` (20 lines)
- `addons/survey/data/mail_template_data.xml` (92 lines)
- `addons/survey/data/res_users_demo.xml` (12 lines)
- `addons/survey/data/survey_demo_certification.xml` (367 lines)
- `addons/survey/data/survey_demo_certification_user_input.xml` (37 lines)
- `addons/survey/data/survey_demo_certification_user_input_line.xml` (429 lines)
- `addons/survey/data/survey_demo_conditional.xml` (557 lines)
- `addons/survey/data/survey_demo_feedback.xml` (199 lines)
- `addons/survey/data/survey_demo_feedback_user_input.xml` (29 lines)
- `addons/survey/data/survey_demo_feedback_user_input_line.xml` (246 lines)
- `addons/survey/data/survey_tour.xml` (10 lines)
- `addons/survey/i18n/af.po` (5,255 lines)
- `addons/survey/i18n/ar.po` (5,541 lines)
- `addons/survey/i18n/az.po` (5,271 lines)
- `addons/survey/i18n/bg.po` (5,307 lines)
- `addons/survey/i18n/bs.po` (5,269 lines)
- `addons/survey/i18n/ca.po` (5,573 lines)
- `addons/survey/i18n/cs.po` (5,551 lines)
- `addons/survey/i18n/da.po` (5,380 lines)
- `addons/survey/i18n/de.po` (5,712 lines)
- `addons/survey/i18n/el.po` (5,276 lines)
- `addons/survey/i18n/es.po` (5,643 lines)
- `addons/survey/i18n/es_419.po` (5,683 lines)
- `addons/survey/i18n/es_CL.po` (183 lines)
- `addons/survey/i18n/et.po` (5,430 lines)
- `addons/survey/i18n/fa.po` (5,447 lines)
- `addons/survey/i18n/fi.po` (5,635 lines)
- `addons/survey/i18n/fr.po` (5,670 lines)
- `addons/survey/i18n/gl.po` (5,253 lines)
- `addons/survey/i18n/gu.po` (5,271 lines)
- `addons/survey/i18n/he.po` (5,313 lines)
- `addons/survey/i18n/hi.po` (5,274 lines)
- `addons/survey/i18n/hr.po` (5,309 lines)
- `addons/survey/i18n/hu.po` (5,305 lines)
- `addons/survey/i18n/id.po` (5,676 lines)
- `addons/survey/i18n/is.po` (5,261 lines)
- `addons/survey/i18n/it.po` (5,683 lines)
- `addons/survey/i18n/ja.po` (5,595 lines)
- `addons/survey/i18n/ka.po` (5,253 lines)
- `addons/survey/i18n/kab.po` (5,261 lines)
- `addons/survey/i18n/km.po` (5,264 lines)
- `addons/survey/i18n/ko.po` (5,552 lines)
- `addons/survey/i18n/ku.po` (5,271 lines)
- `addons/survey/i18n/lo.po` (5,519 lines)
- `addons/survey/i18n/lt.po` (5,337 lines)
- `addons/survey/i18n/lv.po` (5,357 lines)
- `addons/survey/i18n/mk.po` (5,260 lines)
- `addons/survey/i18n/mn.po` (5,295 lines)
- `addons/survey/i18n/my.po` (5,263 lines)
- `addons/survey/i18n/nb.po` (5,284 lines)
- `addons/survey/i18n/nl.po` (5,670 lines)
- `addons/survey/i18n/pl.po` (5,547 lines)
- `addons/survey/i18n/pt.po` (5,484 lines)
- `addons/survey/i18n/pt_BR.po` (5,662 lines)
- `addons/survey/i18n/ro.po` (5,631 lines)
- `addons/survey/i18n/ru.po` (5,614 lines)
- `addons/survey/i18n/sk.po` (5,301 lines)
- `addons/survey/i18n/sl.po` (5,298 lines)
- `addons/survey/i18n/sr@latin.po` (5,273 lines)
- `addons/survey/i18n/survey.pot` (5,224 lines)
- `addons/survey/i18n/sv.po` (5,529 lines)
- `addons/survey/i18n/th.po` (5,498 lines)
- `addons/survey/i18n/tr.po` (5,619 lines)
- `addons/survey/i18n/uk.po` (5,433 lines)
- `addons/survey/i18n/uz.po` (6,411 lines)
- `addons/survey/i18n/vi.po` (5,606 lines)
- `addons/survey/i18n/zh_CN.po` (5,528 lines)
- `addons/survey/i18n/zh_TW.po` (5,485 lines)
- `addons/survey/models/__init__.py` (13 lines)
- `addons/survey/models/badge.py` (16 lines)
- `addons/survey/models/challenge.py` (12 lines)
- `addons/survey/models/digest.py` (44 lines)
- `addons/survey/models/ir_http.py` (37 lines)
- `addons/survey/models/res_lang.py` (27 lines)
- `addons/survey/models/res_partner.py` (32 lines)
- `addons/survey/models/survey_question.py` (942 lines)
- `addons/survey/models/survey_survey.py` (1,327 lines)
- `addons/survey/models/survey_user_input.py` (907 lines)
- `addons/survey/models/templates/__init__.py` (1 lines)
- `addons/survey/models/templates/survey_survey.py` (302 lines)
- `addons/survey/report/survey_reports.xml` (32 lines)
- `addons/survey/report/survey_templates.xml` (152 lines)
- `addons/survey/security/ir.access.csv` (31 lines)
- `addons/survey/security/survey_security.xml` (26 lines)
- `addons/survey/static/description/icon.png` (14 lines)
- `addons/survey/static/description/icon.svg` (1 lines)
- `addons/survey/static/description/icon_hi.png` (57 lines)
- `addons/survey/static/src/img/burger_quiz_background.txt` (10 lines)
- `addons/survey/static/src/img/burger_quiz_background.webp` (317 lines)
- `addons/survey/static/src/img/burger_quiz_cubism_klein.jpg` (407 lines)
- `addons/survey/static/src/img/burger_quiz_don_quixote.jpg` (340 lines)
- `addons/survey/static/src/img/burger_quiz_guernica.jpg` (303 lines)
- `addons/survey/static/src/img/burger_quiz_self_portrait.jpg` (132 lines)
- `addons/survey/static/src/img/certification_classic-1_bg.svg` (5 lines)
- `addons/survey/static/src/img/certification_classic-2_bg.svg` (8 lines)
- `addons/survey/static/src/img/certification_minimal_number_bg.svg` (7 lines)
- `addons/survey/static/src/img/certification_modern_bg.svg` (53 lines)
- `addons/survey/static/src/img/classic-seal.png` (365 lines)
- `addons/survey/static/src/img/survey_background_2.webp` (691 lines)
- `addons/survey/static/src/img/survey_background_sample.svg` (4 lines)
- `addons/survey/static/src/img/survey_sample_assessment.png` (128 lines)
- `addons/survey/static/src/img/survey_sample_live_session.png` (154 lines)
- `addons/survey/static/src/img/survey_sample_survey.png` (144 lines)
- `addons/survey/static/src/img/watermark.png` (571 lines)
- `addons/survey/static/src/interactions/survey_breadcrumb_templates.xml` (34 lines)
- `addons/survey/static/src/interactions/survey_enter_tooltip.js` (58 lines)
- `addons/survey/static/src/interactions/survey_form.js` (1,524 lines)
- `addons/survey/static/src/interactions/survey_image_zoomer.js` (88 lines)
- `addons/survey/static/src/interactions/survey_image_zoomer_templates.xml` (27 lines)
- `addons/survey/static/src/interactions/survey_print.js` (24 lines)
- `addons/survey/static/src/interactions/survey_quick_access.js` (73 lines)
- `addons/survey/static/src/interactions/survey_result.js` (168 lines)
- `addons/survey/static/src/interactions/survey_result_chart.js` (356 lines)
- `addons/survey/static/src/interactions/survey_result_pagination.js` (116 lines)
- `addons/survey/static/src/interactions/survey_session_chart.js` (366 lines)
- `addons/survey/static/src/interactions/survey_session_leaderboard.js` (322 lines)
- `addons/survey/static/src/interactions/survey_session_manage.js` (717 lines)
- `addons/survey/static/src/interactions/survey_session_text_answers.js` (67 lines)
- `addons/survey/static/src/interactions/survey_timer.js` (96 lines)
- `addons/survey/static/src/interactions/utils.js` (28 lines)
- `addons/survey/static/src/js/libs/chartjs-plugin-datalabels.js` (1,356 lines)
- `addons/survey/static/src/js/survey_preload_image_mixin.js` (26 lines)
- `addons/survey/static/src/js/tours/survey_tour.js` (78 lines)
- `addons/survey/static/src/question_page/description_page_field.js` (26 lines)
- `addons/survey/static/src/question_page/description_page_field.xml` (25 lines)
- `addons/survey/static/src/question_page/question_page_list_renderer.js` (139 lines)
- `addons/survey/static/src/question_page/question_page_one2many_field.js` (111 lines)
- `addons/survey/static/src/scss/survey_question_views.scss` (15 lines)
- `addons/survey/static/src/scss/survey_reports.scss` (98 lines)
- `addons/survey/static/src/scss/survey_survey_views.dark.scss` (11 lines)
- `addons/survey/static/src/scss/survey_survey_views.scss` (161 lines)
- `addons/survey/static/src/scss/survey_templates_form.scss` (361 lines)
- `addons/survey/static/src/scss/survey_templates_results.scss` (86 lines)
- `addons/survey/static/src/utils.js` (53 lines)
- `addons/survey/static/src/views/components/survey_survey_action_helper/survey_survey_action_helper.js` (37 lines)
- `addons/survey/static/src/views/components/survey_survey_action_helper/survey_survey_action_helper.xml` (36 lines)
- `addons/survey/static/src/views/form/survey_invite_form_controller.js` (25 lines)
- `addons/survey/static/src/views/kanban/kanban_record.js` (16 lines)
- `addons/survey/static/src/views/kanban/kanban_renderer.js` (12 lines)
- `addons/survey/static/src/views/kanban/kanban_renderer.xml` (16 lines)
- `addons/survey/static/src/views/kanban/kanban_view.js` (10 lines)
- `addons/survey/static/src/views/list/list_renderer.js` (10 lines)
- `addons/survey/static/src/views/list/list_renderer.xml` (10 lines)
- `addons/survey/static/src/views/list/list_view.js` (10 lines)
- `addons/survey/static/src/views/widgets/boolean_update_flag_field/boolean_update_flag_fields.js` (52 lines)
- `addons/survey/static/src/views/widgets/integer_update_flag_field/integer_update_flag_fields.js` (54 lines)
- `addons/survey/static/src/views/widgets/radio_selection_with_filter/radio_selection_field_with_filter.js` (31 lines)
- `addons/survey/static/src/views/widgets/survey_question_trigger/survey_question_trigger.js` (120 lines)
- `addons/survey/static/src/views/widgets/survey_question_trigger/survey_question_trigger.xml` (15 lines)
- `addons/survey/static/src/xml/survey_paginated_results_rows_template.xml` (32 lines)
- `addons/survey/static/src/xml/survey_session_text_answer_template.xml` (11 lines)
- `addons/survey/static/tests/components/description_page_field.test.js` (75 lines)

Additional files not expanded here: 46. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
