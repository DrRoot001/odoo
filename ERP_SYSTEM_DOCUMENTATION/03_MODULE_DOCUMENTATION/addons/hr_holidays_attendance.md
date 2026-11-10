# Module: hr_holidays_attendance

- **Module ID:** MOD-090
- **Path:** `addons/hr_holidays_attendance`
- **Manifest:** `addons/hr_holidays_attendance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Attendance Holidays


Convert employee's extra hours to leave allocations.
    

Declared dependencies: `hr_attendance`, `hr_holidays`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 26 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 11 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_attendance",
    "hr_holidays"
  ],
  "data": [
    "views/hr_leave_allocation_views.xml",
    "views/hr_leave_accrual_level_views.xml",
    "views/hr_leave_attendance_report_views.xml",
    "views/hr_attendance_overtime_views.xml",
    "views/hr_attendance_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_holidays_attendance_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_holidays_attendance/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_holidays_attendance/__init__.py` (6 lines)
- `addons/hr_holidays_attendance/__manifest__.py` (29 lines)
- `addons/hr_holidays_attendance/controllers/__init__.py` (3 lines)
- `addons/hr_holidays_attendance/controllers/main.py` (18 lines)
- `addons/hr_holidays_attendance/data/hr_holidays_attendance_demo.xml` (7 lines)
- `addons/hr_holidays_attendance/i18n/ar.po` (372 lines)
- `addons/hr_holidays_attendance/i18n/az.po` (331 lines)
- `addons/hr_holidays_attendance/i18n/bg.po` (331 lines)
- `addons/hr_holidays_attendance/i18n/bs.po` (321 lines)
- `addons/hr_holidays_attendance/i18n/ca.po` (362 lines)
- `addons/hr_holidays_attendance/i18n/cs.po` (354 lines)
- `addons/hr_holidays_attendance/i18n/da.po` (372 lines)
- `addons/hr_holidays_attendance/i18n/de.po` (432 lines)
- `addons/hr_holidays_attendance/i18n/el.po` (332 lines)
- `addons/hr_holidays_attendance/i18n/es.po` (396 lines)
- `addons/hr_holidays_attendance/i18n/es_419.po` (428 lines)
- `addons/hr_holidays_attendance/i18n/et.po` (361 lines)
- `addons/hr_holidays_attendance/i18n/fa.po` (359 lines)
- `addons/hr_holidays_attendance/i18n/fi.po` (393 lines)
- `addons/hr_holidays_attendance/i18n/fr.po` (419 lines)
- `addons/hr_holidays_attendance/i18n/he.po` (335 lines)
- `addons/hr_holidays_attendance/i18n/hi.po` (334 lines)
- `addons/hr_holidays_attendance/i18n/hr.po` (367 lines)
- `addons/hr_holidays_attendance/i18n/hr_holidays_attendance.pot` (315 lines)
- `addons/hr_holidays_attendance/i18n/hu.po` (332 lines)
- `addons/hr_holidays_attendance/i18n/id.po` (392 lines)
- `addons/hr_holidays_attendance/i18n/it.po` (428 lines)
- `addons/hr_holidays_attendance/i18n/ja.po` (419 lines)
- `addons/hr_holidays_attendance/i18n/kab.po` (320 lines)
- `addons/hr_holidays_attendance/i18n/ko.po` (385 lines)
- `addons/hr_holidays_attendance/i18n/ku.po` (323 lines)
- `addons/hr_holidays_attendance/i18n/lo.po` (330 lines)
- `addons/hr_holidays_attendance/i18n/lt.po` (333 lines)
- `addons/hr_holidays_attendance/i18n/lv.po` (320 lines)
- `addons/hr_holidays_attendance/i18n/mn.po` (331 lines)
- `addons/hr_holidays_attendance/i18n/my.po` (332 lines)
- `addons/hr_holidays_attendance/i18n/nb.po` (331 lines)
- `addons/hr_holidays_attendance/i18n/nl.po` (427 lines)
- `addons/hr_holidays_attendance/i18n/pl.po` (397 lines)
- `addons/hr_holidays_attendance/i18n/pt.po` (375 lines)
- `addons/hr_holidays_attendance/i18n/pt_BR.po` (422 lines)
- `addons/hr_holidays_attendance/i18n/ro.po` (394 lines)
- `addons/hr_holidays_attendance/i18n/ru.po` (397 lines)
- `addons/hr_holidays_attendance/i18n/sk.po` (319 lines)
- `addons/hr_holidays_attendance/i18n/sl.po` (371 lines)
- `addons/hr_holidays_attendance/i18n/sr@latin.po` (332 lines)
- `addons/hr_holidays_attendance/i18n/sv.po` (395 lines)
- `addons/hr_holidays_attendance/i18n/th.po` (369 lines)
- `addons/hr_holidays_attendance/i18n/tr.po` (392 lines)
- `addons/hr_holidays_attendance/i18n/uk.po` (365 lines)
- `addons/hr_holidays_attendance/i18n/uz.po` (450 lines)
- `addons/hr_holidays_attendance/i18n/vi.po` (374 lines)
- `addons/hr_holidays_attendance/i18n/zh_CN.po` (373 lines)
- `addons/hr_holidays_attendance/i18n/zh_TW.po` (368 lines)
- `addons/hr_holidays_attendance/models/__init__.py` (12 lines)
- `addons/hr_holidays_attendance/models/hr_attendance.py` (40 lines)
- `addons/hr_holidays_attendance/models/hr_employee.py` (56 lines)
- `addons/hr_holidays_attendance/models/hr_leave.py` (20 lines)
- `addons/hr_holidays_attendance/models/hr_leave_accrual_plan_level.py` (47 lines)
- `addons/hr_holidays_attendance/models/hr_leave_allocation.py` (40 lines)
- `addons/hr_holidays_attendance/models/hr_time_rule.py` (19 lines)
- `addons/hr_holidays_attendance/models/hr_version.py` (227 lines)
- `addons/hr_holidays_attendance/models/ir_ui_menu.py` (16 lines)
- `addons/hr_holidays_attendance/models/res_company.py` (11 lines)
- `addons/hr_holidays_attendance/models/resource_calendar_leaves.py` (80 lines)
- `addons/hr_holidays_attendance/report/__init__.py` (1 lines)
- `addons/hr_holidays_attendance/report/hr_leave_attendance_report.py` (432 lines)
- `addons/hr_holidays_attendance/security/ir.access.csv` (2 lines)
- `addons/hr_holidays_attendance/static/src/components/accrual_levels/accrual_levels.xml` (11 lines)
- `addons/hr_holidays_attendance/tests/__init__.py` (11 lines)
- `addons/hr_holidays_attendance/tests/common.py` (54 lines)
- `addons/hr_holidays_attendance/tests/test_accrual_allocations.py` (199 lines)
- `addons/hr_holidays_attendance/tests/test_holidays_overtime.py` (201 lines)
- `addons/hr_holidays_attendance/tests/test_leave_attendance_report.py` (573 lines)
- `addons/hr_holidays_attendance/tests/test_performance.py` (109 lines)
- `addons/hr_holidays_attendance/tests/test_time_rule_allocation_log.py` (449 lines)
- `addons/hr_holidays_attendance/tests/test_time_rule_pipeline.py` (4,521 lines)
- `addons/hr_holidays_attendance/tests/test_work_entry_attendance.py` (267 lines)
- `addons/hr_holidays_attendance/views/hr_attendance_overtime_views.xml` (27 lines)
- `addons/hr_holidays_attendance/views/hr_attendance_views.xml` (32 lines)
- `addons/hr_holidays_attendance/views/hr_leave_accrual_level_views.xml` (19 lines)
- `addons/hr_holidays_attendance/views/hr_leave_allocation_views.xml` (31 lines)
- `addons/hr_holidays_attendance/views/hr_leave_attendance_report_views.xml` (132 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
