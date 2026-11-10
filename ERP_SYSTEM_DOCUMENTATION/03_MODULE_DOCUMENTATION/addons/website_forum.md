# Module: website_forum

- **Module ID:** MOD-618
- **Path:** `addons/website_forum`
- **Manifest:** `addons/website_forum/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage a forum with FAQ and Q&A


Ask questions, get answers, no distractions
        

Declared dependencies: `auth_signup`, `website_mail`, `website_profile`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 34 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 5 | Files under `controllers/` or `controllers.py`. |
| XML files | 35 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 21 | Client behavior/assets. |
| Tests | 13 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 41 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "auth_signup",
    "website_mail",
    "website_profile"
  ],
  "data": [
    "data/ir_config_parameter_data.xml",
    "data/forum_forum_template_faq.xml",
    "data/forum_forum_data.xml",
    "data/forum_post_reason_data.xml",
    "data/ir_actions_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_templates.xml",
    "data/website_menu_data.xml",
    "data/website_forum_tour.xml",
    "views/forum_post_views.xml",
    "views/forum_post_reason_views.xml",
    "views/forum_tag_views.xml",
    "views/forum_forum_views.xml",
    "views/gamification_karma_tracking_views.xml",
    "views/forum_menus.xml",
    "views/base_contact_templates.xml",
    "views/forum_forum_templates.xml",
    "views/forum_forum_templates_follow.xml",
    "views/forum_forum_templates_forum_all.xml",
    "views/forum_forum_templates_layout.xml",
    "views/forum_forum_templates_moderation.xml",
    "views/forum_forum_templates_post.xml",
    "views/forum_forum_templates_tools.xml",
    "views/website_profile_templates.xml",
    "data/gamification_badge_data_question.xml",
    "data/gamification_badge_data_answer.xml",
    "data/gamification_badge_data_participation.xml",
    "data/gamification_badge_data_moderation.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/forum_tag_demo.xml",
    "data/forum_post_demo.xml"
  ],
  "assets": {
    "website.assets_editor": [
      "website_forum/static/src/js/systray_items/*.js"
    ],
    "web.assets_tests": [
      "website_forum/static/tests/**/*",
      [
        "remove",
        "website_forum/static/tests/interactions/**/*"
      ]
    ],
    "web.assets_backend": [
      "website_forum/static/src/js/tours/website_forum.js"
    ],
    "web.assets_frontend": [
      "website_forum/static/src/interactions/**/*",
      "website_forum/static/src/js/tours/website_forum.js",
      "website_forum/static/src/scss/website_forum.scss",
      "website_forum/static/src/scss/website_forum_wysiwyg.scss",
      "website_forum/static/src/xml/public_templates.xml",
      "website_forum/static/src/xml/website_forum_tags_wrapper.xml",
      "website_forum/static/src/components/**/*",
      "website_forum/static/src/plugins/**/*"
    ],
    "web.assets_unit_tests": [
      "website_forum/static/tests/interactions/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_forum/static/src/interactions/website_forum_share.js",
      "website_forum/static/src/interactions/website_forum_spam.js",
      "website_forum/static/src/interactions/website_forum.js",
      "website_forum/static/src/components/**/*",
      "website_forum/static/src/plugins/**/*",
      "website_forum/static/src/xml/public_templates.xml"
    ],
    "website.website_builder_assets": [
      "website_forum/static/src/website_builder/**/*"
    ],
    "web.assets_frontend_minimal": [
      "website_forum/static/src/interactions/loader_loading.js"
    ]
  }
}
```

### Representative source files

- `addons/website_forum/__init__.py` (4 lines)
- `addons/website_forum/__manifest__.py` (98 lines)
- `addons/website_forum/controllers/__init__.py` (6 lines)
- `addons/website_forum/controllers/legacy.py` (12 lines)
- `addons/website_forum/controllers/website.py` (16 lines)
- `addons/website_forum/controllers/website_forum.py` (855 lines)
- `addons/website_forum/controllers/website_mail.py` (39 lines)
- `addons/website_forum/data/forum_forum_data.xml` (10 lines)
- `addons/website_forum/data/forum_forum_template_faq.xml` (90 lines)
- `addons/website_forum/data/forum_post_demo.xml` (72 lines)
- `addons/website_forum/data/forum_post_reason_data.xml` (59 lines)
- `addons/website_forum/data/forum_tag_demo.xml` (24 lines)
- `addons/website_forum/data/gamification_badge_data_answer.xml` (256 lines)
- `addons/website_forum/data/gamification_badge_data_moderation.xml` (193 lines)
- `addons/website_forum/data/gamification_badge_data_participation.xml` (176 lines)
- `addons/website_forum/data/gamification_badge_data_question.xml` (399 lines)
- `addons/website_forum/data/ir_actions_data.xml` (14 lines)
- `addons/website_forum/data/ir_config_parameter_data.xml` (4 lines)
- `addons/website_forum/data/mail_message_subtype_data.xml` (63 lines)
- `addons/website_forum/data/mail_templates.xml` (41 lines)
- `addons/website_forum/data/website_forum_tour.xml` (7 lines)
- `addons/website_forum/data/website_menu_data.xml` (9 lines)
- `addons/website_forum/i18n/af.po` (4,188 lines)
- `addons/website_forum/i18n/ar.po` (4,440 lines)
- `addons/website_forum/i18n/az.po` (4,280 lines)
- `addons/website_forum/i18n/bg.po` (4,356 lines)
- `addons/website_forum/i18n/bs.po` (4,285 lines)
- `addons/website_forum/i18n/ca.po` (4,431 lines)
- `addons/website_forum/i18n/cs.po` (4,404 lines)
- `addons/website_forum/i18n/da.po` (4,474 lines)
- `addons/website_forum/i18n/de.po` (4,529 lines)
- `addons/website_forum/i18n/el.po` (4,284 lines)
- `addons/website_forum/i18n/es.po` (4,496 lines)
- `addons/website_forum/i18n/es_419.po` (4,489 lines)
- `addons/website_forum/i18n/et.po` (4,404 lines)
- `addons/website_forum/i18n/fa.po` (4,454 lines)
- `addons/website_forum/i18n/fi.po` (4,509 lines)
- `addons/website_forum/i18n/fr.po` (4,503 lines)
- `addons/website_forum/i18n/gu.po` (4,199 lines)
- `addons/website_forum/i18n/he.po` (4,338 lines)
- `addons/website_forum/i18n/hi.po` (4,287 lines)
- `addons/website_forum/i18n/hr.po` (4,301 lines)
- `addons/website_forum/i18n/hu.po` (4,341 lines)
- `addons/website_forum/i18n/id.po` (4,483 lines)
- `addons/website_forum/i18n/is.po` (4,190 lines)
- `addons/website_forum/i18n/it.po` (4,485 lines)
- `addons/website_forum/i18n/ja.po` (4,455 lines)
- `addons/website_forum/i18n/ka.po` (4,186 lines)
- `addons/website_forum/i18n/kab.po` (4,277 lines)
- `addons/website_forum/i18n/km.po` (4,197 lines)
- `addons/website_forum/i18n/ko.po` (4,440 lines)
- `addons/website_forum/i18n/ku.po` (4,283 lines)
- `addons/website_forum/i18n/lo.po` (4,409 lines)
- `addons/website_forum/i18n/lt.po` (4,339 lines)
- `addons/website_forum/i18n/lv.po` (4,290 lines)
- `addons/website_forum/i18n/mk.po` (4,204 lines)
- `addons/website_forum/i18n/mn.po` (4,339 lines)
- `addons/website_forum/i18n/my.po` (4,278 lines)
- `addons/website_forum/i18n/nb.po` (4,290 lines)
- `addons/website_forum/i18n/nl.po` (4,498 lines)
- `addons/website_forum/i18n/pl.po` (4,496 lines)
- `addons/website_forum/i18n/pt.po` (4,422 lines)
- `addons/website_forum/i18n/pt_BR.po` (4,488 lines)
- `addons/website_forum/i18n/ro.po` (4,486 lines)
- `addons/website_forum/i18n/ru.po` (4,474 lines)
- `addons/website_forum/i18n/sk.po` (4,331 lines)
- `addons/website_forum/i18n/sl.po` (4,290 lines)
- `addons/website_forum/i18n/sr@latin.po` (4,337 lines)
- `addons/website_forum/i18n/sv.po` (4,473 lines)
- `addons/website_forum/i18n/th.po` (4,408 lines)
- `addons/website_forum/i18n/tr.po` (4,481 lines)
- `addons/website_forum/i18n/uk.po` (4,442 lines)
- `addons/website_forum/i18n/uz.po` (5,075 lines)
- `addons/website_forum/i18n/vi.po` (4,471 lines)
- `addons/website_forum/i18n/website_forum.pot` (4,262 lines)
- `addons/website_forum/i18n/zh_CN.po` (4,389 lines)
- `addons/website_forum/i18n/zh_TW.po` (4,392 lines)
- `addons/website_forum/models/__init__.py` (15 lines)
- `addons/website_forum/models/forum_forum.py` (424 lines)
- `addons/website_forum/models/forum_post.py` (1,051 lines)
- `addons/website_forum/models/forum_post_comment.py` (92 lines)
- `addons/website_forum/models/forum_post_reason.py` (14 lines)
- `addons/website_forum/models/forum_post_vote.py` (126 lines)
- `addons/website_forum/models/forum_tag.py` (112 lines)
- `addons/website_forum/models/gamification_challenge.py` (11 lines)
- `addons/website_forum/models/gamification_karma_tracking.py` (10 lines)
- `addons/website_forum/models/ir_attachment.py` (21 lines)
- `addons/website_forum/models/ir_http.py` (13 lines)
- `addons/website_forum/models/mail_thread.py` (38 lines)
- `addons/website_forum/models/res_users.py` (21 lines)
- `addons/website_forum/models/website.py` (59 lines)
- `addons/website_forum/security/ir.access.csv` (21 lines)
- `addons/website_forum/static/description/icon.png` (33 lines)
- `addons/website_forum/static/description/icon.svg` (1 lines)
- `addons/website_forum/static/description/icon_hi.png` (125 lines)
- `addons/website_forum/static/src/components/flag_mark_as_offensive/flag_mark_as_offensive.js` (21 lines)
- `addons/website_forum/static/src/components/flag_mark_as_offensive/flag_mark_as_offensive.xml` (10 lines)
- `addons/website_forum/static/src/components/website_forum_tags_wrapper.js` (63 lines)
- `addons/website_forum/static/src/components/website_forum_wysiwyg/resizer.scss` (15 lines)
- `addons/website_forum/static/src/components/website_forum_wysiwyg/resizer_hook.js` (26 lines)
- `addons/website_forum/static/src/components/website_forum_wysiwyg/website_forum_wysiwyg.js` (110 lines)
- `addons/website_forum/static/src/components/website_forum_wysiwyg/website_forum_wysiwyg.xml` (11 lines)
- `addons/website_forum/static/src/img/empty.svg` (1 lines)
- `addons/website_forum/static/src/img/help.jpg` (513 lines)
- `addons/website_forum/static/src/img/tasks.svg` (5 lines)
- `addons/website_forum/static/src/interactions/loader_loading.js` (36 lines)
- `addons/website_forum/static/src/interactions/website_forum.js` (591 lines)
- `addons/website_forum/static/src/interactions/website_forum_activity.js` (43 lines)
- `addons/website_forum/static/src/interactions/website_forum_share.js` (40 lines)
- `addons/website_forum/static/src/interactions/website_forum_spam.js` (71 lines)
- `addons/website_forum/static/src/js/systray_items/forum_forum_add_form.js` (18 lines)
- `addons/website_forum/static/src/js/systray_items/new_content.js` (16 lines)
- `addons/website_forum/static/src/js/tours/website_forum.js` (131 lines)
- `addons/website_forum/static/src/plugins/font_type_plugin.js` (16 lines)
- `addons/website_forum/static/src/plugins/plugin_sets.js` (16 lines)
- `addons/website_forum/static/src/scss/website_forum.scss` (333 lines)
- `addons/website_forum/static/src/scss/website_forum_wysiwyg.scss` (32 lines)
- `addons/website_forum/static/src/website_builder/forum_floating_snippets_plugin.js` (18 lines)
- `addons/website_forum/static/src/website_builder/forum_page_option.xml` (32 lines)
- `addons/website_forum/static/src/website_builder/forum_searchbar_option_plugin.js` (24 lines)
- `addons/website_forum/static/src/xml/public_templates.xml` (62 lines)
- `addons/website_forum/static/src/xml/website_forum_tags_wrapper.xml` (28 lines)
- `addons/website_forum/static/tests/interactions/website_forum_editor.test.js` (59 lines)
- `addons/website_forum/static/tests/interactions/website_forum_share.test.js` (117 lines)
- `addons/website_forum/static/tests/interactions/website_forum_spam.test.js` (108 lines)
- `addons/website_forum/static/tests/tours/forum_cover_dropzone.js` (59 lines)
- `addons/website_forum/static/tests/tours/website_forum_question.js` (233 lines)
- `addons/website_forum/tests/__init__.py` (14 lines)
- `addons/website_forum/tests/common.py` (126 lines)
- `addons/website_forum/tests/test_forum_controller.py` (122 lines)
- `addons/website_forum/tests/test_forum_internals.py` (177 lines)
- `addons/website_forum/tests/test_forum_karma_access.py` (545 lines)
- `addons/website_forum/tests/test_forum_notifications.py` (105 lines)
- `addons/website_forum/tests/test_forum_post.py` (145 lines)
- `addons/website_forum/tests/test_forum_tag.py` (40 lines)
- `addons/website_forum/tests/test_forum_tours.py` (40 lines)
- `addons/website_forum/tests/test_performance.py` (83 lines)
- `addons/website_forum/tests/test_sitemap.py` (28 lines)
- `addons/website_forum/tests/test_web_editor.py` (113 lines)
- `addons/website_forum/tests/test_website_forum_technical_page.py` (9 lines)
- `addons/website_forum/views/base_contact_templates.xml` (42 lines)
- `addons/website_forum/views/forum_forum_templates.xml` (296 lines)
- `addons/website_forum/views/forum_forum_templates_follow.xml` (74 lines)
- `addons/website_forum/views/forum_forum_templates_forum_all.xml` (107 lines)
- `addons/website_forum/views/forum_forum_templates_layout.xml` (428 lines)
- `addons/website_forum/views/forum_forum_templates_moderation.xml` (236 lines)
- `addons/website_forum/views/forum_forum_templates_post.xml` (618 lines)
- `addons/website_forum/views/forum_forum_templates_tools.xml` (169 lines)
- `addons/website_forum/views/forum_forum_views.xml` (177 lines)
- `addons/website_forum/views/forum_menus.xml` (50 lines)
- `addons/website_forum/views/forum_post_reason_views.xml` (21 lines)
- `addons/website_forum/views/forum_post_views.xml` (188 lines)
- `addons/website_forum/views/forum_tag_views.xml` (44 lines)
- `addons/website_forum/views/gamification_karma_tracking_views.xml` (14 lines)
- `addons/website_forum/views/website_profile_templates.xml` (254 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
