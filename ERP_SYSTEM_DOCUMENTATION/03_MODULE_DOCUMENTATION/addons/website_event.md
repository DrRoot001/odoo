# Module: website_event

- **Module ID:** MOD-606
- **Path:** `addons/website_event`
- **Manifest:** `addons/website_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Publish events, sell tickets

No manifest description declared.

Declared dependencies: `event`, `website`, `website_partner`, `website_mail`, `html_builder`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 28 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 35 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 23 | Client behavior/assets. |
| Tests | 10 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 9 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "website",
    "website_partner",
    "website_mail",
    "html_builder"
  ],
  "data": [
    "data/event_data.xml",
    "data/website_snippet_data.xml",
    "views/snippets/s_events.xml",
    "views/snippets/s_events_carousel.xml",
    "views/snippets/s_event_upcoming_snippet_preview_data.xml",
    "views/snippets/s_event_carousel_preview_data.xml",
    "views/snippets/snippets.xml",
    "views/event_templates_list.xml",
    "views/event_templates_svg.xml",
    "views/event_templates_page.xml",
    "views/event_templates_page_registration.xml",
    "views/event_templates_page_misc.xml",
    "views/event_templates_widgets.xml",
    "views/event_event_views.xml",
    "views/event_registration_views.xml",
    "views/event_tag_category_views.xml",
    "views/event_tag_views.xml",
    "views/event_type_views.xml",
    "views/portal_templates.xml",
    "views/website_event_menu_views.xml",
    "views/website_visitor_views.xml",
    "views/event_menus.xml",
    "views/website_pages_views.xml",
    "views/event_event_add.xml",
    "security/event_security.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_partner_demo.xml",
    "data/event_demo.xml",
    "data/event_question_demo.xml",
    "data/event_registration_demo.xml",
    "data/event_registration_answer_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "website_event/static/src/js/tours/**/*"
    ],
    "web.assets_tests": [
      "website_event/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "website_event/static/tests/interactions/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_event/static/src/snippets/**/*.js"
    ],
    "web.assets_frontend": [
      "website_event/static/src/js/tours/**/*",
      "website_event/static/src/scss/event_templates_common.scss",
      "website_event/static/src/scss/event_templates_list.scss",
      "website_event/static/src/scss/event_templates_page.scss",
      "website_event/static/src/interactions/*.js",
      "website_event/static/src/snippets/**/*.js"
    ],
    "website.assets_editor": [
      "website_event/static/src/js/systray_items/*.js"
    ],
    "website.website_builder_assets": [
      "website_event/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_event/README.md` (115 lines)
- `addons/website_event/__init__.py` (5 lines)
- `addons/website_event/__manifest__.py` (83 lines)
- `addons/website_event/controllers/__init__.py` (4 lines)
- `addons/website_event/controllers/community.py` (13 lines)
- `addons/website_event/controllers/main.py` (594 lines)
- `addons/website_event/data/event_data.xml` (47 lines)
- `addons/website_event/data/event_demo.xml` (173 lines)
- `addons/website_event/data/event_question_demo.xml` (150 lines)
- `addons/website_event/data/event_registration_answer_demo.xml` (64 lines)
- `addons/website_event/data/event_registration_demo.xml` (18 lines)
- `addons/website_event/data/res_partner_demo.xml` (311 lines)
- `addons/website_event/data/website_snippet_data.xml` (37 lines)
- `addons/website_event/i18n/af.po` (2,178 lines)
- `addons/website_event/i18n/ar.po` (2,232 lines)
- `addons/website_event/i18n/az.po` (2,186 lines)
- `addons/website_event/i18n/bg.po` (2,189 lines)
- `addons/website_event/i18n/bs.po` (2,182 lines)
- `addons/website_event/i18n/ca.po` (2,256 lines)
- `addons/website_event/i18n/cs.po` (2,210 lines)
- `addons/website_event/i18n/da.po` (2,239 lines)
- `addons/website_event/i18n/de.po` (2,457 lines)
- `addons/website_event/i18n/el.po` (2,184 lines)
- `addons/website_event/i18n/es.po` (2,396 lines)
- `addons/website_event/i18n/es_419.po` (2,396 lines)
- `addons/website_event/i18n/et.po` (2,215 lines)
- `addons/website_event/i18n/fa.po` (2,208 lines)
- `addons/website_event/i18n/fi.po` (2,400 lines)
- `addons/website_event/i18n/fr.po` (2,262 lines)
- `addons/website_event/i18n/gl.po` (2,176 lines)
- `addons/website_event/i18n/gu.po` (2,178 lines)
- `addons/website_event/i18n/he.po` (2,205 lines)
- `addons/website_event/i18n/hi.po` (2,178 lines)
- `addons/website_event/i18n/hr.po` (2,189 lines)
- `addons/website_event/i18n/hu.po` (2,193 lines)
- `addons/website_event/i18n/id.po` (2,385 lines)
- `addons/website_event/i18n/is.po` (2,174 lines)
- `addons/website_event/i18n/it.po` (2,435 lines)
- `addons/website_event/i18n/ja.po` (2,240 lines)
- `addons/website_event/i18n/ka.po` (2,176 lines)
- `addons/website_event/i18n/kab.po` (2,178 lines)
- `addons/website_event/i18n/km.po` (2,178 lines)
- `addons/website_event/i18n/ko.po` (2,226 lines)
- `addons/website_event/i18n/ku.po` (2,178 lines)
- `addons/website_event/i18n/lo.po` (2,390 lines)
- `addons/website_event/i18n/lt.po` (2,215 lines)
- `addons/website_event/i18n/lv.po` (2,183 lines)
- `addons/website_event/i18n/mk.po` (2,182 lines)
- `addons/website_event/i18n/mn.po` (2,186 lines)
- `addons/website_event/i18n/my.po` (2,179 lines)
- `addons/website_event/i18n/nb.po` (2,187 lines)
- `addons/website_event/i18n/nl.po` (2,435 lines)
- `addons/website_event/i18n/pl.po` (2,414 lines)
- `addons/website_event/i18n/pt.po` (2,221 lines)
- `addons/website_event/i18n/pt_BR.po` (2,430 lines)
- `addons/website_event/i18n/ro.po` (2,246 lines)
- `addons/website_event/i18n/ru.po` (2,434 lines)
- `addons/website_event/i18n/sk.po` (2,192 lines)
- `addons/website_event/i18n/sl.po` (2,195 lines)
- `addons/website_event/i18n/sr@latin.po` (2,246 lines)
- `addons/website_event/i18n/sv.po` (2,237 lines)
- `addons/website_event/i18n/th.po` (2,354 lines)
- `addons/website_event/i18n/tr.po` (2,404 lines)
- `addons/website_event/i18n/uk.po` (2,211 lines)
- `addons/website_event/i18n/uz.po` (2,516 lines)
- `addons/website_event/i18n/vi.po` (2,234 lines)
- `addons/website_event/i18n/website_event.pot` (2,141 lines)
- `addons/website_event/i18n/zh_CN.po` (2,264 lines)
- `addons/website_event/i18n/zh_TW.po` (2,228 lines)
- `addons/website_event/models/__init__.py` (15 lines)
- `addons/website_event/models/event_event.py` (779 lines)
- `addons/website_event/models/event_registration.py` (17 lines)
- `addons/website_event/models/event_slot.py` (18 lines)
- `addons/website_event/models/event_tag.py` (15 lines)
- `addons/website_event/models/event_tag_category.py` (12 lines)
- `addons/website_event/models/event_type.py` (18 lines)
- `addons/website_event/models/website.py` (96 lines)
- `addons/website_event/models/website_event_menu.py` (79 lines)
- `addons/website_event/models/website_menu.py` (121 lines)
- `addons/website_event/models/website_snippet_filter.py` (58 lines)
- `addons/website_event/models/website_track.py` (11 lines)
- `addons/website_event/models/website_visitor.py` (105 lines)
- `addons/website_event/security/event_security.xml` (5 lines)
- `addons/website_event/security/ir.access.csv` (18 lines)
- `addons/website_event/static/description/icon.png` (33 lines)
- `addons/website_event/static/description/icon.svg` (1 lines)
- `addons/website_event/static/description/icon_hi.png` (121 lines)
- `addons/website_event/static/src/img/event_cover_0.jpg` (1,853 lines)
- `addons/website_event/static/src/img/event_cover_1.jpg` (404 lines)
- `addons/website_event/static/src/img/event_cover_2.jpg` (954 lines)
- `addons/website_event/static/src/img/event_cover_3.jpg` (1,580 lines)
- `addons/website_event/static/src/img/event_cover_4.jpg` (1,421 lines)
- `addons/website_event/static/src/img/event_cover_5.jpg` (1,216 lines)
- `addons/website_event/static/src/img/event_cover_7.jpg` (455 lines)
- `addons/website_event/static/src/img/event_past_0.jpg` (2,358 lines)
- `addons/website_event/static/src/img/event_previews/event_1.jpg` (114 lines)
- `addons/website_event/static/src/img/event_previews/event_2.jpg` (230 lines)
- `addons/website_event/static/src/img/event_previews/event_3.jpg` (123 lines)
- `addons/website_event/static/src/img/event_training_0.jpg` (2,126 lines)
- `addons/website_event/static/src/img/openerp_enterprise_of_the_year.png` (246 lines)
- `addons/website_event/static/src/img/speaker.png` (19 lines)
- `addons/website_event/static/src/img/training.jpg` (348 lines)
- `addons/website_event/static/src/interactions/display_timer.js` (102 lines)
- `addons/website_event/static/src/interactions/event_page.js` (15 lines)
- `addons/website_event/static/src/interactions/modal_registration.js` (125 lines)
- `addons/website_event/static/src/interactions/register_toaster.js` (21 lines)
- `addons/website_event/static/src/interactions/website_event_slot_details.js` (149 lines)
- `addons/website_event/static/src/interactions/website_event_ticket_details.js` (97 lines)
- `addons/website_event/static/src/js/systray_items/new_content.js` (16 lines)
- `addons/website_event/static/src/js/tours/event_tour.js` (76 lines)
- `addons/website_event/static/src/scss/event_templates_common.scss` (94 lines)
- `addons/website_event/static/src/scss/event_templates_list.scss` (127 lines)
- `addons/website_event/static/src/scss/event_templates_page.scss` (129 lines)
- `addons/website_event/static/src/snippets/s_events/000.scss` (67 lines)
- `addons/website_event/static/src/snippets/s_events/events.js` (32 lines)
- `addons/website_event/static/src/snippets/s_events/events_carousel.js` (20 lines)
- `addons/website_event/static/src/snippets/s_events/events_mixin.js` (20 lines)
- `addons/website_event/static/src/website_builder/dark_palette_content.js` (13 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_carousel_option.js` (11 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_carousel_option.xml` (19 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_option.js` (28 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_option.xml` (25 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_option_plugin.js` (51 lines)
- `addons/website_event/static/src/website_builder/dynamic_snippet_events_shared_option.xml` (24 lines)
- `addons/website_event/static/src/website_builder/event_page_option.xml` (63 lines)
- `addons/website_event/static/src/website_builder/event_page_option_plugin.js` (76 lines)
- `addons/website_event/static/src/website_builder/event_searchbar_option_plugin.js` (24 lines)
- `addons/website_event/static/src/website_builder/events_list_page_option.xml` (69 lines)
- `addons/website_event/static/tests/interactions/snippets/events.test.js` (84 lines)
- `addons/website_event/static/tests/tours/sub_templates_config.js` (11 lines)
- `addons/website_event/static/tests/tours/tickets_questions.js` (120 lines)
- `addons/website_event/static/tests/tours/website_event.js` (160 lines)
- `addons/website_event/static/tests/tours/website_event_pages_seo.js` (41 lines)
- `addons/website_event/static/tests/tours/website_event_search.js` (40 lines)
- `addons/website_event/tests/__init__.py` (11 lines)
- `addons/website_event/tests/common.py` (115 lines)
- `addons/website_event/tests/test_event_ics.py` (78 lines)
- `addons/website_event/tests/test_event_internals.py` (319 lines)
- `addons/website_event/tests/test_event_mail.py` (116 lines)
- `addons/website_event/tests/test_event_menus.py` (243 lines)
- `addons/website_event/tests/test_event_visitor.py` (75 lines)
- `addons/website_event/tests/test_fuzzy.py` (42 lines)
- `addons/website_event/tests/test_website_event.py` (341 lines)
- `addons/website_event/tests/test_website_event_technical_page.py` (9 lines)
- `addons/website_event/views/event_event_add.xml` (31 lines)
- `addons/website_event/views/event_event_views.xml` (93 lines)
- `addons/website_event/views/event_menus.xml` (11 lines)
- `addons/website_event/views/event_registration_views.xml` (61 lines)
- `addons/website_event/views/event_tag_category_views.xml` (27 lines)
- `addons/website_event/views/event_tag_views.xml` (16 lines)
- `addons/website_event/views/event_templates_list.xml` (546 lines)
- `addons/website_event/views/event_templates_page.xml` (105 lines)
- `addons/website_event/views/event_templates_page_misc.xml` (19 lines)
- `addons/website_event/views/event_templates_page_registration.xml` (737 lines)
- `addons/website_event/views/event_templates_svg.xml` (49 lines)
- `addons/website_event/views/event_templates_widgets.xml` (37 lines)
- `addons/website_event/views/event_type_views.xml` (24 lines)
- `addons/website_event/views/portal_templates.xml` (15 lines)
- `addons/website_event/views/snippets/s_event_carousel_preview_data.xml` (56 lines)
- `addons/website_event/views/snippets/s_event_upcoming_snippet_preview_data.xml` (280 lines)

Additional files not expanded here: 6. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
