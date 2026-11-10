# Module: hr_recruitment

- **Module ID:** MOD-094
- **Path:** `addons/hr_recruitment`
- **Manifest:** `addons/hr_recruitment/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Track your recruitment pipeline

No manifest description declared.

Declared dependencies: `hr`, `calendar`, `utm`, `attachment_indexation`, `web_tour`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 40 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 25 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 34 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 18 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "calendar",
    "utm",
    "attachment_indexation",
    "web_tour",
    "digest"
  ],
  "data": [
    "security/hr_recruitment_security.xml",
    "data/digest_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_template_data.xml",
    "data/mail_templates.xml",
    "data/hr_recruitment_data.xml",
    "data/hr_recruitment_tour.xml",
    "views/hr_recruitment_degree_views.xml",
    "views/hr_recruitment_source_views.xml",
    "views/hr_recruitment_stage_views.xml",
    "views/ir_attachment_views.xml",
    "views/hr_applicant_category_views.xml",
    "views/hr_applicant_refuse_reason_views.xml",
    "views/hr_applicant_views.xml",
    "views/hr_talent_pool_views.xml",
    "views/hr_employee_views.xml",
    "views/res_config_settings_views.xml",
    "views/hr_department_views.xml",
    "views/hr_job_views.xml",
    "views/hr_job_tag_views.xml",
    "views/mail_activity_views.xml",
    "views/mail_activity_plan_views.xml",
    "views/digest_views.xml",
    "wizard/applicant_refuse_reason_views.xml",
    "wizard/talent_pool_add_applicants_views.xml",
    "wizard/job_add_applicants_views.xml",
    "views/menuitems.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_recruitment_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_recruitment/static/src/**/*.js",
      "hr_recruitment/static/src/**/*.scss",
      "hr_recruitment/static/src/**/*.xml",
      "hr_recruitment/static/src/js/tours/hr_recruitment.js"
    ],
    "web.assets_unit_tests": [
      "hr_recruitment/static/tests/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "hr_recruitment/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "hr_recruitment/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "hr_recruitment/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_recruitment/README.md` (39 lines)
- `addons/hr_recruitment/__init__.py` (10 lines)
- `addons/hr_recruitment/__manifest__.py` (78 lines)
- `addons/hr_recruitment/data/digest_data.xml` (28 lines)
- `addons/hr_recruitment/data/hr_recruitment_data.xml` (126 lines)
- `addons/hr_recruitment/data/hr_recruitment_demo.xml` (962 lines)
- `addons/hr_recruitment/data/hr_recruitment_demo_jones_cv.pdf` (196 lines)
- `addons/hr_recruitment/data/hr_recruitment_demo_jose_cv.txt` (9 lines)
- `addons/hr_recruitment/data/hr_recruitment_demo_williams_cv.doc` (36 lines)
- `addons/hr_recruitment/data/hr_recruitment_tour.xml` (10 lines)
- `addons/hr_recruitment/data/mail_message_subtype_data.xml` (68 lines)
- `addons/hr_recruitment/data/mail_template_data.xml` (257 lines)
- `addons/hr_recruitment/data/mail_templates.xml` (14 lines)
- `addons/hr_recruitment/data/scenarios/hr_recruitment_scenario.xml` (556 lines)
- `addons/hr_recruitment/i18n/af.po` (3,856 lines)
- `addons/hr_recruitment/i18n/am.po` (3,852 lines)
- `addons/hr_recruitment/i18n/ar.po` (4,463 lines)
- `addons/hr_recruitment/i18n/az.po` (3,931 lines)
- `addons/hr_recruitment/i18n/bg.po` (3,968 lines)
- `addons/hr_recruitment/i18n/bs.po` (3,878 lines)
- `addons/hr_recruitment/i18n/ca.po` (4,495 lines)
- `addons/hr_recruitment/i18n/cs.po` (4,000 lines)
- `addons/hr_recruitment/i18n/da.po` (3,949 lines)
- `addons/hr_recruitment/i18n/de.po` (4,676 lines)
- `addons/hr_recruitment/i18n/el.po` (3,930 lines)
- `addons/hr_recruitment/i18n/es.po` (4,439 lines)
- `addons/hr_recruitment/i18n/es_419.po` (4,660 lines)
- `addons/hr_recruitment/i18n/es_CL.po` (187 lines)
- `addons/hr_recruitment/i18n/et.po` (3,994 lines)
- `addons/hr_recruitment/i18n/eu.po` (3,855 lines)
- `addons/hr_recruitment/i18n/fa.po` (3,970 lines)
- `addons/hr_recruitment/i18n/fi.po` (4,634 lines)
- `addons/hr_recruitment/i18n/fo.po` (3,855 lines)
- `addons/hr_recruitment/i18n/fr.po` (4,613 lines)
- `addons/hr_recruitment/i18n/fr_BE.po` (247 lines)
- `addons/hr_recruitment/i18n/fr_CA.po` (176 lines)
- `addons/hr_recruitment/i18n/gl.po` (3,855 lines)
- `addons/hr_recruitment/i18n/gu.po` (3,872 lines)
- `addons/hr_recruitment/i18n/he.po` (3,928 lines)
- `addons/hr_recruitment/i18n/hi.po` (3,919 lines)
- `addons/hr_recruitment/i18n/hr.po` (3,942 lines)
- `addons/hr_recruitment/i18n/hr_recruitment.pot` (3,779 lines)
- `addons/hr_recruitment/i18n/hu.po` (3,925 lines)
- `addons/hr_recruitment/i18n/id.po` (4,563 lines)
- `addons/hr_recruitment/i18n/is.po` (3,880 lines)
- `addons/hr_recruitment/i18n/it.po` (4,652 lines)
- `addons/hr_recruitment/i18n/ja.po` (4,557 lines)
- `addons/hr_recruitment/i18n/ka.po` (3,855 lines)
- `addons/hr_recruitment/i18n/kab.po` (3,864 lines)
- `addons/hr_recruitment/i18n/km.po` (3,864 lines)
- `addons/hr_recruitment/i18n/ko.po` (4,530 lines)
- `addons/hr_recruitment/i18n/ku.po` (3,880 lines)
- `addons/hr_recruitment/i18n/lb.po` (3,857 lines)
- `addons/hr_recruitment/i18n/lo.po` (4,523 lines)
- `addons/hr_recruitment/i18n/lt.po` (3,938 lines)
- `addons/hr_recruitment/i18n/lv.po` (3,926 lines)
- `addons/hr_recruitment/i18n/mk.po` (3,855 lines)
- `addons/hr_recruitment/i18n/mn.po` (3,951 lines)
- `addons/hr_recruitment/i18n/my.po` (3,892 lines)
- `addons/hr_recruitment/i18n/nb.po` (3,912 lines)
- `addons/hr_recruitment/i18n/nl.po` (4,599 lines)
- `addons/hr_recruitment/i18n/pl.po` (4,047 lines)
- `addons/hr_recruitment/i18n/pt.po` (4,458 lines)
- `addons/hr_recruitment/i18n/pt_BR.po` (4,611 lines)
- `addons/hr_recruitment/i18n/ro.po` (4,033 lines)
- `addons/hr_recruitment/i18n/ru.po` (4,522 lines)
- `addons/hr_recruitment/i18n/sk.po` (3,935 lines)
- `addons/hr_recruitment/i18n/sl.po` (4,015 lines)
- `addons/hr_recruitment/i18n/sq.po` (3,855 lines)
- `addons/hr_recruitment/i18n/sr@latin.po` (3,978 lines)
- `addons/hr_recruitment/i18n/sv.po` (4,437 lines)
- `addons/hr_recruitment/i18n/th.po` (4,515 lines)
- `addons/hr_recruitment/i18n/tr.po` (4,548 lines)
- `addons/hr_recruitment/i18n/uk.po` (3,975 lines)
- `addons/hr_recruitment/i18n/uz.po` (4,572 lines)
- `addons/hr_recruitment/i18n/vi.po` (4,569 lines)
- `addons/hr_recruitment/i18n/zh_CN.po` (4,519 lines)
- `addons/hr_recruitment/i18n/zh_TW.po` (4,261 lines)
- `addons/hr_recruitment/models/__init__.py` (27 lines)
- `addons/hr_recruitment/models/calendar.py` (61 lines)
- `addons/hr_recruitment/models/digest.py` (25 lines)
- `addons/hr_recruitment/models/hr_applicant.py` (1,129 lines)
- `addons/hr_recruitment/models/hr_applicant_category.py` (22 lines)
- `addons/hr_recruitment/models/hr_applicant_refuse_reason.py` (15 lines)
- `addons/hr_recruitment/models/hr_department.py` (35 lines)
- `addons/hr_recruitment/models/hr_employee.py` (52 lines)
- `addons/hr_recruitment/models/hr_job.py` (482 lines)
- `addons/hr_recruitment/models/hr_job_platform.py` (33 lines)
- `addons/hr_recruitment/models/hr_job_tag.py` (16 lines)
- `addons/hr_recruitment/models/hr_recruitment_degree.py` (21 lines)
- `addons/hr_recruitment/models/hr_recruitment_source.py` (61 lines)
- `addons/hr_recruitment/models/hr_recruitment_stage.py` (51 lines)
- `addons/hr_recruitment/models/hr_talent_pool.py` (65 lines)
- `addons/hr_recruitment/models/ir_attachment.py` (19 lines)
- `addons/hr_recruitment/models/ir_ui_menu.py` (22 lines)
- `addons/hr_recruitment/models/mail_activity_plan.py` (13 lines)
- `addons/hr_recruitment/models/res_company.py` (10 lines)
- `addons/hr_recruitment/models/res_config_settings.py` (11 lines)
- `addons/hr_recruitment/models/res_groups.py` (13 lines)
- `addons/hr_recruitment/models/res_partner.py` (7 lines)
- `addons/hr_recruitment/models/res_users.py` (37 lines)
- `addons/hr_recruitment/models/utm_campaign.py` (19 lines)
- `addons/hr_recruitment/models/utm_source.py` (23 lines)
- `addons/hr_recruitment/security/hr_recruitment_security.xml` (45 lines)
- `addons/hr_recruitment/security/ir.access.csv` (40 lines)
- `addons/hr_recruitment/static/applicant_cvs/Cecile_Donth_CV.pdf` (761 lines)
- `addons/hr_recruitment/static/applicant_cvs/David_Armstrong_CV.pdf` (692 lines)
- `addons/hr_recruitment/static/applicant_cvs/David_Billy_CV.pdf` (624 lines)
- `addons/hr_recruitment/static/applicant_cvs/Enrique_Jones_CV.pdf` (511 lines)
- `addons/hr_recruitment/static/applicant_cvs/Hubert_Blank_CV.pdf` (494 lines)
- `addons/hr_recruitment/static/applicant_cvs/Johan_Duck_CV.pdf` (612 lines)
- `addons/hr_recruitment/static/applicant_cvs/John_Bruno_CV.pdf` (672 lines)
- `addons/hr_recruitment/static/applicant_cvs/Joren_Jacob_CV.pdf` (532 lines)
- `addons/hr_recruitment/static/applicant_cvs/Jose_CV.pdf` (409 lines)
- `addons/hr_recruitment/static/applicant_cvs/Kelly_Wallant_CV.pdf` (555 lines)
- `addons/hr_recruitment/static/applicant_cvs/Marie_Justine_CV.pdf` (530 lines)
- `addons/hr_recruitment/static/applicant_cvs/Meldona_Thang_CV.pdf` (226 lines)
- `addons/hr_recruitment/static/applicant_cvs/Ohen_Rizome_CV.pdf` (490 lines)
- `addons/hr_recruitment/static/applicant_cvs/Sandra_Elvis_CV.pdf` (807 lines)
- `addons/hr_recruitment/static/applicant_cvs/Shane_Williams_CV.pdf` (477 lines)
- `addons/hr_recruitment/static/applicant_cvs/Tina_Augustie_CV.pdf` (551 lines)
- `addons/hr_recruitment/static/applicant_cvs/Yin_Lee_CV.pdf` (513 lines)
- `addons/hr_recruitment/static/description/icon.png` (38 lines)
- `addons/hr_recruitment/static/description/icon.svg` (1 lines)
- `addons/hr_recruitment/static/description/icon_hi.png` (130 lines)
- `addons/hr_recruitment/static/src/applicant_char/applicant_char.js` (34 lines)
- `addons/hr_recruitment/static/src/applicant_char/applicant_char.scss` (7 lines)
- `addons/hr_recruitment/static/src/applicant_char/applicant_char.xml` (8 lines)
- `addons/hr_recruitment/static/src/core/common/@types/models.d.ts` (16 lines)
- `addons/hr_recruitment/static/src/core/common/hr_applicant_model.js` (15 lines)
- `addons/hr_recruitment/static/src/core/common/res_partner_model_patch.js` (12 lines)
- `addons/hr_recruitment/static/src/hr_applicant_state_selection/hr_applicant_state_selection.js` (25 lines)
- `addons/hr_recruitment/static/src/img/congratulations.png` (340 lines)
- `addons/hr_recruitment/static/src/js/buttons/generate_content_and_copy_button.js` (22 lines)
- `addons/hr_recruitment/static/src/js/fields/applicant_line_many2many.js` (34 lines)
- `addons/hr_recruitment/static/src/js/fields/recruitment_copy_clipboard_char_field/recruitment_copy_clipboard_char_field.js` (52 lines)
- `addons/hr_recruitment/static/src/js/fields/recruitment_copy_clipboard_char_field/recruitment_copy_clipboard_char_field.xml` (11 lines)
- `addons/hr_recruitment/static/src/js/tours/hr_recruitment.js` (136 lines)
- `addons/hr_recruitment/static/src/scss/hr_applicant.scss` (27 lines)
- `addons/hr_recruitment/static/src/scss/hr_job.scss` (177 lines)
- `addons/hr_recruitment/static/src/scss/hr_recruitment_widgets.scss` (3 lines)
- `addons/hr_recruitment/static/src/scss/job_add_applicants.scss` (6 lines)
- `addons/hr_recruitment/static/src/views/form_view.js` (26 lines)
- `addons/hr_recruitment/static/src/views/recruitment_form_controller.js` (18 lines)
- `addons/hr_recruitment/static/src/views/recruitment_form_view.js` (11 lines)
- `addons/hr_recruitment/static/src/views/recruitment_helper_view.js` (33 lines)
- `addons/hr_recruitment/static/src/views/recruitment_helper_view.xml` (28 lines)
- `addons/hr_recruitment/static/src/views/recruitment_kanban_view.js` (45 lines)
- `addons/hr_recruitment/static/src/views/recruitment_kanban_view.xml` (10 lines)
- `addons/hr_recruitment/static/src/views/recruitment_list_controller.js` (22 lines)
- `addons/hr_recruitment/static/src/views/recruitment_list_view.js` (22 lines)
- `addons/hr_recruitment/static/src/views/recruitment_list_view.xml` (10 lines)
- `addons/hr_recruitment/static/tests/ir_attachments.test.js` (42 lines)
- `addons/hr_recruitment/static/tests/mock_server/mock_models/hr_applicant.js` (13 lines)
- `addons/hr_recruitment/tests/__init__.py` (10 lines)
- `addons/hr_recruitment/tests/resume.eml` (1,604 lines)
- `addons/hr_recruitment/tests/test_recruitment.py` (720 lines)
- `addons/hr_recruitment/tests/test_recruitment_allowed_user_ids.py` (152 lines)
- `addons/hr_recruitment/tests/test_recruitment_interviewer.py` (164 lines)
- `addons/hr_recruitment/tests/test_recruitment_mail.py` (59 lines)

Additional files not expanded here: 28. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
