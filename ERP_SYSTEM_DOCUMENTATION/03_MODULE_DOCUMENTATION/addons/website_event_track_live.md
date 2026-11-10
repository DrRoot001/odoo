# Module: website_event_track_live

- **Module ID:** MOD-615
- **Path:** `addons/website_event_track_live`
- **Manifest:** `addons/website_event_track_live/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Support live tracks: streaming, participation, youtube

No manifest description declared.

Declared dependencies: `website_event_track`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event_track"
  ],
  "data": [
    "views/event_track_templates_list.xml",
    "views/event_track_templates_page.xml",
    "views/event_track_views.xml"
  ],
  "demo": [
    "data/event_track_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_event_track_live/static/src/scss/website_event_track_live.scss",
      "website_event_track_live/static/src/interactions/*.js",
      "website_event_track_live/static/src/xml/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_event_track_live/__init__.py` (5 lines)
- `addons/website_event_track_live/__manifest__.py` (30 lines)
- `addons/website_event_track_live/controllers/__init__.py` (5 lines)
- `addons/website_event_track_live/controllers/session.py` (21 lines)
- `addons/website_event_track_live/controllers/track_live.py` (37 lines)
- `addons/website_event_track_live/data/event_track_demo.xml` (59 lines)
- `addons/website_event_track_live/i18n/ar.po` (128 lines)
- `addons/website_event_track_live/i18n/az.po` (119 lines)
- `addons/website_event_track_live/i18n/bg.po` (119 lines)
- `addons/website_event_track_live/i18n/bs.po` (121 lines)
- `addons/website_event_track_live/i18n/ca.po` (126 lines)
- `addons/website_event_track_live/i18n/cs.po` (126 lines)
- `addons/website_event_track_live/i18n/da.po` (127 lines)
- `addons/website_event_track_live/i18n/de.po` (127 lines)
- `addons/website_event_track_live/i18n/el.po` (120 lines)
- `addons/website_event_track_live/i18n/es.po` (127 lines)
- `addons/website_event_track_live/i18n/es_419.po` (127 lines)
- `addons/website_event_track_live/i18n/et.po` (119 lines)
- `addons/website_event_track_live/i18n/fa.po` (119 lines)
- `addons/website_event_track_live/i18n/fi.po` (127 lines)
- `addons/website_event_track_live/i18n/fr.po` (129 lines)
- `addons/website_event_track_live/i18n/he.po` (120 lines)
- `addons/website_event_track_live/i18n/hi.po` (119 lines)
- `addons/website_event_track_live/i18n/hr.po` (120 lines)
- `addons/website_event_track_live/i18n/hu.po` (120 lines)
- `addons/website_event_track_live/i18n/id.po` (126 lines)
- `addons/website_event_track_live/i18n/it.po` (127 lines)
- `addons/website_event_track_live/i18n/ja.po` (127 lines)
- `addons/website_event_track_live/i18n/kab.po` (120 lines)
- `addons/website_event_track_live/i18n/ko.po` (126 lines)
- `addons/website_event_track_live/i18n/ku.po` (119 lines)
- `addons/website_event_track_live/i18n/lo.po` (119 lines)
- `addons/website_event_track_live/i18n/lt.po` (121 lines)
- `addons/website_event_track_live/i18n/lv.po` (120 lines)
- `addons/website_event_track_live/i18n/mn.po` (119 lines)
- `addons/website_event_track_live/i18n/my.po` (119 lines)
- `addons/website_event_track_live/i18n/nb.po` (120 lines)
- `addons/website_event_track_live/i18n/nl.po` (127 lines)
- `addons/website_event_track_live/i18n/pl.po` (127 lines)
- `addons/website_event_track_live/i18n/pt.po` (127 lines)
- `addons/website_event_track_live/i18n/pt_BR.po` (130 lines)
- `addons/website_event_track_live/i18n/ro.po` (127 lines)
- `addons/website_event_track_live/i18n/ru.po` (129 lines)
- `addons/website_event_track_live/i18n/sk.po` (119 lines)
- `addons/website_event_track_live/i18n/sl.po` (121 lines)
- `addons/website_event_track_live/i18n/sr@latin.po` (120 lines)
- `addons/website_event_track_live/i18n/sv.po` (128 lines)
- `addons/website_event_track_live/i18n/th.po` (124 lines)
- `addons/website_event_track_live/i18n/tr.po` (128 lines)
- `addons/website_event_track_live/i18n/uk.po` (120 lines)
- `addons/website_event_track_live/i18n/uz.po` (146 lines)
- `addons/website_event_track_live/i18n/vi.po` (126 lines)
- `addons/website_event_track_live/i18n/website_event_track_live.pot` (116 lines)
- `addons/website_event_track_live/i18n/zh_CN.po` (123 lines)
- `addons/website_event_track_live/i18n/zh_TW.po` (126 lines)
- `addons/website_event_track_live/models/__init__.py` (4 lines)
- `addons/website_event_track_live/models/event_track.py` (41 lines)
- `addons/website_event_track_live/static/src/interactions/website_event_track_live.js` (140 lines)
- `addons/website_event_track_live/static/src/interactions/website_event_track_replay_suggestion.js` (23 lines)
- `addons/website_event_track_live/static/src/interactions/website_event_track_suggestion.js` (56 lines)
- `addons/website_event_track_live/static/src/scss/website_event_track_live.scss` (53 lines)
- `addons/website_event_track_live/static/src/xml/website_event_track_live_templates.xml` (50 lines)
- `addons/website_event_track_live/views/event_track_templates_list.xml` (18 lines)
- `addons/website_event_track_live/views/event_track_templates_page.xml` (67 lines)
- `addons/website_event_track_live/views/event_track_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
