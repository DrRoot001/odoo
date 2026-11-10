# Module: project_todo

- **Module ID:** MOD-492
- **Path:** `addons/project_todo`
- **Manifest:** `addons/project_todo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Organize your work with memos and to-do lists

No manifest description declared.

Declared dependencies: `project`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 17 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 28 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "project"
  ],
  "data": [
    "data/digest_data.xml",
    "data/todo_template.xml",
    "views/project_task_views.xml",
    "views/project_todo_menus.xml",
    "wizard/mail_activity_todo_create.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "project_todo/static/src/components/**/*",
      "project_todo/static/src/scss/todo.scss",
      "project_todo/static/src/views/**/*",
      "project_todo/static/src/core/web/**/*",
      "project_todo/static/src/webclient/**/*"
    ],
    "web.assets_tests": [
      "project_todo/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "project_todo/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/project_todo/__init__.py` (6 lines)
- `addons/project_todo/__manifest__.py` (39 lines)
- `addons/project_todo/data/digest_data.xml` (22 lines)
- `addons/project_todo/data/todo_template.xml` (218 lines)
- `addons/project_todo/i18n/ar.po` (858 lines)
- `addons/project_todo/i18n/az.po` (723 lines)
- `addons/project_todo/i18n/bg.po` (723 lines)
- `addons/project_todo/i18n/bs.po` (725 lines)
- `addons/project_todo/i18n/ca.po` (779 lines)
- `addons/project_todo/i18n/cs.po` (743 lines)
- `addons/project_todo/i18n/da.po` (751 lines)
- `addons/project_todo/i18n/de.po` (905 lines)
- `addons/project_todo/i18n/el.po` (724 lines)
- `addons/project_todo/i18n/es.po` (869 lines)
- `addons/project_todo/i18n/es_419.po` (897 lines)
- `addons/project_todo/i18n/et.po` (860 lines)
- `addons/project_todo/i18n/fa.po` (723 lines)
- `addons/project_todo/i18n/fi.po` (869 lines)
- `addons/project_todo/i18n/fr.po` (896 lines)
- `addons/project_todo/i18n/he.po` (724 lines)
- `addons/project_todo/i18n/hi.po` (723 lines)
- `addons/project_todo/i18n/hr.po` (724 lines)
- `addons/project_todo/i18n/hu.po` (837 lines)
- `addons/project_todo/i18n/id.po` (857 lines)
- `addons/project_todo/i18n/it.po` (891 lines)
- `addons/project_todo/i18n/ja.po` (889 lines)
- `addons/project_todo/i18n/kab.po` (724 lines)
- `addons/project_todo/i18n/ko.po` (861 lines)
- `addons/project_todo/i18n/ku.po` (723 lines)
- `addons/project_todo/i18n/lo.po` (872 lines)
- `addons/project_todo/i18n/lt.po` (725 lines)
- `addons/project_todo/i18n/lv.po` (724 lines)
- `addons/project_todo/i18n/mn.po` (724 lines)
- `addons/project_todo/i18n/my.po` (724 lines)
- `addons/project_todo/i18n/nb.po` (726 lines)
- `addons/project_todo/i18n/nl.po` (890 lines)
- `addons/project_todo/i18n/pl.po` (876 lines)
- `addons/project_todo/i18n/project_todo.pot` (704 lines)
- `addons/project_todo/i18n/pt.po` (839 lines)
- `addons/project_todo/i18n/pt_BR.po` (889 lines)
- `addons/project_todo/i18n/ro.po` (831 lines)
- `addons/project_todo/i18n/ru.po` (860 lines)
- `addons/project_todo/i18n/sk.po` (723 lines)
- `addons/project_todo/i18n/sl.po` (744 lines)
- `addons/project_todo/i18n/sr@latin.po` (724 lines)
- `addons/project_todo/i18n/sv.po` (838 lines)
- `addons/project_todo/i18n/th.po` (840 lines)
- `addons/project_todo/i18n/tr.po` (870 lines)
- `addons/project_todo/i18n/uk.po` (724 lines)
- `addons/project_todo/i18n/uz.po` (900 lines)
- `addons/project_todo/i18n/vi.po` (864 lines)
- `addons/project_todo/i18n/zh_CN.po` (872 lines)
- `addons/project_todo/i18n/zh_TW.po` (842 lines)
- `addons/project_todo/models/__init__.py` (2 lines)
- `addons/project_todo/models/project_task.py` (58 lines)
- `addons/project_todo/models/res_users.py` (80 lines)
- `addons/project_todo/security/ir.access.csv` (39 lines)
- `addons/project_todo/static/description/icon.png` (11 lines)
- `addons/project_todo/static/description/icon.svg` (1 lines)
- `addons/project_todo/static/description/icon_hi.png` (23 lines)
- `addons/project_todo/static/img/convert_todo.png` (205 lines)
- `addons/project_todo/static/img/todo_access.png` (383 lines)
- `addons/project_todo/static/src/components/todo_chatter_panel/todo_chatter_panel.js` (33 lines)
- `addons/project_todo/static/src/components/todo_chatter_panel/todo_chatter_panel.scss` (12 lines)
- `addons/project_todo/static/src/components/todo_chatter_panel/todo_chatter_panel.xml` (19 lines)
- `addons/project_todo/static/src/components/todo_done_checkmark/todo_done_checkmark.js` (76 lines)
- `addons/project_todo/static/src/components/todo_done_checkmark/todo_done_checkmark.scss` (6 lines)
- `addons/project_todo/static/src/components/todo_done_checkmark/todo_done_checkmark.xml` (23 lines)
- `addons/project_todo/static/src/core/web/activity_menu_patch.js` (68 lines)
- `addons/project_todo/static/src/scss/todo.scss` (30 lines)
- `addons/project_todo/static/src/views/todo_activity_wizard/todo_activity_wizard_controller.js` (12 lines)
- `addons/project_todo/static/src/views/todo_activity_wizard/todo_activity_wizard_view.js` (10 lines)
- `addons/project_todo/static/src/views/todo_conversion_form/todo_conversion_form_controller.js` (18 lines)
- `addons/project_todo/static/src/views/todo_conversion_form/todo_conversion_form_view.js` (10 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_cog_menu.js` (8 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_control_panel.js` (40 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_control_panel.xml` (19 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_controller.js` (112 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_controller.scss` (12 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_renderer.js` (18 lines)
- `addons/project_todo/static/src/views/todo_form/todo_form_view.js` (14 lines)
- `addons/project_todo/static/src/views/todo_list/todo_list_controller.js` (13 lines)
- `addons/project_todo/static/src/views/todo_list/todo_list_view.js` (12 lines)
- `addons/project_todo/static/src/webclient/share_target/todo_share_target_item.js` (28 lines)
- `addons/project_todo/static/tests/mock_server/mock_models/mail_activity_todo_create.js` (10 lines)
- `addons/project_todo/static/tests/mock_server/mock_models/project_tags.js` (26 lines)
- `addons/project_todo/static/tests/mock_server/mock_models/project_task.js` (33 lines)
- `addons/project_todo/static/tests/todo_activity_wizard_view.test.js` (63 lines)
- `addons/project_todo/static/tests/todo_calendar_view.test.js` (54 lines)
- `addons/project_todo/static/tests/todo_conversion_form_view.test.js` (73 lines)
- `addons/project_todo/static/tests/todo_done_checkmark.test.js` (212 lines)
- `addons/project_todo/static/tests/todo_form_view.test.js` (172 lines)
- `addons/project_todo/static/tests/todo_list_view.test.js` (36 lines)
- `addons/project_todo/static/tests/todo_test_helpers.js` (20 lines)
- `addons/project_todo/static/tests/tours/project_task_activities_split.js` (48 lines)
- `addons/project_todo/static/tests/tours/project_todo_history.js` (130 lines)
- `addons/project_todo/static/tests/tours/project_todo_main_functions.js` (170 lines)
- `addons/project_todo/tests/__init__.py` (11 lines)
- `addons/project_todo/tests/test_access_rights.py` (23 lines)
- `addons/project_todo/tests/test_mail_activity_systray_counter.py` (109 lines)
- `addons/project_todo/tests/test_mail_activity_todo_create.py` (29 lines)
- `addons/project_todo/tests/test_project_tags.py` (67 lines)
- `addons/project_todo/tests/test_project_task_type.py` (52 lines)
- `addons/project_todo/tests/test_todo_mail_features.py` (68 lines)
- `addons/project_todo/tests/test_todo_onboarding_for_users.py` (45 lines)
- `addons/project_todo/tests/test_todo_quick_create.py` (50 lines)
- `addons/project_todo/tests/test_todo_ui.py` (75 lines)
- `addons/project_todo/views/project_task_views.xml` (342 lines)
- `addons/project_todo/views/project_todo_menus.xml` (10 lines)
- `addons/project_todo/wizard/__init__.py` (3 lines)
- `addons/project_todo/wizard/mail_activity_todo_create.py` (38 lines)
- `addons/project_todo/wizard/mail_activity_todo_create.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
