# Module: hr_skills

- **Module ID:** MOD-098
- **Path:** `addons/hr_skills`
- **Manifest:** `addons/hr_skills/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage skills, knowledge and resume of your employees


Skills and Resume for HR
========================

This module introduces skills and resume management for employees.
        

Declared dependencies: `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 27 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 21 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr"
  ],
  "data": [
    "views/hr_views.xml",
    "views/hr_job_views.xml",
    "views/hr_job_skill_views.xml",
    "data/hr_resume_data.xml",
    "data/hr_skill_data.xml",
    "data/ir_actions_server_data.xml",
    "data/ir_cron_data.xml",
    "data/report_paperformat.xml",
    "report/hr_employee_skill_history_report_views.xml",
    "report/hr_employee_skill_report_views.xml",
    "report/hr_employee_cv_report.xml",
    "views/hr_department_views.xml",
    "views/hr_employee_cv_templates.xml",
    "wizard/hr_employee_cv_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_skill_demo.xml",
    "data/hr_resume_demo.xml",
    "data/hr_job_skill_demo.xml",
    "data/hr.job.skill.csv",
    "data/hr.employee.skill.csv",
    "data/hr_employee_skill_demo.xml",
    "data/hr.resume.line.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_skills/static/src/fields/skills_one2many/*",
      "hr_skills/static/src/fields/**/*",
      "hr_skills/static/src/scss/*.scss",
      "hr_skills/static/src/views/skills_list_renderer.js",
      "hr_skills/static/src/components/**/*",
      "hr_skills/static/src/core/common/**/*",
      "hr_skills/static/src/core/web/**/*"
    ],
    "web.assets_backend_lazy": [
      "hr_skills/static/src/views/skills_graph.js"
    ],
    "im_livechat.assets_embed_core": [
      "hr_skills/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "hr_skills/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "hr_skills/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_skills/static/tests/**/*",
      [
        "remove",
        "hr_skills/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "hr_skills/static/tests/tours/**/*"
    ],
    "web.report_assets_pdf": [
      "/hr_skills/static/src/scss/report_employee_cv.scss"
    ]
  }
}
```

### Representative source files

- `addons/hr_skills/__init__.py` (7 lines)
- `addons/hr_skills/__manifest__.py` (82 lines)
- `addons/hr_skills/controllers/__init__.py` (4 lines)
- `addons/hr_skills/controllers/main.py` (54 lines)
- `addons/hr_skills/data/hr.employee.skill.csv` (111 lines)
- `addons/hr_skills/data/hr.job.skill.csv` (26 lines)
- `addons/hr_skills/data/hr.resume.line.csv` (96 lines)
- `addons/hr_skills/data/hr_employee_skill_demo.xml` (28 lines)
- `addons/hr_skills/data/hr_job_skill_demo.xml` (21 lines)
- `addons/hr_skills/data/hr_resume_data.xml` (21 lines)
- `addons/hr_skills/data/hr_resume_demo.xml` (83 lines)
- `addons/hr_skills/data/hr_skill_data.xml` (260 lines)
- `addons/hr_skills/data/hr_skill_demo.xml` (384 lines)
- `addons/hr_skills/data/ir_actions_server_data.xml` (26 lines)
- `addons/hr_skills/data/ir_cron_data.xml` (11 lines)
- `addons/hr_skills/data/report_paperformat.xml` (16 lines)
- `addons/hr_skills/data/scenarios/hr_skills_scenario.xml` (367 lines)
- `addons/hr_skills/i18n/ar.po` (2,444 lines)
- `addons/hr_skills/i18n/az.po` (2,410 lines)
- `addons/hr_skills/i18n/bg.po` (2,414 lines)
- `addons/hr_skills/i18n/bs.po` (2,407 lines)
- `addons/hr_skills/i18n/ca.po` (2,415 lines)
- `addons/hr_skills/i18n/cs.po` (2,419 lines)
- `addons/hr_skills/i18n/da.po` (2,416 lines)
- `addons/hr_skills/i18n/de.po` (2,481 lines)
- `addons/hr_skills/i18n/el.po` (2,411 lines)
- `addons/hr_skills/i18n/es.po` (2,474 lines)
- `addons/hr_skills/i18n/es_419.po` (2,469 lines)
- `addons/hr_skills/i18n/et.po` (2,416 lines)
- `addons/hr_skills/i18n/fa.po` (2,425 lines)
- `addons/hr_skills/i18n/fi.po` (2,448 lines)
- `addons/hr_skills/i18n/fr.po` (2,468 lines)
- `addons/hr_skills/i18n/he.po` (2,420 lines)
- `addons/hr_skills/i18n/hi.po` (2,408 lines)
- `addons/hr_skills/i18n/hr.po` (2,419 lines)
- `addons/hr_skills/i18n/hr_skills.pot` (2,391 lines)
- `addons/hr_skills/i18n/hu.po` (2,423 lines)
- `addons/hr_skills/i18n/id.po` (2,450 lines)
- `addons/hr_skills/i18n/it.po` (2,471 lines)
- `addons/hr_skills/i18n/ja.po` (2,446 lines)
- `addons/hr_skills/i18n/kab.po` (2,406 lines)
- `addons/hr_skills/i18n/ko.po` (2,438 lines)
- `addons/hr_skills/i18n/ku.po` (2,406 lines)
- `addons/hr_skills/i18n/lo.po` (2,441 lines)
- `addons/hr_skills/i18n/lt.po` (2,422 lines)
- `addons/hr_skills/i18n/lv.po` (2,406 lines)
- `addons/hr_skills/i18n/mn.po` (2,421 lines)
- `addons/hr_skills/i18n/my.po` (2,407 lines)
- `addons/hr_skills/i18n/nb.po` (2,412 lines)
- `addons/hr_skills/i18n/nl.po` (2,466 lines)
- `addons/hr_skills/i18n/pl.po` (2,465 lines)
- `addons/hr_skills/i18n/pt.po` (2,427 lines)
- `addons/hr_skills/i18n/pt_BR.po` (2,473 lines)
- `addons/hr_skills/i18n/ro.po` (2,450 lines)
- `addons/hr_skills/i18n/ru.po` (2,448 lines)
- `addons/hr_skills/i18n/sk.po` (2,405 lines)
- `addons/hr_skills/i18n/sl.po` (2,436 lines)
- `addons/hr_skills/i18n/sr@latin.po` (2,410 lines)
- `addons/hr_skills/i18n/sv.po` (2,442 lines)
- `addons/hr_skills/i18n/th.po` (2,432 lines)
- `addons/hr_skills/i18n/tr.po` (2,459 lines)
- `addons/hr_skills/i18n/uk.po` (2,426 lines)
- `addons/hr_skills/i18n/uz.po` (2,842 lines)
- `addons/hr_skills/i18n/vi.po` (2,442 lines)
- `addons/hr_skills/i18n/zh_CN.po` (2,444 lines)
- `addons/hr_skills/i18n/zh_TW.po` (2,434 lines)
- `addons/hr_skills/models/__init__.py` (14 lines)
- `addons/hr_skills/models/hr_employee.py` (219 lines)
- `addons/hr_skills/models/hr_employee_public.py` (14 lines)
- `addons/hr_skills/models/hr_employee_skill.py` (72 lines)
- `addons/hr_skills/models/hr_individual_skill_mixin.py` (541 lines)
- `addons/hr_skills/models/hr_job.py` (67 lines)
- `addons/hr_skills/models/hr_job_skill.py` (23 lines)
- `addons/hr_skills/models/hr_resume_line.py` (60 lines)
- `addons/hr_skills/models/hr_resume_line_type.py` (15 lines)
- `addons/hr_skills/models/hr_skill.py` (23 lines)
- `addons/hr_skills/models/hr_skill_level.py` (45 lines)
- `addons/hr_skills/models/hr_skill_type.py` (72 lines)
- `addons/hr_skills/models/resource_resource.py` (9 lines)
- `addons/hr_skills/report/__init__.py` (5 lines)
- `addons/hr_skills/report/hr_employee_cv_report.py` (29 lines)
- `addons/hr_skills/report/hr_employee_cv_report.xml` (13 lines)
- `addons/hr_skills/report/hr_employee_skill_history_report.py` (69 lines)
- `addons/hr_skills/report/hr_employee_skill_history_report_views.xml` (28 lines)
- `addons/hr_skills/report/hr_employee_skill_report.py` (53 lines)
- `addons/hr_skills/report/hr_employee_skill_report_views.xml` (94 lines)
- `addons/hr_skills/security/ir.access.csv` (23 lines)
- `addons/hr_skills/static/description/icon.png` (23 lines)
- `addons/hr_skills/static/description/icon.svg` (1 lines)
- `addons/hr_skills/static/description/icon_hi.png` (64 lines)
- `addons/hr_skills/static/src/components/internal_resume_lines/internal_resume_one2many.js` (57 lines)
- `addons/hr_skills/static/src/components/internal_resume_lines/internal_resume_one2many.scss` (54 lines)
- `addons/hr_skills/static/src/components/internal_resume_lines/internal_resume_one2many.xml` (54 lines)
- `addons/hr_skills/static/src/core/common/hr_employee_model_patch.js` (10 lines)
- `addons/hr_skills/static/src/core/common/hr_employee_public_model_patch.js` (10 lines)
- `addons/hr_skills/static/src/core/common/hr_employee_skill_model.js` (14 lines)
- `addons/hr_skills/static/src/core/web/avatar_card/avatar_card_patch.js` (25 lines)
- `addons/hr_skills/static/src/core/web/avatar_card/avatar_card_patch.xml` (15 lines)
- `addons/hr_skills/static/src/fields/boolean_toggle_load/boolean_toggle_load.js` (21 lines)
- `addons/hr_skills/static/src/fields/form_view_one2many/form_view_one2many.xml` (11 lines)
- `addons/hr_skills/static/src/fields/formatted_date/formatted_date.js` (79 lines)
- `addons/hr_skills/static/src/fields/formatted_date/formatted_date.xml` (7 lines)
- `addons/hr_skills/static/src/fields/many2many_tags_skills/many2many_tags_skills.js` (39 lines)
- `addons/hr_skills/static/src/fields/many2many_tags_skills/many2many_tags_skills.xml` (10 lines)
- `addons/hr_skills/static/src/fields/one2many_tags_skills/one2many_tags_skills.js` (61 lines)
- `addons/hr_skills/static/src/fields/one2many_tags_skills/one2many_tags_skills.scss` (3 lines)
- `addons/hr_skills/static/src/fields/one2many_tags_skills/one2many_tags_skills.xml` (20 lines)
- `addons/hr_skills/static/src/fields/resume_one2many/resume_one2many.js` (66 lines)
- `addons/hr_skills/static/src/fields/resume_one2many/resume_one2many.scss` (58 lines)
- `addons/hr_skills/static/src/fields/resume_one2many/resume_one2many.xml` (69 lines)
- `addons/hr_skills/static/src/fields/skills_one2many/skills_one2many.js` (124 lines)
- `addons/hr_skills/static/src/fields/skills_one2many/skills_one2many.scss` (52 lines)
- `addons/hr_skills/static/src/fields/skills_one2many/skills_one2many.xml` (64 lines)
- `addons/hr_skills/static/src/scss/hr_employee.scss` (20 lines)
- `addons/hr_skills/static/src/scss/report_employee_cv.scss` (242 lines)
- `addons/hr_skills/static/src/views/skills_graph.js` (22 lines)
- `addons/hr_skills/static/src/views/skills_list_renderer.js` (56 lines)
- `addons/hr_skills/static/tests/hr_skills_test_helpers.js` (16 lines)
- `addons/hr_skills/static/tests/many2one_avatar_employee.test.js` (53 lines)
- `addons/hr_skills/static/tests/mock_server/mock_models/hr_employee.js` (10 lines)
- `addons/hr_skills/static/tests/mock_server/mock_models/hr_employee_skill.js` (5 lines)
- `addons/hr_skills/static/tests/mock_server/mock_models/hr_skill.js` (5 lines)
- `addons/hr_skills/static/tests/mock_server/mock_models/m2o_avatar_employee.js` (7 lines)
- `addons/hr_skills/static/tests/tours/skills_tour.js` (174 lines)
- `addons/hr_skills/static/tests/tours/skills_type_tours.js` (86 lines)
- `addons/hr_skills/tests/__init__.py` (7 lines)
- `addons/hr_skills/tests/test_certification_activities.py` (277 lines)
- `addons/hr_skills/tests/test_employee_skill.py` (555 lines)
- `addons/hr_skills/tests/test_report.py` (52 lines)
- `addons/hr_skills/tests/test_resource.py` (49 lines)
- `addons/hr_skills/tests/test_ui.py` (43 lines)
- `addons/hr_skills/views/hr_department_views.xml` (17 lines)
- `addons/hr_skills/views/hr_employee_cv_templates.xml` (150 lines)
- `addons/hr_skills/views/hr_job_skill_views.xml` (27 lines)
- `addons/hr_skills/views/hr_job_views.xml` (38 lines)
- `addons/hr_skills/views/hr_views.xml` (629 lines)
- `addons/hr_skills/wizard/__init__.py` (4 lines)
- `addons/hr_skills/wizard/hr_employee_cv_wizard.py` (44 lines)
- `addons/hr_skills/wizard/hr_employee_cv_wizard_views.xml` (38 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
