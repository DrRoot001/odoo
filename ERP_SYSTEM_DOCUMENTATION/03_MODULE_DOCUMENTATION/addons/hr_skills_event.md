# Module: hr_skills_event

- **Module ID:** MOD-099
- **Path:** `addons/hr_skills_event`
- **Manifest:** `addons/hr_skills_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link training events to resume of your employees


Events and Skills for HR
============================

This module add completed course events to resume for employees.
        

Declared dependencies: `hr_skills`, `event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_skills",
    "event"
  ],
  "data": [
    "views/hr_resume_line_views.xml",
    "views/event_event_views.xml",
    "views/hr_views.xml"
  ],
  "assets": {
    "web.assets_tests": [
      "hr_skills_event/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_skills_event/static/tests/**/*",
      [
        "remove",
        "hr_skills_event/static/tests/tours/**/*"
      ]
    ]
  }
}
```

### Representative source files

- `addons/hr_skills_event/__init__.py` (3 lines)
- `addons/hr_skills_event/__manifest__.py` (32 lines)
- `addons/hr_skills_event/i18n/ar.po` (98 lines)
- `addons/hr_skills_event/i18n/az.po` (94 lines)
- `addons/hr_skills_event/i18n/bg.po` (94 lines)
- `addons/hr_skills_event/i18n/bs.po` (96 lines)
- `addons/hr_skills_event/i18n/ca.po` (95 lines)
- `addons/hr_skills_event/i18n/cs.po` (95 lines)
- `addons/hr_skills_event/i18n/da.po` (94 lines)
- `addons/hr_skills_event/i18n/de.po` (106 lines)
- `addons/hr_skills_event/i18n/el.po` (94 lines)
- `addons/hr_skills_event/i18n/es.po` (102 lines)
- `addons/hr_skills_event/i18n/es_419.po` (103 lines)
- `addons/hr_skills_event/i18n/et.po` (94 lines)
- `addons/hr_skills_event/i18n/fa.po` (94 lines)
- `addons/hr_skills_event/i18n/fi.po` (103 lines)
- `addons/hr_skills_event/i18n/fr.po` (97 lines)
- `addons/hr_skills_event/i18n/he.po` (95 lines)
- `addons/hr_skills_event/i18n/hi.po` (94 lines)
- `addons/hr_skills_event/i18n/hr.po` (95 lines)
- `addons/hr_skills_event/i18n/hr_skills_event.pot` (91 lines)
- `addons/hr_skills_event/i18n/hu.po` (94 lines)
- `addons/hr_skills_event/i18n/id.po` (95 lines)
- `addons/hr_skills_event/i18n/it.po` (103 lines)
- `addons/hr_skills_event/i18n/ja.po` (97 lines)
- `addons/hr_skills_event/i18n/kab.po` (95 lines)
- `addons/hr_skills_event/i18n/ko.po` (95 lines)
- `addons/hr_skills_event/i18n/ku.po` (94 lines)
- `addons/hr_skills_event/i18n/lo.po` (94 lines)
- `addons/hr_skills_event/i18n/lt.po` (96 lines)
- `addons/hr_skills_event/i18n/lv.po` (95 lines)
- `addons/hr_skills_event/i18n/mn.po` (94 lines)
- `addons/hr_skills_event/i18n/my.po` (94 lines)
- `addons/hr_skills_event/i18n/nb.po` (94 lines)
- `addons/hr_skills_event/i18n/nl.po` (98 lines)
- `addons/hr_skills_event/i18n/pl.po` (98 lines)
- `addons/hr_skills_event/i18n/pt.po` (94 lines)
- `addons/hr_skills_event/i18n/pt_BR.po` (105 lines)
- `addons/hr_skills_event/i18n/ro.po` (99 lines)
- `addons/hr_skills_event/i18n/ru.po` (98 lines)
- `addons/hr_skills_event/i18n/sk.po` (94 lines)
- `addons/hr_skills_event/i18n/sl.po` (95 lines)
- `addons/hr_skills_event/i18n/sr@latin.po` (95 lines)
- `addons/hr_skills_event/i18n/sv.po` (97 lines)
- `addons/hr_skills_event/i18n/th.po` (96 lines)
- `addons/hr_skills_event/i18n/tr.po` (99 lines)
- `addons/hr_skills_event/i18n/uk.po` (95 lines)
- `addons/hr_skills_event/i18n/uz.po` (114 lines)
- `addons/hr_skills_event/i18n/vi.po` (95 lines)
- `addons/hr_skills_event/i18n/zh_CN.po` (101 lines)
- `addons/hr_skills_event/i18n/zh_TW.po` (95 lines)
- `addons/hr_skills_event/models/__init__.py` (4 lines)
- `addons/hr_skills_event/models/event_event.py` (25 lines)
- `addons/hr_skills_event/models/hr_resume_line.py` (35 lines)
- `addons/hr_skills_event/static/tests/tours/onsite_skill_tour.js` (111 lines)
- `addons/hr_skills_event/tests/__init__.py` (3 lines)
- `addons/hr_skills_event/tests/test_onsite.py` (39 lines)
- `addons/hr_skills_event/views/event_event_views.xml` (17 lines)
- `addons/hr_skills_event/views/hr_resume_line_views.xml` (51 lines)
- `addons/hr_skills_event/views/hr_views.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
