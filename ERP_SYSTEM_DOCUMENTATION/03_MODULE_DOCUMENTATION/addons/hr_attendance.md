# Module: hr_attendance

- **Module ID:** MOD-083
- **Path:** `addons/hr_attendance`
- **Manifest:** `addons/hr_attendance/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Track employee attendance


This module aims to manage employee's attendances.
==================================================

Keeps account of the attendances of the employees on the basis of the
actions(Check in/Check out) performed by them.
       

Declared dependencies: `hr`, `hr_work_entry`, `barcodes`, `base_geolocalize`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 29 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 27 | Client behavior/assets. |
| Tests | 13 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 15 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr",
    "hr_work_entry",
    "barcodes",
    "base_geolocalize"
  ],
  "data": [
    "data/hr_attendance_data.xml",
    "security/hr_attendance_security.xml",
    "views/hr_attendance_view.xml",
    "views/hr_department_view.xml",
    "views/hr_employee_view.xml",
    "views/hr_employee_public_views.xml",
    "views/res_config_settings_views.xml",
    "views/hr_attendance_kiosk_templates.xml",
    "views/hr_version_views.xml",
    "views/hr_contract_template_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_attendance_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_attendance/static/src/**/*.js",
      "hr_attendance/static/src/**/*.xml",
      "hr_attendance/static/src/scss/views/*.scss"
    ],
    "web.assets_unit_tests": [
      "hr_attendance/static/tests/*.test.js"
    ],
    "hr_attendance.assets_public_attendance": [
      "hr_attendance/static/src/scss/kiosk/primary_variables.scss",
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_primary_variables"
      ],
      "hr_attendance/static/src/scss/kiosk/bootstrap_overridden.scss",
      [
        "include",
        "web._assets_frontend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_frontend"
      ],
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      "/web/static/lib/bootstrap/scss/_functions.scss",
      "/web/static/lib/bootstrap/scss/_mixins.scss",
      "/web/static/lib/bootstrap/scss/utilities/_api.scss",
      [
        "include",
        "web.icons_fonts"
      ],
      [
        "include",
        "web._assets_core"
      ],
      "hr_attendance/static/src/public_kiosk/**/*",
      "hr_attendance/static/src/components/attendance_video_stream/**/*",
      "hr_attendance/static/src/components/break_duration_dialog/**/*",
      "hr_attendance/static/src/components/card_layout/**/*",
      "hr_attendance/static/src/components/confirmation/**/*",
      "hr_attendance/static/src/components/greetings/**/*",
      "hr_attendance/static/src/components/hooks/use_camera.js",
      "hr_attendance/static/src/components/kiosk_barcode/**/*",
      "hr_attendance/static/src/components/manual_selection/**/*",
      "hr_attendance/static/src/components/new_employee_dialog/**/*",
      "hr_attendance/static/src/components/pin_code/**/*",
      "hr_attendance/static/src/scss/kiosk/hr_attendance.scss",
      "web/static/src/views/fields/formatters.js",
      "web/static/src/session.js",
      "web/static/src/views/widgets/standard_widget_props.js",
      "web/static/src/views/widgets/documentation_link/*",
      "barcodes/static/src/components/barcode_scanner.js",
      "barcodes/static/src/components/barcode_scanner.xml",
      "barcodes/static/src/components/barcode_scanner.scss",
      "barcodes/static/src/barcode_plugin.js"
    ]
  }
}
```

### Representative source files

- `addons/hr_attendance/__init__.py` (12 lines)
- `addons/hr_attendance/__manifest__.py` (102 lines)
- `addons/hr_attendance/controllers/__init__.py` (3 lines)
- `addons/hr_attendance/controllers/main.py` (522 lines)
- `addons/hr_attendance/data/hr_attendance_data.xml` (40 lines)
- `addons/hr_attendance/data/hr_attendance_demo.xml` (146 lines)
- `addons/hr_attendance/data/scenarios/hr_attendance_scenario.xml` (33 lines)
- `addons/hr_attendance/i18n/af.po` (2,897 lines)
- `addons/hr_attendance/i18n/am.po` (2,893 lines)
- `addons/hr_attendance/i18n/ar.po` (2,908 lines)
- `addons/hr_attendance/i18n/az.po` (2,466 lines)
- `addons/hr_attendance/i18n/bg.po` (2,505 lines)
- `addons/hr_attendance/i18n/bs.po` (2,540 lines)
- `addons/hr_attendance/i18n/ca.po` (2,553 lines)
- `addons/hr_attendance/i18n/cs.po` (2,553 lines)
- `addons/hr_attendance/i18n/da.po` (2,636 lines)
- `addons/hr_attendance/i18n/de.po` (3,026 lines)
- `addons/hr_attendance/i18n/el.po` (2,472 lines)
- `addons/hr_attendance/i18n/es.po` (2,935 lines)
- `addons/hr_attendance/i18n/es_419.po` (3,016 lines)
- `addons/hr_attendance/i18n/es_CL.po` (89 lines)
- `addons/hr_attendance/i18n/et.po` (2,602 lines)
- `addons/hr_attendance/i18n/eu.po` (2,896 lines)
- `addons/hr_attendance/i18n/fa.po` (2,553 lines)
- `addons/hr_attendance/i18n/fi.po` (2,987 lines)
- `addons/hr_attendance/i18n/fo.po` (2,896 lines)
- `addons/hr_attendance/i18n/fr.po` (2,907 lines)
- `addons/hr_attendance/i18n/fr_BE.po` (80 lines)
- `addons/hr_attendance/i18n/fr_CA.po` (84 lines)
- `addons/hr_attendance/i18n/gl.po` (2,896 lines)
- `addons/hr_attendance/i18n/gu.po` (2,901 lines)
- `addons/hr_attendance/i18n/he.po` (2,567 lines)
- `addons/hr_attendance/i18n/hi.po` (2,655 lines)
- `addons/hr_attendance/i18n/hr.po` (2,994 lines)
- `addons/hr_attendance/i18n/hr_attendance.pot` (2,334 lines)
- `addons/hr_attendance/i18n/hu.po` (2,512 lines)
- `addons/hr_attendance/i18n/hy.po` (2,895 lines)
- `addons/hr_attendance/i18n/id.po` (2,907 lines)
- `addons/hr_attendance/i18n/is.po` (2,900 lines)
- `addons/hr_attendance/i18n/it.po` (2,973 lines)
- `addons/hr_attendance/i18n/ja.po` (2,926 lines)
- `addons/hr_attendance/i18n/ka.po` (2,896 lines)
- `addons/hr_attendance/i18n/kab.po` (2,458 lines)
- `addons/hr_attendance/i18n/km.po` (2,898 lines)
- `addons/hr_attendance/i18n/ko.po` (2,752 lines)
- `addons/hr_attendance/i18n/ku.po` (2,414 lines)
- `addons/hr_attendance/i18n/lb.po` (2,898 lines)
- `addons/hr_attendance/i18n/lo.po` (2,671 lines)
- `addons/hr_attendance/i18n/lt.po` (2,514 lines)
- `addons/hr_attendance/i18n/lv.po` (2,557 lines)
- `addons/hr_attendance/i18n/mk.po` (2,896 lines)
- `addons/hr_attendance/i18n/mn.po` (2,660 lines)
- `addons/hr_attendance/i18n/my.po` (2,451 lines)
- `addons/hr_attendance/i18n/nb.po` (2,536 lines)
- `addons/hr_attendance/i18n/nl.po` (3,004 lines)
- `addons/hr_attendance/i18n/pl.po` (2,900 lines)
- `addons/hr_attendance/i18n/pt.po` (2,552 lines)
- `addons/hr_attendance/i18n/pt_BR.po` (3,013 lines)
- `addons/hr_attendance/i18n/ro.po` (2,851 lines)
- `addons/hr_attendance/i18n/ru.po` (2,874 lines)
- `addons/hr_attendance/i18n/sk.po` (2,576 lines)
- `addons/hr_attendance/i18n/sl.po` (2,601 lines)
- `addons/hr_attendance/i18n/sq.po` (2,896 lines)
- `addons/hr_attendance/i18n/sr@latin.po` (2,459 lines)
- `addons/hr_attendance/i18n/sv.po` (2,618 lines)
- `addons/hr_attendance/i18n/ta.po` (2,897 lines)
- `addons/hr_attendance/i18n/th.po` (2,645 lines)
- `addons/hr_attendance/i18n/tr.po` (2,840 lines)
- `addons/hr_attendance/i18n/uk.po` (2,668 lines)
- `addons/hr_attendance/i18n/uz.po` (3,165 lines)
- `addons/hr_attendance/i18n/vi.po` (2,652 lines)
- `addons/hr_attendance/i18n/zh_CN.po` (2,668 lines)
- `addons/hr_attendance/i18n/zh_TW.po` (2,738 lines)
- `addons/hr_attendance/models/__init__.py` (11 lines)
- `addons/hr_attendance/models/hr_attendance.py` (892 lines)
- `addons/hr_attendance/models/hr_employee.py` (443 lines)
- `addons/hr_attendance/models/hr_employee_public.py` (31 lines)
- `addons/hr_attendance/models/hr_time_rule.py` (52 lines)
- `addons/hr_attendance/models/hr_version.py` (55 lines)
- `addons/hr_attendance/models/ir_http.py` (24 lines)
- `addons/hr_attendance/models/ir_websocket.py` (27 lines)
- `addons/hr_attendance/models/res_company.py` (133 lines)
- `addons/hr_attendance/models/res_config_settings.py` (40 lines)
- `addons/hr_attendance/models/res_groups.py` (14 lines)
- `addons/hr_attendance/models/res_users.py` (18 lines)
- `addons/hr_attendance/security/hr_attendance_security.xml` (52 lines)
- `addons/hr_attendance/security/ir.access.csv` (8 lines)
- `addons/hr_attendance/static/description/icon.png` (24 lines)
- `addons/hr_attendance/static/description/icon.svg` (1 lines)
- `addons/hr_attendance/static/description/icon_hi.png` (107 lines)
- `addons/hr_attendance/static/img/attendance_dot.gif` (670 lines)
- `addons/hr_attendance/static/img/background-light.svg` (35 lines)
- `addons/hr_attendance/static/img/employee_awa-image.jpg` (67 lines)
- `addons/hr_attendance/static/img/mock-tablet.png` (145 lines)
- `addons/hr_attendance/static/img/partner_root-image.jpg` (35 lines)
- `addons/hr_attendance/static/img/tablet-cam.svg` (56 lines)
- `addons/hr_attendance/static/img/tablet-pin.svg` (38 lines)
- `addons/hr_attendance/static/img/tablet-rfid.svg` (24 lines)
- `addons/hr_attendance/static/src/components/attendance_calendar/attendance_calendar_overview.js` (46 lines)
- `addons/hr_attendance/static/src/components/attendance_calendar/attendance_calendar_overview.xml` (20 lines)
- `addons/hr_attendance/static/src/components/attendance_inline_form/attendance_inline_form.js` (16 lines)
- `addons/hr_attendance/static/src/components/attendance_inline_form/attendance_inline_form.xml` (47 lines)
- `addons/hr_attendance/static/src/components/attendance_menu/attendance_menu.js` (452 lines)
- `addons/hr_attendance/static/src/components/attendance_menu/attendance_menu.xml` (169 lines)
- `addons/hr_attendance/static/src/components/attendance_video_stream/attendance_video_steam.xml` (12 lines)
- `addons/hr_attendance/static/src/components/attendance_video_stream/attendance_video_stream.js` (41 lines)
- `addons/hr_attendance/static/src/components/break_duration_dialog/break_duration_dialog.js` (55 lines)
- `addons/hr_attendance/static/src/components/break_duration_dialog/break_duration_dialog.xml` (35 lines)
- `addons/hr_attendance/static/src/components/card_layout/card_layout.js` (37 lines)
- `addons/hr_attendance/static/src/components/card_layout/card_layout.xml` (58 lines)
- `addons/hr_attendance/static/src/components/confirmation/confirmation.js` (46 lines)
- `addons/hr_attendance/static/src/components/confirmation/confirmation.xml` (68 lines)
- `addons/hr_attendance/static/src/components/greetings/greetings.js` (56 lines)
- `addons/hr_attendance/static/src/components/greetings/greetings.xml` (108 lines)
- `addons/hr_attendance/static/src/components/hooks/use_camera.js` (78 lines)
- `addons/hr_attendance/static/src/components/hr_presence_status/hr_attendance_presence_status.js` (61 lines)
- `addons/hr_attendance/static/src/components/kiosk_barcode/kiosk_barcode.js` (50 lines)
- `addons/hr_attendance/static/src/components/manual_selection/manual_selection.js` (132 lines)
- `addons/hr_attendance/static/src/components/manual_selection/manual_selection.xml` (100 lines)
- `addons/hr_attendance/static/src/components/new_employee_dialog/many2one/many2one.js` (49 lines)
- `addons/hr_attendance/static/src/components/new_employee_dialog/many2one/many2one.xml` (33 lines)
- `addons/hr_attendance/static/src/components/new_employee_dialog/new_employee_dialog.js` (102 lines)
- `addons/hr_attendance/static/src/components/new_employee_dialog/new_employee_dialog.xml` (39 lines)
- `addons/hr_attendance/static/src/components/pin_code/pin_code.js` (85 lines)
- `addons/hr_attendance/static/src/components/pin_code/pin_code.xml` (70 lines)
- `addons/hr_attendance/static/src/public_kiosk/public_kiosk_app.js` (351 lines)
- `addons/hr_attendance/static/src/public_kiosk/public_kiosk_app.xml` (202 lines)
- `addons/hr_attendance/static/src/scss/kiosk/bootstrap_overridden.scss` (9 lines)
- `addons/hr_attendance/static/src/scss/kiosk/hr_attendance.scss` (190 lines)
- `addons/hr_attendance/static/src/scss/kiosk/primary_variables.scss` (5 lines)
- `addons/hr_attendance/static/src/scss/views/attendance_calendar.scss` (33 lines)
- `addons/hr_attendance/static/src/scss/views/badge_scanner.scss` (51 lines)
- `addons/hr_attendance/static/src/scss/views/hr_attendance.scss` (30 lines)
- `addons/hr_attendance/static/src/views/attendance_helper_view.js` (46 lines)
- `addons/hr_attendance/static/src/views/attendance_helper_view.xml` (108 lines)
- `addons/hr_attendance/static/src/views/attendance_list_view.js` (40 lines)
- `addons/hr_attendance/static/src/views/attendance_list_view.xml` (11 lines)
- `addons/hr_attendance/static/src/views/badge_scanner/badge_scanner.js` (51 lines)
- `addons/hr_attendance/static/src/views/badge_scanner/badge_scanner.xml` (24 lines)
- `addons/hr_attendance/static/src/views/calendar/attendance_calendar_controller.js` (47 lines)
- `addons/hr_attendance/static/src/views/calendar/attendance_calendar_renderer.js` (36 lines)
- `addons/hr_attendance/static/src/views/calendar/attendance_calendar_renderer.xml` (9 lines)
- `addons/hr_attendance/static/src/views/calendar/attendance_calendar_view.js` (12 lines)
- `addons/hr_attendance/static/tests/attendance_calendar_overview.test.js` (52 lines)
- `addons/hr_attendance/static/tests/attendance_menu.test.js` (471 lines)
- `addons/hr_attendance/static/tests/employee_presence_state.test.js` (70 lines)
- `addons/hr_attendance/static/tests/greetings.test.js` (169 lines)
- `addons/hr_attendance/static/tests/hr_attendance_kiosk_barcode_scanner.test.js` (37 lines)
- `addons/hr_attendance/tests/__init__.py` (12 lines)
- `addons/hr_attendance/tests/test_hr_attendance_access_rights.py` (29 lines)
- `addons/hr_attendance/tests/test_hr_attendance_constraints.py` (114 lines)
- `addons/hr_attendance/tests/test_hr_attendance_domain_translation.py` (32 lines)
- `addons/hr_attendance/tests/test_hr_attendance_kiosk.py` (171 lines)
- `addons/hr_attendance/tests/test_hr_attendance_manager.py` (128 lines)
- `addons/hr_attendance/tests/test_hr_attendance_process.py` (721 lines)
- `addons/hr_attendance/tests/test_hr_attendance_self_edit_role.py` (126 lines)
- `addons/hr_attendance/tests/test_hr_attendance_systray.py` (54 lines)
- `addons/hr_attendance/tests/test_hr_attendance_work_entry_type_domain.py` (94 lines)
- `addons/hr_attendance/tests/test_hr_time_rule_pipeline.py` (536 lines)
- `addons/hr_attendance/tests/test_load_scenario.py` (8 lines)

Additional files not expanded here: 9. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
