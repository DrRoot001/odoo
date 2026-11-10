# Module: hr_expense

- **Module ID:** MOD-086
- **Path:** `addons/hr_expense`
- **Manifest:** `addons/hr_expense/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Submit, validate and reinvoice employee expenses


Manage expenses by Employees
============================

This application allows you to manage your employees' daily expenses. It gives you access to your employees’ fee notes and give you the right to complete and validate or refuse the notes. After validation it creates an invoice for the employee.
Employee can encode their own expenses and the validation flow puts it automatically in the accounting after validation by managers.


The whole flow is implemented as:
---------------------------------
* Draft expense
* Submitted by the employee to his manager
* Approved by his manager
* Validation by the accountant and accounting entries creation

This module also uses analytic accounting and is compatible with the invoice on timesheet module so that you are able to automatically re-invoice your customers' expenses if your work by project.
    

Declared dependencies: `account`, `web_tour`, `hr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 38 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 18 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 27 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 14 | Client behavior/assets. |
| Tests | 9 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "web_tour",
    "hr"
  ],
  "data": [
    "security/hr_expense_security.xml",
    "data/digest_data.xml",
    "data/mail_activity_type_data.xml",
    "data/mail_alias_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_templates.xml",
    "data/hr_expense_data.xml",
    "data/hr_expense_tour.xml",
    "wizard/hr_expense_refuse_reason_views.xml",
    "wizard/hr_expense_approve_duplicate_views.xml",
    "wizard/hr_expense_split_wizard_views.xml",
    "views/product_product_views.xml",
    "views/hr_expense_views.xml",
    "views/hr_expense_split_views.xml",
    "views/mail_activity_views.xml",
    "report/hr_expense_report.xml",
    "views/account_journal_dashboard_view.xml",
    "views/account_move_views.xml",
    "views/account_payment_views.xml",
    "views/hr_department_views.xml",
    "views/res_config_settings_views.xml",
    "views/hr_employee_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/hr_expense_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "hr_expense/static/src/components/*.js",
      "hr_expense/static/src/components/*.xml",
      "hr_expense/static/src/mixins/*.js",
      "hr_expense/static/src/views/*.js",
      "hr_expense/static/src/views/*.xml",
      "hr_expense/static/src/webclient/**/*",
      "hr_expense/static/src/scss/hr_expense.scss",
      "hr_expense/static/src/js/tours/*.js",
      "hr_expense/static/src/js/web/*.js"
    ],
    "web.assets_tests": [
      "hr_expense/static/tests/tours/*.js"
    ],
    "web.report_assets_common": [
      "hr_expense/static/src/scss/hr_expense.scss"
    ]
  }
}
```

### Representative source files

- `addons/hr_expense/__init__.py` (6 lines)
- `addons/hr_expense/__manifest__.py` (77 lines)
- `addons/hr_expense/controllers/__init__.py` (3 lines)
- `addons/hr_expense/controllers/webmanifest.py` (9 lines)
- `addons/hr_expense/data/digest_data.xml` (17 lines)
- `addons/hr_expense/data/hr_expense_data.xml` (87 lines)
- `addons/hr_expense/data/hr_expense_demo.xml` (212 lines)
- `addons/hr_expense/data/hr_expense_tour.xml` (7 lines)
- `addons/hr_expense/data/mail_activity_type_data.xml` (11 lines)
- `addons/hr_expense/data/mail_alias_data.xml` (11 lines)
- `addons/hr_expense/data/mail_message_subtype_data.xml` (47 lines)
- `addons/hr_expense/data/mail_templates.xml` (110 lines)
- `addons/hr_expense/i18n/af.po` (2,706 lines)
- `addons/hr_expense/i18n/am.po` (2,702 lines)
- `addons/hr_expense/i18n/ar.po` (2,849 lines)
- `addons/hr_expense/i18n/az.po` (2,728 lines)
- `addons/hr_expense/i18n/bg.po` (2,756 lines)
- `addons/hr_expense/i18n/bs.po` (2,718 lines)
- `addons/hr_expense/i18n/ca.po` (2,790 lines)
- `addons/hr_expense/i18n/cs.po` (2,768 lines)
- `addons/hr_expense/i18n/da.po` (2,844 lines)
- `addons/hr_expense/i18n/de.po` (2,988 lines)
- `addons/hr_expense/i18n/el.po` (2,737 lines)
- `addons/hr_expense/i18n/en_AU.po` (81 lines)
- `addons/hr_expense/i18n/es.po` (2,888 lines)
- `addons/hr_expense/i18n/es_419.po` (2,994 lines)
- `addons/hr_expense/i18n/es_CL.po` (213 lines)
- `addons/hr_expense/i18n/et.po` (2,772 lines)
- `addons/hr_expense/i18n/eu.po` (2,705 lines)
- `addons/hr_expense/i18n/fa.po` (2,774 lines)
- `addons/hr_expense/i18n/fi.po` (2,911 lines)
- `addons/hr_expense/i18n/fo.po` (2,705 lines)
- `addons/hr_expense/i18n/fr.po` (2,954 lines)
- `addons/hr_expense/i18n/fr_BE.po` (134 lines)
- `addons/hr_expense/i18n/fr_CA.po` (166 lines)
- `addons/hr_expense/i18n/gl.po` (2,705 lines)
- `addons/hr_expense/i18n/gu.po` (2,716 lines)
- `addons/hr_expense/i18n/he.po` (2,759 lines)
- `addons/hr_expense/i18n/hi.po` (2,823 lines)
- `addons/hr_expense/i18n/hr.po` (2,755 lines)
- `addons/hr_expense/i18n/hr_expense.pot` (2,692 lines)
- `addons/hr_expense/i18n/hu.po` (2,739 lines)
- `addons/hr_expense/i18n/id.po` (2,990 lines)
- `addons/hr_expense/i18n/is.po` (2,713 lines)
- `addons/hr_expense/i18n/it.po` (2,974 lines)
- `addons/hr_expense/i18n/ja.po` (2,906 lines)
- `addons/hr_expense/i18n/ka.po` (2,705 lines)
- `addons/hr_expense/i18n/kab.po` (2,712 lines)
- `addons/hr_expense/i18n/km.po` (2,714 lines)
- `addons/hr_expense/i18n/ko.po` (2,829 lines)
- `addons/hr_expense/i18n/ku.po` (2,724 lines)
- `addons/hr_expense/i18n/lb.po` (2,707 lines)
- `addons/hr_expense/i18n/lo.po` (2,840 lines)
- `addons/hr_expense/i18n/lt.po` (2,752 lines)
- `addons/hr_expense/i18n/lv.po` (2,731 lines)
- `addons/hr_expense/i18n/mk.po` (2,705 lines)
- `addons/hr_expense/i18n/mn.po` (2,747 lines)
- `addons/hr_expense/i18n/my.po` (2,719 lines)
- `addons/hr_expense/i18n/nb.po` (2,737 lines)
- `addons/hr_expense/i18n/nl.po` (3,001 lines)
- `addons/hr_expense/i18n/pl.po` (2,888 lines)
- `addons/hr_expense/i18n/pt.po` (2,776 lines)
- `addons/hr_expense/i18n/pt_BR.po` (3,007 lines)
- `addons/hr_expense/i18n/ro.po` (2,845 lines)
- `addons/hr_expense/i18n/ru.po` (2,870 lines)
- `addons/hr_expense/i18n/sk.po` (2,750 lines)
- `addons/hr_expense/i18n/sl.po` (2,848 lines)
- `addons/hr_expense/i18n/sq.po` (2,705 lines)
- `addons/hr_expense/i18n/sr@latin.po` (2,727 lines)
- `addons/hr_expense/i18n/sv.po` (2,808 lines)
- `addons/hr_expense/i18n/ta.po` (2,706 lines)
- `addons/hr_expense/i18n/te.po` (2,704 lines)
- `addons/hr_expense/i18n/th.po` (2,798 lines)
- `addons/hr_expense/i18n/tr.po` (2,876 lines)
- `addons/hr_expense/i18n/uk.po` (2,771 lines)
- `addons/hr_expense/i18n/uz.po` (3,199 lines)
- `addons/hr_expense/i18n/vi.po` (2,864 lines)
- `addons/hr_expense/i18n/zh_CN.po` (2,901 lines)
- `addons/hr_expense/i18n/zh_TW.po` (2,812 lines)
- `addons/hr_expense/migrations/2.1/pre-migrate.py` (27 lines)
- `addons/hr_expense/models/__init__.py` (19 lines)
- `addons/hr_expense/models/account_journal.py` (49 lines)
- `addons/hr_expense/models/account_move.py` (126 lines)
- `addons/hr_expense/models/account_move_line.py` (47 lines)
- `addons/hr_expense/models/account_payment.py` (44 lines)
- `addons/hr_expense/models/account_tax.py` (46 lines)
- `addons/hr_expense/models/analytic.py` (45 lines)
- `addons/hr_expense/models/hr_department.py` (16 lines)
- `addons/hr_expense/models/hr_employee.py` (80 lines)
- `addons/hr_expense/models/hr_employee_public.py` (28 lines)
- `addons/hr_expense/models/hr_expense.py` (2,329 lines)
- `addons/hr_expense/models/hr_expense_product_job_position_limit.py` (40 lines)
- `addons/hr_expense/models/ir_actions_report.py` (160 lines)
- `addons/hr_expense/models/ir_attachment.py` (49 lines)
- `addons/hr_expense/models/product_product.py` (60 lines)
- `addons/hr_expense/models/product_template.py` (28 lines)
- `addons/hr_expense/models/res_company.py` (30 lines)
- `addons/hr_expense/models/res_config_settings.py` (74 lines)
- `addons/hr_expense/report/hr_expense_report.xml` (122 lines)
- `addons/hr_expense/security/hr_expense_security.xml` (31 lines)
- `addons/hr_expense/security/ir.access.csv` (44 lines)
- `addons/hr_expense/static/description/icon.png` (17 lines)
- `addons/hr_expense/static/description/icon.svg` (1 lines)
- `addons/hr_expense/static/description/icon_hi.png` (94 lines)
- `addons/hr_expense/static/img/app_store.png` (39 lines)
- `addons/hr_expense/static/img/communication.svg` (11 lines)
- `addons/hr_expense/static/img/food.svg` (10 lines)
- `addons/hr_expense/static/img/gift.svg` (11 lines)
- `addons/hr_expense/static/img/mileage.svg` (7 lines)
- `addons/hr_expense/static/img/nocontent.png` (1,279 lines)
- `addons/hr_expense/static/img/other.svg` (23 lines)
- `addons/hr_expense/static/img/play_store.png` (77 lines)
- `addons/hr_expense/static/img/transport.svg` (16 lines)
- `addons/hr_expense/static/src/components/attachment_view.js` (11 lines)
- `addons/hr_expense/static/src/components/expense_dashboard.js` (73 lines)
- `addons/hr_expense/static/src/components/expense_dashboard.xml` (20 lines)
- `addons/hr_expense/static/src/components/hr_expense_product_form_view.js` (46 lines)
- `addons/hr_expense/static/src/components/nb_attachment.js` (15 lines)
- `addons/hr_expense/static/src/components/nb_attachment.xml` (9 lines)
- `addons/hr_expense/static/src/img/milk-expense.png` (250 lines)
- `addons/hr_expense/static/src/js/tours/hr_expense.js` (214 lines)
- `addons/hr_expense/static/src/js/web/activity_menu_patch.js` (17 lines)
- `addons/hr_expense/static/src/mixins/document_upload.js` (173 lines)
- `addons/hr_expense/static/src/scss/hr_expense.scss` (161 lines)
- `addons/hr_expense/static/src/views/expense_form_view.js` (50 lines)
- `addons/hr_expense/static/src/views/kanban.js` (64 lines)
- `addons/hr_expense/static/src/views/kanban.xml` (37 lines)
- `addons/hr_expense/static/src/views/list.js` (119 lines)
- `addons/hr_expense/static/src/views/list.xml` (55 lines)
- `addons/hr_expense/static/src/webclient/share_target/expense_share_target_item.js` (16 lines)
- `addons/hr_expense/static/tests/tours/expense_form_tours.js` (122 lines)
- `addons/hr_expense/static/tests/tours/expense_product_tours.js` (128 lines)
- `addons/hr_expense/static/tests/tours/expense_upload_tours.js` (113 lines)
- `addons/hr_expense/tests/__init__.py` (10 lines)
- `addons/hr_expense/tests/common.py` (155 lines)
- `addons/hr_expense/tests/test_expense_job_position_limits.py` (214 lines)
- `addons/hr_expense/tests/test_expenses.py` (1,403 lines)
- `addons/hr_expense/tests/test_expenses_access_rights.py` (373 lines)
- `addons/hr_expense/tests/test_expenses_mail_import.py` (256 lines)
- `addons/hr_expense/tests/test_expenses_states.py` (220 lines)
- `addons/hr_expense/tests/test_expenses_tour.py` (51 lines)
- `addons/hr_expense/tests/test_ui.py` (35 lines)
- `addons/hr_expense/views/account_journal_dashboard_view.xml` (23 lines)
- `addons/hr_expense/views/account_move_views.xml` (89 lines)
- `addons/hr_expense/views/account_payment_views.xml` (24 lines)
- `addons/hr_expense/views/hr_department_views.xml` (28 lines)
- `addons/hr_expense/views/hr_employee_views.xml` (31 lines)
- `addons/hr_expense/views/hr_expense_split_views.xml` (39 lines)
- `addons/hr_expense/views/hr_expense_views.xml` (728 lines)
- `addons/hr_expense/views/mail_activity_views.xml` (15 lines)
- `addons/hr_expense/views/product_product_views.xml` (191 lines)
- `addons/hr_expense/views/res_config_settings_views.xml` (88 lines)
- `addons/hr_expense/wizard/__init__.py` (5 lines)
- `addons/hr_expense/wizard/account_payment_register.py` (32 lines)
- `addons/hr_expense/wizard/hr_expense_approve_duplicate.py` (30 lines)
- `addons/hr_expense/wizard/hr_expense_approve_duplicate_views.xml` (35 lines)
- `addons/hr_expense/wizard/hr_expense_refuse_reason.py` (17 lines)
- `addons/hr_expense/wizard/hr_expense_refuse_reason_views.xml` (28 lines)
- `addons/hr_expense/wizard/hr_expense_split.py` (122 lines)
- `addons/hr_expense/wizard/hr_expense_split_wizard.py` (69 lines)

Additional files not expanded here: 1. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
