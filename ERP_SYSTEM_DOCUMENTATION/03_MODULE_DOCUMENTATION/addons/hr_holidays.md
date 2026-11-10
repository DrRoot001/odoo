# Module: hr_holidays

- **Module ID:** MOD-089
- **Path:** `addons/hr_holidays`
- **Manifest:** `addons/hr_holidays/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Allocate time off and follow leave requests


Manage time off requests and allocations
========================================

This application controls the time off schedule of your company. It allows employees to request time off. Then, managers can review requests for time off and approve or reject them. This way you can control the overall time off planning for the company or department.

You can configure several kinds of time off (sickness, paid days, ...) and allocate time off to an employee or department quickly using time off allocation. An employee can also make a request for more days off by making a new time off allocation. It will increase the total of available days for that time type (if the request is accepted).

You can keep track of time off in different ways by following reports:

* Time Off Summary
* Time Off by Department
* Time Off Analysis

A synchronization with an internal agenda (Meetings of the CRM module) is also possible in order to automatically create a meeting when a time off request is accepted by setting up a type of meeting in time off Type.


Declared dependencies: `hr_work_entry`, `hr_calendar`, `resource`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 88 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 25 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 53 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 74 | Client behavior/assets. |
| Tests | 44 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_work_entry",
    "hr_calendar",
    "resource"
  ],
  "data": [
    "data/hr_time_rule_data.xml",
    "data/report_paperformat.xml",
    "data/mail_activity_type_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/hr_work_entry_type_data.xml",
    "data/ir_cron_data.xml",
    "data/hr_holidays_tour.xml",
    "data/mail_template_data.xml",
    "security/hr_holidays_security.xml",
    "wizard/hr_holidays_cancel_leave_views.xml",
    "wizard/hr_holidays_summary_employees_views.xml",
    "wizard/hr_leave_generate_multi_wizard_views.xml",
    "wizard/hr_leave_allocation_generate_multi_wizard_views.xml",
    "wizard/load_public_holiday_wizard_views.xml",
    "views/resource_views.xml",
    "views/hr_leave_views.xml",
    "views/hr_work_entry_type_views.xml",
    "views/hr_leave_allocation_views.xml",
    "views/hr_leave_accrual_views.xml",
    "views/hr_leave_mandatory_day_views.xml",
    "views/mail_activity_views.xml",
    "views/calendar_views.xml",
    "report/hr_holidays_templates.xml",
    "report/hr_holidays_reports.xml",
    "report/hr_leave_reports.xml",
    "report/hr_leave_report_calendar.xml",
    "report/hr_leave_employee_type_report.xml",
    "report/hr_leave_employee_report_views.xml",
    "views/hr_views.xml",
    "views/hr_holidays_views.xml",
    "views/hr_time_rule_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_holidays_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_holidays/static/src/core/common/**/*",
      "hr_holidays/static/src/core/web/**/*",
      "hr_holidays/static/src/**/*",
      [
        "remove",
        "hr_holidays/static/src/views/graph/**"
      ],
      [
        "remove",
        "hr_holidays/static/src/**/*.dark.scss"
      ]
    ],
    "web.assets_backend_lazy": [
      "hr_holidays/static/src/views/graph/**"
    ],
    "web.assets_web_dark": [
      "hr_holidays/static/src/**/*.dark.scss"
    ],
    "im_livechat.assets_embed_core": [
      "hr_holidays/static/src/core/common/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      "hr_holidays/static/tests/hr_holidays_test_helpers.js",
      "hr_holidays/static/tests/mock_server/**/*"
    ],
    "mail.assets_public": [
      "hr_holidays/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "hr_holidays/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_holidays/static/tests/**/*",
      [
        "remove",
        "hr_holidays/static/tests/tours/**/*"
      ]
    ],
    "web.assets_tests": [
      "/hr_holidays/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_holidays/__init__.py` (6 lines)
- `addons/hr_holidays/__manifest__.py` (141 lines)
- `addons/hr_holidays/controllers/__init__.py` (3 lines)
- `addons/hr_holidays/controllers/main.py` (58 lines)
- `addons/hr_holidays/controllers/webmanifest.py` (9 lines)
- `addons/hr_holidays/data/hr_holidays_demo.xml` (435 lines)
- `addons/hr_holidays/data/hr_holidays_tour.xml` (7 lines)
- `addons/hr_holidays/data/hr_time_rule_data.xml` (69 lines)
- `addons/hr_holidays/data/hr_work_entry_type_data.xml` (1,627 lines)
- `addons/hr_holidays/data/ir_cron_data.xml` (49 lines)
- `addons/hr_holidays/data/mail_activity_type_data.xml` (34 lines)
- `addons/hr_holidays/data/mail_message_subtype_data.xml` (28 lines)
- `addons/hr_holidays/data/mail_template_data.xml` (51 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ar.csv` (391 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_au.csv` (176 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_be.csv` (251 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_br.csv` (339 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ca.csv` (261 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ch.csv` (26 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_cl.csv` (411 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_co.csv` (451 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_do.csv` (301 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ec.csv` (287 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_eg.csv` (496 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_gt.csv` (251 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_hk.csv` (481 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_in.csv` (386 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_jo.csv` (385 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ke.csv` (295 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_lt.csv` (401 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_lu.csv` (276 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ma.csv` (444 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_mx.csv` (253 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_my.csv` (358 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_nl.csv` (276 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_pa.csv` (342 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_pe.csv` (401 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_pl.csv` (351 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_ro.csv` (426 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_sa.csv` (237 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_sk.csv` (287 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_tr.csv` (358 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_us.csv` (314 lines)
- `addons/hr_holidays/data/public_holidays/public_holidays_uy.csv` (456 lines)
- `addons/hr_holidays/data/report_paperformat.xml` (18 lines)
- `addons/hr_holidays/i18n/af.po` (5,475 lines)
- `addons/hr_holidays/i18n/am.po` (5,471 lines)
- `addons/hr_holidays/i18n/ar.po` (5,960 lines)
- `addons/hr_holidays/i18n/az.po` (5,816 lines)
- `addons/hr_holidays/i18n/bg.po` (5,795 lines)
- `addons/hr_holidays/i18n/bs.po` (5,767 lines)
- `addons/hr_holidays/i18n/ca.po` (5,884 lines)
- `addons/hr_holidays/i18n/cs.po` (5,848 lines)
- `addons/hr_holidays/i18n/da.po` (5,997 lines)
- `addons/hr_holidays/i18n/de.po` (6,361 lines)
- `addons/hr_holidays/i18n/el.po` (5,782 lines)
- `addons/hr_holidays/i18n/es.po` (6,125 lines)
- `addons/hr_holidays/i18n/es_419.po` (6,364 lines)
- `addons/hr_holidays/i18n/es_CL.po` (233 lines)
- `addons/hr_holidays/i18n/et.po` (5,903 lines)
- `addons/hr_holidays/i18n/eu.po` (5,474 lines)
- `addons/hr_holidays/i18n/fa.po` (5,867 lines)
- `addons/hr_holidays/i18n/fi.po` (6,058 lines)
- `addons/hr_holidays/i18n/fo.po` (5,474 lines)
- `addons/hr_holidays/i18n/fr.po` (6,198 lines)
- `addons/hr_holidays/i18n/fr_BE.po` (249 lines)
- `addons/hr_holidays/i18n/fr_CA.po` (203 lines)
- `addons/hr_holidays/i18n/gl.po` (5,474 lines)
- `addons/hr_holidays/i18n/gu.po` (5,480 lines)
- `addons/hr_holidays/i18n/he.po` (5,805 lines)
- `addons/hr_holidays/i18n/hi.po` (5,941 lines)
- `addons/hr_holidays/i18n/hr.po` (5,854 lines)
- `addons/hr_holidays/i18n/hr_holidays.pot` (5,716 lines)
- `addons/hr_holidays/i18n/hu.po` (5,800 lines)
- `addons/hr_holidays/i18n/id.po` (6,036 lines)
- `addons/hr_holidays/i18n/is.po` (5,475 lines)
- `addons/hr_holidays/i18n/it.po` (6,227 lines)
- `addons/hr_holidays/i18n/ja.po` (6,056 lines)
- `addons/hr_holidays/i18n/ka.po` (5,474 lines)
- `addons/hr_holidays/i18n/kab.po` (5,761 lines)
- `addons/hr_holidays/i18n/km.po` (5,476 lines)
- `addons/hr_holidays/i18n/ko.po` (5,922 lines)
- `addons/hr_holidays/i18n/ku.po` (5,773 lines)
- `addons/hr_holidays/i18n/lb.po` (5,476 lines)
- `addons/hr_holidays/i18n/lo.po` (6,084 lines)
- `addons/hr_holidays/i18n/lt.po` (5,818 lines)
- `addons/hr_holidays/i18n/lv.po` (5,777 lines)
- `addons/hr_holidays/i18n/mk.po` (5,474 lines)
- `addons/hr_holidays/i18n/mn.po` (6,257 lines)
- `addons/hr_holidays/i18n/my.po` (5,773 lines)
- `addons/hr_holidays/i18n/nb.po` (5,879 lines)
- `addons/hr_holidays/i18n/nl.po` (6,349 lines)
- `addons/hr_holidays/i18n/pl.po` (6,147 lines)
- `addons/hr_holidays/i18n/pt.po` (6,009 lines)
- `addons/hr_holidays/i18n/pt_BR.po` (6,350 lines)
- `addons/hr_holidays/i18n/ro.po` (6,007 lines)
- `addons/hr_holidays/i18n/ru.po` (6,037 lines)
- `addons/hr_holidays/i18n/sk.po` (5,820 lines)
- `addons/hr_holidays/i18n/sl.po` (5,917 lines)
- `addons/hr_holidays/i18n/sq.po` (5,474 lines)
- `addons/hr_holidays/i18n/sr@latin.po` (5,783 lines)
- `addons/hr_holidays/i18n/sv.po` (5,933 lines)
- `addons/hr_holidays/i18n/th.po` (5,876 lines)
- `addons/hr_holidays/i18n/tr.po` (6,022 lines)
- `addons/hr_holidays/i18n/uk.po` (5,882 lines)
- `addons/hr_holidays/i18n/uz.po` (6,622 lines)
- `addons/hr_holidays/i18n/vi.po` (5,997 lines)
- `addons/hr_holidays/i18n/zh_CN.po` (6,120 lines)
- `addons/hr_holidays/i18n/zh_TW.po` (5,878 lines)
- `addons/hr_holidays/models/__init__.py` (26 lines)
- `addons/hr_holidays/models/calendar_event.py` (23 lines)
- `addons/hr_holidays/models/hr_department.py` (74 lines)
- `addons/hr_holidays/models/hr_employee.py` (1,056 lines)
- `addons/hr_holidays/models/hr_employee_departure.py` (95 lines)
- `addons/hr_holidays/models/hr_employee_public.py` (69 lines)
- `addons/hr_holidays/models/hr_leave.py` (3,128 lines)
- `addons/hr_holidays/models/hr_leave_accrual_plan.py` (179 lines)
- `addons/hr_holidays/models/hr_leave_accrual_plan_level.py` (421 lines)
- `addons/hr_holidays/models/hr_leave_allocation.py` (1,431 lines)
- `addons/hr_holidays/models/hr_leave_display_name_mixin.py` (78 lines)
- `addons/hr_holidays/models/hr_leave_mandatory_day.py` (26 lines)
- `addons/hr_holidays/models/hr_time_rule.py` (287 lines)
- `addons/hr_holidays/models/hr_time_rule_allocation_log.py` (23 lines)
- `addons/hr_holidays/models/hr_version.py` (449 lines)
- `addons/hr_holidays/models/hr_work_entry_type.py` (785 lines)
- `addons/hr_holidays/models/mail_activity_type.py` (14 lines)
- `addons/hr_holidays/models/mail_message_subtype.py` (50 lines)
- `addons/hr_holidays/models/res_company.py` (31 lines)
- `addons/hr_holidays/models/res_groups.py` (13 lines)
- `addons/hr_holidays/models/res_partner.py` (16 lines)
- `addons/hr_holidays/models/res_users.py` (54 lines)
- `addons/hr_holidays/models/resource_calendar.py` (59 lines)
- `addons/hr_holidays/models/resource_calendar_leaves.py` (277 lines)
- `addons/hr_holidays/models/resource_resource.py` (54 lines)
- `addons/hr_holidays/report/__init__.py` (8 lines)
- `addons/hr_holidays/report/holidays_summary_report.py` (176 lines)
- `addons/hr_holidays/report/hr_holidays_reports.xml` (12 lines)
- `addons/hr_holidays/report/hr_holidays_templates.xml` (84 lines)
- `addons/hr_holidays/report/hr_leave_employee_report.py` (138 lines)
- `addons/hr_holidays/report/hr_leave_employee_report_views.xml` (105 lines)
- `addons/hr_holidays/report/hr_leave_employee_type_report.py` (273 lines)
- `addons/hr_holidays/report/hr_leave_employee_type_report.xml` (41 lines)
- `addons/hr_holidays/report/hr_leave_report.py` (97 lines)
- `addons/hr_holidays/report/hr_leave_report_calendar.py` (183 lines)
- `addons/hr_holidays/report/hr_leave_report_calendar.xml` (181 lines)
- `addons/hr_holidays/report/hr_leave_reports.xml` (112 lines)
- `addons/hr_holidays/security/hr_holidays_security.xml` (46 lines)
- `addons/hr_holidays/security/ir.access.csv` (95 lines)
- `addons/hr_holidays/static/description/icon.png` (13 lines)
- `addons/hr_holidays/static/description/icon.svg` (1 lines)
- `addons/hr_holidays/static/description/icon_hi.png` (97 lines)
- `addons/hr_holidays/static/src/components/accrual_level/accrual_levels.js` (154 lines)
- `addons/hr_holidays/static/src/components/accrual_level/accrual_levels.scss` (133 lines)
- `addons/hr_holidays/static/src/components/accrual_level/accrual_levels.xml` (122 lines)
- `addons/hr_holidays/static/src/components/day_selection/day_selection.js` (46 lines)
- `addons/hr_holidays/static/src/components/hr_leave_chatter_patch/hr_leave_chatter_patch.js` (37 lines)
- `addons/hr_holidays/static/src/components/hr_presence_status/hr_presence_status.js` (107 lines)
- `addons/hr_holidays/static/src/components/selection_badge_with_filter/selection_badge_with_filter.js` (29 lines)
- `addons/hr_holidays/static/src/core/common/@types/models.d.ts` (12 lines)
- `addons/hr_holidays/static/src/core/common/chat_window_patch.js` (12 lines)

Additional files not expanded here: 170. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
