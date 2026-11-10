# Module: hr_skills_survey

- **Module ID:** MOD-101
- **Path:** `addons/hr_skills_survey`
- **Manifest:** `addons/hr_skills_survey/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add certification to resume of your employees


Certification and Skills for HR
===============================

This module adds certification to resume for employees.
        

Declared dependencies: `hr_skills`, `survey`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_skills",
    "survey"
  ],
  "data": [
    "data/hr_resume_data.xml",
    "views/hr_templates.xml",
    "views/survey_survey_views.xml"
  ],
  "demo": [
    "data/hr_resume_demo.xml"
  ]
}
```

### Representative source files

- `addons/hr_skills_survey/__init__.py` (4 lines)
- `addons/hr_skills_survey/__manifest__.py` (26 lines)
- `addons/hr_skills_survey/data/hr_resume_data.xml` (11 lines)
- `addons/hr_skills_survey/data/hr_resume_demo.xml` (31 lines)
- `addons/hr_skills_survey/i18n/ar.po` (138 lines)
- `addons/hr_skills_survey/i18n/az.po` (131 lines)
- `addons/hr_skills_survey/i18n/bg.po` (131 lines)
- `addons/hr_skills_survey/i18n/bs.po` (132 lines)
- `addons/hr_skills_survey/i18n/ca.po` (132 lines)
- `addons/hr_skills_survey/i18n/cs.po` (138 lines)
- `addons/hr_skills_survey/i18n/da.po` (136 lines)
- `addons/hr_skills_survey/i18n/de.po` (143 lines)
- `addons/hr_skills_survey/i18n/el.po` (132 lines)
- `addons/hr_skills_survey/i18n/es.po` (144 lines)
- `addons/hr_skills_survey/i18n/es_419.po` (140 lines)
- `addons/hr_skills_survey/i18n/et.po` (131 lines)
- `addons/hr_skills_survey/i18n/fa.po` (131 lines)
- `addons/hr_skills_survey/i18n/fi.po` (140 lines)
- `addons/hr_skills_survey/i18n/fr.po` (139 lines)
- `addons/hr_skills_survey/i18n/he.po` (135 lines)
- `addons/hr_skills_survey/i18n/hi.po` (131 lines)
- `addons/hr_skills_survey/i18n/hr.po` (135 lines)
- `addons/hr_skills_survey/i18n/hr_skills_survey.pot` (127 lines)
- `addons/hr_skills_survey/i18n/hu.po` (135 lines)
- `addons/hr_skills_survey/i18n/id.po` (135 lines)
- `addons/hr_skills_survey/i18n/it.po` (143 lines)
- `addons/hr_skills_survey/i18n/ja.po` (133 lines)
- `addons/hr_skills_survey/i18n/kab.po` (131 lines)
- `addons/hr_skills_survey/i18n/ko.po` (134 lines)
- `addons/hr_skills_survey/i18n/ku.po` (131 lines)
- `addons/hr_skills_survey/i18n/lo.po` (137 lines)
- `addons/hr_skills_survey/i18n/lt.po` (137 lines)
- `addons/hr_skills_survey/i18n/lv.po` (131 lines)
- `addons/hr_skills_survey/i18n/mn.po` (135 lines)
- `addons/hr_skills_survey/i18n/my.po` (131 lines)
- `addons/hr_skills_survey/i18n/nb.po` (135 lines)
- `addons/hr_skills_survey/i18n/nl.po` (138 lines)
- `addons/hr_skills_survey/i18n/pl.po` (141 lines)
- `addons/hr_skills_survey/i18n/pt.po` (136 lines)
- `addons/hr_skills_survey/i18n/pt_BR.po` (146 lines)
- `addons/hr_skills_survey/i18n/ro.po` (137 lines)
- `addons/hr_skills_survey/i18n/ru.po` (138 lines)
- `addons/hr_skills_survey/i18n/sk.po` (130 lines)
- `addons/hr_skills_survey/i18n/sl.po` (135 lines)
- `addons/hr_skills_survey/i18n/sr@latin.po` (132 lines)
- `addons/hr_skills_survey/i18n/sv.po` (135 lines)
- `addons/hr_skills_survey/i18n/th.po` (133 lines)
- `addons/hr_skills_survey/i18n/tr.po` (140 lines)
- `addons/hr_skills_survey/i18n/uk.po` (137 lines)
- `addons/hr_skills_survey/i18n/uz.po` (157 lines)
- `addons/hr_skills_survey/i18n/vi.po` (138 lines)
- `addons/hr_skills_survey/i18n/zh_CN.po` (135 lines)
- `addons/hr_skills_survey/i18n/zh_TW.po` (135 lines)
- `addons/hr_skills_survey/models/__init__.py` (6 lines)
- `addons/hr_skills_survey/models/hr_resume_line.py` (27 lines)
- `addons/hr_skills_survey/models/survey_survey.py` (12 lines)
- `addons/hr_skills_survey/models/survey_user.py` (66 lines)
- `addons/hr_skills_survey/tests/__init__.py` (3 lines)
- `addons/hr_skills_survey/tests/test_certification_flow.py` (128 lines)
- `addons/hr_skills_survey/views/hr_templates.xml` (22 lines)
- `addons/hr_skills_survey/views/survey_survey_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
