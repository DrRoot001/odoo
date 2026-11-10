# Module: website_mass_mailing

- **Module ID:** MOD-626
- **Path:** `addons/website_mass_mailing`
- **Manifest:** `addons/website_mass_mailing/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['website', 'mass_mailing']`
- **License:** `LGPL-3`

## Purpose and dependencies

Attract visitors to subscribe to mailing lists


This module brings a new building block with a mailing list widget to drop on any page of your website.
On a simple click, your visitors can subscribe to mailing lists managed in the Email Marketing app.
    

Declared dependencies: `website`, `mass_mailing`, `google_recaptcha`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 18 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "mass_mailing",
    "google_recaptcha"
  ],
  "data": [
    "data/ir_model_data.xml",
    "views/snippets_templates.xml",
    "views/snippets/s_newsletter_benefits_popup.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_mass_mailing/static/src/scss/website_mass_mailing.scss",
      "website_mass_mailing/static/src/interactions/**/*",
      "website_mass_mailing/static/src/scss/website_mass_mailing_popup.scss",
      "website_mass_mailing/static/src/interactions/fix_newsletter_list_class.edit.js",
      "website_mass_mailing/static/src/xml/*.xml"
    ],
    "website.website_builder_assets": [
      "website_mass_mailing/static/src/plugins/form_option_plugin.js",
      "website_mass_mailing/static/src/website_builder/**/*",
      [
        "remove",
        "website_mass_mailing/static/src/website_builder/**/*.edit.*"
      ]
    ],
    "website.assets_inside_builder_iframe": [
      "website_mass_mailing/static/src/website_builder/mailing_list_subscribe_option.edit.*",
      "website_mass_mailing/static/src/js/**/*.edit.*"
    ],
    "web.assets_tests": [
      "website_mass_mailing/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "website_mass_mailing/static/tests/builder/**/*",
      "website_mass_mailing/static/tests/interactions/**/*"
    ],
    "web.assets_unit_tests_setup": [
      "website_mass_mailing/static/src/interactions/**/*"
    ],
    "html_builder.iframe_add_dialog": [
      "website_mass_mailing/static/src/snippets/**/*.preview.scss"
    ],
    "mass_mailing.assets_builder": [
      "website_mass_mailing/static/snippets/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_mass_mailing/__init__.py` (4 lines)
- `addons/website_mass_mailing/__manifest__.py` (55 lines)
- `addons/website_mass_mailing/controllers/__init__.py` (5 lines)
- `addons/website_mass_mailing/controllers/main.py` (122 lines)
- `addons/website_mass_mailing/controllers/website_form.py` (50 lines)
- `addons/website_mass_mailing/data/ir_model_data.xml` (24 lines)
- `addons/website_mass_mailing/i18n/ar.po` (523 lines)
- `addons/website_mass_mailing/i18n/az.po` (504 lines)
- `addons/website_mass_mailing/i18n/bg.po` (524 lines)
- `addons/website_mass_mailing/i18n/bs.po` (512 lines)
- `addons/website_mass_mailing/i18n/ca.po` (524 lines)
- `addons/website_mass_mailing/i18n/cs.po` (523 lines)
- `addons/website_mass_mailing/i18n/da.po` (524 lines)
- `addons/website_mass_mailing/i18n/de.po` (579 lines)
- `addons/website_mass_mailing/i18n/el.po` (506 lines)
- `addons/website_mass_mailing/i18n/es.po` (531 lines)
- `addons/website_mass_mailing/i18n/es_419.po` (544 lines)
- `addons/website_mass_mailing/i18n/et.po` (519 lines)
- `addons/website_mass_mailing/i18n/fa.po` (507 lines)
- `addons/website_mass_mailing/i18n/fi.po` (529 lines)
- `addons/website_mass_mailing/i18n/fr.po` (555 lines)
- `addons/website_mass_mailing/i18n/gu.po` (495 lines)
- `addons/website_mass_mailing/i18n/he.po` (513 lines)
- `addons/website_mass_mailing/i18n/hi.po` (503 lines)
- `addons/website_mass_mailing/i18n/hr.po` (508 lines)
- `addons/website_mass_mailing/i18n/hu.po` (508 lines)
- `addons/website_mass_mailing/i18n/id.po` (539 lines)
- `addons/website_mass_mailing/i18n/is.po` (491 lines)
- `addons/website_mass_mailing/i18n/it.po` (551 lines)
- `addons/website_mass_mailing/i18n/ja.po` (544 lines)
- `addons/website_mass_mailing/i18n/kab.po` (506 lines)
- `addons/website_mass_mailing/i18n/km.po` (494 lines)
- `addons/website_mass_mailing/i18n/ko.po` (526 lines)
- `addons/website_mass_mailing/i18n/ku.po` (501 lines)
- `addons/website_mass_mailing/i18n/lo.po` (563 lines)
- `addons/website_mass_mailing/i18n/lt.po` (512 lines)
- `addons/website_mass_mailing/i18n/lv.po` (512 lines)
- `addons/website_mass_mailing/i18n/mk.po` (499 lines)
- `addons/website_mass_mailing/i18n/mn.po` (506 lines)
- `addons/website_mass_mailing/i18n/my.po` (501 lines)
- `addons/website_mass_mailing/i18n/nb.po` (505 lines)
- `addons/website_mass_mailing/i18n/nl.po` (577 lines)
- `addons/website_mass_mailing/i18n/pl.po` (555 lines)
- `addons/website_mass_mailing/i18n/pt.po` (525 lines)
- `addons/website_mass_mailing/i18n/pt_BR.po` (598 lines)
- `addons/website_mass_mailing/i18n/ro.po` (523 lines)
- `addons/website_mass_mailing/i18n/ru.po` (522 lines)
- `addons/website_mass_mailing/i18n/sk.po` (519 lines)
- `addons/website_mass_mailing/i18n/sl.po` (509 lines)
- `addons/website_mass_mailing/i18n/sr@latin.po` (571 lines)
- `addons/website_mass_mailing/i18n/sv.po` (522 lines)
- `addons/website_mass_mailing/i18n/th.po` (518 lines)
- `addons/website_mass_mailing/i18n/tr.po` (528 lines)
- `addons/website_mass_mailing/i18n/uk.po` (517 lines)
- `addons/website_mass_mailing/i18n/uz.po` (570 lines)
- `addons/website_mass_mailing/i18n/vi.po` (526 lines)
- `addons/website_mass_mailing/i18n/website_mass_mailing.pot` (484 lines)
- `addons/website_mass_mailing/i18n/zh_CN.po` (557 lines)
- `addons/website_mass_mailing/i18n/zh_TW.po` (531 lines)
- `addons/website_mass_mailing/security/ir.access.csv` (2 lines)
- `addons/website_mass_mailing/static/description/icon.png` (17 lines)
- `addons/website_mass_mailing/static/description/icon.svg` (1 lines)
- `addons/website_mass_mailing/static/description/icon_hi.png` (47 lines)
- `addons/website_mass_mailing/static/shapes/s_newsletter_benefits_popup.svg` (243 lines)
- `addons/website_mass_mailing/static/snippets/snippets_templates.xml` (15 lines)
- `addons/website_mass_mailing/static/src/img/snippets_thumbs/s_newsletter_block.svg` (71 lines)
- `addons/website_mass_mailing/static/src/interactions/fix_newsletter_list_class.edit.js` (28 lines)
- `addons/website_mass_mailing/static/src/interactions/popup.js` (30 lines)
- `addons/website_mass_mailing/static/src/interactions/subscribe.js` (145 lines)
- `addons/website_mass_mailing/static/src/interactions/subscribe_list_missing_error.xml` (9 lines)
- `addons/website_mass_mailing/static/src/js/mass_mailing_form_editor.edit.js` (26 lines)
- `addons/website_mass_mailing/static/src/plugins/form_option_plugin.js` (15 lines)
- `addons/website_mass_mailing/static/src/scss/website_mass_mailing.scss` (7 lines)
- `addons/website_mass_mailing/static/src/scss/website_mass_mailing_edit_mode.scss` (10 lines)
- `addons/website_mass_mailing/static/src/scss/website_mass_mailing_popup.scss` (22 lines)
- `addons/website_mass_mailing/static/src/snippets/s_newsletter_benefits_popup/s_newsletter_benefits_popup.preview.scss` (8 lines)
- `addons/website_mass_mailing/static/src/website_builder/mailing_list_subscribe_option.edit.scss` (9 lines)
- `addons/website_mass_mailing/static/src/website_builder/mailing_list_subscribe_option.js` (16 lines)
- `addons/website_mass_mailing/static/src/website_builder/mailing_list_subscribe_option.xml` (38 lines)
- `addons/website_mass_mailing/static/src/website_builder/mailing_list_subscribe_option_plugin.js` (129 lines)
- `addons/website_mass_mailing/static/src/website_builder/mailing_list_subscribe_translation_option_plugin.js` (29 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_layout_option.xml` (28 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_layout_option_plugin.js` (41 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_options.xml` (19 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_subscribe_common_option.js` (18 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_subscribe_common_option.xml` (23 lines)
- `addons/website_mass_mailing/static/src/website_builder/newsletter_subscribe_common_option_plugin.js` (48 lines)
- `addons/website_mass_mailing/static/src/website_builder/recaptcha_subscribe_option.js` (11 lines)
- `addons/website_mass_mailing/static/src/website_builder/recaptcha_subscribe_option.xml` (11 lines)
- `addons/website_mass_mailing/static/src/website_builder/recaptcha_subscribe_option_plugin.js` (37 lines)
- `addons/website_mass_mailing/static/src/website_builder/toggle_thanks_message_translation_option.xml` (25 lines)
- `addons/website_mass_mailing/static/src/xml/website_mass_mailing.xml` (15 lines)
- `addons/website_mass_mailing/static/tests/builder/mailing_list_subscribe_translation_option_plugin.test.js` (29 lines)
- `addons/website_mass_mailing/static/tests/interactions/popup.test.js` (56 lines)
- `addons/website_mass_mailing/static/tests/tours/snippet_newsletter_block_with_edit.js` (60 lines)
- `addons/website_mass_mailing/static/tests/tours/snippet_newsletter_popup_edition.js` (28 lines)
- `addons/website_mass_mailing/static/tests/tours/snippet_newsletter_popup_use.js` (25 lines)
- `addons/website_mass_mailing/tests/__init__.py` (7 lines)
- `addons/website_mass_mailing/tests/common.py` (22 lines)
- `addons/website_mass_mailing/tests/test_controllers.py` (89 lines)
- `addons/website_mass_mailing/tests/test_mailing_controllers.py` (36 lines)
- `addons/website_mass_mailing/tests/test_property_field_mailing_contact.py` (33 lines)
- `addons/website_mass_mailing/tests/test_snippets.py` (33 lines)
- `addons/website_mass_mailing/tests/test_website_mass_mailing.py` (99 lines)
- `addons/website_mass_mailing/views/snippets/s_newsletter_benefits_popup.xml` (40 lines)
- `addons/website_mass_mailing/views/snippets_templates.xml` (394 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
