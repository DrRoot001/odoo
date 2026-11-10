# Module: hr_work_entry

- **Module ID:** MOD-104
- **Path:** `addons/hr_work_entry`
- **Manifest:** `addons/hr_work_entry/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage work entries

No manifest description declared.

Declared dependencies: `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 23 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 15 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr"
  ],
  "data": [
    "data/hr_work_entry_type_data.xml",
    "data/hr_time_rule_data.xml",
    "wizard/hr_work_entry_export_views.xml",
    "views/hr_work_entry_type_views.xml",
    "views/hr_employee_views.xml",
    "views/res_company_views.xml",
    "views/resource_calendar_views.xml",
    "views/hr_time_rule_views.xml",
    "views/menuitems.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_work_entry_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_work_entry/static/src/**/*"
    ],
    "web.assets_unit_tests": [
      "hr_work_entry/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/hr_work_entry/__init__.py` (5 lines)
- `addons/hr_work_entry/__manifest__.py` (36 lines)
- `addons/hr_work_entry/controllers/__init__.py` (3 lines)
- `addons/hr_work_entry/controllers/main.py` (18 lines)
- `addons/hr_work_entry/data/hr_time_rule_data.xml` (519 lines)
- `addons/hr_work_entry/data/hr_work_entry_demo.xml` (24 lines)
- `addons/hr_work_entry/data/hr_work_entry_type_data.xml` (5,918 lines)
- `addons/hr_work_entry/i18n/ar.po` (4,638 lines)
- `addons/hr_work_entry/i18n/az.po` (4,326 lines)
- `addons/hr_work_entry/i18n/bg.po` (4,331 lines)
- `addons/hr_work_entry/i18n/bs.po` (4,322 lines)
- `addons/hr_work_entry/i18n/ca.po` (4,334 lines)
- `addons/hr_work_entry/i18n/cs.po` (4,339 lines)
- `addons/hr_work_entry/i18n/da.po` (4,349 lines)
- `addons/hr_work_entry/i18n/de.po` (4,887 lines)
- `addons/hr_work_entry/i18n/el.po` (4,325 lines)
- `addons/hr_work_entry/i18n/en_AU.po` (21 lines)
- `addons/hr_work_entry/i18n/es.po` (4,416 lines)
- `addons/hr_work_entry/i18n/es_419.po` (4,912 lines)
- `addons/hr_work_entry/i18n/et.po` (4,342 lines)
- `addons/hr_work_entry/i18n/fa.po` (4,332 lines)
- `addons/hr_work_entry/i18n/fi.po` (4,417 lines)
- `addons/hr_work_entry/i18n/fr.po` (4,755 lines)
- `addons/hr_work_entry/i18n/he.po` (4,340 lines)
- `addons/hr_work_entry/i18n/hi.po` (4,341 lines)
- `addons/hr_work_entry/i18n/hr.po` (4,341 lines)
- `addons/hr_work_entry/i18n/hr_work_entry.pot` (4,309 lines)
- `addons/hr_work_entry/i18n/hu.po` (4,336 lines)
- `addons/hr_work_entry/i18n/id.po` (4,660 lines)
- `addons/hr_work_entry/i18n/it.po` (4,844 lines)
- `addons/hr_work_entry/i18n/ja.po` (4,760 lines)
- `addons/hr_work_entry/i18n/kab.po` (4,321 lines)
- `addons/hr_work_entry/i18n/ko.po` (4,490 lines)
- `addons/hr_work_entry/i18n/ku.po` (4,321 lines)
- `addons/hr_work_entry/i18n/lo.po` (4,368 lines)
- `addons/hr_work_entry/i18n/lt.po` (4,345 lines)
- `addons/hr_work_entry/i18n/lv.po` (4,321 lines)
- `addons/hr_work_entry/i18n/mn.po` (4,341 lines)
- `addons/hr_work_entry/i18n/my.po` (4,331 lines)
- `addons/hr_work_entry/i18n/nb.po` (4,338 lines)
- `addons/hr_work_entry/i18n/nl.po` (4,916 lines)
- `addons/hr_work_entry/i18n/pl.po` (4,688 lines)
- `addons/hr_work_entry/i18n/pt.po` (4,357 lines)
- `addons/hr_work_entry/i18n/pt_BR.po` (4,892 lines)
- `addons/hr_work_entry/i18n/ro.po` (4,420 lines)
- `addons/hr_work_entry/i18n/ru.po` (4,396 lines)
- `addons/hr_work_entry/i18n/sk.po` (4,320 lines)
- `addons/hr_work_entry/i18n/sl.po` (4,337 lines)
- `addons/hr_work_entry/i18n/sr@latin.po` (4,327 lines)
- `addons/hr_work_entry/i18n/sv.po` (4,343 lines)
- `addons/hr_work_entry/i18n/th.po` (4,359 lines)
- `addons/hr_work_entry/i18n/tr.po` (4,421 lines)
- `addons/hr_work_entry/i18n/uk.po` (4,341 lines)
- `addons/hr_work_entry/i18n/uz.po` (4,550 lines)
- `addons/hr_work_entry/i18n/vi.po` (4,469 lines)
- `addons/hr_work_entry/i18n/zh_CN.po` (4,551 lines)
- `addons/hr_work_entry/i18n/zh_TW.po` (4,410 lines)
- `addons/hr_work_entry/models/__init__.py` (13 lines)
- `addons/hr_work_entry/models/hr_employee.py` (33 lines)
- `addons/hr_work_entry/models/hr_time_rule.py` (1,273 lines)
- `addons/hr_work_entry/models/hr_time_rule_source_mixin.py` (494 lines)
- `addons/hr_work_entry/models/hr_user_work_entry_employee.py` (20 lines)
- `addons/hr_work_entry/models/hr_version.py` (895 lines)
- `addons/hr_work_entry/models/hr_work_entry_type.py` (116 lines)
- `addons/hr_work_entry/models/res_company.py` (36 lines)
- `addons/hr_work_entry/models/res_config_settings.py` (10 lines)
- `addons/hr_work_entry/models/resource_calendar.py` (68 lines)
- `addons/hr_work_entry/models/resource_calendar_attendance.py` (77 lines)
- `addons/hr_work_entry/models/resource_calendar_leaves.py` (49 lines)
- `addons/hr_work_entry/security/ir.access.csv` (10 lines)
- `addons/hr_work_entry/static/description/icon.png` (19 lines)
- `addons/hr_work_entry/static/description/icon.svg` (1 lines)
- `addons/hr_work_entry/static/description/icon_hi.png` (65 lines)
- `addons/hr_work_entry/static/src/components/domain_count_field/domain_count_field.js` (29 lines)
- `addons/hr_work_entry/static/src/components/domain_count_field/domain_count_field.xml` (22 lines)
- `addons/hr_work_entry/static/src/components/resource_calendar_attendance_popover/resource_calendar_attendance_popover.xml` (8 lines)
- `addons/hr_work_entry/static/src/components/work_entry_type_field/work_entry_type_field.js` (81 lines)
- `addons/hr_work_entry/static/src/components/work_entry_type_field/work_entry_type_field.xml` (35 lines)
- `addons/hr_work_entry/static/src/export_cog_menu/export_cog_menu.js` (43 lines)
- `addons/hr_work_entry/static/src/export_cog_menu/export_cog_menu.xml` (13 lines)
- `addons/hr_work_entry/static/src/search/hr_work_entry_action_menus/hr_work_entry_action_menus.js` (15 lines)
- `addons/hr_work_entry/static/src/search/hr_work_entry_action_menus/hr_work_entry_action_menus.xml` (8 lines)
- `addons/hr_work_entry/static/tests/work_entry_type_field.test.js` (160 lines)
- `addons/hr_work_entry/tests/__init__.py` (5 lines)
- `addons/hr_work_entry/tests/common.py` (63 lines)
- `addons/hr_work_entry/tests/test_work_entry.py` (545 lines)
- `addons/hr_work_entry/tests/test_work_entry_type.py` (211 lines)
- `addons/hr_work_entry/tests/test_work_entry_type_data.py` (85 lines)
- `addons/hr_work_entry/views/hr_employee_views.xml` (26 lines)
- `addons/hr_work_entry/views/hr_time_rule_views.xml` (154 lines)
- `addons/hr_work_entry/views/hr_work_entry_type_views.xml` (131 lines)
- `addons/hr_work_entry/views/menuitems.xml` (9 lines)
- `addons/hr_work_entry/views/res_company_views.xml` (13 lines)
- `addons/hr_work_entry/views/resource_calendar_views.xml` (84 lines)
- `addons/hr_work_entry/wizard/__init__.py` (3 lines)
- `addons/hr_work_entry/wizard/hr_export_work_entries.py` (206 lines)
- `addons/hr_work_entry/wizard/hr_work_entry_export_views.xml` (29 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
