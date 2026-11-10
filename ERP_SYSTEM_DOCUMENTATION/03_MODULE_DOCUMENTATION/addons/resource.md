# Module: resource

- **Module ID:** MOD-506
- **Path:** `addons/resource`
- **Manifest:** `addons/resource/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Module for resource management.
===============================

A resource represent something that can be scheduled (a developer on a task or a
work center on manufacturing orders). This module manages a resource calendar
associated to every resource. It also manages the leaves of every resource.
    

Declared dependencies: `base`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 27 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web"
  ],
  "data": [
    "data/resource_data.xml",
    "data/ir_cron.xml",
    "views/resource_resource_views.xml",
    "views/res_company_views.xml",
    "views/resource_calendar_leaves_views.xml",
    "views/resource_calendar_attendance_views.xml",
    "views/resource_calendar_views.xml",
    "views/menuitems.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/resource_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "resource/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "resource/static/tests/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      "resource/static/tests/mock_server/**/*"
    ]
  }
}
```

### Representative source files

- `addons/resource/__init__.py` (4 lines)
- `addons/resource/__manifest__.py` (43 lines)
- `addons/resource/data/ir_cron.xml` (13 lines)
- `addons/resource/data/resource_data.xml` (19 lines)
- `addons/resource/data/resource_demo.xml` (18 lines)
- `addons/resource/i18n/af.po` (970 lines)
- `addons/resource/i18n/am.po` (966 lines)
- `addons/resource/i18n/ar.po` (1,115 lines)
- `addons/resource/i18n/az.po` (1,054 lines)
- `addons/resource/i18n/bg.po` (1,065 lines)
- `addons/resource/i18n/bs.po` (1,044 lines)
- `addons/resource/i18n/ca.po` (1,131 lines)
- `addons/resource/i18n/cs.po` (1,100 lines)
- `addons/resource/i18n/da.po` (1,099 lines)
- `addons/resource/i18n/de.po` (1,227 lines)
- `addons/resource/i18n/el.po` (1,073 lines)
- `addons/resource/i18n/es.po` (1,144 lines)
- `addons/resource/i18n/es_419.po` (1,212 lines)
- `addons/resource/i18n/es_CL.po` (173 lines)
- `addons/resource/i18n/et.po` (1,096 lines)
- `addons/resource/i18n/eu.po` (969 lines)
- `addons/resource/i18n/fa.po` (1,102 lines)
- `addons/resource/i18n/fi.po` (1,140 lines)
- `addons/resource/i18n/fo.po` (968 lines)
- `addons/resource/i18n/fr.po` (1,207 lines)
- `addons/resource/i18n/fr_BE.po` (149 lines)
- `addons/resource/i18n/fr_CA.po` (155 lines)
- `addons/resource/i18n/gl.po` (973 lines)
- `addons/resource/i18n/gu.po` (972 lines)
- `addons/resource/i18n/he.po` (1,093 lines)
- `addons/resource/i18n/hi.po` (1,057 lines)
- `addons/resource/i18n/hr.po` (1,093 lines)
- `addons/resource/i18n/hu.po` (1,083 lines)
- `addons/resource/i18n/id.po` (1,151 lines)
- `addons/resource/i18n/is.po` (972 lines)
- `addons/resource/i18n/it.po` (1,212 lines)
- `addons/resource/i18n/ja.po` (1,174 lines)
- `addons/resource/i18n/ka.po` (968 lines)
- `addons/resource/i18n/kab.po` (1,033 lines)
- `addons/resource/i18n/kk.po` (968 lines)
- `addons/resource/i18n/km.po` (972 lines)
- `addons/resource/i18n/ko.po` (1,140 lines)
- `addons/resource/i18n/ku.po` (1,036 lines)
- `addons/resource/i18n/ln.po` (968 lines)
- `addons/resource/i18n/lo.po` (1,072 lines)
- `addons/resource/i18n/lt.po` (1,078 lines)
- `addons/resource/i18n/lv.po` (1,048 lines)
- `addons/resource/i18n/mk.po` (975 lines)
- `addons/resource/i18n/mn.po` (1,070 lines)
- `addons/resource/i18n/my.po` (1,043 lines)
- `addons/resource/i18n/nb.po` (1,067 lines)
- `addons/resource/i18n/nl.po` (1,225 lines)
- `addons/resource/i18n/pl.po` (1,204 lines)
- `addons/resource/i18n/pt.po` (1,113 lines)
- `addons/resource/i18n/pt_BR.po` (1,222 lines)
- `addons/resource/i18n/resource.pot` (1,026 lines)
- `addons/resource/i18n/ro.po` (1,125 lines)
- `addons/resource/i18n/ru.po` (1,124 lines)
- `addons/resource/i18n/sk.po` (1,063 lines)
- `addons/resource/i18n/sl.po` (1,089 lines)
- `addons/resource/i18n/sq.po` (968 lines)
- `addons/resource/i18n/sr@latin.po` (1,050 lines)
- `addons/resource/i18n/sv.po` (1,121 lines)
- `addons/resource/i18n/ta.po` (970 lines)
- `addons/resource/i18n/th.po` (1,101 lines)
- `addons/resource/i18n/tr.po` (1,174 lines)
- `addons/resource/i18n/uk.po` (1,098 lines)
- `addons/resource/i18n/uz.po` (1,295 lines)
- `addons/resource/i18n/vi.po` (1,131 lines)
- `addons/resource/i18n/zh_CN.po` (1,126 lines)
- `addons/resource/i18n/zh_TW.po` (1,100 lines)
- `addons/resource/models/__init__.py` (11 lines)
- `addons/resource/models/res_company.py` (72 lines)
- `addons/resource/models/res_users.py` (14 lines)
- `addons/resource/models/resource_calendar.py` (1,165 lines)
- `addons/resource/models/resource_calendar_attendance.py` (515 lines)
- `addons/resource/models/resource_calendar_leaves.py` (87 lines)
- `addons/resource/models/resource_mixin.py` (252 lines)
- `addons/resource/models/resource_resource.py` (540 lines)
- `addons/resource/models/utils.py` (256 lines)
- `addons/resource/security/ir.access.csv` (11 lines)
- `addons/resource/static/src/components/resource_avatar/resource_avatar.js` (20 lines)
- `addons/resource/static/src/components/resource_avatar/resource_avatar.scss` (4 lines)
- `addons/resource/static/src/components/resource_avatar/resource_avatar.xml` (13 lines)
- `addons/resource/static/src/components/resource_calendar_attendance_popover/resource_calendar_attendance_popover.js` (201 lines)
- `addons/resource/static/src/components/resource_calendar_attendance_popover/resource_calendar_attendance_popover.xml` (96 lines)
- `addons/resource/static/src/plugins/resource_calendar_attendance_popover_loader.js` (36 lines)
- `addons/resource/static/src/plugins/resource_calendar_plugin.js` (21 lines)
- `addons/resource/static/src/scss/resource_form.scss` (15 lines)
- `addons/resource/static/src/scss/resource_list.scss` (5 lines)
- `addons/resource/static/src/views/fields/calendar_type_confirm_radio/calendar_type_confirm_radio_field.js` (57 lines)
- `addons/resource/static/src/views/fields/resource_calendar_attendance_calendar_one2many/resource_calendar_attendance_calendar_one2many_field.js` (51 lines)
- `addons/resource/static/src/views/fields/resource_calendar_attendance_calendar_one2many/resource_calendar_attendance_calendar_one2many_field.xml` (6 lines)
- `addons/resource/static/src/views/fields/resource_calendar_attendance_filtered_one2many/resource_calendar_attendance_filtered_one2many.js` (51 lines)
- `addons/resource/static/src/views/fields/resource_calendar_hours_by_day/resource_calendar_hours_by_day.js` (80 lines)
- `addons/resource/static/src/views/fields/resource_calendar_hours_by_day/resource_calendar_hours_by_day.xml` (13 lines)
- `addons/resource/static/src/views/fields/resource_calendar_many2one/resource_calendar_many2one.js` (80 lines)
- `addons/resource/static/src/views/fields/resource_calendar_many2one/resource_calendar_many2one.xml` (27 lines)
- `addons/resource/static/src/views/form_with_html_expander/form_controller_with_html_expander.js` (39 lines)
- `addons/resource/static/src/views/form_with_html_expander/form_controller_with_html_expander.xml` (11 lines)
- `addons/resource/static/src/views/form_with_html_expander/form_renderer_with_html_expander.js` (63 lines)
- `addons/resource/static/src/views/form_with_html_expander/form_view_with_html_expander.js` (12 lines)
- `addons/resource/static/src/views/resource_calendar_attendance_calendar/resource_calendar_attendance_calendar_common_renderer.js` (252 lines)
- `addons/resource/static/src/views/resource_calendar_attendance_calendar/resource_calendar_attendance_calendar_controller.js` (18 lines)
- `addons/resource/static/src/views/resource_calendar_attendance_calendar/resource_calendar_attendance_calendar_model.js` (194 lines)
- `addons/resource/static/src/views/resource_calendar_attendance_calendar/resource_calendar_attendance_calendar_renderer.js` (10 lines)
- `addons/resource/static/src/views/resource_calendar_attendance_calendar/resource_calendar_attendance_calendar_view.js` (16 lines)
- `addons/resource/static/src/views/view_components/resource_multi_selection_buttons.js` (14 lines)
- `addons/resource/static/tests/mock_server/mock_models/resource_calendar.js` (24 lines)
- `addons/resource/static/tests/mock_server/mock_models/resource_calendar_attendance.js` (48 lines)
- `addons/resource/static/tests/mock_server/mock_models/resource_resource.js` (5 lines)
- `addons/resource/static/tests/mock_server/mock_models/resource_task.js` (10 lines)
- `addons/resource/static/tests/resource_avatar.test.js` (35 lines)
- `addons/resource/static/tests/resource_test_helpers.js` (16 lines)
- `addons/resource/static/tests/views/fields/calendar_one2many_field.test.js` (40 lines)
- `addons/resource/static/tests/views/fields/calendar_type_confirm_radio_field.test.js` (31 lines)
- `addons/resource/static/tests/views/resource_calendar_attendance_calendar_view.test.js` (616 lines)
- `addons/resource/tests/__init__.py` (10 lines)
- `addons/resource/tests/test_filter_map_domain.py` (467 lines)
- `addons/resource/tests/test_flexible_resource_calendar.py` (222 lines)
- `addons/resource/tests/test_performance.py` (36 lines)
- `addons/resource/tests/test_resource_calendar.py` (356 lines)
- `addons/resource/tests/test_stress_check_collision.py` (373 lines)
- `addons/resource/tests/test_utils.py` (51 lines)
- `addons/resource/tests/test_variable_resource_calendar.py` (581 lines)
- `addons/resource/views/menuitems.xml` (18 lines)
- `addons/resource/views/res_company_views.xml` (13 lines)
- `addons/resource/views/resource_calendar_attendance_views.xml` (87 lines)
- `addons/resource/views/resource_calendar_leaves_views.xml` (110 lines)
- `addons/resource/views/resource_calendar_views.xml` (116 lines)
- `addons/resource/views/resource_resource_views.xml` (107 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
