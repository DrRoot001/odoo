# Module: project_hr_skills

- **Module ID:** MOD-478
- **Path:** `addons/project_hr_skills`
- **Manifest:** `addons/project_hr_skills/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Project skills


        Search project tasks according to the assignees' skills
    

Declared dependencies: `project`, `hr_skills`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project",
    "hr_skills"
  ],
  "data": [
    "views/project_task_views.xml",
    "report/project_report_views.xml"
  ]
}
```

### Representative source files

- `addons/project_hr_skills/__init__.py` (4 lines)
- `addons/project_hr_skills/__manifest__.py` (18 lines)
- `addons/project_hr_skills/i18n/ar.po` (109 lines)
- `addons/project_hr_skills/i18n/az.po` (94 lines)
- `addons/project_hr_skills/i18n/bg.po` (94 lines)
- `addons/project_hr_skills/i18n/bs.po` (96 lines)
- `addons/project_hr_skills/i18n/ca.po` (95 lines)
- `addons/project_hr_skills/i18n/cs.po` (96 lines)
- `addons/project_hr_skills/i18n/da.po` (95 lines)
- `addons/project_hr_skills/i18n/de.po` (111 lines)
- `addons/project_hr_skills/i18n/el.po` (95 lines)
- `addons/project_hr_skills/i18n/es.po` (110 lines)
- `addons/project_hr_skills/i18n/es_419.po` (107 lines)
- `addons/project_hr_skills/i18n/et.po` (106 lines)
- `addons/project_hr_skills/i18n/fa.po` (94 lines)
- `addons/project_hr_skills/i18n/fi.po` (107 lines)
- `addons/project_hr_skills/i18n/fr.po` (107 lines)
- `addons/project_hr_skills/i18n/he.po` (95 lines)
- `addons/project_hr_skills/i18n/hi.po` (94 lines)
- `addons/project_hr_skills/i18n/hr.po` (95 lines)
- `addons/project_hr_skills/i18n/hu.po` (95 lines)
- `addons/project_hr_skills/i18n/id.po` (108 lines)
- `addons/project_hr_skills/i18n/it.po` (107 lines)
- `addons/project_hr_skills/i18n/ja.po` (107 lines)
- `addons/project_hr_skills/i18n/kab.po` (95 lines)
- `addons/project_hr_skills/i18n/ko.po` (107 lines)
- `addons/project_hr_skills/i18n/ku.po` (94 lines)
- `addons/project_hr_skills/i18n/lo.po` (94 lines)
- `addons/project_hr_skills/i18n/lt.po` (96 lines)
- `addons/project_hr_skills/i18n/lv.po` (95 lines)
- `addons/project_hr_skills/i18n/mn.po` (94 lines)
- `addons/project_hr_skills/i18n/my.po` (94 lines)
- `addons/project_hr_skills/i18n/nb.po` (95 lines)
- `addons/project_hr_skills/i18n/nl.po` (107 lines)
- `addons/project_hr_skills/i18n/pl.po` (109 lines)
- `addons/project_hr_skills/i18n/project_hr_skills.pot` (90 lines)
- `addons/project_hr_skills/i18n/pt.po` (95 lines)
- `addons/project_hr_skills/i18n/pt_BR.po` (110 lines)
- `addons/project_hr_skills/i18n/ro.po` (107 lines)
- `addons/project_hr_skills/i18n/ru.po` (109 lines)
- `addons/project_hr_skills/i18n/sk.po` (94 lines)
- `addons/project_hr_skills/i18n/sl.po` (96 lines)
- `addons/project_hr_skills/i18n/sr@latin.po` (95 lines)
- `addons/project_hr_skills/i18n/sv.po` (107 lines)
- `addons/project_hr_skills/i18n/th.po` (107 lines)
- `addons/project_hr_skills/i18n/tr.po` (109 lines)
- `addons/project_hr_skills/i18n/uk.po` (95 lines)
- `addons/project_hr_skills/i18n/uz.po` (117 lines)
- `addons/project_hr_skills/i18n/vi.po` (107 lines)
- `addons/project_hr_skills/i18n/zh_CN.po` (107 lines)
- `addons/project_hr_skills/i18n/zh_TW.po` (98 lines)
- `addons/project_hr_skills/models/__init__.py` (4 lines)
- `addons/project_hr_skills/models/project_task.py` (9 lines)
- `addons/project_hr_skills/models/res_users.py` (7 lines)
- `addons/project_hr_skills/report/__init__.py` (3 lines)
- `addons/project_hr_skills/report/project_report_views.xml` (11 lines)
- `addons/project_hr_skills/report/report_project_task_user.py` (9 lines)
- `addons/project_hr_skills/views/project_task_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
