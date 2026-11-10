# Module: website_slides_survey

- **Module ID:** MOD-645
- **Path:** `addons/website_slides_survey`
- **Manifest:** `addons/website_slides_survey/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add certification capabilities to your courses

This module lets you use the full power of certifications within your courses.

Declared dependencies: `website_slides`, `survey`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 21 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_slides",
    "survey"
  ],
  "data": [
    "views/slide_channel_partner_views.xml",
    "views/slide_channel_views.xml",
    "views/slide_slide_partner_views.xml",
    "views/slide_slide_views.xml",
    "views/survey_survey_views.xml",
    "views/website_slides_menu_views.xml",
    "views/website_slides_templates_course.xml",
    "views/website_slides_templates_lesson.xml",
    "views/website_slides_templates_lesson_fullscreen.xml",
    "views/website_slides_templates_homepage.xml",
    "views/website_slides_templates_utils.xml",
    "views/survey_templates.xml",
    "views/website_profile.xml",
    "data/mail_template_data.xml",
    "data/gamification_data.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/survey_demo.xml",
    "data/slide_slide_demo.xml",
    "data/survey.user_input.line.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_slides_survey/static/src/scss/website_slides_survey.scss",
      "website_slides_survey/static/src/interactions/*.js",
      "website_slides_survey/static/src/xml/website_slides_fullscreen.xml",
      "website_slides_survey/static/src/js/public/**/*"
    ],
    "survey.survey_assets": [
      "website_slides_survey/static/src/scss/website_slides_survey_result.scss"
    ]
  }
}
```

### Representative source files

- `addons/website_slides_survey/__init__.py` (10 lines)
- `addons/website_slides_survey/__manifest__.py` (47 lines)
- `addons/website_slides_survey/controllers/__init__.py` (6 lines)
- `addons/website_slides_survey/controllers/slides.py` (163 lines)
- `addons/website_slides_survey/controllers/survey.py` (22 lines)
- `addons/website_slides_survey/controllers/website_profile.py` (37 lines)
- `addons/website_slides_survey/data/gamification_data.xml` (12 lines)
- `addons/website_slides_survey/data/mail_template_data.xml` (31 lines)
- `addons/website_slides_survey/data/slide_slide_demo.xml` (36 lines)
- `addons/website_slides_survey/data/survey.user_input.line.csv` (9 lines)
- `addons/website_slides_survey/data/survey_demo.xml` (124 lines)
- `addons/website_slides_survey/i18n/ar.po` (779 lines)
- `addons/website_slides_survey/i18n/az.po` (693 lines)
- `addons/website_slides_survey/i18n/bg.po` (693 lines)
- `addons/website_slides_survey/i18n/bs.po` (694 lines)
- `addons/website_slides_survey/i18n/ca.po` (775 lines)
- `addons/website_slides_survey/i18n/cs.po` (728 lines)
- `addons/website_slides_survey/i18n/da.po` (784 lines)
- `addons/website_slides_survey/i18n/de.po` (804 lines)
- `addons/website_slides_survey/i18n/el.po` (694 lines)
- `addons/website_slides_survey/i18n/es.po` (793 lines)
- `addons/website_slides_survey/i18n/es_419.po` (792 lines)
- `addons/website_slides_survey/i18n/et.po` (722 lines)
- `addons/website_slides_survey/i18n/fa.po` (722 lines)
- `addons/website_slides_survey/i18n/fi.po` (780 lines)
- `addons/website_slides_survey/i18n/fr.po` (795 lines)
- `addons/website_slides_survey/i18n/he.po` (719 lines)
- `addons/website_slides_survey/i18n/hi.po` (693 lines)
- `addons/website_slides_survey/i18n/hr.po` (701 lines)
- `addons/website_slides_survey/i18n/hu.po` (704 lines)
- `addons/website_slides_survey/i18n/id.po` (784 lines)
- `addons/website_slides_survey/i18n/it.po` (799 lines)
- `addons/website_slides_survey/i18n/ja.po` (775 lines)
- `addons/website_slides_survey/i18n/kab.po` (693 lines)
- `addons/website_slides_survey/i18n/ko.po` (775 lines)
- `addons/website_slides_survey/i18n/ku.po` (693 lines)
- `addons/website_slides_survey/i18n/lo.po` (763 lines)
- `addons/website_slides_survey/i18n/lt.po` (714 lines)
- `addons/website_slides_survey/i18n/lv.po` (693 lines)
- `addons/website_slides_survey/i18n/mn.po` (704 lines)
- `addons/website_slides_survey/i18n/my.po` (694 lines)
- `addons/website_slides_survey/i18n/nb.po` (698 lines)
- `addons/website_slides_survey/i18n/nl.po` (788 lines)
- `addons/website_slides_survey/i18n/pl.po` (738 lines)
- `addons/website_slides_survey/i18n/pt.po` (737 lines)
- `addons/website_slides_survey/i18n/pt_BR.po` (797 lines)
- `addons/website_slides_survey/i18n/ro.po` (787 lines)
- `addons/website_slides_survey/i18n/ru.po` (783 lines)
- `addons/website_slides_survey/i18n/sk.po` (692 lines)
- `addons/website_slides_survey/i18n/sl.po` (694 lines)
- `addons/website_slides_survey/i18n/sr@latin.po` (723 lines)
- `addons/website_slides_survey/i18n/sv.po` (728 lines)
- `addons/website_slides_survey/i18n/th.po` (764 lines)
- `addons/website_slides_survey/i18n/tr.po` (791 lines)
- `addons/website_slides_survey/i18n/uk.po` (728 lines)
- `addons/website_slides_survey/i18n/uz.po` (857 lines)
- `addons/website_slides_survey/i18n/vi.po` (779 lines)
- `addons/website_slides_survey/i18n/website_slides_survey.pot` (676 lines)
- `addons/website_slides_survey/i18n/zh_CN.po` (779 lines)
- `addons/website_slides_survey/i18n/zh_TW.po` (765 lines)
- `addons/website_slides_survey/models/__init__.py` (6 lines)
- `addons/website_slides_survey/models/slide_channel.py` (54 lines)
- `addons/website_slides_survey/models/slide_slide.py` (171 lines)
- `addons/website_slides_survey/models/survey_survey.py` (75 lines)
- `addons/website_slides_survey/models/survey_user.py` (63 lines)
- `addons/website_slides_survey/security/ir.access.csv` (22 lines)
- `addons/website_slides_survey/static/src/img/certification.svg` (1 lines)
- `addons/website_slides_survey/static/src/interactions/slides_course_fullscreen.js` (23 lines)
- `addons/website_slides_survey/static/src/js/public/components/slide_upload_dialog/slide_upload_category.js` (75 lines)
- `addons/website_slides_survey/static/src/js/public/components/slide_upload_dialog/slide_upload_category.xml` (22 lines)
- `addons/website_slides_survey/static/src/js/public/components/slide_upload_dialog/slide_upload_dialog.js` (34 lines)
- `addons/website_slides_survey/static/src/js/public/components/slide_upload_dialog/slide_upload_dialog.xml` (7 lines)
- `addons/website_slides_survey/static/src/scss/website_slides_survey.scss` (31 lines)
- `addons/website_slides_survey/static/src/scss/website_slides_survey_result.scss` (15 lines)
- `addons/website_slides_survey/static/src/xml/website_slides_fullscreen.xml` (26 lines)
- `addons/website_slides_survey/tests/__init__.py` (6 lines)
- `addons/website_slides_survey/tests/test_course_certification_failure.py` (138 lines)
- `addons/website_slides_survey/tests/test_course_certification_stats.py` (61 lines)
- `addons/website_slides_survey/tests/test_course_certification_unlink.py` (41 lines)
- `addons/website_slides_survey/views/res_config_settings_views.xml` (16 lines)
- `addons/website_slides_survey/views/slide_channel_partner_views.xml` (26 lines)
- `addons/website_slides_survey/views/slide_channel_views.xml` (30 lines)
- `addons/website_slides_survey/views/slide_slide_partner_views.xml` (44 lines)
- `addons/website_slides_survey/views/slide_slide_views.xml` (33 lines)
- `addons/website_slides_survey/views/survey_survey_views.xml` (107 lines)
- `addons/website_slides_survey/views/survey_templates.xml` (30 lines)
- `addons/website_slides_survey/views/website_profile.xml` (155 lines)
- `addons/website_slides_survey/views/website_slides_menu_views.xml` (8 lines)
- `addons/website_slides_survey/views/website_slides_templates_course.xml` (39 lines)
- `addons/website_slides_survey/views/website_slides_templates_homepage.xml` (38 lines)
- `addons/website_slides_survey/views/website_slides_templates_lesson.xml` (46 lines)
- `addons/website_slides_survey/views/website_slides_templates_lesson_fullscreen.xml` (12 lines)
- `addons/website_slides_survey/views/website_slides_templates_utils.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
