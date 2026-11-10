# Module: crm

- **Module ID:** MOD-054
- **Path:** `addons/crm`
- **Manifest:** `addons/crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Track leads and close opportunities

No manifest description declared.

Declared dependencies: `base_setup`, `base_install_request`, `sales_team`, `mail`, `calendar`, `resource`, `utm`, `web_tour`, `contacts`, `digest`, `phone_validation`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 50 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 18 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 49 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 48 | Client behavior/assets. |
| Tests | 20 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup",
    "base_install_request",
    "sales_team",
    "mail",
    "calendar",
    "resource",
    "utm",
    "web_tour",
    "contacts",
    "digest",
    "phone_validation"
  ],
  "data": [
    "security/crm_security.xml",
    "data/crm_lead_merge_template.xml",
    "data/crm_lead_prediction_data.xml",
    "data/crm_lost_reason_data.xml",
    "data/crm_stage_data.xml",
    "data/crm_team_data.xml",
    "data/digest_data.xml",
    "data/ir_cron_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/crm_recurring_plan_data.xml",
    "data/mail_templates.xml",
    "data/crm_tour.xml",
    "wizard/crm_lead_lost_views.xml",
    "wizard/crm_lead_to_opportunity_mass_views.xml",
    "wizard/crm_merge_opportunities_views.xml",
    "wizard/crm_lead_pls_update_views.xml",
    "views/calendar_views.xml",
    "views/crm_recurring_plan_views.xml",
    "views/crm_lost_reason_views.xml",
    "views/crm_stage_views.xml",
    "views/crm_lead_views.xml",
    "views/crm_team_member_views.xml",
    "views/digest_views.xml",
    "views/mail_activity_plan_views.xml",
    "views/mail_activity_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/utm_campaign_views.xml",
    "report/crm_activity_report_views.xml",
    "report/crm_opportunity_report_views.xml",
    "views/crm_team_views.xml",
    "views/crm_menu_views.xml",
    "views/crm_helper_templates.xml",
    "views/crm_lead_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/crm_team_demo.xml",
    "data/crm_stage_demo.xml",
    "data/mail_template_demo.xml",
    "data/crm_team_member_demo.xml",
    "data/crm_lead_demo.xml"
  ],
  "assets": {
    "im_livechat.assets_embed_core": [
      "crm/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "crm/static/src/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "crm/static/src/core/common/**/*"
    ],
    "web.assets_backend": [
      "crm/static/src/**",
      [
        "remove",
        "crm/static/src/views/crm_activity/**"
      ],
      [
        "remove",
        "crm/static/src/views/crm_graph/**"
      ],
      [
        "remove",
        "crm/static/src/views/crm_pivot/**"
      ],
      [
        "remove",
        "crm/static/src/views/forecast_graph/**"
      ],
      [
        "remove",
        "crm/static/src/views/forecast_pivot/**"
      ]
    ],
    "web.assets_backend_lazy": [
      "crm/static/src/views/crm_activity/**",
      "crm/static/src/views/crm_graph/**",
      "crm/static/src/views/crm_pivot/**",
      "crm/static/src/views/forecast_graph/**",
      "crm/static/src/views/forecast_pivot/**"
    ],
    "web.assets_tests": [
      "crm/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "crm/static/tests/mock_server/**/*",
      "crm/static/tests/crm_test_helpers.js",
      "crm/static/tests/**/*.test.js",
      "crm/static/tests/crm_mock_server.js"
    ]
  }
}
```

### Representative source files

- `addons/crm/README.md` (97 lines)
- `addons/crm/__init__.py` (7 lines)
- `addons/crm/__manifest__.py` (109 lines)
- `addons/crm/controllers/__init__.py` (4 lines)
- `addons/crm/controllers/main.py` (44 lines)
- `addons/crm/controllers/webmanifest.py` (9 lines)
- `addons/crm/data/crm_lead_demo.xml` (1,321 lines)
- `addons/crm/data/crm_lead_merge_template.xml` (176 lines)
- `addons/crm/data/crm_lead_prediction_data.xml` (45 lines)
- `addons/crm/data/crm_lost_reason_data.xml` (13 lines)
- `addons/crm/data/crm_recurring_plan_data.xml` (24 lines)
- `addons/crm/data/crm_stage_data.xml` (21 lines)
- `addons/crm/data/crm_stage_demo.xml` (7 lines)
- `addons/crm/data/crm_team_data.xml` (15 lines)
- `addons/crm/data/crm_team_demo.xml` (13 lines)
- `addons/crm/data/crm_team_member_demo.xml` (13 lines)
- `addons/crm/data/crm_tour.xml` (8 lines)
- `addons/crm/data/digest_data.xml` (114 lines)
- `addons/crm/data/ir_cron_data.xml` (13 lines)
- `addons/crm/data/mail_message_subtype_data.xml` (76 lines)
- `addons/crm/data/mail_template_demo.xml` (28 lines)
- `addons/crm/data/mail_templates.xml` (8 lines)
- `addons/crm/doc/changelog.rst` (17 lines)
- `addons/crm/doc/index.rst` (18 lines)
- `addons/crm/doc/stage_status.rst` (61 lines)
- `addons/crm/i18n/af.po` (4,590 lines)
- `addons/crm/i18n/am.po` (4,586 lines)
- `addons/crm/i18n/ar.po` (4,867 lines)
- `addons/crm/i18n/az.po` (4,794 lines)
- `addons/crm/i18n/bg.po` (4,822 lines)
- `addons/crm/i18n/bs.po` (4,624 lines)
- `addons/crm/i18n/ca.po` (4,860 lines)
- `addons/crm/i18n/crm.pot` (4,553 lines)
- `addons/crm/i18n/cs.po` (4,820 lines)
- `addons/crm/i18n/da.po` (4,910 lines)
- `addons/crm/i18n/de.po` (5,120 lines)
- `addons/crm/i18n/el.po` (4,683 lines)
- `addons/crm/i18n/es.po` (5,084 lines)
- `addons/crm/i18n/es_419.po` (5,067 lines)
- `addons/crm/i18n/es_CL.po` (186 lines)
- `addons/crm/i18n/et.po` (4,827 lines)
- `addons/crm/i18n/eu.po` (4,589 lines)
- `addons/crm/i18n/fa.po` (4,787 lines)
- `addons/crm/i18n/fi.po` (5,067 lines)
- `addons/crm/i18n/fo.po` (4,589 lines)
- `addons/crm/i18n/fr.po` (5,089 lines)
- `addons/crm/i18n/fr_CA.po` (170 lines)
- `addons/crm/i18n/gl.po` (4,589 lines)
- `addons/crm/i18n/gu.po` (4,601 lines)
- `addons/crm/i18n/he.po` (4,773 lines)
- `addons/crm/i18n/hi.po` (4,658 lines)
- `addons/crm/i18n/hr.po` (4,745 lines)
- `addons/crm/i18n/hu.po` (4,728 lines)
- `addons/crm/i18n/id.po` (5,043 lines)
- `addons/crm/i18n/is.po` (4,623 lines)
- `addons/crm/i18n/it.po` (5,064 lines)
- `addons/crm/i18n/ja.po` (4,992 lines)
- `addons/crm/i18n/ka.po` (4,589 lines)
- `addons/crm/i18n/kab.po` (4,600 lines)
- `addons/crm/i18n/km.po` (4,598 lines)
- `addons/crm/i18n/ko.po` (4,834 lines)
- `addons/crm/i18n/ku.po` (4,608 lines)
- `addons/crm/i18n/lb.po` (4,591 lines)
- `addons/crm/i18n/lo.po` (4,882 lines)
- `addons/crm/i18n/lt.po` (4,705 lines)
- `addons/crm/i18n/lv.po` (4,680 lines)
- `addons/crm/i18n/mk.po` (4,589 lines)
- `addons/crm/i18n/mn.po` (4,698 lines)
- `addons/crm/i18n/my.po` (4,621 lines)
- `addons/crm/i18n/nb.po` (4,645 lines)
- `addons/crm/i18n/nl.po` (5,034 lines)
- `addons/crm/i18n/pl.po` (4,987 lines)
- `addons/crm/i18n/pt.po` (4,887 lines)
- `addons/crm/i18n/pt_BR.po` (5,068 lines)
- `addons/crm/i18n/ro.po` (4,857 lines)
- `addons/crm/i18n/ru.po` (5,012 lines)
- `addons/crm/i18n/sk.po` (4,758 lines)
- `addons/crm/i18n/sl.po` (4,839 lines)
- `addons/crm/i18n/sq.po` (4,589 lines)
- `addons/crm/i18n/sr@latin.po` (4,796 lines)
- `addons/crm/i18n/sv.po` (4,858 lines)
- `addons/crm/i18n/th.po` (4,886 lines)
- `addons/crm/i18n/tr.po` (4,864 lines)
- `addons/crm/i18n/uk.po` (4,800 lines)
- `addons/crm/i18n/uz.po` (5,492 lines)
- `addons/crm/i18n/vi.po` (4,871 lines)
- `addons/crm/i18n/zh_CN.po` (4,868 lines)
- `addons/crm/i18n/zh_TW.po` (4,710 lines)
- `addons/crm/models/__init__.py` (21 lines)
- `addons/crm/models/calendar.py` (55 lines)
- `addons/crm/models/crm_lead.py` (2,876 lines)
- `addons/crm/models/crm_lead_scoring_frequency.py` (30 lines)
- `addons/crm/models/crm_lost_reason.py` (34 lines)
- `addons/crm/models/crm_recurring_plan.py` (21 lines)
- `addons/crm/models/crm_stage.py` (85 lines)
- `addons/crm/models/crm_team.py` (837 lines)
- `addons/crm/models/crm_team_member.py` (126 lines)
- `addons/crm/models/digest.py` (39 lines)
- `addons/crm/models/discuss_channel.py` (23 lines)
- `addons/crm/models/ir_config_parameter.py` (31 lines)
- `addons/crm/models/mail_activity.py` (34 lines)
- `addons/crm/models/res_config_settings.py` (175 lines)
- `addons/crm/models/res_groups.py` (14 lines)
- `addons/crm/models/res_partner.py` (61 lines)
- `addons/crm/models/res_users.py` (17 lines)
- `addons/crm/models/utm.py` (30 lines)
- `addons/crm/report/__init__.py` (4 lines)
- `addons/crm/report/crm_activity_report.py` (103 lines)
- `addons/crm/report/crm_activity_report_views.xml` (123 lines)
- `addons/crm/report/crm_opportunity_report_views.xml` (231 lines)
- `addons/crm/security/crm_security.xml` (15 lines)
- `addons/crm/security/ir.access.csv` (35 lines)
- `addons/crm/static/description/icon.png` (11 lines)
- `addons/crm/static/description/icon.svg` (1 lines)
- `addons/crm/static/description/icon_hi.png` (44 lines)
- `addons/crm/static/src/activity_menu_patch.js` (55 lines)
- `addons/crm/static/src/components/breadcrumbs/crm_breadcrumbs.js` (14 lines)
- `addons/crm/static/src/components/breadcrumbs/crm_breadcrumbs.xml` (17 lines)
- `addons/crm/static/src/components/lead_generation_dropdown/lead_generation_dropdown.js` (267 lines)
- `addons/crm/static/src/components/lead_generation_dropdown/lead_generation_dropdown.scss` (33 lines)
- `addons/crm/static/src/components/lead_generation_dropdown/lead_generation_dropdown.xml` (40 lines)
- `addons/crm/static/src/components/promote_mail_plugins_dialog/promote_mail_plugins_dialog.js` (10 lines)
- `addons/crm/static/src/components/promote_mail_plugins_dialog/promote_mail_plugins_dialog.xml` (46 lines)
- `addons/crm/static/src/components/team_switcher/team_switcher.js` (62 lines)
- `addons/crm/static/src/components/team_switcher/team_switcher.xml` (31 lines)
- `addons/crm/static/src/core/common/@types/models.d.ts` (13 lines)
- `addons/crm/static/src/core/common/crm_lead_model.js` (14 lines)
- `addons/crm/static/src/core/common/res_partner_model_patch.js` (11 lines)
- `addons/crm/static/src/img/lead_sourcing.png` (13 lines)
- `addons/crm/static/src/img/mail.png` (16 lines)
- `addons/crm/static/src/img/mail_plugins.png` (38 lines)
- `addons/crm/static/src/img/milk-autofill.gif` (215 lines)
- `addons/crm/static/src/img/milk-generate-leads.gif` (306 lines)
- `addons/crm/static/src/img/milk-mapview-toggle.gif` (527 lines)
- `addons/crm/static/src/img/milk-pipeline-progress.gif` (335 lines)
- `addons/crm/static/src/img/milk-probability-rate.gif` (382 lines)
- `addons/crm/static/src/img/pls-tooltip-ai-icon.png` (25 lines)
- `addons/crm/static/src/img/settings.png` (18 lines)
- `addons/crm/static/src/img/survey.png` (14 lines)
- `addons/crm/static/src/img/website.png` (32 lines)
- `addons/crm/static/src/js/fields/many2one_avatar_leader_user.js` (33 lines)
- `addons/crm/static/src/js/tours/crm.js` (105 lines)
- `addons/crm/static/src/scss/crm.scss` (19 lines)
- `addons/crm/static/src/scss/crm_team.scss` (11 lines)
- `addons/crm/static/src/scss/crm_team_member_views.scss` (16 lines)
- `addons/crm/static/src/views/check_rainbowman_message.js` (9 lines)
- `addons/crm/static/src/views/crm_activity/crm_activity_view.js` (12 lines)
- `addons/crm/static/src/views/crm_calendar/crm_calendar_view.js` (11 lines)
- `addons/crm/static/src/views/crm_control_panel.js` (9 lines)
- `addons/crm/static/src/views/crm_form/crm_form.js` (70 lines)
- `addons/crm/static/src/views/crm_form/crm_form.scss` (5 lines)
- `addons/crm/static/src/views/crm_form/crm_pls_tooltip_button.js` (80 lines)
- `addons/crm/static/src/views/crm_form/crm_pls_tooltip_button.scss` (33 lines)
- `addons/crm/static/src/views/crm_form/crm_pls_tooltip_button.xml` (146 lines)
- `addons/crm/static/src/views/crm_graph/crm_graph_view.js` (12 lines)
- `addons/crm/static/src/views/crm_kanban/crm_column_progress.js` (31 lines)
- `addons/crm/static/src/views/crm_kanban/crm_column_progress.xml` (47 lines)
- `addons/crm/static/src/views/crm_kanban/crm_kanban_arch_parser.js` (14 lines)
- `addons/crm/static/src/views/crm_kanban/crm_kanban_model.js` (35 lines)
- `addons/crm/static/src/views/crm_kanban/crm_kanban_renderer.js` (17 lines)

Additional files not expanded here: 77. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
