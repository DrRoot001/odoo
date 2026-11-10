# Module: website_blog

- **Module ID:** MOD-598
- **Path:** `addons/website_blog`
- **Manifest:** `addons/website_blog/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Publish blog posts, announces, news

No manifest description declared.

Declared dependencies: `website_mail`, `website_partner`, `html_builder`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 27 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 33 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_mail",
    "website_partner",
    "html_builder"
  ],
  "data": [
    "data/mail_message_subtype_data.xml",
    "data/mail_templates.xml",
    "data/website_blog_data.xml",
    "data/blog_snippet_template_data.xml",
    "data/website_blog_tour.xml",
    "views/website_blog_views.xml",
    "views/website_blog_components.xml",
    "views/website_blog_posts_loop.xml",
    "views/website_blog_templates.xml",
    "views/snippets/snippets.xml",
    "views/snippets/s_blog_posts.xml",
    "views/snippets/s_blog_posts_carousel.xml",
    "views/snippets/s_dynamic_snippet_blog_posts_preview_data.xml",
    "views/snippets/s_dynamic_snippet_blog_posts_carousel_preview_data.xml",
    "views/website_blog_visitor_views.xml",
    "views/website_pages_views.xml",
    "views/blog_post_add.xml",
    "security/website_blog_security.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/website_blog_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "website_blog/static/src/tours/website_blog.js"
    ],
    "web.assets_tests": [
      "website_blog/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "website_blog/static/tests/interactions/**/*",
      "website_blog/static/tests/website_builder/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_blog/static/src/interactions/**/*.js",
      "website_blog/static/src/snippets/**/*.js"
    ],
    "web.assets_frontend": [
      "website_blog/static/src/interactions/**/*",
      "website_blog/static/src/scss/website_blog.scss",
      "website_blog/static/src/snippets/**/*.js"
    ],
    "website.assets_editor": [
      "website_blog/static/src/js/systray_items/*.js"
    ],
    "website.website_builder_assets": [
      "website_blog/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_blog/README.md` (91 lines)
- `addons/website_blog/__init__.py` (5 lines)
- `addons/website_blog/__manifest__.py` (64 lines)
- `addons/website_blog/controllers/__init__.py` (4 lines)
- `addons/website_blog/controllers/main.py` (360 lines)
- `addons/website_blog/data/blog_snippet_template_data.xml` (35 lines)
- `addons/website_blog/data/mail_message_subtype_data.xml` (12 lines)
- `addons/website_blog/data/mail_templates.xml` (12 lines)
- `addons/website_blog/data/website_blog_data.xml` (41 lines)
- `addons/website_blog/data/website_blog_demo.xml` (556 lines)
- `addons/website_blog/data/website_blog_tour.xml` (7 lines)
- `addons/website_blog/i18n/af.po` (3,037 lines)
- `addons/website_blog/i18n/ar.po` (3,097 lines)
- `addons/website_blog/i18n/az.po` (3,058 lines)
- `addons/website_blog/i18n/bg.po` (3,102 lines)
- `addons/website_blog/i18n/bs.po` (3,058 lines)
- `addons/website_blog/i18n/ca.po` (3,110 lines)
- `addons/website_blog/i18n/cs.po` (3,078 lines)
- `addons/website_blog/i18n/da.po` (3,107 lines)
- `addons/website_blog/i18n/de.po` (3,613 lines)
- `addons/website_blog/i18n/el.po` (3,073 lines)
- `addons/website_blog/i18n/es.po` (3,235 lines)
- `addons/website_blog/i18n/es_419.po` (3,387 lines)
- `addons/website_blog/i18n/es_CL.po` (130 lines)
- `addons/website_blog/i18n/et.po` (3,108 lines)
- `addons/website_blog/i18n/eu.po` (3,029 lines)
- `addons/website_blog/i18n/fa.po` (3,098 lines)
- `addons/website_blog/i18n/fi.po` (3,234 lines)
- `addons/website_blog/i18n/fr.po` (3,119 lines)
- `addons/website_blog/i18n/fr_BE.po` (83 lines)
- `addons/website_blog/i18n/fr_CA.po` (114 lines)
- `addons/website_blog/i18n/gl.po` (3,029 lines)
- `addons/website_blog/i18n/gu.po` (3,037 lines)
- `addons/website_blog/i18n/he.po` (3,077 lines)
- `addons/website_blog/i18n/hi.po` (3,059 lines)
- `addons/website_blog/i18n/hr.po` (3,076 lines)
- `addons/website_blog/i18n/hu.po` (3,075 lines)
- `addons/website_blog/i18n/id.po` (3,219 lines)
- `addons/website_blog/i18n/is.po` (3,033 lines)
- `addons/website_blog/i18n/it.po` (3,664 lines)
- `addons/website_blog/i18n/ja.po` (3,102 lines)
- `addons/website_blog/i18n/ka.po` (3,029 lines)
- `addons/website_blog/i18n/kab.po` (3,054 lines)
- `addons/website_blog/i18n/km.po` (3,039 lines)
- `addons/website_blog/i18n/ko.po` (3,103 lines)
- `addons/website_blog/i18n/ku.po` (3,054 lines)
- `addons/website_blog/i18n/lo.po` (3,518 lines)
- `addons/website_blog/i18n/lt.po` (3,081 lines)
- `addons/website_blog/i18n/lv.po` (3,064 lines)
- `addons/website_blog/i18n/mk.po` (3,041 lines)
- `addons/website_blog/i18n/mn.po` (3,079 lines)
- `addons/website_blog/i18n/my.po` (3,052 lines)
- `addons/website_blog/i18n/nb.po` (3,072 lines)
- `addons/website_blog/i18n/nl.po` (3,193 lines)
- `addons/website_blog/i18n/pl.po` (3,240 lines)
- `addons/website_blog/i18n/pt.po` (3,107 lines)
- `addons/website_blog/i18n/pt_BR.po` (3,635 lines)
- `addons/website_blog/i18n/ro.po` (3,100 lines)
- `addons/website_blog/i18n/ru.po` (3,097 lines)
- `addons/website_blog/i18n/sk.po` (3,071 lines)
- `addons/website_blog/i18n/sl.po` (3,067 lines)
- `addons/website_blog/i18n/sq.po` (3,035 lines)
- `addons/website_blog/i18n/sr@latin.po` (3,056 lines)
- `addons/website_blog/i18n/sv.po` (3,109 lines)
- `addons/website_blog/i18n/th.po` (3,169 lines)
- `addons/website_blog/i18n/tr.po` (3,124 lines)
- `addons/website_blog/i18n/uk.po` (3,099 lines)
- `addons/website_blog/i18n/uz.po` (3,278 lines)
- `addons/website_blog/i18n/vi.po` (3,104 lines)
- `addons/website_blog/i18n/website_blog.pot` (2,997 lines)
- `addons/website_blog/i18n/zh_CN.po` (3,459 lines)
- `addons/website_blog/i18n/zh_TW.po` (3,096 lines)
- `addons/website_blog/models/__init__.py` (9 lines)
- `addons/website_blog/models/res_partner.py` (9 lines)
- `addons/website_blog/models/website.py` (46 lines)
- `addons/website_blog/models/website_blog.py` (456 lines)
- `addons/website_blog/models/website_snippet_filter.py` (64 lines)
- `addons/website_blog/models/website_track.py` (11 lines)
- `addons/website_blog/models/website_visitor.py` (25 lines)
- `addons/website_blog/security/ir.access.csv` (11 lines)
- `addons/website_blog/security/website_blog_security.xml` (15 lines)
- `addons/website_blog/static/description/icon.png` (18 lines)
- `addons/website_blog/static/description/icon.svg` (1 lines)
- `addons/website_blog/static/description/icon_hi.png` (94 lines)
- `addons/website_blog/static/src/@types/plugins.d.ts` (7 lines)
- `addons/website_blog/static/src/img/anonymous.png` (17 lines)
- `addons/website_blog/static/src/img/blog_1.webp` (402 lines)
- `addons/website_blog/static/src/img/blog_2.webp` (181 lines)
- `addons/website_blog/static/src/img/blog_3.webp` (299 lines)
- `addons/website_blog/static/src/img/blog_4.webp` (603 lines)
- `addons/website_blog/static/src/img/content_1_1.webp` (333 lines)
- `addons/website_blog/static/src/img/content_2_1.webp` (284 lines)
- `addons/website_blog/static/src/img/content_3_1.webp` (231 lines)
- `addons/website_blog/static/src/img/content_4_1.webp` (162 lines)
- `addons/website_blog/static/src/img/content_5_1.webp` (354 lines)
- `addons/website_blog/static/src/img/content_6_1.webp` (147 lines)
- `addons/website_blog/static/src/img/content_7_1.webp` (121 lines)
- `addons/website_blog/static/src/img/cover_1.webp` (735 lines)
- `addons/website_blog/static/src/img/cover_2.webp` (410 lines)
- `addons/website_blog/static/src/img/cover_3.webp` (701 lines)
- `addons/website_blog/static/src/img/cover_4.webp` (433 lines)
- `addons/website_blog/static/src/img/cover_5.webp` (531 lines)
- `addons/website_blog/static/src/img/cover_6.webp` (765 lines)
- `addons/website_blog/static/src/img/cover_7.webp` (464 lines)
- `addons/website_blog/static/src/interactions/blog_table_of_contents.edit.js` (36 lines)
- `addons/website_blog/static/src/interactions/blog_table_of_contents.js` (170 lines)
- `addons/website_blog/static/src/interactions/components/blog_nav_sheet.js` (6 lines)
- `addons/website_blog/static/src/interactions/components/blog_nav_sheet.xml` (19 lines)
- `addons/website_blog/static/src/interactions/website_blog.edit.js` (19 lines)
- `addons/website_blog/static/src/interactions/website_blog.js` (170 lines)
- `addons/website_blog/static/src/js/systray_items/new_content.js` (39 lines)
- `addons/website_blog/static/src/scss/website_blog.scss` (216 lines)
- `addons/website_blog/static/src/snippets/s_blog_posts/000.scss` (227 lines)
- `addons/website_blog/static/src/snippets/s_blog_posts/blog_posts.js` (24 lines)
- `addons/website_blog/static/src/snippets/s_blog_posts/blog_posts_carousel.js` (20 lines)
- `addons/website_blog/static/src/snippets/s_blog_posts/blog_posts_mixin.js` (32 lines)
- `addons/website_blog/static/src/tours/website_blog.js` (115 lines)
- `addons/website_blog/static/src/website_builder/author_avatar_sync_plugin.js` (39 lines)
- `addons/website_blog/static/src/website_builder/blog_content_width_option.xml` (10 lines)
- `addons/website_blog/static/src/website_builder/blog_page_option.xml` (119 lines)
- `addons/website_blog/static/src/website_builder/blog_page_option_plugin.js` (82 lines)
- `addons/website_blog/static/src/website_builder/blog_post_page_option.xml` (181 lines)
- `addons/website_blog/static/src/website_builder/blog_post_page_option_plugin.js` (98 lines)
- `addons/website_blog/static/src/website_builder/blog_post_tags_option.js` (22 lines)
- `addons/website_blog/static/src/website_builder/blog_post_tags_option.xml` (23 lines)
- `addons/website_blog/static/src/website_builder/blog_searchbar_option_plugin.js` (25 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_carousel_option.js` (11 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_carousel_option.xml` (19 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_option.js` (76 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_option.xml` (25 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_option_plugin.js` (36 lines)
- `addons/website_blog/static/src/website_builder/dynamic_snippet_blog_posts_shared_option.xml` (67 lines)
- `addons/website_blog/static/tests/interactions/snippets/blog_posts.test.js` (84 lines)
- `addons/website_blog/static/tests/interactions/snippets/website_blog.test.js` (26 lines)
- `addons/website_blog/static/tests/tours/blog_context.js` (68 lines)
- `addons/website_blog/static/tests/tours/blog_manager_tour.js` (79 lines)
- `addons/website_blog/static/tests/tours/blog_posts_dynamic_snippet.js` (52 lines)
- `addons/website_blog/static/tests/tours/blog_posts_dynamic_snippet_visibility.js` (67 lines)
- `addons/website_blog/static/tests/tours/blog_search_with_date.js` (42 lines)
- `addons/website_blog/static/tests/tours/blog_sidebar_with_date_and_tag.js` (55 lines)
- `addons/website_blog/static/tests/tours/blog_tags_tour.js` (85 lines)
- `addons/website_blog/static/tests/tours/blog_tags_with_date.js` (65 lines)
- `addons/website_blog/static/tests/tours/snippet_blog_post.js` (41 lines)
- `addons/website_blog/static/tests/tours/sub_templates_config.js` (12 lines)
- `addons/website_blog/static/tests/website_builder/many2one_option.test.js` (159 lines)
- `addons/website_blog/static/tests/website_builder/snippet_filter.test.js` (92 lines)
- `addons/website_blog/tests/__init__.py` (8 lines)
- `addons/website_blog/tests/common.py` (46 lines)
- `addons/website_blog/tests/test_performance.py` (75 lines)
- `addons/website_blog/tests/test_sitemap.py` (53 lines)
- `addons/website_blog/tests/test_ui.py` (249 lines)
- `addons/website_blog/tests/test_website_blog_flow.py` (413 lines)
- `addons/website_blog/tests/test_website_blog_technical_page.py` (9 lines)
- `addons/website_blog/views/blog_post_add.xml` (26 lines)
- `addons/website_blog/views/snippets/s_blog_posts.xml` (335 lines)
- `addons/website_blog/views/snippets/s_blog_posts_carousel.xml` (16 lines)
- `addons/website_blog/views/snippets/s_dynamic_snippet_blog_posts_carousel_preview_data.xml` (51 lines)
- `addons/website_blog/views/snippets/s_dynamic_snippet_blog_posts_preview_data.xml` (322 lines)
- `addons/website_blog/views/snippets/snippets.xml` (22 lines)
- `addons/website_blog/views/website_blog_components.xml` (389 lines)

Additional files not expanded here: 5. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
