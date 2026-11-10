# Module: hr_timesheet

- **Module ID:** MOD-102
- **Path:** `addons/hr_timesheet`
- **Manifest:** `addons/hr_timesheet/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Track employee time on tasks


This module implements a timesheet system.
==========================================

Each employee can encode and track their time spent on the different projects.

Lots of reporting on time and employee tracking are provided.

It is completely integrated with the cost accounting module. It allows you to set
up a management by affair.
    

Declared dependencies: `hr`, `analytic`, `project`, `uom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 16 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 22 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 21 | Client behavior/assets. |
| Tests | 12 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "analytic",
    "project",
    "uom"
  ],
  "data": [
    "security/hr_timesheet_security.xml",
    "data/portal_entry_data.xml",
    "views/account_analytic_line_views.xml",
    "views/res_config_settings_views.xml",
    "views/project_project_views.xml",
    "views/project_task_views.xml",
    "views/project_task_portal_templates.xml",
    "views/hr_timesheet_portal_templates.xml",
    "report/hr_timesheet_report_view.xml",
    "report/project_report_view.xml",
    "report/report_timesheet_templates.xml",
    "views/hr_department_views.xml",
    "views/hr_employee_views.xml",
    "views/hr_employee_public_views.xml",
    "data/hr_timesheet_data.xml",
    "views/project_task_sharing_views.xml",
    "views/project_update_views.xml",
    "views/hr_timesheet_menus.xml",
    "security/ir.access.csv",
    "wizard/hr_employee_delete_wizard_views.xml"
  ],
  "demo": [
    "data/hr_timesheet_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_timesheet/static/src/**/*",
      [
        "remove",
        "hr_timesheet/static/src/views/project_task_analysis_graph/**/*"
      ],
      [
        "remove",
        "hr_timesheet/static/src/views/project_task_graph/**/*"
      ],
      [
        "remove",
        "hr_timesheet/static/src/views/timesheet_graph/**/*"
      ]
    ],
    "web.assets_backend_lazy": [
      "hr_timesheet/static/src/views/project_task_analysis_graph/**/*",
      "hr_timesheet/static/src/views/project_task_graph/**/*",
      "hr_timesheet/static/src/views/timesheet_graph/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_timesheet/static/tests/hr_timesheet_models.js",
      "hr_timesheet/static/tests/**/*.test.js"
    ],
    "project.webclient": [
      "hr_timesheet/static/src/services/**/*",
      "hr_timesheet/static/src/components/**/*",
      "hr_timesheet/static/src/scss/timesheets_task_form.scss"
    ]
  }
}
```

### Representative source files

- `addons/hr_timesheet/__init__.py` (52 lines)
- `addons/hr_timesheet/__manifest__.py` (73 lines)
- `addons/hr_timesheet/controllers/__init__.py` (5 lines)
- `addons/hr_timesheet/controllers/portal.py` (187 lines)
- `addons/hr_timesheet/controllers/project.py` (45 lines)
- `addons/hr_timesheet/data/hr_timesheet_data.xml` (71 lines)
- `addons/hr_timesheet/data/hr_timesheet_demo.xml` (3,824 lines)
- `addons/hr_timesheet/data/portal_entry_data.xml` (12 lines)
- `addons/hr_timesheet/i18n/af.po` (1,552 lines)
- `addons/hr_timesheet/i18n/am.po` (1,548 lines)
- `addons/hr_timesheet/i18n/ar.po` (1,644 lines)
- `addons/hr_timesheet/i18n/az.po` (1,583 lines)
- `addons/hr_timesheet/i18n/bg.po` (1,593 lines)
- `addons/hr_timesheet/i18n/bs.po` (1,580 lines)
- `addons/hr_timesheet/i18n/ca.po` (1,621 lines)
- `addons/hr_timesheet/i18n/cs.po` (1,605 lines)
- `addons/hr_timesheet/i18n/da.po` (1,607 lines)
- `addons/hr_timesheet/i18n/de.po` (1,722 lines)
- `addons/hr_timesheet/i18n/el.po` (1,582 lines)
- `addons/hr_timesheet/i18n/es.po` (1,664 lines)
- `addons/hr_timesheet/i18n/es_419.po` (1,709 lines)
- `addons/hr_timesheet/i18n/es_CL.po` (41 lines)
- `addons/hr_timesheet/i18n/et.po` (1,627 lines)
- `addons/hr_timesheet/i18n/eu.po` (1,551 lines)
- `addons/hr_timesheet/i18n/fa.po` (1,612 lines)
- `addons/hr_timesheet/i18n/fi.po` (1,679 lines)
- `addons/hr_timesheet/i18n/fo.po` (1,551 lines)
- `addons/hr_timesheet/i18n/fr.po` (1,678 lines)
- `addons/hr_timesheet/i18n/fr_BE.po` (61 lines)
- `addons/hr_timesheet/i18n/fr_CA.po` (36 lines)
- `addons/hr_timesheet/i18n/gl.po` (1,551 lines)
- `addons/hr_timesheet/i18n/gu.po` (1,552 lines)
- `addons/hr_timesheet/i18n/he.po` (1,603 lines)
- `addons/hr_timesheet/i18n/hi.po` (1,577 lines)
- `addons/hr_timesheet/i18n/hr.po` (1,605 lines)
- `addons/hr_timesheet/i18n/hr_timesheet.pot` (1,557 lines)
- `addons/hr_timesheet/i18n/hu.po` (1,648 lines)
- `addons/hr_timesheet/i18n/hy.po` (1,550 lines)
- `addons/hr_timesheet/i18n/id.po` (1,692 lines)
- `addons/hr_timesheet/i18n/is.po` (1,555 lines)
- `addons/hr_timesheet/i18n/it.po` (1,708 lines)
- `addons/hr_timesheet/i18n/ja.po` (1,655 lines)
- `addons/hr_timesheet/i18n/ka.po` (1,551 lines)
- `addons/hr_timesheet/i18n/kab.po` (1,577 lines)
- `addons/hr_timesheet/i18n/kk.po` (1,550 lines)
- `addons/hr_timesheet/i18n/km.po` (1,553 lines)
- `addons/hr_timesheet/i18n/ko.po` (1,631 lines)
- `addons/hr_timesheet/i18n/ku.po` (1,576 lines)
- `addons/hr_timesheet/i18n/lb.po` (1,553 lines)
- `addons/hr_timesheet/i18n/lo.po` (1,665 lines)
- `addons/hr_timesheet/i18n/lt.po` (1,600 lines)
- `addons/hr_timesheet/i18n/lv.po` (1,585 lines)
- `addons/hr_timesheet/i18n/mk.po` (1,551 lines)
- `addons/hr_timesheet/i18n/mn.po` (1,589 lines)
- `addons/hr_timesheet/i18n/my.po` (1,577 lines)
- `addons/hr_timesheet/i18n/nb.po` (1,586 lines)
- `addons/hr_timesheet/i18n/nl.po` (1,706 lines)
- `addons/hr_timesheet/i18n/pl.po` (1,672 lines)
- `addons/hr_timesheet/i18n/pt.po` (1,645 lines)
- `addons/hr_timesheet/i18n/pt_BR.po` (1,718 lines)
- `addons/hr_timesheet/i18n/ro.po` (1,643 lines)
- `addons/hr_timesheet/i18n/ru.po` (1,653 lines)
- `addons/hr_timesheet/i18n/sk.po` (1,604 lines)
- `addons/hr_timesheet/i18n/sl.po` (1,637 lines)
- `addons/hr_timesheet/i18n/sq.po` (1,551 lines)
- `addons/hr_timesheet/i18n/sr@latin.po` (1,582 lines)
- `addons/hr_timesheet/i18n/sv.po` (1,640 lines)
- `addons/hr_timesheet/i18n/ta.po` (1,551 lines)
- `addons/hr_timesheet/i18n/te.po` (1,550 lines)
- `addons/hr_timesheet/i18n/th.po` (1,619 lines)
- `addons/hr_timesheet/i18n/tr.po` (1,662 lines)
- `addons/hr_timesheet/i18n/uk.po` (1,611 lines)
- `addons/hr_timesheet/i18n/uz.po` (1,843 lines)
- `addons/hr_timesheet/i18n/vi.po` (1,647 lines)
- `addons/hr_timesheet/i18n/zh_CN.po` (1,665 lines)
- `addons/hr_timesheet/i18n/zh_TW.po` (1,604 lines)
- `addons/hr_timesheet/models/__init__.py` (17 lines)
- `addons/hr_timesheet/models/account_analytic_line.py` (563 lines)
- `addons/hr_timesheet/models/account_analytic_line_calendar_employee.py` (12 lines)
- `addons/hr_timesheet/models/analytic_applicability.py` (15 lines)
- `addons/hr_timesheet/models/hr_employee.py` (75 lines)
- `addons/hr_timesheet/models/hr_employee_departure.py` (26 lines)
- `addons/hr_timesheet/models/hr_employee_public.py` (14 lines)
- `addons/hr_timesheet/models/ir_http.py` (42 lines)
- `addons/hr_timesheet/models/ir_ui_menu.py` (13 lines)
- `addons/hr_timesheet/models/project_collaborator.py` (16 lines)
- `addons/hr_timesheet/models/project_project.py` (281 lines)
- `addons/hr_timesheet/models/project_task.py` (327 lines)
- `addons/hr_timesheet/models/project_update.py` (39 lines)
- `addons/hr_timesheet/models/res_company.py` (66 lines)
- `addons/hr_timesheet/models/res_config_settings.py` (46 lines)
- `addons/hr_timesheet/models/uom_uom.py` (20 lines)
- `addons/hr_timesheet/report/__init__.py` (5 lines)
- `addons/hr_timesheet/report/hr_timesheet_report_view.xml` (257 lines)
- `addons/hr_timesheet/report/project_report.py` (34 lines)
- `addons/hr_timesheet/report/project_report_view.xml` (34 lines)
- `addons/hr_timesheet/report/report_timesheet_templates.xml` (257 lines)
- `addons/hr_timesheet/report/timesheets_analysis_report.py` (74 lines)
- `addons/hr_timesheet/security/hr_timesheet_security.xml` (57 lines)
- `addons/hr_timesheet/security/ir.access.csv` (47 lines)
- `addons/hr_timesheet/static/description/icon.png` (28 lines)
- `addons/hr_timesheet/static/description/icon.svg` (1 lines)
- `addons/hr_timesheet/static/description/icon_hi.png` (149 lines)
- `addons/hr_timesheet/static/description/icon_timesheet.png` (28 lines)
- `addons/hr_timesheet/static/img/digest_tip_timesheets_hotkeys.gif` (97 lines)
- `addons/hr_timesheet/static/img/employee7-image.jpg` (62 lines)
- `addons/hr_timesheet/static/img/employee_phu-image.jpg` (45 lines)
- `addons/hr_timesheet/static/img/product_product_consultant-image.jpg` (56 lines)
- `addons/hr_timesheet/static/img/timesheet.svg` (13 lines)
- `addons/hr_timesheet/static/src/components/progress_bar/project_task_progress_bar_field.js` (25 lines)
- `addons/hr_timesheet/static/src/components/task_with_hours/task_with_hours.js` (43 lines)
- `addons/hr_timesheet/static/src/components/task_with_hours/task_with_hours.xml` (8 lines)
- `addons/hr_timesheet/static/src/components/time_hour_field/time_hour_field.js` (18 lines)
- `addons/hr_timesheet/static/src/components/timesheet_duration_uom/timesheet_duration_uom.js` (20 lines)
- `addons/hr_timesheet/static/src/components/timesheet_duration_uom/timesheet_duration_uom.scss` (3 lines)
- `addons/hr_timesheet/static/src/components/timesheet_uom/timesheet_uom.js` (33 lines)
- `addons/hr_timesheet/static/src/components/timesheet_uom/timesheet_uom.scss` (7 lines)
- `addons/hr_timesheet/static/src/components/timesheet_uom/timesheet_uom.xml` (11 lines)
- `addons/hr_timesheet/static/src/components/timesheet_uom_no_toggle/timesheet_uom_no_toggle.js` (22 lines)
- `addons/hr_timesheet/static/src/scss/timesheet_kanban.scss` (3 lines)
- `addons/hr_timesheet/static/src/scss/timesheets_task_form.scss` (3 lines)
- `addons/hr_timesheet/static/src/services/timesheet_uom_service.js` (59 lines)
- `addons/hr_timesheet/static/src/views/graph_model_patch.js` (26 lines)
- `addons/hr_timesheet/static/src/views/project_task_analysis_graph/project_task_analysis_graph_model.js` (5 lines)
- `addons/hr_timesheet/static/src/views/project_task_graph/project_task_graph_model.js` (4 lines)
- `addons/hr_timesheet/static/src/views/timesheet_calendar/timesheet_calendar_model.js` (21 lines)
- `addons/hr_timesheet/static/src/views/timesheet_calendar/timesheet_calendar_view.js` (10 lines)
- `addons/hr_timesheet/static/src/views/timesheet_calendar_my_timesheets/timesheet_calendar_my_timesheets_model.js` (12 lines)
- `addons/hr_timesheet/static/src/views/timesheet_calendar_my_timesheets/timesheet_calendar_my_timesheets_view.js` (12 lines)
- `addons/hr_timesheet/static/src/views/timesheet_graph/timesheet_graph_model.js` (6 lines)
- `addons/hr_timesheet/static/src/views/timesheet_graph/timesheet_graph_view.js` (12 lines)
- `addons/hr_timesheet/static/tests/hr_timesheet_models.js` (129 lines)
- `addons/hr_timesheet/static/tests/task_with_hours.test.js` (82 lines)
- `addons/hr_timesheet/static/tests/timesheet_graph.test.js` (29 lines)
- `addons/hr_timesheet/static/tests/timesheet_uom.test.js` (94 lines)
- `addons/hr_timesheet/static/tests/timesheet_uom_no_toggle.test.js` (87 lines)
- `addons/hr_timesheet/static/xls/timesheets_import_template.xlsx` (83 lines)
- `addons/hr_timesheet/tests/__init__.py` (13 lines)
- `addons/hr_timesheet/tests/test_employee_delete_wizard.py` (64 lines)
- `addons/hr_timesheet/tests/test_portal_timesheet.py` (180 lines)
- `addons/hr_timesheet/tests/test_project_project.py` (93 lines)
- `addons/hr_timesheet/tests/test_project_sharing.py` (34 lines)
- `addons/hr_timesheet/tests/test_project_task_quick_create.py` (39 lines)
- `addons/hr_timesheet/tests/test_project_template.py` (56 lines)
- `addons/hr_timesheet/tests/test_report_timesheet.py` (77 lines)
- `addons/hr_timesheet/tests/test_task_analysis.py` (52 lines)
- `addons/hr_timesheet/tests/test_task_templates.py` (33 lines)
- `addons/hr_timesheet/tests/test_timesheet.py` (1,290 lines)
- `addons/hr_timesheet/tests/test_timesheet_import_template.py` (23 lines)
- `addons/hr_timesheet/views/account_analytic_line_views.xml` (646 lines)
- `addons/hr_timesheet/views/hr_department_views.xml` (21 lines)
- `addons/hr_timesheet/views/hr_employee_public_views.xml` (18 lines)
- `addons/hr_timesheet/views/hr_employee_views.xml` (63 lines)
- `addons/hr_timesheet/views/hr_timesheet_menus.xml` (64 lines)
- `addons/hr_timesheet/views/hr_timesheet_portal_templates.xml` (175 lines)
- `addons/hr_timesheet/views/project_project_views.xml` (131 lines)
- `addons/hr_timesheet/views/project_task_portal_templates.xml` (109 lines)
- `addons/hr_timesheet/views/project_task_sharing_views.xml` (159 lines)
- `addons/hr_timesheet/views/project_task_views.xml` (274 lines)
- `addons/hr_timesheet/views/project_update_views.xml` (36 lines)

Additional files not expanded here: 4. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
