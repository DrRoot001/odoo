# Module: website_event_booth_exhibitor

- **Module ID:** MOD-608
- **Path:** `addons/website_event_booth_exhibitor`
- **Manifest:** `addons/website_event_booth_exhibitor/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Event Booths, automatically create a sponsor.


Automatically create a sponsor when renting a booth.
    

Declared dependencies: `website_event_exhibitor`, `website_event_booth`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event_exhibitor",
    "website_event_booth"
  ],
  "data": [
    "data/event_booth_category_data.xml",
    "views/event_booth_category_views.xml",
    "views/event_booth_views.xml",
    "views/event_booth_registration_templates.xml",
    "views/event_booth_templates.xml",
    "views/mail_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "/website_event_booth_exhibitor/static/src/interactions/booth_sponsor_details.js"
    ],
    "web.assets_tests": [
      "website_event_booth_exhibitor/static/tests/tours/website_event_booth_exhibitor_steps.js",
      "website_event_booth_exhibitor/static/tests/tours/website_event_booth_exhibitor.js"
    ]
  }
}
```

### Representative source files

- `addons/website_event_booth_exhibitor/__init__.py` (5 lines)
- `addons/website_event_booth_exhibitor/__manifest__.py` (33 lines)
- `addons/website_event_booth_exhibitor/controllers/__init__.py` (4 lines)
- `addons/website_event_booth_exhibitor/controllers/event_booth.py` (47 lines)
- `addons/website_event_booth_exhibitor/data/event_booth_category_data.xml` (16 lines)
- `addons/website_event_booth_exhibitor/i18n/ar.po` (192 lines)
- `addons/website_event_booth_exhibitor/i18n/az.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/bg.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/bs.po` (188 lines)
- `addons/website_event_booth_exhibitor/i18n/ca.po` (193 lines)
- `addons/website_event_booth_exhibitor/i18n/cs.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/da.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/de.po` (196 lines)
- `addons/website_event_booth_exhibitor/i18n/el.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/es.po` (196 lines)
- `addons/website_event_booth_exhibitor/i18n/es_419.po` (193 lines)
- `addons/website_event_booth_exhibitor/i18n/et.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/fa.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/fi.po` (191 lines)
- `addons/website_event_booth_exhibitor/i18n/fr.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/he.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/hi.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/hr.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/hu.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/id.po` (191 lines)
- `addons/website_event_booth_exhibitor/i18n/it.po` (193 lines)
- `addons/website_event_booth_exhibitor/i18n/ja.po` (191 lines)
- `addons/website_event_booth_exhibitor/i18n/kab.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/ko.po` (191 lines)
- `addons/website_event_booth_exhibitor/i18n/ku.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/lo.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/lt.po` (188 lines)
- `addons/website_event_booth_exhibitor/i18n/lv.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/mn.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/my.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/nb.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/nl.po` (193 lines)
- `addons/website_event_booth_exhibitor/i18n/pl.po` (195 lines)
- `addons/website_event_booth_exhibitor/i18n/pt.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/pt_BR.po` (197 lines)
- `addons/website_event_booth_exhibitor/i18n/ro.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/ru.po` (196 lines)
- `addons/website_event_booth_exhibitor/i18n/sk.po` (186 lines)
- `addons/website_event_booth_exhibitor/i18n/sl.po` (188 lines)
- `addons/website_event_booth_exhibitor/i18n/sr@latin.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/sv.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/th.po` (191 lines)
- `addons/website_event_booth_exhibitor/i18n/tr.po` (197 lines)
- `addons/website_event_booth_exhibitor/i18n/uk.po` (187 lines)
- `addons/website_event_booth_exhibitor/i18n/uz.po` (223 lines)
- `addons/website_event_booth_exhibitor/i18n/vi.po` (192 lines)
- `addons/website_event_booth_exhibitor/i18n/website_event_booth_exhibitor.pot` (183 lines)
- `addons/website_event_booth_exhibitor/i18n/zh_CN.po` (194 lines)
- `addons/website_event_booth_exhibitor/i18n/zh_TW.po` (194 lines)
- `addons/website_event_booth_exhibitor/models/__init__.py` (5 lines)
- `addons/website_event_booth_exhibitor/models/event_booth.py` (52 lines)
- `addons/website_event_booth_exhibitor/models/event_booth_category.py` (24 lines)
- `addons/website_event_booth_exhibitor/static/src/interactions/booth_sponsor_details.js` (33 lines)
- `addons/website_event_booth_exhibitor/static/tests/tours/website_event_booth_exhibitor.js` (45 lines)
- `addons/website_event_booth_exhibitor/static/tests/tours/website_event_booth_exhibitor_steps.js` (15 lines)
- `addons/website_event_booth_exhibitor/tests/__init__.py` (4 lines)
- `addons/website_event_booth_exhibitor/tests/test_wevent_booth_exhibitor.py` (52 lines)
- `addons/website_event_booth_exhibitor/views/event_booth_category_views.xml` (51 lines)
- `addons/website_event_booth_exhibitor/views/event_booth_registration_templates.xml` (75 lines)
- `addons/website_event_booth_exhibitor/views/event_booth_templates.xml` (10 lines)
- `addons/website_event_booth_exhibitor/views/event_booth_views.xml` (18 lines)
- `addons/website_event_booth_exhibitor/views/mail_templates.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
