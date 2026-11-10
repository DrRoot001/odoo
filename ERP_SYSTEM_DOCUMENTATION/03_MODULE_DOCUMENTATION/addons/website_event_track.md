# Module: website_event_track

- **Module ID:** MOD-614
- **Path:** `addons/website_event_track`
- **Manifest:** `addons/website_event_track/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Sponsors, Tracks, Agenda, Event News

No manifest description declared.

Declared dependencies: `website_event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 29 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 5 | Files under `controllers/` or `controllers.py`. |
| XML files | 33 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 11 | Client behavior/assets. |
| Tests | 8 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 14 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event"
  ],
  "data": [
    "data/event_data.xml",
    "data/mail_template_data.xml",
    "data/mail_templates.xml",
    "data/mail_message_subtype_data.xml",
    "data/event_track_data.xml",
    "views/event_templates.xml",
    "views/event_track_templates_agenda.xml",
    "views/event_track_templates_list.xml",
    "views/event_track_templates_location_display.xml",
    "views/event_track_templates_reminder.xml",
    "views/event_track_templates_page.xml",
    "views/event_track_templates_proposal.xml",
    "views/event_track_views.xml",
    "views/event_track_location_views.xml",
    "views/event_track_tag_views.xml",
    "views/event_track_stage_views.xml",
    "views/event_track_visitor_views.xml",
    "views/event_event_views.xml",
    "views/event_type_views.xml",
    "views/res_config_settings_view.xml",
    "views/website_visitor_views.xml",
    "views/event_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_demo.xml",
    "data/event_track_location_demo.xml",
    "data/event_track_tag_demo.xml",
    "data/event_track_demo.xml",
    "data/event_track_demo_description.xml",
    "data/event_track_visitor_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_event_track/static/src/scss/event_track_location_display.scss",
      "website_event_track/static/src/scss/event_track_templates.scss",
      "website_event_track/static/src/scss/event_track_templates_online.scss",
      "website_event_track/static/src/scss/pwa_frontend.scss",
      "website_event_track/static/lib/idb-keyval/idb-keyval.js",
      "website_event_track/static/src/xml/event_track_proposal_templates.xml",
      "website_event_track/static/src/xml/website_event_pwa.xml",
      "website_event_track/static/src/xml/website_event_track_form_tags_wrapper.xml",
      "website_event_track/static/src/xml/website_event_track_email_reminder.xml",
      "website_event_track/static/src/interactions/*"
    ],
    "web.assets_tests": [
      "website_event_track/static/tests/tours/*.js"
    ],
    "website.website_builder_assets": [
      "website_event_track/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_event_track/README.md` (38 lines)
- `addons/website_event_track/__init__.py` (5 lines)
- `addons/website_event_track/__manifest__.py` (64 lines)
- `addons/website_event_track/controllers/__init__.py` (4 lines)
- `addons/website_event_track/controllers/event.py` (12 lines)
- `addons/website_event_track/controllers/event_track.py` (587 lines)
- `addons/website_event_track/controllers/location_display.py` (123 lines)
- `addons/website_event_track/controllers/webmanifest.py` (63 lines)
- `addons/website_event_track/data/event_data.xml` (10 lines)
- `addons/website_event_track/data/event_demo.xml` (13 lines)
- `addons/website_event_track/data/event_track_data.xml` (41 lines)
- `addons/website_event_track/data/event_track_demo.xml` (766 lines)
- `addons/website_event_track/data/event_track_demo_description.xml` (74 lines)
- `addons/website_event_track/data/event_track_location_demo.xml` (33 lines)
- `addons/website_event_track/data/event_track_tag_demo.xml` (49 lines)
- `addons/website_event_track/data/event_track_visitor_demo.xml` (15 lines)
- `addons/website_event_track/data/mail_message_subtype_data.xml` (25 lines)
- `addons/website_event_track/data/mail_template_data.xml` (274 lines)
- `addons/website_event_track/data/mail_templates.xml` (32 lines)
- `addons/website_event_track/i18n/af.po` (3,250 lines)
- `addons/website_event_track/i18n/ar.po` (4,232 lines)
- `addons/website_event_track/i18n/az.po` (3,271 lines)
- `addons/website_event_track/i18n/bg.po` (3,278 lines)
- `addons/website_event_track/i18n/bs.po` (3,258 lines)
- `addons/website_event_track/i18n/ca.po` (4,191 lines)
- `addons/website_event_track/i18n/cs.po` (4,154 lines)
- `addons/website_event_track/i18n/da.po` (3,362 lines)
- `addons/website_event_track/i18n/de.po` (5,173 lines)
- `addons/website_event_track/i18n/el.po` (3,267 lines)
- `addons/website_event_track/i18n/es.po` (5,135 lines)
- `addons/website_event_track/i18n/es_419.po` (5,150 lines)
- `addons/website_event_track/i18n/es_CL.po` (154 lines)
- `addons/website_event_track/i18n/et.po` (3,327 lines)
- `addons/website_event_track/i18n/eu.po` (3,249 lines)
- `addons/website_event_track/i18n/fa.po` (3,282 lines)
- `addons/website_event_track/i18n/fi.po` (5,137 lines)
- `addons/website_event_track/i18n/fr.po` (4,298 lines)
- `addons/website_event_track/i18n/fr_BE.po` (135 lines)
- `addons/website_event_track/i18n/fr_CA.po` (157 lines)
- `addons/website_event_track/i18n/gl.po` (3,248 lines)
- `addons/website_event_track/i18n/gu.po` (3,260 lines)
- `addons/website_event_track/i18n/he.po` (3,294 lines)
- `addons/website_event_track/i18n/hi.po` (3,248 lines)
- `addons/website_event_track/i18n/hr.po` (3,279 lines)
- `addons/website_event_track/i18n/hu.po` (3,280 lines)
- `addons/website_event_track/i18n/id.po` (5,041 lines)
- `addons/website_event_track/i18n/is.po` (3,254 lines)
- `addons/website_event_track/i18n/it.po` (5,141 lines)
- `addons/website_event_track/i18n/ja.po` (4,257 lines)
- `addons/website_event_track/i18n/ka.po` (3,248 lines)
- `addons/website_event_track/i18n/kab.po` (3,249 lines)
- `addons/website_event_track/i18n/km.po` (3,257 lines)
- `addons/website_event_track/i18n/ko.po` (4,204 lines)
- `addons/website_event_track/i18n/ku.po` (3,248 lines)
- `addons/website_event_track/i18n/lo.po` (4,224 lines)
- `addons/website_event_track/i18n/lt.po` (3,289 lines)
- `addons/website_event_track/i18n/lv.po` (3,273 lines)
- `addons/website_event_track/i18n/mk.po` (3,250 lines)
- `addons/website_event_track/i18n/mn.po` (3,282 lines)
- `addons/website_event_track/i18n/my.po` (3,249 lines)
- `addons/website_event_track/i18n/nb.po` (3,270 lines)
- `addons/website_event_track/i18n/nl.po` (5,142 lines)
- `addons/website_event_track/i18n/pl.po` (4,202 lines)
- `addons/website_event_track/i18n/pt.po` (4,228 lines)
- `addons/website_event_track/i18n/pt_BR.po` (5,125 lines)
- `addons/website_event_track/i18n/ro.po` (4,081 lines)
- `addons/website_event_track/i18n/ru.po` (5,142 lines)
- `addons/website_event_track/i18n/sk.po` (3,280 lines)
- `addons/website_event_track/i18n/sl.po` (3,279 lines)
- `addons/website_event_track/i18n/sq.po` (3,248 lines)
- `addons/website_event_track/i18n/sr@latin.po` (3,270 lines)
- `addons/website_event_track/i18n/sv.po` (4,228 lines)
- `addons/website_event_track/i18n/th.po` (4,964 lines)
- `addons/website_event_track/i18n/tr.po` (4,239 lines)
- `addons/website_event_track/i18n/uk.po` (3,364 lines)
- `addons/website_event_track/i18n/uz.po` (3,855 lines)
- `addons/website_event_track/i18n/vi.po` (4,217 lines)
- `addons/website_event_track/i18n/website_event_track.pot` (3,050 lines)
- `addons/website_event_track/i18n/zh_CN.po` (5,026 lines)
- `addons/website_event_track/i18n/zh_TW.po` (4,121 lines)
- `addons/website_event_track/models/__init__.py` (16 lines)
- `addons/website_event_track/models/event_event.py` (138 lines)
- `addons/website_event_track/models/event_track.py` (763 lines)
- `addons/website_event_track/models/event_track_location.py` (27 lines)
- `addons/website_event_track/models/event_track_stage.py` (48 lines)
- `addons/website_event_track/models/event_track_tag.py` (28 lines)
- `addons/website_event_track/models/event_track_tag_category.py` (14 lines)
- `addons/website_event_track/models/event_track_visitor.py` (32 lines)
- `addons/website_event_track/models/event_type.py` (22 lines)
- `addons/website_event_track/models/res_config_settings.py` (10 lines)
- `addons/website_event_track/models/website.py` (62 lines)
- `addons/website_event_track/models/website_event_menu.py` (12 lines)
- `addons/website_event_track/models/website_menu.py` (30 lines)
- `addons/website_event_track/models/website_visitor.py` (60 lines)
- `addons/website_event_track/security/ir.access.csv` (15 lines)
- `addons/website_event_track/static/description/blog.png` (416 lines)
- `addons/website_event_track/static/description/event.png` (322 lines)
- `addons/website_event_track/static/description/icon.png` (31 lines)
- `addons/website_event_track/static/description/icon.svg` (1 lines)
- `addons/website_event_track/static/description/icon_hi.png` (122 lines)
- `addons/website_event_track/static/description/index.html` (97 lines)
- `addons/website_event_track/static/description/sponsor.png` (684 lines)
- `addons/website_event_track/static/description/tracks.png` (381 lines)
- `addons/website_event_track/static/lib/idb-keyval/idb-keyval.js` (81 lines)
- `addons/website_event_track/static/src/img/event_track_default_0.jpeg` (60 lines)
- `addons/website_event_track/static/src/img/event_track_default_1.jpeg` (106 lines)
- `addons/website_event_track/static/src/interactions/event_track_location_display.js` (91 lines)
- `addons/website_event_track/static/src/interactions/event_track_reminder.js` (132 lines)
- `addons/website_event_track/static/src/interactions/event_track_timer.js` (78 lines)
- `addons/website_event_track/static/src/interactions/track_wishlist_counter.js` (38 lines)
- `addons/website_event_track/static/src/interactions/website_event_pwa.js` (121 lines)
- `addons/website_event_track/static/src/interactions/website_event_track.js` (151 lines)
- `addons/website_event_track/static/src/interactions/website_event_track_proposal_form.js` (169 lines)
- `addons/website_event_track/static/src/interactions/website_event_track_proposal_form_tags.js` (50 lines)
- `addons/website_event_track/static/src/js/service_worker.js` (380 lines)
- `addons/website_event_track/static/src/scss/event_track_location_display.scss` (47 lines)
- `addons/website_event_track/static/src/scss/event_track_templates.scss` (199 lines)
- `addons/website_event_track/static/src/scss/event_track_templates_online.scss` (81 lines)
- `addons/website_event_track/static/src/scss/pwa_frontend.scss` (35 lines)
- `addons/website_event_track/static/src/website_builder/event_track_page_option.xml` (38 lines)
- `addons/website_event_track/static/src/xml/event_track_proposal_templates.xml` (11 lines)
- `addons/website_event_track/static/src/xml/website_event_pwa.xml` (11 lines)
- `addons/website_event_track/static/src/xml/website_event_track_email_reminder.xml` (45 lines)
- `addons/website_event_track/static/src/xml/website_event_track_form_tags_wrapper.xml` (15 lines)
- `addons/website_event_track/static/tests/tours/email_reminder_tour.js` (31 lines)
- `addons/website_event_track/tests/__init__.py` (10 lines)
- `addons/website_event_track/tests/test_event_menus.py` (81 lines)
- `addons/website_event_track/tests/test_location_display.py` (198 lines)
- `addons/website_event_track/tests/test_mail_features.py` (179 lines)
- `addons/website_event_track/tests/test_track_internals.py` (293 lines)
- `addons/website_event_track/tests/test_website_event.py` (78 lines)
- `addons/website_event_track/tests/test_website_event_track.py` (72 lines)
- `addons/website_event_track/tests/test_website_visitor.py` (71 lines)
- `addons/website_event_track/views/event_event_views.xml` (50 lines)
- `addons/website_event_track/views/event_menus.xml` (48 lines)
- `addons/website_event_track/views/event_templates.xml` (110 lines)
- `addons/website_event_track/views/event_track_location_views.xml` (44 lines)
- `addons/website_event_track/views/event_track_stage_views.xml` (106 lines)
- `addons/website_event_track/views/event_track_tag_views.xml` (83 lines)
- `addons/website_event_track/views/event_track_templates_agenda.xml` (217 lines)
- `addons/website_event_track/views/event_track_templates_list.xml` (445 lines)
- `addons/website_event_track/views/event_track_templates_location_display.xml` (153 lines)
- `addons/website_event_track/views/event_track_templates_page.xml` (248 lines)
- `addons/website_event_track/views/event_track_templates_proposal.xml` (189 lines)
- `addons/website_event_track/views/event_track_templates_reminder.xml` (24 lines)
- `addons/website_event_track/views/event_track_views.xml` (299 lines)
- `addons/website_event_track/views/event_track_visitor_views.xml` (72 lines)
- `addons/website_event_track/views/event_type_views.xml` (22 lines)
- `addons/website_event_track/views/res_config_settings_view.xml` (27 lines)
- `addons/website_event_track/views/website_visitor_views.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
