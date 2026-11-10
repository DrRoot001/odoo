# Module: hr

- **Module ID:** MOD-081
- **Path:** `addons/hr`
- **Manifest:** `addons/hr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Centralize employee information

No manifest description declared.

Declared dependencies: `auth_signup`, `base_setup`, `digest`, `phone_validation`, `resource_mail`, `web_hierarchy`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 70 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 30 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 55 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 79 | Client behavior/assets. |
| Tests | 28 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_signup",
    "base_setup",
    "digest",
    "phone_validation",
    "resource_mail",
    "web_hierarchy"
  ],
  "data": [
    "security/hr_security.xml",
    "data/digest_data.xml",
    "data/report_paperformat.xml",
    "wizard/mail_activity_schedule_views.xml",
    "wizard/hr_bank_account_allocation_wizard.xml",
    "wizard/hr_bank_account_allocation_wizard_line.xml",
    "wizard/hr_employee_create_version_wizard.xml",
    "views/mail_activity_plan_views.xml",
    "views/hr_version_views.xml",
    "views/hr_contract_template_views.xml",
    "views/hr_departure_reason_views.xml",
    "views/hr_employee_type_views.xml",
    "views/hr_job_views.xml",
    "views/hr_employee_category_views.xml",
    "views/hr_employee_public_views.xml",
    "report/hr_employee_badge.xml",
    "views/hr_employee_views.xml",
    "views/hr_employee_departure_views.xml",
    "views/hr_department_views.xml",
    "views/hr_work_location_views.xml",
    "views/hr_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/res_partner_bank_views.xml",
    "views/discuss_channel_views.xml",
    "views/res_users.xml",
    "views/hr_templates.xml",
    "views/resource_resource_views.xml",
    "views/resource_calendar_views.xml",
    "data/hr_data.xml",
    "data/ir_cron_data.xml",
    "data/hr_employee_type_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_demo.xml"
  ],
  "assets": {
    "web._assets_primary_variables": [
      "hr/static/src/scss/variables.scss"
    ],
    "web.assets_backend": [
      "hr/static/src/core/common/**/*",
      "hr/static/src/core/web/**/*",
      "hr/static/src/**/*",
      [
        "remove",
        "hr/static/src/views/hr_employee_hierarchy/*"
      ]
    ],
    "web.assets_backend_lazy": [
      "hr/static/src/views/hr_employee_hierarchy/*"
    ],
    "im_livechat.assets_embed_core": [
      "hr/static/src/core/common/**/*"
    ],
    "im_livechat.embed_assets_unit_tests_setup": [
      "hr/static/tests/hr_test_helpers.js",
      "hr/static/tests/mock_server/**/*"
    ],
    "mail.assets_public": [
      "hr/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "hr/static/src/core/common/**/*"
    ],
    "web.assets_unit_tests": [
      "hr/static/tests/**/*",
      [
        "remove",
        "hr/static/tests/tours/**/*"
      ],
      [
        "remove",
        "hr/static/tests/legacy/**/*"
      ]
    ],
    "web.assets_tests": [
      "hr/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr/README.md` (92 lines)
- `addons/hr/__init__.py` (14 lines)
- `addons/hr/__manifest__.py` (101 lines)
- `addons/hr/controllers/__init__.py` (2 lines)
- `addons/hr/controllers/hr_org_chart.py` (97 lines)
- `addons/hr/controllers/webclient.py` (18 lines)
- `addons/hr/data/digest_data.xml` (17 lines)
- `addons/hr/data/hr_data.xml` (154 lines)
- `addons/hr/data/hr_demo.xml` (906 lines)
- `addons/hr/data/hr_employee_type_data.xml` (44 lines)
- `addons/hr/data/ir_cron_data.xml` (13 lines)
- `addons/hr/data/report_paperformat.xml` (15 lines)
- `addons/hr/data/scenarios/hr_scenario.xml` (180 lines)
- `addons/hr/i18n/af.po` (6,608 lines)
- `addons/hr/i18n/am.po` (6,604 lines)
- `addons/hr/i18n/ar.po` (6,779 lines)
- `addons/hr/i18n/az.po` (6,626 lines)
- `addons/hr/i18n/bg.po` (6,670 lines)
- `addons/hr/i18n/bs.po` (6,595 lines)
- `addons/hr/i18n/ca.po` (6,687 lines)
- `addons/hr/i18n/cs.po` (6,663 lines)
- `addons/hr/i18n/da.po` (6,792 lines)
- `addons/hr/i18n/de.po` (7,141 lines)
- `addons/hr/i18n/el.po` (6,633 lines)
- `addons/hr/i18n/en_AU.po` (22 lines)
- `addons/hr/i18n/es.po` (6,873 lines)
- `addons/hr/i18n/es_419.po` (7,113 lines)
- `addons/hr/i18n/es_CL.po` (191 lines)
- `addons/hr/i18n/et.po` (6,709 lines)
- `addons/hr/i18n/eu.po` (6,607 lines)
- `addons/hr/i18n/fa.po` (6,757 lines)
- `addons/hr/i18n/fi.po` (6,960 lines)
- `addons/hr/i18n/fo.po` (6,607 lines)
- `addons/hr/i18n/fr.po` (6,944 lines)
- `addons/hr/i18n/fr_CA.po` (179 lines)
- `addons/hr/i18n/gl.po` (6,607 lines)
- `addons/hr/i18n/gu.po` (6,616 lines)
- `addons/hr/i18n/he.po` (6,661 lines)
- `addons/hr/i18n/hi.po` (6,748 lines)
- `addons/hr/i18n/hr.po` (6,667 lines)
- `addons/hr/i18n/hr.pot` (6,529 lines)
- `addons/hr/i18n/hu.po` (6,644 lines)
- `addons/hr/i18n/id.po` (7,017 lines)
- `addons/hr/i18n/is.po` (6,616 lines)
- `addons/hr/i18n/it.po` (7,052 lines)
- `addons/hr/i18n/ja.po` (6,867 lines)
- `addons/hr/i18n/ka.po` (6,607 lines)
- `addons/hr/i18n/kab.po` (6,587 lines)
- `addons/hr/i18n/km.po` (6,610 lines)
- `addons/hr/i18n/ko.po` (6,746 lines)
- `addons/hr/i18n/ku.po` (6,597 lines)
- `addons/hr/i18n/lb.po` (6,609 lines)
- `addons/hr/i18n/lo.po` (6,874 lines)
- `addons/hr/i18n/lt.po` (6,637 lines)
- `addons/hr/i18n/lv.po` (6,614 lines)
- `addons/hr/i18n/mk.po` (6,607 lines)
- `addons/hr/i18n/mn.po` (7,024 lines)
- `addons/hr/i18n/my.po` (6,592 lines)
- `addons/hr/i18n/nb.po` (6,626 lines)
- `addons/hr/i18n/nl.po` (7,088 lines)
- `addons/hr/i18n/pl.po` (6,858 lines)
- `addons/hr/i18n/pt.po` (6,811 lines)
- `addons/hr/i18n/pt_BR.po` (7,112 lines)
- `addons/hr/i18n/ro.po` (6,830 lines)
- `addons/hr/i18n/ru.po` (6,833 lines)
- `addons/hr/i18n/sk.po` (6,643 lines)
- `addons/hr/i18n/sl.po` (6,768 lines)
- `addons/hr/i18n/sq.po` (6,607 lines)
- `addons/hr/i18n/sr@latin.po` (6,632 lines)
- `addons/hr/i18n/sv.po` (6,754 lines)
- `addons/hr/i18n/th.po` (6,923 lines)
- `addons/hr/i18n/tr.po` (6,841 lines)
- `addons/hr/i18n/uk.po` (6,685 lines)
- `addons/hr/i18n/uz.po` (7,564 lines)
- `addons/hr/i18n/vi.po` (6,796 lines)
- `addons/hr/i18n/zh_CN.po` (6,916 lines)
- `addons/hr/i18n/zh_TW.po` (6,719 lines)
- `addons/hr/models/__init__.py` (31 lines)
- `addons/hr/models/discuss_channel.py` (35 lines)
- `addons/hr/models/hr_department.py` (257 lines)
- `addons/hr/models/hr_departure_reason.py` (30 lines)
- `addons/hr/models/hr_employee.py` (3,231 lines)
- `addons/hr/models/hr_employee_category.py` (24 lines)
- `addons/hr/models/hr_employee_departure.py` (281 lines)
- `addons/hr/models/hr_employee_location.py` (29 lines)
- `addons/hr/models/hr_employee_public.py` (292 lines)
- `addons/hr/models/hr_employee_type.py` (72 lines)
- `addons/hr/models/hr_job.py` (72 lines)
- `addons/hr/models/hr_mixin.py` (26 lines)
- `addons/hr/models/hr_payroll_structure_type.py` (20 lines)
- `addons/hr/models/hr_version.py` (972 lines)
- `addons/hr/models/hr_work_location.py` (50 lines)
- `addons/hr/models/ir_ui_menu.py` (17 lines)
- `addons/hr/models/mail_activity.py` (12 lines)
- `addons/hr/models/mail_activity_plan.py` (45 lines)
- `addons/hr/models/mail_activity_plan_template.py` (90 lines)
- `addons/hr/models/mail_alias.py` (17 lines)
- `addons/hr/models/models.py` (21 lines)
- `addons/hr/models/res_company.py` (21 lines)
- `addons/hr/models/res_config_settings.py` (27 lines)
- `addons/hr/models/res_partner.py` (119 lines)
- `addons/hr/models/res_partner_bank.py` (70 lines)
- `addons/hr/models/res_users.py` (417 lines)
- `addons/hr/models/resource.py` (220 lines)
- `addons/hr/models/resource_calendar.py` (117 lines)
- `addons/hr/models/resource_calendar_leaves.py` (41 lines)
- `addons/hr/models/update.py` (16 lines)
- `addons/hr/report/__init__.py` (3 lines)
- `addons/hr/report/hr_employee_badge.xml` (59 lines)
- `addons/hr/report/hr_manager_department_report.py` (33 lines)
- `addons/hr/security/hr_security.xml` (35 lines)
- `addons/hr/security/ir.access.csv` (55 lines)
- `addons/hr/static/description/icon.png` (20 lines)
- `addons/hr/static/description/icon.svg` (1 lines)
- `addons/hr/static/description/icon_hi.png` (81 lines)
- `addons/hr/static/img/employee-image.webp` (27 lines)
- `addons/hr/static/img/employee_admin-image.webp` (30 lines)
- `addons/hr/static/img/employee_al-image.webp` (48 lines)
- `addons/hr/static/img/employee_awa-image.webp` (36 lines)
- `addons/hr/static/img/employee_chs-image.webp` (33 lines)
- `addons/hr/static/img/employee_fme-image.webp` (40 lines)
- `addons/hr/static/img/employee_fpi-image.webp` (25 lines)
- `addons/hr/static/img/employee_han-image.webp` (28 lines)
- `addons/hr/static/img/employee_hne-image.webp` (33 lines)
- `addons/hr/static/img/employee_jep-image.webp` (26 lines)
- `addons/hr/static/img/employee_jgo-image.webp` (24 lines)
- `addons/hr/static/img/employee_jod-image.webp` (41 lines)
- `addons/hr/static/img/employee_jog-image.webp` (22 lines)
- `addons/hr/static/img/employee_jth-image.webp` (37 lines)
- `addons/hr/static/img/employee_jve-image.webp` (26 lines)
- `addons/hr/static/img/employee_lur-image.webp` (24 lines)
- `addons/hr/static/img/employee_md-image.webp` (28 lines)
- `addons/hr/static/img/employee_mit-image.webp` (41 lines)
- `addons/hr/static/img/employee_ngh-image.webp` (39 lines)
- `addons/hr/static/img/employee_niv-image.webp` (43 lines)
- `addons/hr/static/img/employee_qdp-image.webp` (33 lines)
- `addons/hr/static/img/employee_stw-image.webp` (37 lines)
- `addons/hr/static/img/employee_vad-image.webp` (23 lines)
- `addons/hr/static/src/components/background_image/background_image.js` (14 lines)
- `addons/hr/static/src/components/background_image/background_image.scss` (21 lines)
- `addons/hr/static/src/components/background_image/background_image.xml` (13 lines)
- `addons/hr/static/src/components/button_new_contract/button_new_contract.js` (73 lines)
- `addons/hr/static/src/components/button_new_contract/button_new_contract.xml` (9 lines)
- `addons/hr/static/src/components/contract_end_dialog/contract_end_dialog.js` (65 lines)
- `addons/hr/static/src/components/contract_end_dialog/contract_end_dialog.xml` (81 lines)
- `addons/hr/static/src/components/department_chart/department_chart.js` (41 lines)
- `addons/hr/static/src/components/department_chart/department_chart.scss` (16 lines)
- `addons/hr/static/src/components/department_chart/department_chart.xml` (48 lines)
- `addons/hr/static/src/components/employee_user_status/employee_user_status.js` (124 lines)
- `addons/hr/static/src/components/employee_user_status/employee_user_status.scss` (4 lines)
- `addons/hr/static/src/components/employee_user_status/employee_user_status.xml` (20 lines)
- `addons/hr/static/src/components/employee_user_status/user_deactivation_dialog.js` (28 lines)
- `addons/hr/static/src/components/employee_user_status/user_deactivation_dialog.xml` (20 lines)
- `addons/hr/static/src/components/float_time_selection/float_time_selection.js` (105 lines)
- `addons/hr/static/src/components/float_time_selection/float_time_selection.xml` (10 lines)
- `addons/hr/static/src/components/float_time_selection/float_time_selection_popover.js` (35 lines)
- `addons/hr/static/src/components/float_time_selection/float_time_selection_popover.xml` (18 lines)
- `addons/hr/static/src/components/float_without_trailing_zeros/float_without_trailing_zeros.js` (14 lines)
- `addons/hr/static/src/components/hr_presence_status/hr_presence_status.js` (95 lines)
- `addons/hr/static/src/components/hr_presence_status/hr_presence_status.xml` (8 lines)

Additional files not expanded here: 155. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
