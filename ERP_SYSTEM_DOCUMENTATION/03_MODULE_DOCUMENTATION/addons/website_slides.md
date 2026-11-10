# Module: website_slides

- **Module ID:** MOD-643
- **Path:** `addons/website_slides`
- **Manifest:** `addons/website_slides/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage and publish an eLearning platform


Create Online Courses
=====================

Featuring

 * Integrated course and lesson management
 * Fullscreen navigation
 * Support Youtube videos, Google documents, PDF, images, articles
 * Test knowledge with quizzes
 * Filter and Tag
 * Statistics


Declared dependencies: `portal_rating`, `website`, `website_mail`, `website_profile`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 47 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 23 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 65 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 75 | Client behavior/assets. |
| Tests | 16 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 39 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "portal_rating",
    "website",
    "website_mail",
    "website_profile",
    "digest"
  ],
  "data": [
    "security/website_slides_security.xml",
    "views/digest_views.xml",
    "views/gamification_karma_tracking_views.xml",
    "views/mail_activity_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/rating_rating_views.xml",
    "views/slide_embed_views.xml",
    "views/slide_question_views.xml",
    "views/slide_slide_partner_views.xml",
    "views/slide_slide_views.xml",
    "views/slide_channel_partner_views.xml",
    "views/slide_channel_views.xml",
    "views/slide_channel_tag_views.xml",
    "views/website_slides_menu_views.xml",
    "views/website_slides_templates_homepage.xml",
    "views/website_slides_templates_course.xml",
    "views/website_slides_templates_lesson.xml",
    "views/website_slides_templates_lesson_fullscreen.xml",
    "views/website_slides_templates_lesson_embed.xml",
    "views/website_slides_templates_profile.xml",
    "views/website_slides_templates_utils.xml",
    "views/website_slides_visitor_views.xml",
    "views/website_pages_views.xml",
    "views/slide_channel_add.xml",
    "views/website_slides_snippet_templates.xml",
    "wizard/slide_channel_invite_views.xml",
    "data/digest_data.xml",
    "data/gamification_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_template_data.xml",
    "data/portal_entry_data.xml",
    "data/slide_data.xml",
    "data/website_data.xml",
    "data/slides_tour.xml",
    "data/website_snippet_filter_data.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_users_demo.xml",
    "data/slide_channel_tag_demo.xml",
    "data/slide_channel_demo.xml",
    "data/slide_slide_demo.xml",
    "data/slide_user_demo.xml",
    "data/slide_user_gamification_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "website_slides/static/src/core/**/*",
      "website_slides/static/src/slide_category_one2many_field.js",
      "website_slides/static/src/slide_category_list_renderer.js",
      "website_slides/static/src/scss/slide_views.scss",
      "website_slides/static/src/js/tours/slides_tour.js",
      "website_slides/static/src/js/components/**/*.js",
      "website_slides/static/src/views/**/*.js",
      "website_slides/static/src/views/**/*.xml"
    ],
    "web.assets_frontend": [
      "website_slides/static/src/interactions/**/*",
      "website_slides/static/src/js/slides_course_service.js",
      "website_slides/static/src/js/utils.js",
      "website_slides/static/src/scss/website_slides.scss",
      "website_slides/static/src/scss/website_slides_profile.scss",
      "website_slides/static/src/scss/slides_slide_fullscreen.scss",
      "website_slides/static/src/xml/website_slides_sidebar.xml",
      "website_slides/static/src/xml/website_slides_fullscreen.xml",
      "website_slides/static/src/xml/slide_management.xml",
      "website_slides/static/src/xml/slide_course_join.xml",
      "website_slides/static/src/xml/slide_course_prerequisite.xml",
      "website_slides/static/src/xml/slide_quiz.xml",
      "website_slides/static/src/js/public/**/*"
    ],
    "website.assets_editor": [
      "website_slides/static/src/js/systray_items/*.js"
    ],
    "web.assets_tests": [
      "website_slides/static/tests/tours/*.js"
    ],
    "website_slides.slide_embed_assets": [
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
      "web/static/lib/bootstrap/scss/_maps.scss",
      [
        "include",
        "web._assets_bootstrap_frontend"
      ],
      [
        "include",
        "web.icons_fonts"
      ],
      "web/static/src/module_loader.js",
      "web/static/src/session.js",
      "web/static/lib/luxon/luxon.js",
      "web/static/src/libs/luxon.js",
      "web/static/lib/owl/owl.js",
      "web/static/src/owl2/owl3_compatibility_layer.js",
      "web/static/src/owl2/utils.js",
      "web/static/lib/owl/odoo_module.js",
      "web/static/src/core/utils/transitions.scss",
      "web/static/src/core/**/*",
      "web/static/src/env.js",
      [
        "remove",
        "web/static/src/core/emoji_picker/emoji_data.js"
      ],
      "website_slides/static/src/scss/website_slides.scss",
      "website_slides/static/src/js/slides_embed.js",
      "website_slides/static/src/js/public/components/slide_share_dialog/*",
      "web/static/src/public/**/*.js",
      "web/static/src/public/**/*.xml",
      [
        "remove",
        "web/static/src/public/database_manager.js"
      ]
    ],
    "web.assets_unit_tests": [
      "website_slides/static/tests/**/*",
      [
        "remove",
        "website_slides/static/tests/tours/**/*"
      ]
    ],
    "web.assets_unit_tests_setup": [
      "website_slides/static/src/interactions/**/*",
      "website_slides/static/src/js/public/**/*",
      "website_slides/static/src/js/slides_course_service.js",
      "website_slides/static/src/js/utils.js"
    ],
    "website.website_builder_assets": [
      "website_slides/static/src/website_builder/**/*"
    ],
    "im_livechat.assets_embed_core": [
      "website_slides/static/src/core/common/**/*"
    ],
    "mail.assets_public": [
      "website_slides/static/src/core/common/**/*"
    ],
    "portal.assets_chatter": [
      "website_slides/static/src/chatter/portal/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "website_slides/static/src/core/common/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_slides/__init__.py` (6 lines)
- `addons/website_slides/__manifest__.py` (170 lines)
- `addons/website_slides/controllers/__init__.py` (5 lines)
- `addons/website_slides/controllers/legacy.py` (21 lines)
- `addons/website_slides/controllers/main.py` (1,646 lines)
- `addons/website_slides/controllers/portal.py` (9 lines)
- `addons/website_slides/data/digest_data.xml` (9 lines)
- `addons/website_slides/data/gamification_data.xml` (207 lines)
- `addons/website_slides/data/mail_message_subtype_data.xml` (10 lines)
- `addons/website_slides/data/mail_template_data.xml` (201 lines)
- `addons/website_slides/data/portal_entry_data.xml` (12 lines)
- `addons/website_slides/data/res_users_demo.xml` (16 lines)
- `addons/website_slides/data/slide_channel_demo.xml` (158 lines)
- `addons/website_slides/data/slide_channel_tag_demo.xml` (31 lines)
- `addons/website_slides/data/slide_data.xml` (29 lines)
- `addons/website_slides/data/slide_slide_demo.xml` (831 lines)
- `addons/website_slides/data/slide_user_demo.xml` (235 lines)
- `addons/website_slides/data/slide_user_gamification_demo.xml` (42 lines)
- `addons/website_slides/data/slides_tour.xml` (7 lines)
- `addons/website_slides/data/website_data.xml` (21 lines)
- `addons/website_slides/data/website_snippet_filter_data.xml` (19 lines)
- `addons/website_slides/i18n/af.po` (7,043 lines)
- `addons/website_slides/i18n/ar.po` (7,671 lines)
- `addons/website_slides/i18n/az.po` (7,057 lines)
- `addons/website_slides/i18n/bg.po` (7,170 lines)
- `addons/website_slides/i18n/bs.po` (7,234 lines)
- `addons/website_slides/i18n/ca.po` (7,722 lines)
- `addons/website_slides/i18n/cs.po` (7,270 lines)
- `addons/website_slides/i18n/da.po` (7,341 lines)
- `addons/website_slides/i18n/de.po` (7,959 lines)
- `addons/website_slides/i18n/el.po` (7,057 lines)
- `addons/website_slides/i18n/es.po` (7,759 lines)
- `addons/website_slides/i18n/es_419.po` (7,913 lines)
- `addons/website_slides/i18n/es_CL.po` (250 lines)
- `addons/website_slides/i18n/et.po` (7,163 lines)
- `addons/website_slides/i18n/eu.po` (7,035 lines)
- `addons/website_slides/i18n/fa.po` (7,305 lines)
- `addons/website_slides/i18n/fi.po` (7,767 lines)
- `addons/website_slides/i18n/fr.po` (7,773 lines)
- `addons/website_slides/i18n/gl.po` (7,035 lines)
- `addons/website_slides/i18n/gu.po` (7,050 lines)
- `addons/website_slides/i18n/he.po` (7,117 lines)
- `addons/website_slides/i18n/hi.po` (7,089 lines)
- `addons/website_slides/i18n/hr.po` (7,105 lines)
- `addons/website_slides/i18n/hu.po` (7,078 lines)
- `addons/website_slides/i18n/id.po` (7,720 lines)
- `addons/website_slides/i18n/is.po` (7,043 lines)
- `addons/website_slides/i18n/it.po` (7,759 lines)
- `addons/website_slides/i18n/ja.po` (7,701 lines)
- `addons/website_slides/i18n/ka.po` (7,035 lines)
- `addons/website_slides/i18n/kab.po` (7,121 lines)
- `addons/website_slides/i18n/km.po` (7,040 lines)
- `addons/website_slides/i18n/ko.po` (7,684 lines)
- `addons/website_slides/i18n/ku.po` (7,045 lines)
- `addons/website_slides/i18n/lb.po` (7,038 lines)
- `addons/website_slides/i18n/lo.po` (7,605 lines)
- `addons/website_slides/i18n/lt.po` (7,180 lines)
- `addons/website_slides/i18n/lv.po` (7,145 lines)
- `addons/website_slides/i18n/mk.po` (7,047 lines)
- `addons/website_slides/i18n/mn.po` (7,076 lines)
- `addons/website_slides/i18n/my.po` (7,053 lines)
- `addons/website_slides/i18n/nb.po` (7,056 lines)
- `addons/website_slides/i18n/nl.po` (7,906 lines)
- `addons/website_slides/i18n/pl.po` (7,376 lines)
- `addons/website_slides/i18n/pt.po` (7,687 lines)
- `addons/website_slides/i18n/pt_BR.po` (7,872 lines)
- `addons/website_slides/i18n/ro.po` (7,369 lines)
- `addons/website_slides/i18n/ru.po` (7,752 lines)
- `addons/website_slides/i18n/sk.po` (7,137 lines)
- `addons/website_slides/i18n/sl.po` (7,070 lines)
- `addons/website_slides/i18n/sq.po` (7,041 lines)
- `addons/website_slides/i18n/sr@latin.po` (7,325 lines)
- `addons/website_slides/i18n/sv.po` (7,356 lines)
- `addons/website_slides/i18n/th.po` (7,594 lines)
- `addons/website_slides/i18n/tr.po` (7,693 lines)
- `addons/website_slides/i18n/uk.po` (7,296 lines)
- `addons/website_slides/i18n/uz.po` (8,292 lines)
- `addons/website_slides/i18n/vi.po` (7,716 lines)
- `addons/website_slides/i18n/website_slides.pot` (6,955 lines)
- `addons/website_slides/i18n/zh_CN.po` (7,646 lines)
- `addons/website_slides/i18n/zh_TW.po` (7,243 lines)
- `addons/website_slides/models/__init__.py` (24 lines)
- `addons/website_slides/models/base_partner_merge.py` (25 lines)
- `addons/website_slides/models/digest.py` (39 lines)
- `addons/website_slides/models/gamification_challenge.py` (12 lines)
- `addons/website_slides/models/gamification_karma_tracking.py` (14 lines)
- `addons/website_slides/models/mail_activity.py` (14 lines)
- `addons/website_slides/models/mail_message.py` (21 lines)
- `addons/website_slides/models/res_config_settings.py` (14 lines)
- `addons/website_slides/models/res_groups.py` (16 lines)
- `addons/website_slides/models/res_partner.py` (90 lines)
- `addons/website_slides/models/res_users.py` (36 lines)
- `addons/website_slides/models/slide_channel.py` (1,178 lines)
- `addons/website_slides/models/slide_channel_partner.py` (278 lines)
- `addons/website_slides/models/slide_channel_tag.py` (37 lines)
- `addons/website_slides/models/slide_embed.py` (23 lines)
- `addons/website_slides/models/slide_question.py` (72 lines)
- `addons/website_slides/models/slide_slide.py` (1,386 lines)
- `addons/website_slides/models/slide_slide_partner.py` (55 lines)
- `addons/website_slides/models/slide_slide_resource.py` (73 lines)
- `addons/website_slides/models/slide_tag.py` (14 lines)
- `addons/website_slides/models/website.py` (37 lines)
- `addons/website_slides/models/website_track.py` (11 lines)
- `addons/website_slides/models/website_visitor.py` (25 lines)
- `addons/website_slides/security/ir.access.csv` (99 lines)
- `addons/website_slides/security/website_slides_security.xml` (23 lines)
- `addons/website_slides/static/description/icon.png` (14 lines)
- `addons/website_slides/static/description/icon.svg` (1 lines)
- `addons/website_slides/static/description/icon_hi.png` (109 lines)
- `addons/website_slides/static/src/chatter/portal/chatter_patch.js` (15 lines)
- `addons/website_slides/static/src/chatter/portal/message_model_patch.js` (26 lines)
- `addons/website_slides/static/src/core/common/@types/models.d.ts` (8 lines)
- `addons/website_slides/static/src/core/common/activity_model_patch.js` (12 lines)
- `addons/website_slides/static/src/core/common/thread_model_patch.js` (11 lines)
- `addons/website_slides/static/src/core/web/activity_patch.js` (31 lines)
- `addons/website_slides/static/src/core/web/activity_patch.xml` (16 lines)
- `addons/website_slides/static/src/img/banner_default.svg` (1 lines)
- `addons/website_slides/static/src/img/banner_default_all.svg` (1 lines)
- `addons/website_slides/static/src/img/banner_heroes_default.svg` (1 lines)
- `addons/website_slides/static/src/img/channel-documentation-default.jpg` (365 lines)
- `addons/website_slides/static/src/img/channel-documentation-layout.png` (54 lines)
- `addons/website_slides/static/src/img/channel-training-default.jpg` (442 lines)
- `addons/website_slides/static/src/img/channel-training-layout.png` (48 lines)
- `addons/website_slides/static/src/img/channel_demo_furniture.jpg` (270 lines)
- `addons/website_slides/static/src/img/channel_demo_furniture_2.jpg` (227 lines)
- `addons/website_slides/static/src/img/channel_demo_furniture_3.jpg` (573 lines)
- `addons/website_slides/static/src/img/channel_demo_gardening.jpg` (423 lines)
- `addons/website_slides/static/src/img/channel_demo_gardening_2.jpg` (1,375 lines)
- `addons/website_slides/static/src/img/channel_demo_gardening_3.jpg` (1,284 lines)
- `addons/website_slides/static/src/img/channel_demo_tree_1.jpg` (747 lines)
- `addons/website_slides/static/src/img/courses.svg` (21 lines)
- `addons/website_slides/static/src/img/document.png` (47 lines)
- `addons/website_slides/static/src/img/onboarding-quiz.png` (142 lines)
- `addons/website_slides/static/src/img/presentation.pdf` (214 lines)
- `addons/website_slides/static/src/img/quiz_modal_success.svg` (1 lines)
- `addons/website_slides/static/src/img/slide_demo_furniture.jpg` (636 lines)
- `addons/website_slides/static/src/img/slide_demo_furniture_2.jpg` (226 lines)
- `addons/website_slides/static/src/img/slide_demo_furniture_img.jpg` (273 lines)
- `addons/website_slides/static/src/img/slide_demo_furniture_img_1.jpg` (208 lines)
- `addons/website_slides/static/src/img/slide_demo_gardening.jpg` (1,011 lines)
- `addons/website_slides/static/src/img/slide_demo_gardening_1.jpg` (744 lines)
- `addons/website_slides/static/src/img/slide_demo_gardening_2.jpg` (1,965 lines)
- `addons/website_slides/static/src/img/slide_demo_owl.jpg` (282 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_5WMqwTnZ-qs.jpg` (418 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_PYr1rK8pS30.jpg` (760 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_QYmgrw0PgLU.jpg` (521 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_bvSe6r5BpaY.jpg` (172 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_ebBez6bcSEc.jpg` (192 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_grrXe1QZNzQ.jpg` (374 lines)
- `addons/website_slides/static/src/img/slide_demo_thumb_l0JZ25VvbwE.jpg` (1,774 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_img_1.jpg` (776 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_img_2.jpg` (590 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_img_3.jpg` (1,034 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_infographic_1.jpg` (1,332 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_infographic_2.jpg` (1,600 lines)
- `addons/website_slides/static/src/img/slide_demo_tree_infographic_3.jpg` (1,248 lines)
- `addons/website_slides/static/src/img/slide_demo_wood_infographic_1.jpg` (3,048 lines)
- `addons/website_slides/static/src/img/standard_badge_bronze.svg` (1 lines)
- `addons/website_slides/static/src/img/standard_badge_gold.svg` (1 lines)
- `addons/website_slides/static/src/img/standard_badge_silver.svg` (1 lines)

Additional files not expanded here: 140. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
