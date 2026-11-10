# Module: website_slides_forum

- **Module ID:** MOD-644
- **Path:** `addons/website_slides_forum`
- **Manifest:** `addons/website_slides_forum/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Allows to link forum on a course

A Slide channel can be linked to forum. Also, profiles from slide and forum are regrouped together

Declared dependencies: `website_slides`, `website_forum`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 9 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_slides",
    "website_forum"
  ],
  "data": [
    "views/forum_forum_views.xml",
    "views/forum_post_views.xml",
    "views/res_config_settings_views.xml",
    "views/slide_channel_views.xml",
    "views/website_slides_menu_views.xml",
    "views/forum_forum_templates.xml",
    "views/website_slides_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/slide_channel_demo.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_slides_forum/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_slides_forum/__init__.py` (5 lines)
- `addons/website_slides_forum/__manifest__.py` (33 lines)
- `addons/website_slides_forum/controllers/__init__.py` (3 lines)
- `addons/website_slides_forum/controllers/main.py` (24 lines)
- `addons/website_slides_forum/data/slide_channel_demo.xml` (44 lines)
- `addons/website_slides_forum/i18n/ar.po` (561 lines)
- `addons/website_slides_forum/i18n/az.po` (494 lines)
- `addons/website_slides_forum/i18n/bg.po` (494 lines)
- `addons/website_slides_forum/i18n/bs.po` (496 lines)
- `addons/website_slides_forum/i18n/ca.po` (570 lines)
- `addons/website_slides_forum/i18n/cs.po` (566 lines)
- `addons/website_slides_forum/i18n/da.po` (570 lines)
- `addons/website_slides_forum/i18n/de.po` (592 lines)
- `addons/website_slides_forum/i18n/el.po` (495 lines)
- `addons/website_slides_forum/i18n/es.po` (589 lines)
- `addons/website_slides_forum/i18n/es_419.po` (582 lines)
- `addons/website_slides_forum/i18n/et.po` (494 lines)
- `addons/website_slides_forum/i18n/fa.po` (494 lines)
- `addons/website_slides_forum/i18n/fi.po` (580 lines)
- `addons/website_slides_forum/i18n/fr.po` (589 lines)
- `addons/website_slides_forum/i18n/he.po` (542 lines)
- `addons/website_slides_forum/i18n/hi.po` (494 lines)
- `addons/website_slides_forum/i18n/hr.po` (508 lines)
- `addons/website_slides_forum/i18n/hu.po` (528 lines)
- `addons/website_slides_forum/i18n/id.po` (585 lines)
- `addons/website_slides_forum/i18n/it.po` (579 lines)
- `addons/website_slides_forum/i18n/ja.po` (567 lines)
- `addons/website_slides_forum/i18n/kab.po` (495 lines)
- `addons/website_slides_forum/i18n/ko.po` (558 lines)
- `addons/website_slides_forum/i18n/ku.po` (494 lines)
- `addons/website_slides_forum/i18n/lo.po` (551 lines)
- `addons/website_slides_forum/i18n/lt.po` (522 lines)
- `addons/website_slides_forum/i18n/lv.po` (495 lines)
- `addons/website_slides_forum/i18n/mn.po` (518 lines)
- `addons/website_slides_forum/i18n/my.po` (494 lines)
- `addons/website_slides_forum/i18n/nb.po` (500 lines)
- `addons/website_slides_forum/i18n/nl.po` (587 lines)
- `addons/website_slides_forum/i18n/pl.po` (590 lines)
- `addons/website_slides_forum/i18n/pt.po` (574 lines)
- `addons/website_slides_forum/i18n/pt_BR.po` (586 lines)
- `addons/website_slides_forum/i18n/ro.po` (561 lines)
- `addons/website_slides_forum/i18n/ru.po` (578 lines)
- `addons/website_slides_forum/i18n/sk.po` (494 lines)
- `addons/website_slides_forum/i18n/sl.po` (496 lines)
- `addons/website_slides_forum/i18n/sr@latin.po` (495 lines)
- `addons/website_slides_forum/i18n/sv.po` (568 lines)
- `addons/website_slides_forum/i18n/th.po` (546 lines)
- `addons/website_slides_forum/i18n/tr.po` (585 lines)
- `addons/website_slides_forum/i18n/uk.po` (556 lines)
- `addons/website_slides_forum/i18n/uz.po` (647 lines)
- `addons/website_slides_forum/i18n/vi.po` (573 lines)
- `addons/website_slides_forum/i18n/website_slides_forum.pot` (490 lines)
- `addons/website_slides_forum/i18n/zh_CN.po` (536 lines)
- `addons/website_slides_forum/i18n/zh_TW.po` (502 lines)
- `addons/website_slides_forum/models/__init__.py` (4 lines)
- `addons/website_slides_forum/models/forum_forum.py` (73 lines)
- `addons/website_slides_forum/models/slide_channel.py` (46 lines)
- `addons/website_slides_forum/security/ir.access.csv` (2 lines)
- `addons/website_slides_forum/static/src/website_builder/slides_forum_page_option.xml` (12 lines)
- `addons/website_slides_forum/tests/__init__.py` (3 lines)
- `addons/website_slides_forum/tests/test_website_slides_forum.py` (140 lines)
- `addons/website_slides_forum/views/forum_forum_templates.xml` (51 lines)
- `addons/website_slides_forum/views/forum_forum_views.xml` (55 lines)
- `addons/website_slides_forum/views/forum_post_views.xml` (29 lines)
- `addons/website_slides_forum/views/res_config_settings_views.xml` (16 lines)
- `addons/website_slides_forum/views/slide_channel_views.xml` (23 lines)
- `addons/website_slides_forum/views/website_slides_menu_views.xml` (17 lines)
- `addons/website_slides_forum/views/website_slides_templates.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
