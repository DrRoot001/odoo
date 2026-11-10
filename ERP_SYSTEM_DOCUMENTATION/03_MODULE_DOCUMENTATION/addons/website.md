# Module: website

- **Module ID:** MOD-596
- **Path:** `addons/website`
- **Manifest:** `addons/website/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Enterprise website builder

No manifest description declared.

Declared dependencies: `digest`, `web`, `html_editor`, `http_routing`, `portal`, `social_media`, `auth_signup`, `mail`, `google_recaptcha`, `utm`, `html_builder`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 103 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 38 | Files under `models/` or `models.py`. |
| Controller-path Python files | 7 | Files under `controllers/` or `controllers.py`. |
| XML files | 418 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 674 | Client behavior/assets. |
| Tests | 49 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 65 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "digest",
    "web",
    "html_editor",
    "http_routing",
    "portal",
    "social_media",
    "auth_signup",
    "mail",
    "google_recaptcha",
    "utm",
    "html_builder"
  ],
  "data": [
    "security/website_security.xml",
    "data/image_library.xml",
    "data/ir_asset.xml",
    "data/ir_cron_data.xml",
    "data/mail_mail_data.xml",
    "data/website_data.xml",
    "data/website_visitor_cron.xml",
    "data/digest_data.xml",
    "views/website_technical_views.xml",
    "views/website_templates.xml",
    "views/theme_colors_preview.xml",
    "views/snippets/snippets.xml",
    "views/snippets/s_announcement_scroll.xml",
    "views/snippets/s_animated_number.xml",
    "views/snippets/s_framed_intro.xml",
    "views/snippets/s_title.xml",
    "views/snippets/s_cover.xml",
    "views/snippets/s_text_cover.xml",
    "views/snippets/s_image_text_box.xml",
    "views/snippets/s_striped_top.xml",
    "views/snippets/s_text_image.xml",
    "views/snippets/s_image_text.xml",
    "views/snippets/s_text_image_full.xml",
    "views/snippets/s_image_text_full.xml",
    "views/snippets/s_mockup_image.xml",
    "views/snippets/s_instagram_page.xml",
    "views/snippets/s_image_text_overlap.xml",
    "views/snippets/s_banner.xml",
    "views/snippets/s_bento_block.xml",
    "views/snippets/s_snippet_group.xml",
    "views/snippets/s_text_block.xml",
    "views/snippets/s_features.xml",
    "views/snippets/s_features_wall.xml",
    "views/snippets/s_three_columns.xml",
    "views/snippets/s_key_benefits.xml",
    "views/snippets/s_picture.xml",
    "views/snippets/s_image_punchy.xml",
    "views/snippets/s_bento_grid.xml",
    "views/snippets/s_carousel.xml",
    "views/snippets/s_carousel_intro.xml",
    "views/snippets/s_carousel_cards.xml",
    "views/snippets/s_alert.xml",
    "views/snippets/s_icon_list.xml",
    "views/snippets/s_motto.xml",
    "views/snippets/s_card.xml",
    "views/snippets/s_cards_grid.xml",
    "views/snippets/s_cards_soft.xml",
    "views/snippets/s_share.xml",
    "views/snippets/s_social_media.xml",
    "views/snippets/s_rating.xml",
    "views/snippets/s_hr.xml",
    "views/snippets/s_closer_look.xml",
    "views/snippets/s_awards_list.xml",
    "views/snippets/s_facebook_page.xml",
    "views/snippets/s_whatsapp.xml",
    "views/snippets/s_image_gallery.xml",
    "views/snippets/s_countdown.xml",
    "views/snippets/s_product_catalog.xml",
    "views/snippets/s_comparisons.xml",
    "views/snippets/s_comparisons_horizontal.xml",
    "views/snippets/s_company_team.xml",
    "views/snippets/s_company_team_basic.xml",
    "views/snippets/s_company_team_shapes.xml",
    "views/snippets/s_company_team_detail.xml",
    "views/snippets/s_company_team_spotlight.xml",
    "views/snippets/s_company_team_grid.xml",
    "views/snippets/s_company_team_card.xml",
    "views/snippets/s_call_to_action.xml",
    "views/snippets/s_references.xml",
    "views/snippets/s_references_social.xml",
    "views/snippets/s_references_grid.xml",
    "views/snippets/s_references_lite.xml",
    "views/snippets/s_references_tiles.xml",
    "views/snippets/s_popup.xml",
    "views/snippets/s_faq_list.xml",
    "views/snippets/s_faq_collapse.xml",
    "views/snippets/s_faq_collapse_centered.xml",
    "views/snippets/s_features_grid.xml",
    "views/snippets/s_features_wave.xml",
    "views/snippets/s_tabs.xml",
    "views/snippets/s_tabs_images.xml",
    "views/snippets/s_table_of_content.xml",
    "views/snippets/s_images_constellation.xml",
    "views/snippets/s_chart.xml",
    "views/snippets/s_parallax.xml",
    "views/snippets/s_quotes_carousel.xml",
    "views/snippets/s_numbers_grid.xml",
    "views/snippets/s_quotes_carousel_minimal.xml",
    "views/snippets/s_quotes_carousel_compact.xml",
    "views/snippets/s_numbers.xml",
    "views/snippets/s_numbers_inline.xml",
    "views/snippets/s_contact_info.xml",
    "views/snippets/s_numbers_boxed.xml",
    "views/snippets/s_cta_box.xml",
    "views/snippets/s_cta_centered.xml",
    "views/snippets/s_numbers_framed.xml",
    "views/snippets/s_masonry_block.xml",
    "views/snippets/s_sidegrid.xml",
    "views/snippets/s_media_list.xml",
    "views/snippets/s_services_pack.xml",
    "views/snippets/s_showcase.xml",
    "views/snippets/s_faq_horizontal.xml",
    "views/snippets/s_floating_blocks.xml",
    "views/snippets/s_opening_hours.xml",
    "views/snippets/s_opening_hours_alt.xml",
    "views/snippets/s_timeline.xml",
    "views/snippets/s_timeline_images.xml",
    "views/snippets/s_timeline_list.xml",
    "views/snippets/s_process_steps.xml",
    "views/snippets/s_accordion.xml",
    "views/snippets/s_website_form_info.xml",
    "views/snippets/s_numbers_showcase.xml",
    "views/snippets/s_numbers_charts.xml",
    "views/snippets/s_text_chart.xml",
    "views/snippets/s_chart_text.xml",
    "views/snippets/s_accordion_image.xml",
    "views/snippets/s_pricelist_boxed.xml",
    "views/snippets/s_adventure.xml",
    "views/snippets/s_image_title.xml",
    "views/snippets/s_banner_glow.xml",
    "views/snippets/s_intro_spotlight.xml",
    "views/snippets/s_bento_grid_avatars.xml",
    "views/snippets/s_key_images.xml",
    "views/snippets/s_kickoff.xml",
    "views/snippets/s_discovery.xml",
    "views/snippets/s_bento_banner.xml",
    "views/snippets/s_striped.xml",
    "views/snippets/s_intro_pill.xml",
    "views/snippets/s_big_number.xml",
    "views/snippets/s_wavy_grid.xml",
    "views/snippets/s_images_mosaic.xml",
    "views/snippets/s_shape_image.xml",
    "views/snippets/s_empowerment.xml",
    "views/snippets/s_split_intro.xml",
    "views/snippets/s_splash_intro.xml",
    "views/snippets/s_text_highlight.xml",
    "views/snippets/s_pricelist_cafe.xml",
    "views/snippets/s_progress_bar.xml",
    "views/snippets/s_blockquote.xml",
    "views/snippets/s_badge.xml",
    "views/snippets/s_color_blocks_2.xml",
    "views/snippets/s_attributes_horizontal.xml",
    "views/snippets/s_attributes_vertical.xml",
    "views/snippets/s_product_list.xml",
    "views/snippets/s_mega_menu_multi_menus.xml",
    "views/snippets/s_mega_menu_menu_image_menu.xml",
    "views/snippets/s_mega_menu_thumbnails.xml",
    "views/snippets/s_mega_menu_little_icons.xml",
    "views/snippets/s_mega_menu_images_subtitles.xml",
    "views/snippets/s_mega_menu_menus_logos.xml",
    "views/snippets/s_mega_menu_odoo_menu.xml",
    "views/snippets/s_mega_menu_dropzone.xml",
    "views/snippets/s_mega_menu_big_icons_subtitles.xml",
    "views/snippets/s_mega_menu_cards.xml",
    "views/snippets/s_google_map.xml",
    "views/snippets/s_cta_mockups.xml",
    "views/snippets/s_map.xml",
    "views/snippets/s_text_block_split.xml",
    "views/snippets/s_manifesto.xml",
    "views/snippets/s_bento_features.xml",
    "views/snippets/s_projects_grid.xml",
    "views/snippets/s_banner_contained.xml",
    "views/snippets/s_duo_images.xml",
    "views/snippets/s_hero_about.xml",
    "views/snippets/s_website_form_bold.xml",
    "views/snippets/s_title_split.xml",
    "views/snippets/s_hero_maintenance.xml",
    "views/snippets/s_hero_minimalist.xml",
    "views/snippets/s_launch_countdown.xml",
    "views/snippets/s_projects_grid_minimal.xml",
    "views/snippets/s_features_cards.xml",
    "views/snippets/s_achievements_list.xml",
    "views/snippets/s_text_bold.xml",
    "views/snippets/s_features_image.xml",
    "views/snippets/s_image_features.xml",
    "views/snippets/s_numbers_lite.xml",
    "views/snippets/s_hours_and_place.xml",
    "views/snippets/s_showcase_square.xml",
    "views/snippets/s_services_grid.xml",
    "views/snippets/s_dynamic_snippet.xml",
    "views/snippets/s_dynamic_snippet_carousel.xml",
    "views/snippets/s_banner_product.xml",
    "views/snippets/s_embed_code.xml",
    "views/snippets/s_website_form.xml",
    "views/snippets/s_website_form_overlay.xml",
    "views/snippets/s_title_form.xml",
    "views/snippets/s_searchbar.xml",
    "views/snippets/s_inline_text.xml",
    "views/snippets/s_button.xml",
    "views/snippets/s_freegrid.xml",
    "views/snippets/s_card_offset.xml",
    "views/snippets/s_image.xml",
    "views/snippets/s_icon.xml",
    "views/snippets/s_video.xml",
    "views/snippets/s_cta_badge.xml",
    "views/snippets/s_avatars.xml",
    "views/snippets/s_unveil.xml",
    "views/snippets/s_image_hexagonal.xml",
    "views/snippets/s_striped_center_top.xml",
    "views/snippets/s_numbers_list.xml",
    "views/snippets/s_quadrant.xml",
    "views/snippets/s_cta_card.xml",
    "views/snippets/s_image_frame.xml",
    "views/snippets/s_cta_mobile.xml",
    "views/snippets/s_reviews_wall.xml",
    "views/snippets/s_website_form_cover.xml",
    "views/snippets/s_form_aside.xml",
    "views/snippets/s_banner_connected.xml",
    "views/snippets/s_ecomm_categories_showcase.xml",
    "views/snippets/s_banner_categories.xml",
    "views/snippets/s_animated_cover.xml",
    "views/snippets/s_projects_list.xml",
    "views/snippets/s_about_bold.xml",
    "views/snippets/s_age_verification_popup.xml",
    "views/http_routing_template.xml",
    "views/new_page_template_templates.xml",
    "views/website_views.xml",
    "views/website_pages_views.xml",
    "views/website_controller_pages_views.xml",
    "views/website_visitor_views.xml",
    "views/res_config_settings_views.xml",
    "views/website_rewrite.xml",
    "views/ir_actions_server_views.xml",
    "views/ir_asset_views.xml",
    "views/ir_attachment_views.xml",
    "views/ir_model_views.xml",
    "views/res_partner_views.xml",
    "views/neutralize_views.xml",
    "views/digest_digest_views.xml",
    "wizard/base_language_install_views.xml",
    "wizard/blocked_third_party_domains.xml",
    "wizard/website_robots.xml",
    "wizard/website_llms.xml",
    "data/update_theme_images.xml",
    "views/website_templates_svg.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/website_demo.xml",
    "data/website_visitor_demo.xml"
  ],
  "assets": {
    "im_livechat.assets_embed_core": [
      "website/static/src/mail/core/common/**/*"
    ],
    "mail.assets_public": [
      "website/static/src/mail/core/common/**/*"
    ],
    "portal.assets_chatter_helpers": [
      "website/static/src/mail/core/common/**/*"
    ],
    "web.assets_frontend": [
      "html_builder/static/src/utils/scrolling.js",
      "website/static/src/interactions/**/*",
      "website/static/src/core/**/*",
      "website/static/src/services/google_maps_service.js",
      "website/static/src/utils/**/*",
      [
        "remove",
        "website/static/src/interactions/**/*.edit.js"
      ],
      [
        "remove",
        "website/static/src/interactions/multirange_input.js"
      ],
      [
        "remove",
        "website/static/src/interactions/ripple_effect.js"
      ],
      [
        "remove",
        "website/static/src/core/website_edit_service.js"
      ],
      [
        "replace",
        "web/static/src/public/public_root_instance.js",
        "website/static/src/js/content/website_root_instance.js"
      ],
      "website/static/src/snippets/**/*.js",
      [
        "remove",
        "website/static/src/snippets/**/*.edit.js"
      ],
      "website/static/src/scss/website.scss",
      "website/static/src/scss/portal.scss",
      "website/static/src/scss/website_common.scss",
      "website/static/src/scss/website_controller_page.scss",
      "website/static/src/scss/website.ui.scss",
      "website/static/src/libs/bootstrap/bootstrap.js",
      "website/static/src/js/utils.js",
      "web/static/src/core/autocomplete/*",
      "website/static/src/components/autocomplete_with_pages/*",
      "website/static/src/js/tours/tour_utils.js",
      "website/static/src/js/content/compatibility.js",
      "website/static/src/js/user_custom_javascript.js",
      "website/static/src/js/http_cookie.js",
      "website/static/src/js/text_processing.js",
      "website/static/src/js/highlight_utils.js",
      "website/static/src/client_actions/website_preview/website
```

### Representative source files

- `addons/website/README.md` (112 lines)
- `addons/website/__init__.py` (43 lines)
- `addons/website/__manifest__.py` (581 lines)
- `addons/website/controllers/__init__.py` (8 lines)
- `addons/website/controllers/backend.py` (63 lines)
- `addons/website/controllers/binary.py` (13 lines)
- `addons/website/controllers/form.py` (328 lines)
- `addons/website/controllers/main.py` (2,290 lines)
- `addons/website/controllers/model_page.py` (111 lines)
- `addons/website/controllers/webclient.py` (14 lines)
- `addons/website/data/digest_data.xml` (72 lines)
- `addons/website/data/image_library.xml` (1,589 lines)
- `addons/website/data/ir_asset.xml` (22 lines)
- `addons/website/data/ir_cron_data.xml` (25 lines)
- `addons/website/data/mail_mail_data.xml` (19 lines)
- `addons/website/data/neutralize.sql` (16 lines)
- `addons/website/data/update_theme_images.xml` (5 lines)
- `addons/website/data/website_data.xml` (601 lines)
- `addons/website/data/website_demo.xml` (655 lines)
- `addons/website/data/website_visitor_cron.xml` (12 lines)
- `addons/website/data/website_visitor_demo.xml` (23 lines)
- `addons/website/doc/website.snippet.rst` (153 lines)
- `addons/website/i18n/ar.po` (24,279 lines)
- `addons/website/i18n/az.po` (22,952 lines)
- `addons/website/i18n/bg.po` (22,922 lines)
- `addons/website/i18n/bs.po` (22,867 lines)
- `addons/website/i18n/ca.po` (23,430 lines)
- `addons/website/i18n/cs.po` (23,561 lines)
- `addons/website/i18n/da.po` (23,743 lines)
- `addons/website/i18n/de.po` (25,000 lines)
- `addons/website/i18n/el.po` (22,903 lines)
- `addons/website/i18n/es.po` (24,147 lines)
- `addons/website/i18n/es_419.po` (24,513 lines)
- `addons/website/i18n/et.po` (23,206 lines)
- `addons/website/i18n/fa.po` (23,234 lines)
- `addons/website/i18n/fi.po` (24,162 lines)
- `addons/website/i18n/fr.po` (24,212 lines)
- `addons/website/i18n/gu.po` (22,586 lines)
- `addons/website/i18n/he.po` (23,097 lines)
- `addons/website/i18n/hi.po` (22,913 lines)
- `addons/website/i18n/hr.po` (22,986 lines)
- `addons/website/i18n/hu.po` (23,035 lines)
- `addons/website/i18n/id.po` (24,931 lines)
- `addons/website/i18n/is.po` (22,600 lines)
- `addons/website/i18n/it.po` (25,036 lines)
- `addons/website/i18n/ja.po` (23,934 lines)
- `addons/website/i18n/ka.po` (22,581 lines)
- `addons/website/i18n/kab.po` (22,853 lines)
- `addons/website/i18n/km.po` (22,585 lines)
- `addons/website/i18n/ko.po` (23,657 lines)
- `addons/website/i18n/ku.po` (22,856 lines)
- `addons/website/i18n/lb.po` (22,584 lines)
- `addons/website/i18n/lo.po` (24,392 lines)
- `addons/website/i18n/lt.po` (22,971 lines)
- `addons/website/i18n/lv.po` (22,884 lines)
- `addons/website/i18n/mk.po` (22,590 lines)
- `addons/website/i18n/mn.po` (22,960 lines)
- `addons/website/i18n/my.po` (22,876 lines)
- `addons/website/i18n/nb.po` (22,983 lines)
- `addons/website/i18n/nl.po` (24,998 lines)
- `addons/website/i18n/pl.po` (24,203 lines)
- `addons/website/i18n/pt.po` (23,782 lines)
- `addons/website/i18n/pt_BR.po` (24,954 lines)
- `addons/website/i18n/ro.po` (23,952 lines)
- `addons/website/i18n/ru.po` (23,921 lines)
- `addons/website/i18n/sk.po` (23,020 lines)
- `addons/website/i18n/sl.po` (23,183 lines)
- `addons/website/i18n/sr@latin.po` (22,859 lines)
- `addons/website/i18n/sv.po` (23,619 lines)
- `addons/website/i18n/th.po` (23,431 lines)
- `addons/website/i18n/tr.po` (23,954 lines)
- `addons/website/i18n/uk.po` (23,238 lines)
- `addons/website/i18n/uz.po` (27,352 lines)
- `addons/website/i18n/vi.po` (23,932 lines)
- `addons/website/i18n/website.pot` (22,665 lines)
- `addons/website/i18n/zh_CN.po` (24,202 lines)
- `addons/website/i18n/zh_TW.po` (23,541 lines)
- `addons/website/models/__init__.py` (40 lines)
- `addons/website/models/assets.py` (369 lines)
- `addons/website/models/base_partner_merge.py` (31 lines)
- `addons/website/models/digest.py` (86 lines)
- `addons/website/models/html_text_processor.py` (358 lines)
- `addons/website/models/ir_access.py` (15 lines)
- `addons/website/models/ir_actions_server.py` (60 lines)
- `addons/website/models/ir_asset.py` (106 lines)
- `addons/website/models/ir_attachment.py` (31 lines)
- `addons/website/models/ir_binary.py` (25 lines)
- `addons/website/models/ir_http.py` (507 lines)
- `addons/website/models/ir_model.py` (47 lines)
- `addons/website/models/ir_model_data.py` (29 lines)
- `addons/website/models/ir_module_module.py` (799 lines)
- `addons/website/models/ir_qweb.py` (119 lines)
- `addons/website/models/ir_qweb_fields.py` (42 lines)
- `addons/website/models/ir_ui_menu.py` (25 lines)
- `addons/website/models/ir_ui_view.py` (776 lines)
- `addons/website/models/mixins.py` (1,099 lines)
- `addons/website/models/models.py` (17 lines)
- `addons/website/models/res_company.py` (40 lines)
- `addons/website/models/res_config_settings.py` (269 lines)
- `addons/website/models/res_groups.py` (13 lines)
- `addons/website/models/res_lang.py` (68 lines)
- `addons/website/models/res_partner.py` (42 lines)
- `addons/website/models/res_users.py` (110 lines)
- `addons/website/models/theme_models.py` (457 lines)
- `addons/website/models/website.py` (2,715 lines)
- `addons/website/models/website_configurator_feature.py` (29 lines)
- `addons/website/models/website_controller_page.py` (134 lines)
- `addons/website/models/website_form.py` (251 lines)
- `addons/website/models/website_menu.py` (390 lines)
- `addons/website/models/website_page.py` (452 lines)
- `addons/website/models/website_page_properties.py` (294 lines)
- `addons/website/models/website_rewrite.py` (197 lines)
- `addons/website/models/website_snippet_filter.py` (301 lines)
- `addons/website/models/website_technical_page.py` (75 lines)
- `addons/website/models/website_visitor.py` (382 lines)
- `addons/website/security/ir.access.csv` (34 lines)
- `addons/website/security/website_security.xml` (38 lines)
- `addons/website/static/description/icon.png` (32 lines)
- `addons/website/static/description/icon.svg` (1 lines)
- `addons/website/static/description/icon_hi.png` (112 lines)
- `addons/website/static/lib/multirange/LICENSE` (21 lines)
- `addons/website/static/lib/multirange/multirange_custom.js` (303 lines)
- `addons/website/static/lib/multirange/multirange_custom.scss` (75 lines)
- `addons/website/static/shapes/footer_mega_cards_image.svg` (73 lines)
- `addons/website/static/shapes/s_attributes_1.svg` (7 lines)
- `addons/website/static/shapes/s_attributes_2.svg` (13 lines)
- `addons/website/static/shapes/s_attributes_3.svg` (11 lines)
- `addons/website/static/shapes/s_attributes_4.svg` (8 lines)
- `addons/website/static/shapes/s_hero_maintenance.svg` (1 lines)
- `addons/website/static/src/@types/plugins.d.ts` (111 lines)
- `addons/website/static/src/@types/registries.d.ts` (30 lines)
- `addons/website/static/src/@types/services.d.ts` (19 lines)
- `addons/website/static/src/builder/builder_urlpicker.js` (67 lines)
- `addons/website/static/src/builder/builder_urlpicker.xml` (37 lines)
- `addons/website/static/src/builder/icon_selector.js` (12 lines)
- `addons/website/static/src/builder/plugins/achievements_list_option.xml` (16 lines)
- `addons/website/static/src/builder/plugins/achievements_list_option_plugin.js` (14 lines)
- `addons/website/static/src/builder/plugins/bootstrap_option_plugin.js` (77 lines)
- `addons/website/static/src/builder/plugins/carousel_bottom_controllers_option.xml` (34 lines)
- `addons/website/static/src/builder/plugins/carousel_cards.edit.xml` (10 lines)
- `addons/website/static/src/builder/plugins/carousel_cards_option.xml` (47 lines)
- `addons/website/static/src/builder/plugins/carousel_item_header_buttons.js` (49 lines)
- `addons/website/static/src/builder/plugins/carousel_option.js` (32 lines)
- `addons/website/static/src/builder/plugins/carousel_option.xml` (135 lines)
- `addons/website/static/src/builder/plugins/carousel_option_plugin.js` (556 lines)
- `addons/website/static/src/builder/plugins/collapse_plugin.js` (75 lines)
- `addons/website/static/src/builder/plugins/company_team_plugin.js` (20 lines)
- `addons/website/static/src/builder/plugins/content_width_option.edit.scss` (4 lines)
- `addons/website/static/src/builder/plugins/content_width_option.xml` (14 lines)
- `addons/website/static/src/builder/plugins/content_width_option_plugin.js` (23 lines)
- `addons/website/static/src/builder/plugins/customize_website_plugin.js` (1,134 lines)
- `addons/website/static/src/builder/plugins/dynamic_svg_option.js` (35 lines)
- `addons/website/static/src/builder/plugins/dynamic_svg_option.xml` (12 lines)
- `addons/website/static/src/builder/plugins/dynamic_svg_option_plugin.js` (69 lines)
- `addons/website/static/src/builder/plugins/edit_interaction_plugin.js` (86 lines)
- `addons/website/static/src/builder/plugins/editable_button_plugin.js` (46 lines)
- `addons/website/static/src/builder/plugins/floating_blocks/floating_blocks.edit.xml` (21 lines)
- `addons/website/static/src/builder/plugins/floating_blocks/floating_blocks_block_mobile_option.js` (18 lines)
- `addons/website/static/src/builder/plugins/floating_blocks/floating_blocks_block_option.js` (8 lines)
- `addons/website/static/src/builder/plugins/floating_blocks/floating_blocks_block_option_plugin.js` (27 lines)

Additional files not expanded here: 1652. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
