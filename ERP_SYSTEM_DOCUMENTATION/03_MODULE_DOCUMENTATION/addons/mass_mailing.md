# Module: mass_mailing

- **Module ID:** MOD-362
- **Path:** `addons/mass_mailing`
- **Manifest:** `addons/mass_mailing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Design, send and track emails

No manifest description declared.

Declared dependencies: `contacts`, `mail`, `html_builder`, `utm`, `link_tracker`, `social_media`, `web_tour`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 55 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 26 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 103 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 97 | Client behavior/assets. |
| Tests | 16 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 17 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "contacts",
    "mail",
    "html_builder",
    "utm",
    "link_tracker",
    "social_media",
    "web_tour",
    "digest"
  ],
  "data": [
    "data/res_groups_privilege_data.xml",
    "security/res_groups_data.xml",
    "data/digest_data.xml",
    "data/ir_attachment_data.xml",
    "data/ir_config_parameter_data.xml",
    "data/ir_cron_data.xml",
    "data/ir_actions_server_data.xml",
    "data/mailing_data_templates.xml",
    "data/mailing_list_contact.xml",
    "data/mailing_subscription_optout.xml",
    "data/mailing_subscription.xml",
    "data/mass_mailing_tour.xml",
    "data/portal_entry_data.xml",
    "wizard/mail_compose_message_views.xml",
    "wizard/mailing_contact_import_views.xml",
    "wizard/mailing_contact_to_list_views.xml",
    "wizard/mailing_mailing_test_views.xml",
    "wizard/mailing_mailing_schedule_date_views.xml",
    "report/mailing_trace_report_views.xml",
    "views/mail_blacklist_views.xml",
    "views/mailing_filter_views.xml",
    "views/mailing_mobile_preview_content.xml",
    "views/mailing_trace_views.xml",
    "views/link_tracker_views.xml",
    "views/mailing_contact_views.xml",
    "views/mailing_list_views.xml",
    "views/mailing_mailing_views.xml",
    "views/mailing_subscription_optout_views.xml",
    "views/mailing_subscription_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/utm_campaign_views.xml",
    "views/mailing_menus.xml",
    "views/mailing_templates_portal_layouts.xml",
    "views/mailing_templates_portal_management.xml",
    "views/mailing_templates_portal_unsubscribe.xml",
    "views/themes_templates.xml",
    "views/themes_templates_blocks.xml",
    "views/snippets_themes.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/utm.xml",
    "demo/mailing_list_contact.xml",
    "demo/mailing_subscription.xml",
    "demo/mailing_mailing.xml",
    "demo/mailing_trace.xml",
    "demo/res_users.xml"
  ],
  "assets": {
    "mass_mailing.assets_builder": [
      [
        "include",
        "html_builder.assets"
      ],
      [
        "remove",
        "web/static/fonts/fonts.scss"
      ],
      "mass_mailing/static/src/builder/**/*",
      "mass_mailing/static/src/snippets/**/*.xml",
      [
        "remove",
        "mass_mailing/static/src/builder/**/*.inside.scss"
      ]
    ],
    "mass_mailing.assets_iframe_helpers": [
      [
        "include",
        "web._assets_helpers"
      ],
      "web/static/src/scss/bootstrap_overridden.scss",
      [
        "include",
        "web._assets_frontend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_maps.scss",
      "web/static/lib/bootstrap/scss/_alert.scss",
      [
        "include",
        "web._assets_bootstrap_frontend"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/scss/animation.scss",
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss"
    ],
    "mass_mailing.assets_iframe_theme_selector": [
      [
        "include",
        "mass_mailing.assets_iframe_helpers"
      ],
      "mass_mailing/static/src/themes/iframe_assets/**/*"
    ],
    "mass_mailing.assets_theme_selector_template_shadowdom": [
      "mass_mailing/static/src/fields/template_preview_field/theme_selector_template_preview/**/*.shadowdom.scss"
    ],
    "mass_mailing.assets_mailing_template_kanban_card_shadowdom": [
      "mass_mailing/static/src/fields/template_preview_field/mailing_template_kanban_card/**/*.shadowdom.scss"
    ],
    "mass_mailing.assets_iframe_style_base": [
      "html_editor/static/src/scss/html_editor.common.scss",
      "html_editor/static/src/scss/html_editor.frontend.scss",
      "html_editor/static/src/scss/base_style.scss",
      [
        "after",
        "web/static/lib/bootstrap/scss/_maps.scss",
        "mass_mailing/static/src/scss/mass_mailing.ui.scss"
      ],
      "html_builder/static/src/scss/background.scss",
      [
        "include",
        "mass_mailing.assets_mail_themes"
      ],
      "mass_mailing/static/src/scss/mass_mailing_mail.scss",
      "mass_mailing/static/src/iframe_assets/**/*",
      "mass_mailing/static/src/snippets/**/*.scss"
    ],
    "mass_mailing.assets_iframe_style": [
      [
        "include",
        "mass_mailing.assets_iframe_helpers"
      ],
      [
        "include",
        "html_editor.assets_readonly"
      ],
      [
        "include",
        "mass_mailing.assets_iframe_style_base"
      ]
    ],
    "mass_mailing.assets_inside_basic_editor_iframe": [
      [
        "include",
        "mass_mailing.assets_iframe_helpers"
      ],
      [
        "include",
        "html_editor.assets_editor"
      ],
      [
        "include",
        "mass_mailing.assets_iframe_style_base"
      ]
    ],
    "mass_mailing.assets_inside_builder_iframe": [
      [
        "include",
        "mass_mailing.assets_iframe_helpers"
      ],
      [
        "include",
        "html_editor.assets_editor"
      ],
      [
        "include",
        "html_builder.assets_inside_builder_iframe"
      ],
      [
        "include",
        "mass_mailing.assets_iframe_style_base"
      ],
      "mass_mailing/static/src/builder/**/*.inside.scss"
    ],
    "mass_mailing.iframe_add_dialog": [
      [
        "include",
        "html_builder.iframe_add_dialog"
      ],
      "mass_mailing/static/src/builder/snippet_viewer/*.scss"
    ],
    "mass_mailing.mailing_assets": [
      "mass_mailing/static/src/scss/mailing_portal.scss",
      "mass_mailing/static/src/interactions/subscribe.js",
      "mass_mailing/static/src/xml/mailing_portal_subscription_blocklist.xml",
      "mass_mailing/static/src/xml/mailing_portal_subscription_feedback.xml",
      "mass_mailing/static/src/xml/mailing_portal_subscription_form.xml"
    ],
    "web.assets_backend": [
      "mass_mailing/static/src/action/**/*",
      "mass_mailing/static/src/components/**/*",
      "mass_mailing/static/src/views/mailing_preview_form_view.js",
      "mass_mailing/static/src/views/mailing_preview_form_view.xml",
      "mass_mailing/static/src/views/format_utils.js",
      "mass_mailing/static/src/views/fields/**/*",
      "mass_mailing/static/src/views/mailing_filter*/**/*.js",
      "mass_mailing/static/src/views/mailing_template_kanban_view/**/*",
      "mass_mailing/static/src/editor/**/*",
      "mass_mailing/static/src/fields/**/*",
      "mass_mailing/static/src/themes/*",
      "mass_mailing/static/src/utils/**/*",
      "mass_mailing/static/src/themes/theme_selector/**/*",
      "mass_mailing/static/src/iframe/**/*",
      "mass_mailing/static/src/scss/mass_mailing.scss",
      "mass_mailing/static/src/scss/mass_mailing_mobile.scss",
      "mass_mailing/static/src/scss/mass_mailing_mobile_preview.scss",
      "mass_mailing/static/src/js/tours/**/*",
      [
        "remove",
        "mass_mailing/static/src/**/*.dark.scss"
      ],
      [
        "remove",
        "mass_mailing/static/src/**/*.shadowdom.scss"
      ]
    ],
    "web.assets_backend_lazy": [
      "mass_mailing/static/src/views/mass_mailing_subscription_graph_renderer.js"
    ],
    "web.assets_web_dark": [
      "mass_mailing/static/src/**/*.dark.scss"
    ],
    "mass_mailing.assets_mail_themes": [
      "mass_mailing/static/src/scss/themes/**/*"
    ],
    "web.assets_frontend": [
      "mass_mailing/static/src/js/tours/**/*"
    ],
    "web.assets_tests": [
      "mass_mailing/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      [
        "include",
        "mass_mailing.assets_builder"
      ],
      "mass_mailing/static/tests/**/*",
      [
        "remove",
        "mass_mailing/static/tests/tours/**/*"
      ]
    ]
  }
}
```

### Representative source files

- `addons/mass_mailing/README.md` (97 lines)
- `addons/mass_mailing/__init__.py` (45 lines)
- `addons/mass_mailing/__manifest__.py` (205 lines)
- `addons/mass_mailing/controllers/__init__.py` (5 lines)
- `addons/mass_mailing/controllers/legacy.py` (21 lines)
- `addons/mass_mailing/controllers/main.py` (564 lines)
- `addons/mass_mailing/data/digest_data.xml` (16 lines)
- `addons/mass_mailing/data/ir_actions_server_data.xml` (9 lines)
- `addons/mass_mailing/data/ir_attachment_data.xml` (204 lines)
- `addons/mass_mailing/data/ir_config_parameter_data.xml` (13 lines)
- `addons/mass_mailing/data/ir_cron_data.xml` (27 lines)
- `addons/mass_mailing/data/mailing_data_templates.xml` (117 lines)
- `addons/mass_mailing/data/mailing_list_contact.xml` (14 lines)
- `addons/mass_mailing/data/mailing_subscription.xml` (9 lines)
- `addons/mass_mailing/data/mailing_subscription_optout.xml` (24 lines)
- `addons/mass_mailing/data/mass_mailing_tour.xml` (10 lines)
- `addons/mass_mailing/data/portal_entry_data.xml` (10 lines)
- `addons/mass_mailing/data/res_groups_privilege_data.xml` (8 lines)
- `addons/mass_mailing/demo/mailing_list_contact.xml` (48 lines)
- `addons/mass_mailing/demo/mailing_mailing.xml` (90 lines)
- `addons/mass_mailing/demo/mailing_subscription.xml` (54 lines)
- `addons/mass_mailing/demo/mailing_trace.xml` (132 lines)
- `addons/mass_mailing/demo/res_users.xml` (8 lines)
- `addons/mass_mailing/demo/utm.xml` (12 lines)
- `addons/mass_mailing/doc/changelog.rst` (9 lines)
- `addons/mass_mailing/doc/index.rst` (13 lines)
- `addons/mass_mailing/i18n/af.po` (7,266 lines)
- `addons/mass_mailing/i18n/am.po` (7,262 lines)
- `addons/mass_mailing/i18n/ar.po` (7,679 lines)
- `addons/mass_mailing/i18n/az.po` (7,499 lines)
- `addons/mass_mailing/i18n/bg.po` (7,469 lines)
- `addons/mass_mailing/i18n/bs.po` (7,426 lines)
- `addons/mass_mailing/i18n/ca.po` (7,612 lines)
- `addons/mass_mailing/i18n/cs.po` (7,686 lines)
- `addons/mass_mailing/i18n/da.po` (7,532 lines)
- `addons/mass_mailing/i18n/de.po` (8,051 lines)
- `addons/mass_mailing/i18n/el.po` (7,446 lines)
- `addons/mass_mailing/i18n/es.po` (7,821 lines)
- `addons/mass_mailing/i18n/es_419.po` (8,027 lines)
- `addons/mass_mailing/i18n/es_CL.po` (194 lines)
- `addons/mass_mailing/i18n/et.po` (7,589 lines)
- `addons/mass_mailing/i18n/eu.po` (7,265 lines)
- `addons/mass_mailing/i18n/fa.po` (7,499 lines)
- `addons/mass_mailing/i18n/fi.po` (7,885 lines)
- `addons/mass_mailing/i18n/fo.po` (7,265 lines)
- `addons/mass_mailing/i18n/fr.po` (7,804 lines)
- `addons/mass_mailing/i18n/fr_BE.po` (189 lines)
- `addons/mass_mailing/i18n/fr_CA.po` (174 lines)
- `addons/mass_mailing/i18n/gl.po` (7,265 lines)
- `addons/mass_mailing/i18n/gu.po` (7,276 lines)
- `addons/mass_mailing/i18n/he.po` (7,506 lines)
- `addons/mass_mailing/i18n/hi.po` (7,454 lines)
- `addons/mass_mailing/i18n/hr.po` (7,461 lines)
- `addons/mass_mailing/i18n/hu.po` (7,469 lines)
- `addons/mass_mailing/i18n/id.po` (7,971 lines)
- `addons/mass_mailing/i18n/is.po` (7,275 lines)
- `addons/mass_mailing/i18n/it.po` (8,019 lines)
- `addons/mass_mailing/i18n/ja.po` (7,753 lines)
- `addons/mass_mailing/i18n/ka.po` (7,265 lines)
- `addons/mass_mailing/i18n/kab.po` (7,420 lines)
- `addons/mass_mailing/i18n/km.po` (7,275 lines)
- `addons/mass_mailing/i18n/ko.po` (7,625 lines)
- `addons/mass_mailing/i18n/ku.po` (7,432 lines)
- `addons/mass_mailing/i18n/lb.po` (7,267 lines)
- `addons/mass_mailing/i18n/lo.po` (7,782 lines)
- `addons/mass_mailing/i18n/lt.po` (7,495 lines)
- `addons/mass_mailing/i18n/lv.po` (7,447 lines)
- `addons/mass_mailing/i18n/mass_mailing.pot` (7,362 lines)
- `addons/mass_mailing/i18n/mk.po` (7,265 lines)
- `addons/mass_mailing/i18n/mn.po` (7,477 lines)
- `addons/mass_mailing/i18n/my.po` (7,424 lines)
- `addons/mass_mailing/i18n/nb.po` (7,458 lines)
- `addons/mass_mailing/i18n/nl.po` (8,030 lines)
- `addons/mass_mailing/i18n/pl.po` (7,910 lines)
- `addons/mass_mailing/i18n/pt.po` (7,650 lines)
- `addons/mass_mailing/i18n/pt_BR.po` (8,015 lines)
- `addons/mass_mailing/i18n/ro.po` (7,692 lines)
- `addons/mass_mailing/i18n/ru.po` (7,749 lines)
- `addons/mass_mailing/i18n/sk.po` (7,471 lines)
- `addons/mass_mailing/i18n/sl.po` (7,519 lines)
- `addons/mass_mailing/i18n/sq.po` (7,265 lines)
- `addons/mass_mailing/i18n/sr@latin.po` (7,443 lines)
- `addons/mass_mailing/i18n/sv.po` (7,681 lines)
- `addons/mass_mailing/i18n/th.po` (7,667 lines)
- `addons/mass_mailing/i18n/tr.po` (7,827 lines)
- `addons/mass_mailing/i18n/uk.po` (7,642 lines)
- `addons/mass_mailing/i18n/uz.po` (8,494 lines)
- `addons/mass_mailing/i18n/vi.po` (7,736 lines)
- `addons/mass_mailing/i18n/zh_CN.po` (7,739 lines)
- `addons/mass_mailing/i18n/zh_TW.po` (7,540 lines)
- `addons/mass_mailing/models/__init__.py` (29 lines)
- `addons/mass_mailing/models/ir_attachment.py` (10 lines)
- `addons/mass_mailing/models/ir_http.py` (12 lines)
- `addons/mass_mailing/models/ir_mail_server.py` (60 lines)
- `addons/mass_mailing/models/ir_model.py` (30 lines)
- `addons/mass_mailing/models/ir_ui_view.py` (7 lines)
- `addons/mass_mailing/models/link_tracker.py` (80 lines)
- `addons/mass_mailing/models/mail_blacklist.py` (20 lines)
- `addons/mass_mailing/models/mail_mail.py` (118 lines)
- `addons/mass_mailing/models/mail_render_mixin.py` (29 lines)
- `addons/mass_mailing/models/mail_thread.py` (104 lines)
- `addons/mass_mailing/models/mailing.py` (1,565 lines)
- `addons/mass_mailing/models/mailing_contact.py` (477 lines)
- `addons/mass_mailing/models/mailing_filter.py` (98 lines)
- `addons/mass_mailing/models/mailing_list.py` (519 lines)
- `addons/mass_mailing/models/mailing_subscription.py` (69 lines)
- `addons/mass_mailing/models/mailing_subscription_optout.py` (15 lines)
- `addons/mass_mailing/models/mailing_trace.py` (308 lines)
- `addons/mass_mailing/models/res_company.py` (48 lines)
- `addons/mass_mailing/models/res_config_settings.py` (56 lines)
- `addons/mass_mailing/models/res_groups.py` (13 lines)
- `addons/mass_mailing/models/res_partner.py` (53 lines)
- `addons/mass_mailing/models/res_users.py` (20 lines)
- `addons/mass_mailing/models/utm_campaign.py` (152 lines)
- `addons/mass_mailing/models/utm_medium.py` (23 lines)
- `addons/mass_mailing/models/utm_source.py` (23 lines)
- `addons/mass_mailing/report/__init__.py` (4 lines)
- `addons/mass_mailing/report/mailing_trace_report.py` (95 lines)
- `addons/mass_mailing/report/mailing_trace_report_views.xml` (102 lines)
- `addons/mass_mailing/security/ir.access.csv` (28 lines)
- `addons/mass_mailing/security/res_groups_data.xml` (16 lines)
- `addons/mass_mailing/static/description/icon.png` (16 lines)
- `addons/mass_mailing/static/description/icon.svg` (1 lines)
- `addons/mass_mailing/static/description/icon_hi.png` (119 lines)
- `addons/mass_mailing/static/shapes/s_attributes_1.svg` (7 lines)
- `addons/mass_mailing/static/shapes/s_attributes_2.svg` (13 lines)
- `addons/mass_mailing/static/shapes/s_attributes_3.svg` (11 lines)
- `addons/mass_mailing/static/shapes/s_attributes_4.svg` (14 lines)
- `addons/mass_mailing/static/shapes/s_attributes_5.svg` (13 lines)
- `addons/mass_mailing/static/shapes/s_newsletter_benefits_popup.svg` (243 lines)
- `addons/mass_mailing/static/shapes/s_newsletter_sms_notifications.svg` (316 lines)
- `addons/mass_mailing/static/src/action/client_actions.js` (21 lines)
- `addons/mass_mailing/static/src/builder/builder_overlay_patch.js` (14 lines)
- `addons/mass_mailing/static/src/builder/components/builder_row.scss` (3 lines)
- `addons/mass_mailing/static/src/builder/components/company_update_dialog.js` (97 lines)
- `addons/mass_mailing/static/src/builder/components/company_update_dialog.xml` (24 lines)
- `addons/mass_mailing/static/src/builder/components/mass_mailing_builder_select_label.js` (10 lines)
- `addons/mass_mailing/static/src/builder/components/mass_mailing_builder_select_label.scss` (26 lines)
- `addons/mass_mailing/static/src/builder/components/mass_mailing_builder_select_label.xml` (9 lines)
- `addons/mass_mailing/static/src/builder/fontfamily_picker.js` (58 lines)
- `addons/mass_mailing/static/src/builder/fontfamily_picker.xml` (12 lines)
- `addons/mass_mailing/static/src/builder/mass_mailing_builder.js` (78 lines)
- `addons/mass_mailing/static/src/builder/mass_mailing_builder.xml` (22 lines)
- `addons/mass_mailing/static/src/builder/mass_mailing_options.xml` (122 lines)
- `addons/mass_mailing/static/src/builder/mass_mailing_snippet_model.js` (29 lines)
- `addons/mass_mailing/static/src/builder/mass_mailing_snippet_preprocessor.js` (82 lines)
- `addons/mass_mailing/static/src/builder/options/alert_option.xml` (7 lines)
- `addons/mass_mailing/static/src/builder/options/alignment_option.xml` (12 lines)
- `addons/mass_mailing/static/src/builder/options/bento_blocks_add_card_option.xml` (13 lines)
- `addons/mass_mailing/static/src/builder/options/blockquote_option.xml` (8 lines)
- `addons/mass_mailing/static/src/builder/options/border_options.xml` (5 lines)
- `addons/mass_mailing/static/src/builder/options/color_picker_option.xml` (7 lines)
- `addons/mass_mailing/static/src/builder/options/company_team_options.xml` (11 lines)
- `addons/mass_mailing/static/src/builder/options/cta_badge_option.xml` (6 lines)
- `addons/mass_mailing/static/src/builder/options/image_tool_option.js` (16 lines)
- `addons/mass_mailing/static/src/builder/options/image_tool_option.xml` (35 lines)
- `addons/mass_mailing/static/src/builder/options/masonry_block_template_option.xml` (256 lines)
- `addons/mass_mailing/static/src/builder/options/options_container.js` (24 lines)
- `addons/mass_mailing/static/src/builder/options/options_container.scss` (11 lines)
- `addons/mass_mailing/static/src/builder/options/options_container.xml` (16 lines)

Additional files not expanded here: 321. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
