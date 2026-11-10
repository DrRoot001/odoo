# Module: sale_project

- **Module ID:** MOD-524
- **Path:** `addons/sale_project`
- **Manifest:** `addons/sale_project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['sale_management', 'project_account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Task Generation from Sales Orders


Allows to create task from your sales order
=============================================
This module allows to generate a project/task from sales orders.


Declared dependencies: `sale_management`, `sale_service`, `project_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 9 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_management",
    "sale_service",
    "project_account"
  ],
  "data": [
    "views/product_views.xml",
    "views/project_task_views.xml",
    "views/sale_order_line_views.xml",
    "views/sale_order_views.xml",
    "views/sale_project_portal_templates.xml",
    "views/project_update_template.xml",
    "views/project_sharing_views.xml",
    "views/project_views.xml",
    "views/project_task_type_views.xml",
    "data/sale_project_data.xml",
    "wizard/project_template_create_wizard.xml",
    "report/account_analytic_line_views.xml",
    "report/sale_report_views.xml",
    "views/project_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/sale_project_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_project/static/src/fields/**/*",
      "sale_project/static/src/core/**/*",
      "sale_project/static/src/views/**/*"
    ],
    "web.assets_tests": [
      "sale_project/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "sale_project/static/tests/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_project/__init__.py` (27 lines)
- `addons/sale_project/__manifest__.py` (50 lines)
- `addons/sale_project/controllers/__init__.py` (4 lines)
- `addons/sale_project/controllers/portal.py` (62 lines)
- `addons/sale_project/data/sale_project_data.xml` (64 lines)
- `addons/sale_project/data/sale_project_demo.xml` (218 lines)
- `addons/sale_project/i18n/ar.po` (989 lines)
- `addons/sale_project/i18n/az.po` (911 lines)
- `addons/sale_project/i18n/bg.po` (912 lines)
- `addons/sale_project/i18n/bs.po` (913 lines)
- `addons/sale_project/i18n/ca.po` (988 lines)
- `addons/sale_project/i18n/cs.po` (952 lines)
- `addons/sale_project/i18n/da.po` (989 lines)
- `addons/sale_project/i18n/de.po` (1,050 lines)
- `addons/sale_project/i18n/el.po` (931 lines)
- `addons/sale_project/i18n/es.po` (1,012 lines)
- `addons/sale_project/i18n/es_419.po` (1,041 lines)
- `addons/sale_project/i18n/et.po` (912 lines)
- `addons/sale_project/i18n/fa.po` (911 lines)
- `addons/sale_project/i18n/fi.po` (1,016 lines)
- `addons/sale_project/i18n/fr.po` (1,035 lines)
- `addons/sale_project/i18n/he.po` (912 lines)
- `addons/sale_project/i18n/hi.po` (911 lines)
- `addons/sale_project/i18n/hr.po` (912 lines)
- `addons/sale_project/i18n/hu.po` (994 lines)
- `addons/sale_project/i18n/id.po` (1,001 lines)
- `addons/sale_project/i18n/it.po` (1,039 lines)
- `addons/sale_project/i18n/ja.po` (1,018 lines)
- `addons/sale_project/i18n/kab.po` (912 lines)
- `addons/sale_project/i18n/ko.po` (988 lines)
- `addons/sale_project/i18n/ku.po` (911 lines)
- `addons/sale_project/i18n/lo.po` (974 lines)
- `addons/sale_project/i18n/lt.po` (913 lines)
- `addons/sale_project/i18n/lv.po` (912 lines)
- `addons/sale_project/i18n/mn.po` (911 lines)
- `addons/sale_project/i18n/my.po` (912 lines)
- `addons/sale_project/i18n/nb.po` (931 lines)
- `addons/sale_project/i18n/nl.po` (1,043 lines)
- `addons/sale_project/i18n/pl.po` (1,033 lines)
- `addons/sale_project/i18n/pt.po` (989 lines)
- `addons/sale_project/i18n/pt_BR.po` (1,037 lines)
- `addons/sale_project/i18n/ro.po` (1,008 lines)
- `addons/sale_project/i18n/ru.po` (1,007 lines)
- `addons/sale_project/i18n/sale_project.pot` (891 lines)
- `addons/sale_project/i18n/sk.po` (911 lines)
- `addons/sale_project/i18n/sl.po` (944 lines)
- `addons/sale_project/i18n/sr@latin.po` (913 lines)
- `addons/sale_project/i18n/sv.po` (991 lines)
- `addons/sale_project/i18n/th.po` (982 lines)
- `addons/sale_project/i18n/tr.po` (1,007 lines)
- `addons/sale_project/i18n/uk.po` (912 lines)
- `addons/sale_project/i18n/uz.po` (1,098 lines)
- `addons/sale_project/i18n/vi.po` (995 lines)
- `addons/sale_project/i18n/zh_CN.po` (987 lines)
- `addons/sale_project/i18n/zh_TW.po` (967 lines)
- `addons/sale_project/models/__init__.py` (12 lines)
- `addons/sale_project/models/account_analytic_line.py` (106 lines)
- `addons/sale_project/models/account_move_line.py` (83 lines)
- `addons/sale_project/models/product_product.py` (31 lines)
- `addons/sale_project/models/product_template.py` (153 lines)
- `addons/sale_project/models/project_milestone.py` (64 lines)
- `addons/sale_project/models/project_project.py` (570 lines)
- `addons/sale_project/models/project_task.py` (253 lines)
- `addons/sale_project/models/project_task_recurrence.py` (11 lines)
- `addons/sale_project/models/project_task_type.py` (17 lines)
- `addons/sale_project/models/sale_order.py` (331 lines)
- `addons/sale_project/models/sale_order_line.py` (476 lines)
- `addons/sale_project/models/sale_order_template_line.py` (16 lines)
- `addons/sale_project/report/__init__.py` (5 lines)
- `addons/sale_project/report/account_analytic_line_views.xml` (137 lines)
- `addons/sale_project/report/project_report.py` (17 lines)
- `addons/sale_project/report/sale_report.py` (12 lines)
- `addons/sale_project/report/sale_report_views.xml` (16 lines)
- `addons/sale_project/security/ir.access.csv` (5 lines)
- `addons/sale_project/static/src/core/bottom_sheet/bottom_sheet.scss` (16 lines)
- `addons/sale_project/static/src/fields/costs_percent_pie/costs_percent_pie.js` (34 lines)
- `addons/sale_project/static/src/fields/costs_percent_pie/costs_percent_pie.xml` (10 lines)
- `addons/sale_project/static/src/views/project_form/project_project_form_controller.js` (36 lines)
- `addons/sale_project/static/src/views/project_task_list/project_task_list_sale_line.js` (12 lines)
- `addons/sale_project/static/tests/project_milestone_form_view.test.js` (61 lines)
- `addons/sale_project/static/tests/project_task_list_sale_line.test.js` (60 lines)
- `addons/sale_project/static/tests/project_task_model.js` (60 lines)
- `addons/sale_project/static/tests/so_line_create_button.test.js` (171 lines)
- `addons/sale_project/static/tests/tours/project_create_sol_tour.js` (58 lines)
- `addons/sale_project/static/tests/tours/project_tour.js` (22 lines)
- `addons/sale_project/tests/__init__.py` (11 lines)
- `addons/sale_project/tests/common.py` (167 lines)
- `addons/sale_project/tests/test_analytic_distribution.py` (281 lines)
- `addons/sale_project/tests/test_child_tasks.py` (292 lines)
- `addons/sale_project/tests/test_project_project.py` (31 lines)
- `addons/sale_project/tests/test_reinvoice.py` (488 lines)
- `addons/sale_project/tests/test_sale_project.py` (2,269 lines)
- `addons/sale_project/tests/test_sale_project_multicompany_access.py` (69 lines)
- `addons/sale_project/tests/test_sale_warning.py` (196 lines)
- `addons/sale_project/tests/test_so_line_milestones.py` (410 lines)
- `addons/sale_project/views/product_views.xml` (60 lines)
- `addons/sale_project/views/project_menus.xml` (11 lines)
- `addons/sale_project/views/project_sharing_views.xml` (68 lines)
- `addons/sale_project/views/project_task_type_views.xml` (25 lines)
- `addons/sale_project/views/project_task_views.xml` (427 lines)
- `addons/sale_project/views/project_update_template.xml` (16 lines)
- `addons/sale_project/views/project_views.xml` (159 lines)
- `addons/sale_project/views/sale_order_line_views.xml` (39 lines)
- `addons/sale_project/views/sale_order_views.xml` (88 lines)
- `addons/sale_project/views/sale_project_portal_templates.xml` (13 lines)
- `addons/sale_project/wizard/__init__.py` (1 lines)
- `addons/sale_project/wizard/project_template_create_wizard.py` (91 lines)
- `addons/sale_project/wizard/project_template_create_wizard.xml` (58 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
