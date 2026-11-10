# Module: project

- **Module ID:** MOD-475
- **Path:** `addons/project`
- **Manifest:** `addons/project/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage tasks and collaborate on projects

No manifest description declared.

Declared dependencies: `analytic`, `base_setup`, `mail`, `portal_rating`, `resource`, `web`, `web_tour`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 82 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 23 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 74 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 145 | Client behavior/assets. |
| Tests | 39 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 9 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "analytic",
    "base_setup",
    "mail",
    "portal_rating",
    "resource",
    "web",
    "web_tour",
    "digest"
  ],
  "data": [
    "security/project_security.xml",
    "data/digest_data.xml",
    "data/portal_entry_data.xml",
    "report/project_task_burndown_chart_report_views.xml",
    "views/account_analytic_account_views.xml",
    "views/digest_digest_views.xml",
    "views/rating_rating_views.xml",
    "views/project_update_views.xml",
    "views/project_update_templates.xml",
    "views/project_project_stage_views.xml",
    "wizard/project_share_wizard_views.xml",
    "views/project_task_type_views.xml",
    "views/project_project_views.xml",
    "views/project_task_views.xml",
    "views/project_role_views.xml",
    "views/project_tags_views.xml",
    "views/project_milestone_views.xml",
    "views/res_partner_views.xml",
    "views/res_config_settings_views.xml",
    "views/mail_activity_plan_views.xml",
    "views/mail_activity_type_views.xml",
    "views/project_sharing_project_task_views.xml",
    "views/project_portal_project_project_templates.xml",
    "views/project_portal_project_task_templates.xml",
    "views/project_task_templates.xml",
    "views/project_sharing_project_task_templates.xml",
    "report/project_report_views.xml",
    "report/project_time_by_stage_report_views.xml",
    "data/ir_cron_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_template_data.xml",
    "data/project_data.xml",
    "data/project_tour.xml",
    "wizard/project_task_type_delete_views.xml",
    "wizard/project_task_share_wizard_views.xml",
    "wizard/project_project_stage_delete_views.xml",
    "wizard/project_template_create_wizard.xml",
    "views/project_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/mail_template_demo.xml",
    "data/project_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "project/static/src/css/project.css",
      "project/static/src/core/web/**/*",
      "project/static/src/utils/**/*",
      "project/static/src/actions/client_actions.js",
      "project/static/src/components/**/*",
      "project/static/src/views/**/*",
      "project/static/src/js/tours/project.js",
      "project/static/src/scss/project_dashboard.scss",
      "project/static/src/scss/project_form.scss",
      "project/static/src/scss/project_widgets.scss",
      "project/static/src/xml/**/*",
      "project/static/src/webclient/**/*",
      [
        "remove",
        "project/static/src/views/project_task_activity/**"
      ],
      [
        "remove",
        "project/static/src/views/project_task_graph/**"
      ],
      [
        "remove",
        "project/static/src/views/project_task_pivot/**"
      ],
      [
        "remove",
        "project/static/src/views/project_task_analysis_renderer_mixin.js"
      ],
      [
        "remove",
        "project/static/src/views/project_task_analysis_graph/**"
      ],
      [
        "remove",
        "project/static/src/views/project_task_analysis_pivot/**"
      ],
      [
        "remove",
        "project/static/src/views/burndown_chart/**"
      ],
      [
        "remove",
        "project/static/src/views/project_project_activity/**"
      ]
    ],
    "web.assets_backend_lazy": [
      "project/static/src/views/project_task_model_mixin",
      "project/static/src/views/project_task_activity/**",
      "project/static/src/views/project_task_graph/**",
      "project/static/src/views/project_task_pivot/**",
      "project/static/src/views/project_task_analysis_renderer_mixin.js",
      "project/static/src/views/project_task_analysis_graph/**",
      "project/static/src/views/project_task_analysis_pivot/**",
      "project/static/src/views/burndown_chart/**",
      "project/static/src/views/project_project_activity/**"
    ],
    "web.assets_frontend": [
      "project/static/src/scss/portal_rating.scss"
    ],
    "web.assets_unit_tests": [
      "project/static/tests/mock_server/**/*",
      "project/static/tests/project_models.js",
      "project/static/tests/**/*.test.js"
    ],
    "web.assets_tests": [
      "project/static/tests/tours/**/*"
    ],
    "project.webclient": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_backend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/webclient/navbar/navbar.scss",
      "web/static/src/scss/animation.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      "web/static/src/module_loader.js",
      "web/static/src/session.js",
      "web/static/lib/luxon/luxon.js",
      "web/static/src/libs/luxon.js",
      "web/static/lib/owl/owl.js",
      "web/static/src/owl2/owl3_compatibility_layer.js",
      "web/static/src/owl2/utils.js",
      "web/static/lib/owl/odoo_module.js",
      "web/static/lib/popper/popper.js",
      "web/static/lib/bootstrap/js/dist/util/index.js",
      "web/static/lib/bootstrap/js/dist/dom/data.js",
      "web/static/lib/bootstrap/js/dist/dom/event-handler.js",
      "web/static/lib/bootstrap/js/dist/dom/manipulator.js",
      "web/static/lib/bootstrap/js/dist/dom/selector-engine.js",
      "web/static/lib/bootstrap/js/dist/util/config.js",
      "web/static/lib/bootstrap/js/dist/util/component-functions.js",
      "web/static/lib/bootstrap/js/dist/util/backdrop.js",
      "web/static/lib/bootstrap/js/dist/util/focustrap.js",
      "web/static/lib/bootstrap/js/dist/util/sanitizer.js",
      "web/static/lib/bootstrap/js/dist/util/scrollbar.js",
      "web/static/lib/bootstrap/js/dist/util/swipe.js",
      "web/static/lib/bootstrap/js/dist/util/template-factory.js",
      "web/static/lib/bootstrap/js/dist/base-component.js",
      "web/static/lib/bootstrap/js/dist/alert.js",
      "web/static/lib/bootstrap/js/dist/button.js",
      "web/static/lib/bootstrap/js/dist/carousel.js",
      "web/static/lib/bootstrap/js/dist/collapse.js",
      "web/static/lib/bootstrap/js/dist/dropdown.js",
      "web/static/lib/bootstrap/js/dist/modal.js",
      "web/static/lib/bootstrap/js/dist/offcanvas.js",
      "web/static/lib/bootstrap/js/dist/tooltip.js",
      "web/static/lib/bootstrap/js/dist/popover.js",
      "web/static/lib/bootstrap/js/dist/scrollspy.js",
      "web/static/lib/bootstrap/js/dist/tab.js",
      "web/static/lib/bootstrap/js/dist/toast.js",
      "web/static/lib/dompurify/DOMpurify.js",
      "web/static/src/libs/bootstrap.js",
      "base/static/src/css/modules.css",
      "web/static/src/core/utils/transitions.scss",
      "web/static/src/core/**/*",
      "web/static/src/model/**/*",
      "web/static/src/search/**/*",
      "web/static/src/webclient/icons.scss",
      "web/static/src/views/**/*.js",
      "web/static/src/views/*.xml",
      "web/static/src/views/*.scss",
      "web/static/src/views/fields/**/*",
      "web/static/src/views/form/**/*",
      "web/static/src/views/card/**/*",
      "web/static/src/views/kanban/**/*",
      "web/static/src/views/list/**/*",
      "web/static/src/views/view_button/**/*",
      "web/static/src/views/view_components/**/*",
      "web/static/src/views/view_dialogs/**/*",
      "web/static/src/views/widgets/**/*",
      "web/static/src/webclient/**/*",
      [
        "remove",
        "web/static/src/webclient/clickbot/clickbot.js"
      ],
      [
        "remove",
        "web/static/src/views/form/button_box/*.scss"
      ],
      [
        "remove",
        "web/static/src/core/emoji_picker/emoji_data.js"
      ],
      [
        "remove",
        "web/static/src/webclient/actions/reports/**/*"
      ],
      "web/static/src/webclient/actions/reports/*.js",
      "web/static/src/webclient/actions/reports/*.xml",
      "web/static/src/env.js",
      "base/static/src/scss/res_partner.scss",
      "web/static/src/views/form/button_box/*.scss",
      "bus/static/src/**/*.js",
      [
        "include",
        "web_tour.assets"
      ],
      "web_tour/static/src/tour_pointer/tour_pointer.scss",
      [
        "include",
        "html_editor.assets_editor"
      ],
      "html_editor/static/src/backend/**/*",
      "html_editor/static/src/fields/**/*",
      "html_editor/static/src/scss/html_editor.common.scss",
      "html_editor/static/src/scss/base_style.scss",
      "mail/static/src/scss/variables/*.scss",
      "mail/static/src/chatter/web/form_renderer.scss",
      "mail/static/src/views/fields/**/*",
      "project/static/src/components/project_task_name_with_subtask_count_char_field/*",
      "project/static/src/components/project_task_state_selection/*",
      "project/static/src/components/project_many2one_field/*",
      "project/static/src/views/project_task_form/*.scss",
      "project/static/src/views/project_task_kanban/*.scss",
      "project/static/src/views/project_task_control_panel/*",
      "project/static/src/views/project_task_model_mixin.js",
      "project/static/src/views/project_task_relational_model.js",
      "project/static/src/views/project_model_mixin.js",
      "project/static/src/views/project_relational_model.js",
      [
        "include",
        "portal.assets_chatter_helpers"
      ],
      "portal/static/src/chatter/portal_project/**/*",
      "project/static/src/project_sharing/**/*",
      "web/static/src/start.js"
    ]
  }
}
```

### Representative source files

- `addons/project/README.md` (69 lines)
- `addons/project/__init__.py` (29 lines)
- `addons/project/__manifest__.py` (239 lines)
- `addons/project/controllers/__init__.py` (5 lines)
- `addons/project/controllers/portal.py` (647 lines)
- `addons/project/controllers/project_sharing_chatter.py` (30 lines)
- `addons/project/controllers/webmanifest.py` (9 lines)
- `addons/project/data/digest_data.xml` (144 lines)
- `addons/project/data/ir_cron_data.xml` (10 lines)
- `addons/project/data/mail_message_subtype_data.xml` (167 lines)
- `addons/project/data/mail_template_data.xml` (137 lines)
- `addons/project/data/mail_template_demo.xml` (26 lines)
- `addons/project/data/portal_entry_data.xml` (22 lines)
- `addons/project/data/project_data.xml` (72 lines)
- `addons/project/data/project_demo.xml` (2,137 lines)
- `addons/project/data/project_tour.xml` (8 lines)
- `addons/project/doc/changelog.rst` (16 lines)
- `addons/project/doc/index.rst` (22 lines)
- `addons/project/doc/stage_status.rst` (55 lines)
- `addons/project/i18n/af.po` (6,101 lines)
- `addons/project/i18n/ar.po` (6,933 lines)
- `addons/project/i18n/az.po` (6,314 lines)
- `addons/project/i18n/bg.po` (6,331 lines)
- `addons/project/i18n/bs.po` (6,279 lines)
- `addons/project/i18n/ca.po` (6,704 lines)
- `addons/project/i18n/cs.po` (6,481 lines)
- `addons/project/i18n/da.po` (6,370 lines)
- `addons/project/i18n/de.po` (7,299 lines)
- `addons/project/i18n/el.po` (6,548 lines)
- `addons/project/i18n/es.po` (7,164 lines)
- `addons/project/i18n/es_419.po` (7,172 lines)
- `addons/project/i18n/es_CL.po` (423 lines)
- `addons/project/i18n/et.po` (6,909 lines)
- `addons/project/i18n/eu.po` (6,099 lines)
- `addons/project/i18n/fa.po` (6,475 lines)
- `addons/project/i18n/fi.po` (7,146 lines)
- `addons/project/i18n/fr.po` (7,271 lines)
- `addons/project/i18n/gl.po` (6,099 lines)
- `addons/project/i18n/gu.po` (6,111 lines)
- `addons/project/i18n/he.po` (6,497 lines)
- `addons/project/i18n/hi.po` (6,323 lines)
- `addons/project/i18n/hr.po` (6,352 lines)
- `addons/project/i18n/hu.po` (6,351 lines)
- `addons/project/i18n/id.po` (7,232 lines)
- `addons/project/i18n/is.po` (6,135 lines)
- `addons/project/i18n/it.po` (7,168 lines)
- `addons/project/i18n/ja.po` (6,981 lines)
- `addons/project/i18n/ka.po` (6,099 lines)
- `addons/project/i18n/kab.po` (6,267 lines)
- `addons/project/i18n/km.po` (6,113 lines)
- `addons/project/i18n/ko.po` (6,904 lines)
- `addons/project/i18n/ku.po` (6,280 lines)
- `addons/project/i18n/lb.po` (6,102 lines)
- `addons/project/i18n/lo.po` (6,885 lines)
- `addons/project/i18n/lt.po` (6,341 lines)
- `addons/project/i18n/lv.po` (6,305 lines)
- `addons/project/i18n/mk.po` (6,117 lines)
- `addons/project/i18n/mn.po` (6,337 lines)
- `addons/project/i18n/my.po` (6,289 lines)
- `addons/project/i18n/nb.po` (6,292 lines)
- `addons/project/i18n/nl.po` (7,223 lines)
- `addons/project/i18n/pl.po` (7,044 lines)
- `addons/project/i18n/project.pot` (6,166 lines)
- `addons/project/i18n/pt.po` (6,871 lines)
- `addons/project/i18n/pt_BR.po` (7,245 lines)
- `addons/project/i18n/ro.po` (6,916 lines)
- `addons/project/i18n/ru.po` (7,002 lines)
- `addons/project/i18n/sk.po` (6,333 lines)
- `addons/project/i18n/sl.po` (6,329 lines)
- `addons/project/i18n/sr@latin.po` (6,307 lines)
- `addons/project/i18n/sv.po` (6,587 lines)
- `addons/project/i18n/th.po` (7,041 lines)
- `addons/project/i18n/tr.po` (6,958 lines)
- `addons/project/i18n/uk.po` (6,478 lines)
- `addons/project/i18n/uz.po` (7,540 lines)
- `addons/project/i18n/vi.po` (6,980 lines)
- `addons/project/i18n/zh_CN.po` (6,998 lines)
- `addons/project/i18n/zh_TW.po` (6,694 lines)
- `addons/project/migrations/1.4/post-migrate.py` (6 lines)
- `addons/project/models/__init__.py` (27 lines)
- `addons/project/models/account_analytic_account.py` (44 lines)
- `addons/project/models/account_analytic_line.py` (18 lines)
- `addons/project/models/digest_digest.py` (31 lines)
- `addons/project/models/ir_ui_menu.py` (20 lines)
- `addons/project/models/mail_activity.py` (9 lines)
- `addons/project/models/mail_message.py` (9 lines)
- `addons/project/models/project_collaborator.py` (57 lines)
- `addons/project/models/project_milestone.py` (141 lines)
- `addons/project/models/project_project.py` (1,441 lines)
- `addons/project/models/project_project_stage.py` (78 lines)
- `addons/project/models/project_role.py` (24 lines)
- `addons/project/models/project_tags.py` (119 lines)
- `addons/project/models/project_task.py` (2,414 lines)
- `addons/project/models/project_task_recurrence.py` (122 lines)
- `addons/project/models/project_task_stage_personal.py` (20 lines)
- `addons/project/models/project_task_type.py` (239 lines)
- `addons/project/models/project_update.py` (147 lines)
- `addons/project/models/res_config_settings.py` (18 lines)
- `addons/project/models/res_groups.py` (16 lines)
- `addons/project/models/res_partner.py` (82 lines)
- `addons/project/models/res_users.py` (44 lines)
- `addons/project/models/res_users_settings.py` (36 lines)
- `addons/project/populate/benchmarks.xml` (299 lines)
- `addons/project/populate/populate_demo.xml` (127 lines)
- `addons/project/report/__init__.py` (6 lines)
- `addons/project/report/project_report.py` (169 lines)
- `addons/project/report/project_report_views.xml` (93 lines)
- `addons/project/report/project_task_burndown_chart_report.py` (189 lines)
- `addons/project/report/project_task_burndown_chart_report_views.xml` (64 lines)
- `addons/project/report/project_time_by_stage_report.py` (107 lines)
- `addons/project/report/project_time_by_stage_report_views.xml` (95 lines)
- `addons/project/security/ir.access.csv` (147 lines)
- `addons/project/security/project_security.xml` (63 lines)
- `addons/project/static/description/icon.png` (25 lines)
- `addons/project/static/description/icon.svg` (1 lines)
- `addons/project/static/description/icon_hi.png` (89 lines)
- `addons/project/static/src/actions/client_actions.js` (186 lines)
- `addons/project/static/src/components/done_checkmark/task_done_checkmark.js` (28 lines)
- `addons/project/static/src/components/done_checkmark/task_done_checkmark.scss` (26 lines)
- `addons/project/static/src/components/done_checkmark/task_done_checkmark.xml` (12 lines)
- `addons/project/static/src/components/float_time_days/float_time_field.js` (19 lines)
- `addons/project/static/src/components/notebook_task_one2many_field/notebook_task_list_renderer.js` (56 lines)
- `addons/project/static/src/components/notebook_task_one2many_field/notebook_task_list_renderer.xml` (20 lines)
- `addons/project/static/src/components/notebook_task_one2many_field/notebook_task_one2many_field.js` (26 lines)
- `addons/project/static/src/components/project_configure_project_cog_menu/project_configure_project_cog_menu.js` (39 lines)
- `addons/project/static/src/components/project_configure_project_cog_menu/project_configure_project_cog_menu.xml` (10 lines)
- `addons/project/static/src/components/project_convert_project_to_template_cog_menu/project_convert_project_to_template_cog_menu.js` (41 lines)
- `addons/project/static/src/components/project_convert_project_to_template_cog_menu/project_convert_project_to_template_cog_menu.xml` (10 lines)
- `addons/project/static/src/components/project_is_favorite/project_is_favorite_field.js` (14 lines)
- `addons/project/static/src/components/project_many2one_field/project_many2one_field.js` (42 lines)
- `addons/project/static/src/components/project_many2one_field/project_many2one_field.scss` (4 lines)
- `addons/project/static/src/components/project_many2one_field/project_many2one_field.xml` (20 lines)
- `addons/project/static/src/components/project_state_selection/project_state_selection.js` (29 lines)
- `addons/project/static/src/components/project_state_selection/project_state_selection.scss` (3 lines)
- `addons/project/static/src/components/project_status_with_color_selection/project_status_with_color_selection_field.js` (49 lines)
- `addons/project/static/src/components/project_status_with_color_selection/project_status_with_color_selection_field.xml` (15 lines)
- `addons/project/static/src/components/project_task_name_with_subtask_count_char_field/project_task_name_with_subtask_count_char_field.js` (16 lines)
- `addons/project/static/src/components/project_task_name_with_subtask_count_char_field/project_task_name_with_subtask_count_char_field.xml` (14 lines)
- `addons/project/static/src/components/project_task_priority_switch_field/project_task_priority_switch_field.js` (29 lines)
- `addons/project/static/src/components/project_task_state_selection/project_task_stage_state_selection/project_task_stage_with_state_selection.js` (48 lines)
- `addons/project/static/src/components/project_task_state_selection/project_task_stage_state_selection/project_task_stage_with_state_selection.xml` (10 lines)
- `addons/project/static/src/components/project_task_state_selection/project_task_state_selection.js` (204 lines)
- `addons/project/static/src/components/project_task_state_selection/project_task_state_selection.scss` (28 lines)
- `addons/project/static/src/components/project_task_state_selection/project_task_state_selection.xml` (112 lines)
- `addons/project/static/src/components/subtask_kanban_list/subtask_kanban_create/subtask_kanban_create.js` (69 lines)
- `addons/project/static/src/components/subtask_kanban_list/subtask_kanban_create/subtask_kanban_create.xml` (18 lines)
- `addons/project/static/src/components/subtask_kanban_list/subtask_kanban_list.js` (113 lines)
- `addons/project/static/src/components/subtask_kanban_list/subtask_kanban_list.scss` (23 lines)
- `addons/project/static/src/components/subtask_kanban_list/subtask_kanban_list.xml` (43 lines)
- `addons/project/static/src/components/subtask_one2many_field/subtask_list_renderer.js` (17 lines)
- `addons/project/static/src/components/subtask_one2many_field/subtask_one2many_field.js` (38 lines)
- `addons/project/static/src/components/task_list_renderer.js` (20 lines)
- `addons/project/static/src/core/web/@types/models.d.ts` (5 lines)
- `addons/project/static/src/core/web/activity_menu_patch.js` (15 lines)
- `addons/project/static/src/core/web/follower_list_patch.js` (33 lines)
- `addons/project/static/src/core/web/thread_model_patch.js` (13 lines)
- `addons/project/static/src/css/project.css` (8 lines)
- `addons/project/static/src/img/app_store.png` (39 lines)
- `addons/project/static/src/img/bird.jpg` (71 lines)
- `addons/project/static/src/img/chrome_store.png` (43 lines)

Additional files not expanded here: 235. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
