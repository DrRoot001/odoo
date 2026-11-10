# Module: hr_skills_slides

- **Module ID:** MOD-100
- **Path:** `addons/hr_skills_slides`
- **Manifest:** `addons/hr_skills_slides/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add completed courses to resume of your employees


E-learning and Skills for HR
============================

This module add completed courses to resume for employees.
        

Declared dependencies: `hr_skills`, `website_slides`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
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
    "website_slides"
  ],
  "data": [
    "views/hr_employee_views.xml",
    "views/hr_employee_public_views.xml",
    "views/hr_resume_line_views.xml",
    "views/slide_channel_views.xml",
    "views/hr_views.xml"
  ],
  "demo": [
    "data/hr_resume_line_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_skills_slides/static/src/scss/**/*",
      "hr_skills_slides/static/src/fields/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_skills_slides/__init__.py` (4 lines)
- `addons/hr_skills_slides/__manifest__.py` (34 lines)
- `addons/hr_skills_slides/data/hr_resume_line_demo.xml` (40 lines)
- `addons/hr_skills_slides/i18n/ar.po` (224 lines)
- `addons/hr_skills_slides/i18n/az.po` (217 lines)
- `addons/hr_skills_slides/i18n/bg.po` (217 lines)
- `addons/hr_skills_slides/i18n/bs.po` (228 lines)
- `addons/hr_skills_slides/i18n/ca.po` (220 lines)
- `addons/hr_skills_slides/i18n/cs.po` (224 lines)
- `addons/hr_skills_slides/i18n/da.po` (227 lines)
- `addons/hr_skills_slides/i18n/de.po` (240 lines)
- `addons/hr_skills_slides/i18n/el.po` (218 lines)
- `addons/hr_skills_slides/i18n/es.po` (238 lines)
- `addons/hr_skills_slides/i18n/es_419.po` (232 lines)
- `addons/hr_skills_slides/i18n/et.po` (217 lines)
- `addons/hr_skills_slides/i18n/fa.po` (217 lines)
- `addons/hr_skills_slides/i18n/fi.po` (234 lines)
- `addons/hr_skills_slides/i18n/fr.po` (234 lines)
- `addons/hr_skills_slides/i18n/he.po` (223 lines)
- `addons/hr_skills_slides/i18n/hi.po` (218 lines)
- `addons/hr_skills_slides/i18n/hr.po` (221 lines)
- `addons/hr_skills_slides/i18n/hr_skills_slides.pot` (213 lines)
- `addons/hr_skills_slides/i18n/hu.po` (223 lines)
- `addons/hr_skills_slides/i18n/id.po` (232 lines)
- `addons/hr_skills_slides/i18n/it.po` (237 lines)
- `addons/hr_skills_slides/i18n/ja.po` (225 lines)
- `addons/hr_skills_slides/i18n/kab.po` (222 lines)
- `addons/hr_skills_slides/i18n/ko.po` (219 lines)
- `addons/hr_skills_slides/i18n/ku.po` (217 lines)
- `addons/hr_skills_slides/i18n/lo.po` (229 lines)
- `addons/hr_skills_slides/i18n/lt.po` (225 lines)
- `addons/hr_skills_slides/i18n/lv.po` (225 lines)
- `addons/hr_skills_slides/i18n/mn.po` (221 lines)
- `addons/hr_skills_slides/i18n/my.po` (217 lines)
- `addons/hr_skills_slides/i18n/nb.po` (222 lines)
- `addons/hr_skills_slides/i18n/nl.po` (233 lines)
- `addons/hr_skills_slides/i18n/pl.po` (236 lines)
- `addons/hr_skills_slides/i18n/pt.po` (223 lines)
- `addons/hr_skills_slides/i18n/pt_BR.po` (238 lines)
- `addons/hr_skills_slides/i18n/ro.po` (226 lines)
- `addons/hr_skills_slides/i18n/ru.po` (231 lines)
- `addons/hr_skills_slides/i18n/sk.po` (232 lines)
- `addons/hr_skills_slides/i18n/sl.po` (219 lines)
- `addons/hr_skills_slides/i18n/sr@latin.po` (220 lines)
- `addons/hr_skills_slides/i18n/sv.po` (219 lines)
- `addons/hr_skills_slides/i18n/th.po` (218 lines)
- `addons/hr_skills_slides/i18n/tr.po` (232 lines)
- `addons/hr_skills_slides/i18n/uk.po` (224 lines)
- `addons/hr_skills_slides/i18n/uz.po` (262 lines)
- `addons/hr_skills_slides/i18n/vi.po` (222 lines)
- `addons/hr_skills_slides/i18n/zh_CN.po` (231 lines)
- `addons/hr_skills_slides/i18n/zh_TW.po` (222 lines)
- `addons/hr_skills_slides/models/__init__.py` (6 lines)
- `addons/hr_skills_slides/models/hr_employee.py` (35 lines)
- `addons/hr_skills_slides/models/hr_employee_public.py` (15 lines)
- `addons/hr_skills_slides/models/hr_resume_line.py` (41 lines)
- `addons/hr_skills_slides/models/slide_channel.py` (110 lines)
- `addons/hr_skills_slides/static/src/fields/resume_one2many/resume_one2many.xml` (12 lines)
- `addons/hr_skills_slides/static/src/scss/hr_skills.scss` (6 lines)
- `addons/hr_skills_slides/tests/__init__.py` (3 lines)
- `addons/hr_skills_slides/tests/test_hr_skills_slides.py` (116 lines)
- `addons/hr_skills_slides/views/hr_employee_public_views.xml` (21 lines)
- `addons/hr_skills_slides/views/hr_employee_views.xml` (44 lines)
- `addons/hr_skills_slides/views/hr_resume_line_views.xml` (50 lines)
- `addons/hr_skills_slides/views/hr_views.xml` (15 lines)
- `addons/hr_skills_slides/views/slide_channel_views.xml` (40 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
