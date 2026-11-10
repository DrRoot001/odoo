# Module: hr_timesheet_attendance

- **Module ID:** MOD-103
- **Path:** `addons/hr_timesheet_attendance`
- **Manifest:** `addons/hr_timesheet_attendance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    Module linking the attendance module to the timesheet app.
    

Declared dependencies: `hr_timesheet`, `hr_attendance`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_timesheet",
    "hr_attendance"
  ],
  "data": [
    "report/hr_timesheet_attendance_report_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/hr_timesheet_attendance/__init__.py` (5 lines)
- `addons/hr_timesheet_attendance/__manifest__.py` (19 lines)
- `addons/hr_timesheet_attendance/i18n/af.po` (134 lines)
- `addons/hr_timesheet_attendance/i18n/ar.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/az.po` (137 lines)
- `addons/hr_timesheet_attendance/i18n/bg.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/bs.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/ca.po` (141 lines)
- `addons/hr_timesheet_attendance/i18n/cs.po` (142 lines)
- `addons/hr_timesheet_attendance/i18n/da.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/de.po` (143 lines)
- `addons/hr_timesheet_attendance/i18n/el.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/es.po` (142 lines)
- `addons/hr_timesheet_attendance/i18n/es_419.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/es_CL.po` (32 lines)
- `addons/hr_timesheet_attendance/i18n/et.po` (143 lines)
- `addons/hr_timesheet_attendance/i18n/eu.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/fa.po` (139 lines)
- `addons/hr_timesheet_attendance/i18n/fi.po` (144 lines)
- `addons/hr_timesheet_attendance/i18n/fo.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/fr.po` (140 lines)
- `addons/hr_timesheet_attendance/i18n/fr_CA.po` (32 lines)
- `addons/hr_timesheet_attendance/i18n/gl.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/gu.po` (134 lines)
- `addons/hr_timesheet_attendance/i18n/he.po` (141 lines)
- `addons/hr_timesheet_attendance/i18n/hi.po` (134 lines)
- `addons/hr_timesheet_attendance/i18n/hr.po` (144 lines)
- `addons/hr_timesheet_attendance/i18n/hr_timesheet_attendance.pot` (130 lines)
- `addons/hr_timesheet_attendance/i18n/hu.po` (142 lines)
- `addons/hr_timesheet_attendance/i18n/id.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/is.po` (130 lines)
- `addons/hr_timesheet_attendance/i18n/it.po` (141 lines)
- `addons/hr_timesheet_attendance/i18n/ja.po` (139 lines)
- `addons/hr_timesheet_attendance/i18n/ka.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/kab.po` (135 lines)
- `addons/hr_timesheet_attendance/i18n/km.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/ko.po` (137 lines)
- `addons/hr_timesheet_attendance/i18n/ku.po` (134 lines)
- `addons/hr_timesheet_attendance/i18n/lo.po` (137 lines)
- `addons/hr_timesheet_attendance/i18n/lt.po` (144 lines)
- `addons/hr_timesheet_attendance/i18n/lv.po` (140 lines)
- `addons/hr_timesheet_attendance/i18n/mk.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/mn.po` (139 lines)
- `addons/hr_timesheet_attendance/i18n/my.po` (134 lines)
- `addons/hr_timesheet_attendance/i18n/nb.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/nl.po` (141 lines)
- `addons/hr_timesheet_attendance/i18n/pl.po` (145 lines)
- `addons/hr_timesheet_attendance/i18n/pt.po` (145 lines)
- `addons/hr_timesheet_attendance/i18n/pt_BR.po` (144 lines)
- `addons/hr_timesheet_attendance/i18n/ro.po` (139 lines)
- `addons/hr_timesheet_attendance/i18n/ru.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/sk.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/sl.po` (142 lines)
- `addons/hr_timesheet_attendance/i18n/sq.po` (133 lines)
- `addons/hr_timesheet_attendance/i18n/sr@latin.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/sv.po` (141 lines)
- `addons/hr_timesheet_attendance/i18n/th.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/tr.po` (140 lines)
- `addons/hr_timesheet_attendance/i18n/uk.po` (140 lines)
- `addons/hr_timesheet_attendance/i18n/uz.po` (161 lines)
- `addons/hr_timesheet_attendance/i18n/vi.po` (140 lines)
- `addons/hr_timesheet_attendance/i18n/zh_CN.po` (138 lines)
- `addons/hr_timesheet_attendance/i18n/zh_TW.po` (136 lines)
- `addons/hr_timesheet_attendance/models/__init__.py` (4 lines)
- `addons/hr_timesheet_attendance/models/ir_ui_menu.py` (13 lines)
- `addons/hr_timesheet_attendance/report/__init__.py` (4 lines)
- `addons/hr_timesheet_attendance/report/hr_timesheet_attendance_report.py` (77 lines)
- `addons/hr_timesheet_attendance/report/hr_timesheet_attendance_report_view.xml` (81 lines)
- `addons/hr_timesheet_attendance/security/ir.access.csv` (3 lines)
- `addons/hr_timesheet_attendance/tests/__init__.py` (4 lines)
- `addons/hr_timesheet_attendance/tests/test_timesheet_attendance.py` (56 lines)
- `addons/hr_timesheet_attendance/upgrades/1.1/pre-migrate.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
