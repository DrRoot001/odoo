# Module: website_links

- **Module ID:** MOD-622
- **Path:** `addons/website_links`
- **Manifest:** `addons/website_links/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate trackable & short URLs


Generate short links with analytics trackers (UTM) to share your pages through marketing campaigns.
Those trackers can be used in Google Analytics to track clicks and visitors, or in Odoo reports to analyze the efficiency of those campaigns in terms of lead generation, related revenues (sales orders), recruitment, etc.
    

Declared dependencies: `website`, `link_tracker`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "link_tracker"
  ],
  "data": [
    "views/link_tracker_views.xml",
    "views/website_links_template.xml",
    "views/website_links_graphs.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_links/static/src/components/*.js",
      "website_links/static/src/interactions/*.js",
      "website_links/static/src/css/website_links.css",
      "website_links/static/src/xml/*.xml"
    ],
    "web.assets_tests": [
      "website_links/static/tests/**/*"
    ],
    "website.assets_editor": [
      "website_links/static/src/services/website_custom_menus.js"
    ]
  }
}
```

### Representative source files

- `addons/website_links/__init__.py` (3 lines)
- `addons/website_links/__manifest__.py` (33 lines)
- `addons/website_links/controller/__init__.py` (2 lines)
- `addons/website_links/controller/main.py` (46 lines)
- `addons/website_links/i18n/af.po` (363 lines)
- `addons/website_links/i18n/ar.po` (397 lines)
- `addons/website_links/i18n/az.po` (375 lines)
- `addons/website_links/i18n/bg.po` (372 lines)
- `addons/website_links/i18n/bs.po` (370 lines)
- `addons/website_links/i18n/ca.po` (391 lines)
- `addons/website_links/i18n/cs.po` (379 lines)
- `addons/website_links/i18n/da.po` (384 lines)
- `addons/website_links/i18n/de.po` (414 lines)
- `addons/website_links/i18n/el.po` (378 lines)
- `addons/website_links/i18n/es.po` (409 lines)
- `addons/website_links/i18n/es_419.po` (410 lines)
- `addons/website_links/i18n/et.po` (385 lines)
- `addons/website_links/i18n/fa.po` (376 lines)
- `addons/website_links/i18n/fi.po` (411 lines)
- `addons/website_links/i18n/fr.po` (409 lines)
- `addons/website_links/i18n/gu.po` (368 lines)
- `addons/website_links/i18n/he.po` (379 lines)
- `addons/website_links/i18n/hi.po` (367 lines)
- `addons/website_links/i18n/hr.po` (377 lines)
- `addons/website_links/i18n/hu.po` (374 lines)
- `addons/website_links/i18n/id.po` (393 lines)
- `addons/website_links/i18n/is.po` (363 lines)
- `addons/website_links/i18n/it.po` (414 lines)
- `addons/website_links/i18n/ja.po` (405 lines)
- `addons/website_links/i18n/kab.po` (367 lines)
- `addons/website_links/i18n/km.po` (367 lines)
- `addons/website_links/i18n/ko.po` (385 lines)
- `addons/website_links/i18n/ku.po` (367 lines)
- `addons/website_links/i18n/lo.po` (404 lines)
- `addons/website_links/i18n/lt.po` (381 lines)
- `addons/website_links/i18n/lv.po` (373 lines)
- `addons/website_links/i18n/mk.po` (371 lines)
- `addons/website_links/i18n/mn.po` (379 lines)
- `addons/website_links/i18n/my.po` (367 lines)
- `addons/website_links/i18n/nb.po` (375 lines)
- `addons/website_links/i18n/nl.po` (406 lines)
- `addons/website_links/i18n/pl.po` (410 lines)
- `addons/website_links/i18n/pt.po` (380 lines)
- `addons/website_links/i18n/pt_BR.po` (416 lines)
- `addons/website_links/i18n/ro.po` (380 lines)
- `addons/website_links/i18n/ru.po` (399 lines)
- `addons/website_links/i18n/sk.po` (375 lines)
- `addons/website_links/i18n/sl.po` (378 lines)
- `addons/website_links/i18n/sr@latin.po` (372 lines)
- `addons/website_links/i18n/sv.po` (382 lines)
- `addons/website_links/i18n/th.po` (404 lines)
- `addons/website_links/i18n/tr.po` (396 lines)
- `addons/website_links/i18n/uk.po` (379 lines)
- `addons/website_links/i18n/uz.po` (456 lines)
- `addons/website_links/i18n/vi.po` (377 lines)
- `addons/website_links/i18n/website_links.pot` (344 lines)
- `addons/website_links/i18n/zh_CN.po` (409 lines)
- `addons/website_links/i18n/zh_TW.po` (382 lines)
- `addons/website_links/models/__init__.py` (3 lines)
- `addons/website_links/models/link_tracker.py` (25 lines)
- `addons/website_links/security/ir.access.csv` (4 lines)
- `addons/website_links/static/description/icon.png` (18 lines)
- `addons/website_links/static/description/icon.svg` (1 lines)
- `addons/website_links/static/description/icon_hi.png` (45 lines)
- `addons/website_links/static/img/default_favicon.png` (6 lines)
- `addons/website_links/static/src/components/website_links_tags_wrapper.js` (130 lines)
- `addons/website_links/static/src/css/website_links.css` (53 lines)
- `addons/website_links/static/src/interactions/website_links.js` (261 lines)
- `addons/website_links/static/src/interactions/website_links_charts.js` (267 lines)
- `addons/website_links/static/src/interactions/website_links_code_editor.js` (140 lines)
- `addons/website_links/static/src/services/website_custom_menus.js` (8 lines)
- `addons/website_links/static/src/xml/recent_link.xml` (34 lines)
- `addons/website_links/static/src/xml/website_links_tags_wrapper.xml` (22 lines)
- `addons/website_links/static/tests/tours/website_links.js` (138 lines)
- `addons/website_links/tests/__init__.py` (5 lines)
- `addons/website_links/tests/test_controller.py` (67 lines)
- `addons/website_links/tests/test_link_tracker.py` (84 lines)
- `addons/website_links/tests/test_ui.py` (27 lines)
- `addons/website_links/views/link_tracker_views.xml` (19 lines)
- `addons/website_links/views/website_links_graphs.xml` (147 lines)
- `addons/website_links/views/website_links_template.xml` (105 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
