# Module: website_event_booth

- **Module ID:** MOD-607
- **Path:** `addons/website_event_booth`
- **Manifest:** `addons/website_event_booth/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Events, display your booths on your website


Display your booths on your website for the users to register.
    

Declared dependencies: `website_event`, `event_booth`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 6 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event",
    "event_booth"
  ],
  "data": [
    "views/event_type_views.xml",
    "views/event_event_views.xml",
    "views/event_booth_registration_templates.xml",
    "views/event_booth_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "/website_event_booth/static/src/interactions/*",
      "/website_event_booth/static/src/scss/website_event_booth.scss",
      "/website_event_booth/static/src/xml/event_booth_registration_templates.xml"
    ]
  }
}
```

### Representative source files

- `addons/website_event_booth/__init__.py` (5 lines)
- `addons/website_event_booth/__manifest__.py` (31 lines)
- `addons/website_event_booth/controllers/__init__.py` (4 lines)
- `addons/website_event_booth/controllers/event_booth.py` (192 lines)
- `addons/website_event_booth/data/event_demo.xml` (15 lines)
- `addons/website_event_booth/i18n/ar.po` (311 lines)
- `addons/website_event_booth/i18n/az.po` (290 lines)
- `addons/website_event_booth/i18n/bg.po` (290 lines)
- `addons/website_event_booth/i18n/bs.po` (292 lines)
- `addons/website_event_booth/i18n/ca.po` (303 lines)
- `addons/website_event_booth/i18n/cs.po` (291 lines)
- `addons/website_event_booth/i18n/da.po` (310 lines)
- `addons/website_event_booth/i18n/de.po` (319 lines)
- `addons/website_event_booth/i18n/el.po` (291 lines)
- `addons/website_event_booth/i18n/es.po` (313 lines)
- `addons/website_event_booth/i18n/es_419.po` (311 lines)
- `addons/website_event_booth/i18n/et.po` (290 lines)
- `addons/website_event_booth/i18n/fa.po` (290 lines)
- `addons/website_event_booth/i18n/fi.po` (314 lines)
- `addons/website_event_booth/i18n/fr.po` (313 lines)
- `addons/website_event_booth/i18n/he.po` (291 lines)
- `addons/website_event_booth/i18n/hi.po` (290 lines)
- `addons/website_event_booth/i18n/hr.po` (291 lines)
- `addons/website_event_booth/i18n/hu.po` (291 lines)
- `addons/website_event_booth/i18n/id.po` (309 lines)
- `addons/website_event_booth/i18n/it.po` (316 lines)
- `addons/website_event_booth/i18n/ja.po` (311 lines)
- `addons/website_event_booth/i18n/kab.po` (291 lines)
- `addons/website_event_booth/i18n/ko.po` (308 lines)
- `addons/website_event_booth/i18n/ku.po` (290 lines)
- `addons/website_event_booth/i18n/lo.po` (311 lines)
- `addons/website_event_booth/i18n/lt.po` (292 lines)
- `addons/website_event_booth/i18n/lv.po` (291 lines)
- `addons/website_event_booth/i18n/mn.po` (290 lines)
- `addons/website_event_booth/i18n/my.po` (290 lines)
- `addons/website_event_booth/i18n/nb.po` (291 lines)
- `addons/website_event_booth/i18n/nl.po` (312 lines)
- `addons/website_event_booth/i18n/pl.po` (312 lines)
- `addons/website_event_booth/i18n/pt.po` (311 lines)
- `addons/website_event_booth/i18n/pt_BR.po` (315 lines)
- `addons/website_event_booth/i18n/ro.po` (291 lines)
- `addons/website_event_booth/i18n/ru.po` (315 lines)
- `addons/website_event_booth/i18n/sk.po` (290 lines)
- `addons/website_event_booth/i18n/sl.po` (292 lines)
- `addons/website_event_booth/i18n/sr@latin.po` (291 lines)
- `addons/website_event_booth/i18n/sv.po` (308 lines)
- `addons/website_event_booth/i18n/th.po` (305 lines)
- `addons/website_event_booth/i18n/tr.po` (312 lines)
- `addons/website_event_booth/i18n/uk.po` (291 lines)
- `addons/website_event_booth/i18n/uz.po` (339 lines)
- `addons/website_event_booth/i18n/vi.po` (311 lines)
- `addons/website_event_booth/i18n/website_event_booth.pot` (284 lines)
- `addons/website_event_booth/i18n/zh_CN.po` (311 lines)
- `addons/website_event_booth/i18n/zh_TW.po` (311 lines)
- `addons/website_event_booth/models/__init__.py` (6 lines)
- `addons/website_event_booth/models/event_event.py` (59 lines)
- `addons/website_event_booth/models/event_type.py` (17 lines)
- `addons/website_event_booth/models/website_event_menu.py` (11 lines)
- `addons/website_event_booth/security/ir.access.csv` (4 lines)
- `addons/website_event_booth/static/src/img/exhibition-map.gif` (584 lines)
- `addons/website_event_booth/static/src/interactions/booth_registration.js` (236 lines)
- `addons/website_event_booth/static/src/scss/website_event_booth.scss` (71 lines)
- `addons/website_event_booth/static/src/xml/event_booth_registration_templates.xml` (33 lines)
- `addons/website_event_booth/tests/__init__.py` (3 lines)
- `addons/website_event_booth/tests/test_event_booth.py` (41 lines)
- `addons/website_event_booth/views/event_booth_registration_templates.xml` (74 lines)
- `addons/website_event_booth/views/event_booth_templates.xml` (141 lines)
- `addons/website_event_booth/views/event_event_views.xml` (21 lines)
- `addons/website_event_booth/views/event_type_views.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
