# Module: portal

- **Module ID:** MOD-419
- **Path:** `addons/portal`
- **Manifest:** `addons/portal/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Customer Portal


This module adds required base code for a fully integrated customer portal.
It contains the base controller class and base templates. Business addons
will add their specific templates and controllers to extend the customer
portal.

This module contains most code coming from odoo v10 website_portal. Purpose
of this module is to allow the display of a customer portal without having
a dependency towards website editing and customization capabilities.

Declared dependencies: `auth_signup`, `base_address_extended`, `html_editor`, `http_routing`, `mail`, `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 32 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 6 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 33 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 16 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_signup",
    "base_address_extended",
    "html_editor",
    "http_routing",
    "mail",
    "web"
  ],
  "data": [
    "data/mail_templates.xml",
    "data/portal_entry_data.xml",
    "views/address_templates.xml",
    "views/mail_templates_public.xml",
    "views/portal_templates.xml",
    "views/res_config_settings_views.xml",
    "wizard/portal_share_views.xml",
    "wizard/portal_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web._assets_primary_variables": [
      "portal/static/src/scss/primary_variables.scss"
    ],
    "web._assets_frontend_helpers": [
      [
        "prepend",
        "portal/static/src/scss/bootstrap_overridden.scss"
      ]
    ],
    "web.assets_backend": [
      "portal/static/src/core/common/**/*",
      "portal/static/src/views/**/*"
    ],
    "mail.assets_public": [
      "portal/static/src/core/common/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "portal/static/src/core/common/**/*"
    ],
    "web.assets_frontend": [
      "portal/static/src/interactions/**/*",
      "portal/static/src/scss/portal.scss",
      "portal/static/src/js/**/*",
      "portal/static/src/xml/**/*",
      "portal/static/src/signature_form/**/*",
      "portal/static/src/chatter/frontend/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "portal/static/src/interactions/**/*",
      "portal/static/src/js/components/input_confirmation_dialog/*",
      "portal/static/src/xml/**/*"
    ],
    "web.assets_tests": [
      "portal/static/tests/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "portal/static/src/core/common/**/*",
      "web/static/src/views/view_dialogs/form_view_dialog.js",
      "web/static/src/views/view_dialogs/export_data_dialog.js",
      "web/static/src/core/debug/*",
      "web/static/src/core/commands/command_hook.js",
      "web/static/src/model/**/*",
      "web/static/src/search/**/*",
      "web/static/src/views/view.js",
      "web/static/src/views/view_hook.js",
      "web/static/src/webclient/actions/action_dialog.js",
      "web/static/src/webclient/actions/reports/utils.js",
      "web/static/src/webclient/actions/reports/report_action.js",
      "web/static/src/views/utils.js",
      "web/static/src/views/fields/formatters.js",
      "web/static/src/views/fields/file_handler.*",
      "mail/static/src/model/**/*",
      "mail/static/src/core/common/core.scss",
      "mail/static/src/core/common/**/*",
      "mail/static/src/core/web_portal_project/**/*",
      "mail/static/src/**/common/**/*",
      "mail/static/src/chatter/web_portal_project/**/*",
      [
        "remove",
        "mail/static/src/**/*.dark.scss"
      ],
      "portal/static/src/chatter/portal/portal_chatter_plugin.js"
    ],
    "portal.assets_chatter": [
      [
        "include",
        "web._assets_helpers"
      ],
      [
        "include",
        "web._assets_frontend_helpers"
      ],
      "web/static/src/scss/pre_variables.scss",
      "web/static/lib/bootstrap/scss/_variables.scss",
      "web/static/lib/bootstrap/scss/_variables-dark.scss",
      [
        "include",
        "html_editor.assets_editor"
      ],
      [
        "include",
        "portal.assets_chatter_helpers"
      ],
      "portal/static/src/chatter/portal/**/*",
      "portal/static/src/chatter/portal_project/**/*",
      [
        "remove",
        "mail/static/src/**/*.scss"
      ]
    ],
    "portal.assets_chatter_style": [
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
      "portal/static/src/chatter/portal/scss/primary_variables.scss",
      [
        "include",
        "web._assets_bootstrap_backend"
      ],
      "web/static/src/scss/mimetypes.scss",
      "web/static/src/scss/ui.scss",
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/webclient/webclient.scss",
      "web/static/src/core/dialog/dialog.scss",
      [
        "include",
        "html_editor.assets_editor"
      ],
      "web/static/src/core/avatar/avatar.scss",
      "web/static/src/core/dropdown/dropdown.scss",
      "web/static/src/core/emoji_picker/**/*",
      [
        "remove",
        "web/static/src/core/emoji_picker/emoji_data.js"
      ],
      "mail/static/src/core/common/core.scss",
      "mail/static/src/core/common/**/*.scss",
      "mail/static/src/chatter/web_portal_project/**/*.scss",
      [
        "remove",
        "mail/static/src/**/*.dark.scss"
      ],
      "portal/static/src/chatter/portal/scss/shadow.scss",
      "portal/static/src/chatter/portal/scss/portal_chatter.scss"
    ]
  }
}
```

### Representative source files

- `addons/portal/__init__.py` (14 lines)
- `addons/portal/__manifest__.py` (137 lines)
- `addons/portal/controllers/__init__.py` (5 lines)
- `addons/portal/controllers/mail.py` (61 lines)
- `addons/portal/controllers/message_reaction.py` (17 lines)
- `addons/portal/controllers/portal.py` (1,184 lines)
- `addons/portal/controllers/thread.py` (166 lines)
- `addons/portal/controllers/web.py` (27 lines)
- `addons/portal/data/mail_templates.xml` (16 lines)
- `addons/portal/data/portal_entry_data.xml` (18 lines)
- `addons/portal/i18n/ar.po` (1,585 lines)
- `addons/portal/i18n/az.po` (1,556 lines)
- `addons/portal/i18n/bg.po` (1,565 lines)
- `addons/portal/i18n/bs.po` (1,499 lines)
- `addons/portal/i18n/ca.po` (1,577 lines)
- `addons/portal/i18n/cs.po` (1,569 lines)
- `addons/portal/i18n/da.po` (1,542 lines)
- `addons/portal/i18n/de.po` (1,676 lines)
- `addons/portal/i18n/el.po` (1,519 lines)
- `addons/portal/i18n/es.po` (1,651 lines)
- `addons/portal/i18n/es_419.po` (1,657 lines)
- `addons/portal/i18n/et.po` (1,568 lines)
- `addons/portal/i18n/fa.po` (1,566 lines)
- `addons/portal/i18n/fi.po` (1,655 lines)
- `addons/portal/i18n/fr.po` (1,650 lines)
- `addons/portal/i18n/gu.po` (1,481 lines)
- `addons/portal/i18n/he.po` (1,540 lines)
- `addons/portal/i18n/hi.po` (1,505 lines)
- `addons/portal/i18n/hr.po` (1,607 lines)
- `addons/portal/i18n/hu.po` (1,580 lines)
- `addons/portal/i18n/id.po` (1,615 lines)
- `addons/portal/i18n/is.po` (1,477 lines)
- `addons/portal/i18n/it.po` (1,655 lines)
- `addons/portal/i18n/ja.po` (1,633 lines)
- `addons/portal/i18n/kab.po` (1,489 lines)
- `addons/portal/i18n/km.po` (1,484 lines)
- `addons/portal/i18n/ko.po` (1,585 lines)
- `addons/portal/i18n/ku.po` (1,502 lines)
- `addons/portal/i18n/lo.po` (1,544 lines)
- `addons/portal/i18n/lt.po` (1,533 lines)
- `addons/portal/i18n/lv.po` (1,513 lines)
- `addons/portal/i18n/mn.po` (1,531 lines)
- `addons/portal/i18n/my.po` (1,500 lines)
- `addons/portal/i18n/nb.po` (1,517 lines)
- `addons/portal/i18n/nl.po` (1,678 lines)
- `addons/portal/i18n/pl.po` (1,622 lines)
- `addons/portal/i18n/portal.pot` (1,482 lines)
- `addons/portal/i18n/pt.po` (1,608 lines)
- `addons/portal/i18n/pt_BR.po` (1,635 lines)
- `addons/portal/i18n/ro.po` (1,583 lines)
- `addons/portal/i18n/ru.po` (1,593 lines)
- `addons/portal/i18n/sk.po` (1,530 lines)
- `addons/portal/i18n/sl.po` (1,532 lines)
- `addons/portal/i18n/sr@latin.po` (1,564 lines)
- `addons/portal/i18n/sv.po` (1,580 lines)
- `addons/portal/i18n/th.po` (1,565 lines)
- `addons/portal/i18n/tr.po` (1,616 lines)
- `addons/portal/i18n/uk.po` (1,577 lines)
- `addons/portal/i18n/uz.po` (1,779 lines)
- `addons/portal/i18n/vi.po` (1,598 lines)
- `addons/portal/i18n/zh_CN.po` (1,614 lines)
- `addons/portal/i18n/zh_TW.po` (1,596 lines)
- `addons/portal/models/__init__.py` (13 lines)
- `addons/portal/models/ir_http.py` (22 lines)
- `addons/portal/models/ir_qweb.py` (25 lines)
- `addons/portal/models/ir_ui_view.py` (10 lines)
- `addons/portal/models/mail_message.py` (196 lines)
- `addons/portal/models/mail_thread.py` (96 lines)
- `addons/portal/models/portal_entry.py` (21 lines)
- `addons/portal/models/portal_mixin.py` (147 lines)
- `addons/portal/models/res_config_settings.py` (13 lines)
- `addons/portal/models/res_country.py` (98 lines)
- `addons/portal/models/res_partner.py` (156 lines)
- `addons/portal/models/res_users_apikeys_description.py` (20 lines)
- `addons/portal/security/ir.access.csv` (5 lines)
- `addons/portal/static/src/chatter/frontend/portal_chatter_boot.js` (33 lines)
- `addons/portal/static/src/chatter/portal/@types/models.d.ts` (5 lines)
- `addons/portal/static/src/chatter/portal/attachment_upload_service_patch.js` (17 lines)
- `addons/portal/static/src/chatter/portal/chat_hub_service_patch.js` (7 lines)
- `addons/portal/static/src/chatter/portal/chatter_patch.js` (44 lines)
- `addons/portal/static/src/chatter/portal/composer_model_patch.js` (10 lines)
- `addons/portal/static/src/chatter/portal/composer_patch.js` (17 lines)
- `addons/portal/static/src/chatter/portal/message_model_patch.js` (15 lines)
- `addons/portal/static/src/chatter/portal/message_patch.js` (12 lines)
- `addons/portal/static/src/chatter/portal/portal_chatter.js` (37 lines)
- `addons/portal/static/src/chatter/portal/portal_chatter_plugin.js` (5 lines)
- `addons/portal/static/src/chatter/portal/portal_chatter_service.js` (83 lines)
- `addons/portal/static/src/chatter/portal/scss/portal_chatter.scss` (17 lines)
- `addons/portal/static/src/chatter/portal/scss/primary_variables.scss` (30 lines)
- `addons/portal/static/src/chatter/portal/scss/shadow.scss` (21 lines)
- `addons/portal/static/src/chatter/portal/suggestion_service_patch.js` (18 lines)
- `addons/portal/static/src/chatter/portal/thread_model_patch.js` (23 lines)
- `addons/portal/static/src/chatter/portal_project/chatter_patch.js` (3 lines)
- `addons/portal/static/src/chatter/portal_project/message_patch.xml` (6 lines)
- `addons/portal/static/src/chatter/portal_project/portal_chatter.xml` (15 lines)
- `addons/portal/static/src/chatter/portal_project/thread_model_patch.js` (9 lines)
- `addons/portal/static/src/core/common/@types/models.d.ts` (7 lines)
- `addons/portal/static/src/core/common/message_model_patch.js` (15 lines)
- `addons/portal/static/src/img/portal-addresses.svg` (6 lines)
- `addons/portal/static/src/img/portal-connection.svg` (13 lines)
- `addons/portal/static/src/interactions/address.js` (289 lines)
- `addons/portal/static/src/interactions/address_card.js` (62 lines)
- `addons/portal/static/src/interactions/bootstrap_tooltip.js` (18 lines)
- `addons/portal/static/src/interactions/portal_composer.js` (219 lines)
- `addons/portal/static/src/interactions/portal_home_counters.js` (68 lines)
- `addons/portal/static/src/interactions/portal_profile_editor.js` (83 lines)
- `addons/portal/static/src/interactions/portal_search_panel.js` (54 lines)
- `addons/portal/static/src/interactions/portal_security.js` (255 lines)
- `addons/portal/static/src/interactions/sidebar.js` (159 lines)
- `addons/portal/static/src/js/components/input_confirmation_dialog/input_confirmation_dialog.js` (45 lines)
- `addons/portal/static/src/js/components/input_confirmation_dialog/input_confirmation_dialog.xml` (10 lines)
- `addons/portal/static/src/scss/bootstrap_overridden.scss` (51 lines)
- `addons/portal/static/src/scss/portal.edit.scss` (3 lines)
- `addons/portal/static/src/scss/portal.scss` (531 lines)
- `addons/portal/static/src/scss/primary_variables.scss` (5 lines)
- `addons/portal/static/src/signature_form/signature_form.js` (112 lines)
- `addons/portal/static/src/signature_form/signature_form.xml` (35 lines)
- `addons/portal/static/src/views/fields/portal_wizard_user_one2many.js` (17 lines)
- `addons/portal/static/src/views/fields/portal_wizard_user_one2many.scss` (3 lines)
- `addons/portal/static/src/views/list/portal_wizard_user_list_controller.js` (26 lines)
- `addons/portal/static/src/xml/portal_chatter.xml` (95 lines)
- `addons/portal/static/src/xml/portal_security.xml` (72 lines)
- `addons/portal/static/tests/tours/portal.js` (36 lines)
- `addons/portal/static/tests/tours/skip_to_content.js` (21 lines)
- `addons/portal/tests/__init__.py` (9 lines)
- `addons/portal/tests/test_addresses.py` (427 lines)
- `addons/portal/tests/test_login.py` (13 lines)
- `addons/portal/tests/test_message_format_portal.py` (52 lines)
- `addons/portal/tests/test_pager.py` (55 lines)
- `addons/portal/tests/test_portal.py` (217 lines)
- `addons/portal/tests/test_portal_wizard.py` (201 lines)
- `addons/portal/tests/test_tours.py` (35 lines)
- `addons/portal/utils.py` (26 lines)
- `addons/portal/views/address_templates.xml` (554 lines)
- `addons/portal/views/mail_templates_public.xml` (8 lines)
- `addons/portal/views/portal_templates.xml` (796 lines)
- `addons/portal/views/res_config_settings_views.xml` (23 lines)
- `addons/portal/wizard/__init__.py` (5 lines)
- `addons/portal/wizard/portal_share.py` (147 lines)
- `addons/portal/wizard/portal_share_views.xml` (32 lines)
- `addons/portal/wizard/portal_wizard.py` (276 lines)
- `addons/portal/wizard/portal_wizard_views.xml` (64 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
