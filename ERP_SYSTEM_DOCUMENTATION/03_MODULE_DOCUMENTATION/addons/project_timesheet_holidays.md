# Module: project_timesheet_holidays

- **Module ID:** MOD-491
- **Path:** `addons/project_timesheet_holidays`
- **Manifest:** `addons/project_timesheet_holidays/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Schedule timesheet when on time off


Bridge module to integrate leaves in timesheet
================================================

This module allows to automatically log timesheets when employees are
on leaves. Project and task can be configured company-wide.
    

Declared dependencies: `hr_timesheet`, `hr_holidays`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_timesheet",
    "hr_holidays"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/project_task_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/holiday_timesheets_demo.xml"
  ]
}
```

### Representative source files

- `addons/project_timesheet_holidays/__init__.py` (45 lines)
- `addons/project_timesheet_holidays/__manifest__.py` (28 lines)
- `addons/project_timesheet_holidays/data/holiday_timesheets_demo.xml` (14 lines)
- `addons/project_timesheet_holidays/i18n/ar.po` (245 lines)
- `addons/project_timesheet_holidays/i18n/az.po` (228 lines)
- `addons/project_timesheet_holidays/i18n/bg.po` (224 lines)
- `addons/project_timesheet_holidays/i18n/bs.po` (228 lines)
- `addons/project_timesheet_holidays/i18n/ca.po` (238 lines)
- `addons/project_timesheet_holidays/i18n/cs.po` (231 lines)
- `addons/project_timesheet_holidays/i18n/da.po` (231 lines)
- `addons/project_timesheet_holidays/i18n/de.po` (264 lines)
- `addons/project_timesheet_holidays/i18n/el.po` (228 lines)
- `addons/project_timesheet_holidays/i18n/es.po` (251 lines)
- `addons/project_timesheet_holidays/i18n/es_419.po` (248 lines)
- `addons/project_timesheet_holidays/i18n/et.po` (248 lines)
- `addons/project_timesheet_holidays/i18n/fa.po` (232 lines)
- `addons/project_timesheet_holidays/i18n/fi.po` (246 lines)
- `addons/project_timesheet_holidays/i18n/fr.po` (257 lines)
- `addons/project_timesheet_holidays/i18n/gu.po` (218 lines)
- `addons/project_timesheet_holidays/i18n/he.po` (232 lines)
- `addons/project_timesheet_holidays/i18n/hi.po` (224 lines)
- `addons/project_timesheet_holidays/i18n/hr.po` (231 lines)
- `addons/project_timesheet_holidays/i18n/hu.po` (236 lines)
- `addons/project_timesheet_holidays/i18n/id.po` (243 lines)
- `addons/project_timesheet_holidays/i18n/is.po` (214 lines)
- `addons/project_timesheet_holidays/i18n/it.po` (259 lines)
- `addons/project_timesheet_holidays/i18n/ja.po` (248 lines)
- `addons/project_timesheet_holidays/i18n/kab.po` (225 lines)
- `addons/project_timesheet_holidays/i18n/km.po` (217 lines)
- `addons/project_timesheet_holidays/i18n/ko.po` (242 lines)
- `addons/project_timesheet_holidays/i18n/ku.po` (224 lines)
- `addons/project_timesheet_holidays/i18n/lo.po` (250 lines)
- `addons/project_timesheet_holidays/i18n/lt.po` (231 lines)
- `addons/project_timesheet_holidays/i18n/lv.po` (229 lines)
- `addons/project_timesheet_holidays/i18n/mn.po` (234 lines)
- `addons/project_timesheet_holidays/i18n/my.po` (225 lines)
- `addons/project_timesheet_holidays/i18n/nb.po` (228 lines)
- `addons/project_timesheet_holidays/i18n/nl.po` (262 lines)
- `addons/project_timesheet_holidays/i18n/pl.po` (260 lines)
- `addons/project_timesheet_holidays/i18n/project_timesheet_holidays.pot` (221 lines)
- `addons/project_timesheet_holidays/i18n/pt.po` (237 lines)
- `addons/project_timesheet_holidays/i18n/pt_BR.po` (260 lines)
- `addons/project_timesheet_holidays/i18n/ro.po` (233 lines)
- `addons/project_timesheet_holidays/i18n/ru.po` (244 lines)
- `addons/project_timesheet_holidays/i18n/sk.po` (229 lines)
- `addons/project_timesheet_holidays/i18n/sl.po` (233 lines)
- `addons/project_timesheet_holidays/i18n/sr@latin.po` (229 lines)
- `addons/project_timesheet_holidays/i18n/sv.po` (233 lines)
- `addons/project_timesheet_holidays/i18n/th.po` (243 lines)
- `addons/project_timesheet_holidays/i18n/tr.po` (252 lines)
- `addons/project_timesheet_holidays/i18n/uk.po` (231 lines)
- `addons/project_timesheet_holidays/i18n/uz.po` (259 lines)
- `addons/project_timesheet_holidays/i18n/vi.po` (242 lines)
- `addons/project_timesheet_holidays/i18n/zh_CN.po` (251 lines)
- `addons/project_timesheet_holidays/i18n/zh_TW.po` (230 lines)
- `addons/project_timesheet_holidays/models/__init__.py` (10 lines)
- `addons/project_timesheet_holidays/models/account_analytic.py` (63 lines)
- `addons/project_timesheet_holidays/models/hr_employee.py` (85 lines)
- `addons/project_timesheet_holidays/models/hr_employee_departure.py` (12 lines)
- `addons/project_timesheet_holidays/models/hr_leave.py` (161 lines)
- `addons/project_timesheet_holidays/models/project_task.py` (33 lines)
- `addons/project_timesheet_holidays/models/res_company.py` (29 lines)
- `addons/project_timesheet_holidays/models/res_config_settings.py` (29 lines)
- `addons/project_timesheet_holidays/models/resource_calendar_leaves.py` (294 lines)
- `addons/project_timesheet_holidays/security/ir.access.csv` (2 lines)
- `addons/project_timesheet_holidays/tests/__init__.py` (7 lines)
- `addons/project_timesheet_holidays/tests/test_cancel_time_off.py` (70 lines)
- `addons/project_timesheet_holidays/tests/test_employee.py` (185 lines)
- `addons/project_timesheet_holidays/tests/test_timesheet_global_time_off.py` (620 lines)
- `addons/project_timesheet_holidays/tests/test_timesheet_holidays.py` (644 lines)
- `addons/project_timesheet_holidays/views/project_task_views.xml` (18 lines)
- `addons/project_timesheet_holidays/views/res_config_settings_views.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
