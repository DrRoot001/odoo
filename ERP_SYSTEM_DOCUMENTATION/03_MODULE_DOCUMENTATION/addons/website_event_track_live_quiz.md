# Module: website_event_track_live_quiz

- **Module ID:** MOD-616
- **Path:** `addons/website_event_track_live_quiz`
- **Manifest:** `addons/website_event_track_live_quiz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Bridge module to support quiz features during "live" tracks. 

No manifest description declared.

Declared dependencies: `website_event_track_live`, `website_event_track_quiz`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event_track_live",
    "website_event_track_quiz"
  ],
  "data": [
    "views/event_track_templates_page.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_event_track_live_quiz/static/src/interactions/**/*",
      "website_event_track_live_quiz/static/src/xml/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_event_track_live_quiz/__init__.py` (4 lines)
- `addons/website_event_track_live_quiz/__manifest__.py` (25 lines)
- `addons/website_event_track_live_quiz/controllers/__init__.py` (4 lines)
- `addons/website_event_track_live_quiz/controllers/track_live_quiz.py` (12 lines)
- `addons/website_event_track_live_quiz/i18n/ar.po` (44 lines)
- `addons/website_event_track_live_quiz/i18n/az.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/bg.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/bs.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/ca.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/cs.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/da.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/de.po` (44 lines)
- `addons/website_event_track_live_quiz/i18n/el.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/es.po` (45 lines)
- `addons/website_event_track_live_quiz/i18n/es_419.po` (45 lines)
- `addons/website_event_track_live_quiz/i18n/et.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/fa.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/fi.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/fr.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/he.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/hi.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/hr.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/hu.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/id.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/it.po` (45 lines)
- `addons/website_event_track_live_quiz/i18n/ja.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/kab.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/ko.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/ku.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/lo.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/lt.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/lv.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/mn.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/my.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/nb.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/nl.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/pl.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/pt.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/pt_BR.po` (48 lines)
- `addons/website_event_track_live_quiz/i18n/ro.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/ru.po` (44 lines)
- `addons/website_event_track_live_quiz/i18n/sk.po` (41 lines)
- `addons/website_event_track_live_quiz/i18n/sl.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/sr@latin.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/sv.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/th.po` (43 lines)
- `addons/website_event_track_live_quiz/i18n/tr.po` (45 lines)
- `addons/website_event_track_live_quiz/i18n/uk.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/uz.po` (50 lines)
- `addons/website_event_track_live_quiz/i18n/vi.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/website_event_track_live_quiz.pot` (38 lines)
- `addons/website_event_track_live_quiz/i18n/zh_CN.po` (42 lines)
- `addons/website_event_track_live_quiz/i18n/zh_TW.po` (44 lines)
- `addons/website_event_track_live_quiz/static/src/interactions/quiz.js` (28 lines)
- `addons/website_event_track_live_quiz/static/src/interactions/website_event_track_suggestion.js` (27 lines)
- `addons/website_event_track_live_quiz/static/src/xml/website_event_track_live_templates.xml` (13 lines)
- `addons/website_event_track_live_quiz/static/src/xml/website_event_track_quiz_templates.xml` (14 lines)
- `addons/website_event_track_live_quiz/views/event_track_templates_page.xml` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
