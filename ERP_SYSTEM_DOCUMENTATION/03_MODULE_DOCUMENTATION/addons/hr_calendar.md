# Module: hr_calendar

- **Module ID:** MOD-084
- **Path:** `addons/hr_calendar`
- **Manifest:** `addons/hr_calendar/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `hr`, `calendar`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "calendar"
  ],
  "data": [
    "views/calendar_views.xml",
    "views/calendar_views_calendarApp.xml",
    "views/res_partner_views.xml",
    "wizard/homework_location_wizard.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_calendar/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_calendar/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_calendar/__init__.py` (4 lines)
- `addons/hr_calendar/__manifest__.py` (25 lines)
- `addons/hr_calendar/i18n/ar.po` (236 lines)
- `addons/hr_calendar/i18n/az.po` (233 lines)
- `addons/hr_calendar/i18n/bg.po` (233 lines)
- `addons/hr_calendar/i18n/bs.po` (235 lines)
- `addons/hr_calendar/i18n/ca.po` (234 lines)
- `addons/hr_calendar/i18n/cs.po` (237 lines)
- `addons/hr_calendar/i18n/da.po` (235 lines)
- `addons/hr_calendar/i18n/de.po` (246 lines)
- `addons/hr_calendar/i18n/el.po` (234 lines)
- `addons/hr_calendar/i18n/es.po` (236 lines)
- `addons/hr_calendar/i18n/es_419.po` (245 lines)
- `addons/hr_calendar/i18n/et.po` (233 lines)
- `addons/hr_calendar/i18n/fa.po` (233 lines)
- `addons/hr_calendar/i18n/fi.po` (235 lines)
- `addons/hr_calendar/i18n/fr.po` (247 lines)
- `addons/hr_calendar/i18n/he.po` (234 lines)
- `addons/hr_calendar/i18n/hi.po` (233 lines)
- `addons/hr_calendar/i18n/hr.po` (234 lines)
- `addons/hr_calendar/i18n/hr_calendar.pot` (230 lines)
- `addons/hr_calendar/i18n/hu.po` (234 lines)
- `addons/hr_calendar/i18n/id.po` (246 lines)
- `addons/hr_calendar/i18n/it.po` (246 lines)
- `addons/hr_calendar/i18n/ja.po` (245 lines)
- `addons/hr_calendar/i18n/kab.po` (234 lines)
- `addons/hr_calendar/i18n/ko.po` (238 lines)
- `addons/hr_calendar/i18n/ku.po` (233 lines)
- `addons/hr_calendar/i18n/lo.po` (235 lines)
- `addons/hr_calendar/i18n/lt.po` (235 lines)
- `addons/hr_calendar/i18n/lv.po` (234 lines)
- `addons/hr_calendar/i18n/mn.po` (233 lines)
- `addons/hr_calendar/i18n/my.po` (234 lines)
- `addons/hr_calendar/i18n/nb.po` (234 lines)
- `addons/hr_calendar/i18n/nl.po` (245 lines)
- `addons/hr_calendar/i18n/pl.po` (236 lines)
- `addons/hr_calendar/i18n/pt.po` (234 lines)
- `addons/hr_calendar/i18n/pt_BR.po` (249 lines)
- `addons/hr_calendar/i18n/ro.po` (235 lines)
- `addons/hr_calendar/i18n/ru.po` (236 lines)
- `addons/hr_calendar/i18n/sk.po` (233 lines)
- `addons/hr_calendar/i18n/sl.po` (235 lines)
- `addons/hr_calendar/i18n/sr@latin.po` (235 lines)
- `addons/hr_calendar/i18n/sv.po` (235 lines)
- `addons/hr_calendar/i18n/th.po` (235 lines)
- `addons/hr_calendar/i18n/tr.po` (236 lines)
- `addons/hr_calendar/i18n/uk.po` (234 lines)
- `addons/hr_calendar/i18n/uz.po` (247 lines)
- `addons/hr_calendar/i18n/vi.po` (235 lines)
- `addons/hr_calendar/i18n/zh_CN.po` (241 lines)
- `addons/hr_calendar/i18n/zh_TW.po` (237 lines)
- `addons/hr_calendar/models/__init__.py` (5 lines)
- `addons/hr_calendar/models/calendar_event.py` (97 lines)
- `addons/hr_calendar/models/hr_employee.py` (50 lines)
- `addons/hr_calendar/models/res_partner.py` (259 lines)
- `addons/hr_calendar/security/ir.access.csv` (5 lines)
- `addons/hr_calendar/static/src/calendar/common/calendar_common_renderer.js` (106 lines)
- `addons/hr_calendar/static/src/calendar/common/calendar_common_renderer.scss` (67 lines)
- `addons/hr_calendar/static/src/calendar/common/calendar_common_renderer.xml` (61 lines)
- `addons/hr_calendar/static/src/calendar/common/calendar_model.js` (239 lines)
- `addons/hr_calendar/static/src/calendar/common/calendar_year_renderer.js` (6 lines)
- `addons/hr_calendar/static/src/calendar/common/hr_homeworking_calendar_controller.js` (110 lines)
- `addons/hr_calendar/static/src/calendar/common/popover/calendar_common_popover.js` (67 lines)
- `addons/hr_calendar/static/src/calendar/common/popover/calendar_common_popover.xml` (60 lines)
- `addons/hr_calendar/static/tests/calendar_homeworking.test.js` (347 lines)
- `addons/hr_calendar/tests/__init__.py` (6 lines)
- `addons/hr_calendar/tests/common.py` (214 lines)
- `addons/hr_calendar/tests/test_event_interval.py` (124 lines)
- `addons/hr_calendar/tests/test_hr_employee_location.py` (183 lines)
- `addons/hr_calendar/tests/test_working_days.py` (534 lines)
- `addons/hr_calendar/tests/test_working_hours.py` (627 lines)
- `addons/hr_calendar/views/calendar_views.xml` (8 lines)
- `addons/hr_calendar/views/calendar_views_calendarApp.xml` (16 lines)
- `addons/hr_calendar/views/res_partner_views.xml` (14 lines)
- `addons/hr_calendar/wizard/__init__.py` (3 lines)
- `addons/hr_calendar/wizard/homework_location_wizard.py` (80 lines)
- `addons/hr_calendar/wizard/homework_location_wizard.xml` (56 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
