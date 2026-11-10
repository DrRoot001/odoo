# Module: hr_recruitment_survey

- **Module ID:** MOD-097
- **Path:** `addons/hr_recruitment_survey`
- **Manifest:** `addons/hr_recruitment_survey/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Surveys


Use interview forms during recruitment process.
This module is integrated with the survey module
to allow you to define interviews for different jobs.
    

Declared dependencies: `survey`, `hr_recruitment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "survey",
    "hr_recruitment"
  ],
  "data": [
    "data/mail_template_data.xml",
    "views/hr_job_views.xml",
    "views/hr_applicant_views.xml",
    "views/survey_survey_views.xml",
    "views/res_config_setting_views.xml",
    "views/survey_templates_statistics.xml",
    "wizard/survey_invite_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/survey_demo.xml",
    "data/hr_job_demo.xml"
  ]
}
```

### Representative source files

- `addons/hr_recruitment_survey/README.md` (6 lines)
- `addons/hr_recruitment_survey/__init__.py` (5 lines)
- `addons/hr_recruitment_survey/__manifest__.py` (27 lines)
- `addons/hr_recruitment_survey/controllers/__init__.py` (3 lines)
- `addons/hr_recruitment_survey/controllers/main.py` (12 lines)
- `addons/hr_recruitment_survey/data/hr_job_demo.xml` (26 lines)
- `addons/hr_recruitment_survey/data/mail_template_data.xml` (38 lines)
- `addons/hr_recruitment_survey/data/survey_demo.xml` (144 lines)
- `addons/hr_recruitment_survey/i18n/af.po` (657 lines)
- `addons/hr_recruitment_survey/i18n/ar.po` (750 lines)
- `addons/hr_recruitment_survey/i18n/az.po` (680 lines)
- `addons/hr_recruitment_survey/i18n/bg.po` (689 lines)
- `addons/hr_recruitment_survey/i18n/bs.po` (690 lines)
- `addons/hr_recruitment_survey/i18n/ca.po` (786 lines)
- `addons/hr_recruitment_survey/i18n/cs.po` (786 lines)
- `addons/hr_recruitment_survey/i18n/da.po` (789 lines)
- `addons/hr_recruitment_survey/i18n/de.po` (772 lines)
- `addons/hr_recruitment_survey/i18n/el.po` (678 lines)
- `addons/hr_recruitment_survey/i18n/es.po` (793 lines)
- `addons/hr_recruitment_survey/i18n/es_419.po` (753 lines)
- `addons/hr_recruitment_survey/i18n/et.po` (715 lines)
- `addons/hr_recruitment_survey/i18n/fa.po` (714 lines)
- `addons/hr_recruitment_survey/i18n/fi.po` (793 lines)
- `addons/hr_recruitment_survey/i18n/fr.po` (764 lines)
- `addons/hr_recruitment_survey/i18n/gu.po` (659 lines)
- `addons/hr_recruitment_survey/i18n/he.po` (696 lines)
- `addons/hr_recruitment_survey/i18n/hi.po` (790 lines)
- `addons/hr_recruitment_survey/i18n/hr.po` (709 lines)
- `addons/hr_recruitment_survey/i18n/hr_recruitment_survey.pot` (644 lines)
- `addons/hr_recruitment_survey/i18n/hu.po` (688 lines)
- `addons/hr_recruitment_survey/i18n/id.po` (763 lines)
- `addons/hr_recruitment_survey/i18n/is.po` (653 lines)
- `addons/hr_recruitment_survey/i18n/it.po` (756 lines)
- `addons/hr_recruitment_survey/i18n/ja.po` (748 lines)
- `addons/hr_recruitment_survey/i18n/kab.po` (671 lines)
- `addons/hr_recruitment_survey/i18n/km.po` (656 lines)
- `addons/hr_recruitment_survey/i18n/ko.po` (753 lines)
- `addons/hr_recruitment_survey/i18n/ku.po` (666 lines)
- `addons/hr_recruitment_survey/i18n/lo.po` (742 lines)
- `addons/hr_recruitment_survey/i18n/lt.po` (697 lines)
- `addons/hr_recruitment_survey/i18n/lv.po` (757 lines)
- `addons/hr_recruitment_survey/i18n/mn.po` (726 lines)
- `addons/hr_recruitment_survey/i18n/my.po` (671 lines)
- `addons/hr_recruitment_survey/i18n/nb.po` (681 lines)
- `addons/hr_recruitment_survey/i18n/nl.po` (761 lines)
- `addons/hr_recruitment_survey/i18n/pl.po` (796 lines)
- `addons/hr_recruitment_survey/i18n/pt.po` (720 lines)
- `addons/hr_recruitment_survey/i18n/pt_BR.po` (768 lines)
- `addons/hr_recruitment_survey/i18n/ro.po` (792 lines)
- `addons/hr_recruitment_survey/i18n/ru.po` (790 lines)
- `addons/hr_recruitment_survey/i18n/sk.po` (699 lines)
- `addons/hr_recruitment_survey/i18n/sl.po` (702 lines)
- `addons/hr_recruitment_survey/i18n/sr@latin.po` (681 lines)
- `addons/hr_recruitment_survey/i18n/sv.po` (786 lines)
- `addons/hr_recruitment_survey/i18n/th.po` (770 lines)
- `addons/hr_recruitment_survey/i18n/tr.po` (796 lines)
- `addons/hr_recruitment_survey/i18n/uk.po` (720 lines)
- `addons/hr_recruitment_survey/i18n/uz.po` (789 lines)
- `addons/hr_recruitment_survey/i18n/vi.po` (774 lines)
- `addons/hr_recruitment_survey/i18n/zh_CN.po` (775 lines)
- `addons/hr_recruitment_survey/i18n/zh_TW.po` (771 lines)
- `addons/hr_recruitment_survey/models/__init__.py` (7 lines)
- `addons/hr_recruitment_survey/models/hr_applicant.py` (98 lines)
- `addons/hr_recruitment_survey/models/hr_job.py` (33 lines)
- `addons/hr_recruitment_survey/models/survey_survey.py` (70 lines)
- `addons/hr_recruitment_survey/models/survey_user_input.py` (17 lines)
- `addons/hr_recruitment_survey/security/ir.access.csv` (42 lines)
- `addons/hr_recruitment_survey/tests/__init__.py` (8 lines)
- `addons/hr_recruitment_survey/tests/recruitment_survey_common.py` (79 lines)
- `addons/hr_recruitment_survey/tests/test_recruitment_survey.py` (190 lines)
- `addons/hr_recruitment_survey/tests/test_recruitment_survey_link_expiration.py` (76 lines)
- `addons/hr_recruitment_survey/tests/test_recruitment_survey_link_permissions.py` (98 lines)
- `addons/hr_recruitment_survey/views/hr_applicant_views.xml` (71 lines)
- `addons/hr_recruitment_survey/views/hr_job_views.xml` (38 lines)
- `addons/hr_recruitment_survey/views/res_config_setting_views.xml` (17 lines)
- `addons/hr_recruitment_survey/views/survey_survey_views.xml` (99 lines)
- `addons/hr_recruitment_survey/views/survey_templates_statistics.xml` (14 lines)
- `addons/hr_recruitment_survey/wizard/__init__.py` (3 lines)
- `addons/hr_recruitment_survey/wizard/hr_recruitment_survey_invite.py` (301 lines)
- `addons/hr_recruitment_survey/wizard/survey_invite_views.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
