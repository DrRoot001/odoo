# Module: hr_recruitment_skills

- **Module ID:** MOD-095
- **Path:** `addons/hr_recruitment_skills`
- **Manifest:** `addons/hr_recruitment_skills/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage skills of your employees

No manifest description declared.

Declared dependencies: `hr_skills`, `hr_recruitment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_skills",
    "hr_recruitment"
  ],
  "data": [
    "views/hr_applicant_views.xml",
    "views/hr_applicant_skill_views.xml",
    "views/hr_job_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_recruitment_skills_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_recruitment_skills/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_recruitment_skills/__init__.py` (4 lines)
- `addons/hr_recruitment_skills/__manifest__.py` (26 lines)
- `addons/hr_recruitment_skills/data/hr_recruitment_skills_demo.xml` (92 lines)
- `addons/hr_recruitment_skills/i18n/ar.po` (327 lines)
- `addons/hr_recruitment_skills/i18n/az.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/bg.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/bs.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/ca.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/cs.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/da.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/de.po` (330 lines)
- `addons/hr_recruitment_skills/i18n/el.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/es.po` (330 lines)
- `addons/hr_recruitment_skills/i18n/es_419.po` (329 lines)
- `addons/hr_recruitment_skills/i18n/et.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/fa.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/fi.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/fr.po` (329 lines)
- `addons/hr_recruitment_skills/i18n/he.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/hi.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/hr.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/hr_recruitment_skills.pot` (319 lines)
- `addons/hr_recruitment_skills/i18n/hu.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/id.po` (326 lines)
- `addons/hr_recruitment_skills/i18n/it.po` (327 lines)
- `addons/hr_recruitment_skills/i18n/ja.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/kab.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/ko.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/ku.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/lo.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/lt.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/lv.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/mn.po` (323 lines)
- `addons/hr_recruitment_skills/i18n/my.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/nb.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/nl.po` (327 lines)
- `addons/hr_recruitment_skills/i18n/pl.po` (327 lines)
- `addons/hr_recruitment_skills/i18n/pt.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/pt_BR.po` (328 lines)
- `addons/hr_recruitment_skills/i18n/ro.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/ru.po` (328 lines)
- `addons/hr_recruitment_skills/i18n/sk.po` (322 lines)
- `addons/hr_recruitment_skills/i18n/sl.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/sr@latin.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/sv.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/th.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/tr.po` (327 lines)
- `addons/hr_recruitment_skills/i18n/uk.po` (324 lines)
- `addons/hr_recruitment_skills/i18n/uz.po` (368 lines)
- `addons/hr_recruitment_skills/i18n/vi.po` (325 lines)
- `addons/hr_recruitment_skills/i18n/zh_CN.po` (326 lines)
- `addons/hr_recruitment_skills/i18n/zh_TW.po` (327 lines)
- `addons/hr_recruitment_skills/models/__init__.py` (6 lines)
- `addons/hr_recruitment_skills/models/hr_applicant.py` (236 lines)
- `addons/hr_recruitment_skills/models/hr_applicant_skill.py` (36 lines)
- `addons/hr_recruitment_skills/models/hr_job.py` (103 lines)
- `addons/hr_recruitment_skills/security/ir.access.csv` (8 lines)
- `addons/hr_recruitment_skills/static/src/components/match_scores_gauge/match_scores_gauge.js` (193 lines)
- `addons/hr_recruitment_skills/static/src/components/match_scores_gauge/match_scores_gauge.xml` (19 lines)
- `addons/hr_recruitment_skills/static/src/components/search_job_applicant_menu/search_job_applicant_menu.js` (52 lines)
- `addons/hr_recruitment_skills/static/src/components/search_job_applicant_menu/search_job_applicant_menu.xml` (8 lines)
- `addons/hr_recruitment_skills/static/src/scss/skills_one2many_recruitment.scss` (5 lines)
- `addons/hr_recruitment_skills/tests/__init__.py` (4 lines)
- `addons/hr_recruitment_skills/tests/test_applicant_skills.py` (638 lines)
- `addons/hr_recruitment_skills/tests/test_recruitment_skills.py` (419 lines)
- `addons/hr_recruitment_skills/views/hr_applicant_skill_views.xml` (44 lines)
- `addons/hr_recruitment_skills/views/hr_applicant_views.xml` (198 lines)
- `addons/hr_recruitment_skills/views/hr_job_views.xml` (49 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
