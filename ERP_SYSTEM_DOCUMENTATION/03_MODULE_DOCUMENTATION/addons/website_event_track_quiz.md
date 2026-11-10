# Module: website_event_track_quiz

- **Module ID:** MOD-617
- **Path:** `addons/website_event_track_quiz`
- **Manifest:** `addons/website_event_track_quiz/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Quizzes on tracks

No manifest description declared.

Declared dependencies: `website_profile`, `website_event_track`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_profile",
    "website_event_track"
  ],
  "data": [
    "views/event_leaderboard_templates.xml",
    "views/event_quiz_views.xml",
    "views/event_quiz_question_views.xml",
    "views/event_track_views.xml",
    "views/event_track_visitor_views.xml",
    "views/event_menus.xml",
    "views/event_quiz_templates.xml",
    "views/event_track_templates_page.xml",
    "views/event_event_views.xml",
    "views/event_type_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/quiz_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_event_track_quiz/static/src/scss/event_quiz.scss",
      "website_event_track_quiz/static/src/interactions/**/*",
      "website_event_track_quiz/static/src/xml/quiz_templates.xml"
    ]
  }
}
```

### Representative source files

- `addons/website_event_track_quiz/__init__.py` (5 lines)
- `addons/website_event_track_quiz/__manifest__.py` (39 lines)
- `addons/website_event_track_quiz/controllers/__init__.py` (5 lines)
- `addons/website_event_track_quiz/controllers/community.py` (88 lines)
- `addons/website_event_track_quiz/controllers/event_track_quiz.py` (81 lines)
- `addons/website_event_track_quiz/data/quiz_demo.xml` (155 lines)
- `addons/website_event_track_quiz/i18n/ar.po` (623 lines)
- `addons/website_event_track_quiz/i18n/az.po` (611 lines)
- `addons/website_event_track_quiz/i18n/bg.po` (611 lines)
- `addons/website_event_track_quiz/i18n/bs.po` (612 lines)
- `addons/website_event_track_quiz/i18n/ca.po` (626 lines)
- `addons/website_event_track_quiz/i18n/cs.po` (623 lines)
- `addons/website_event_track_quiz/i18n/da.po` (626 lines)
- `addons/website_event_track_quiz/i18n/de.po` (630 lines)
- `addons/website_event_track_quiz/i18n/el.po` (612 lines)
- `addons/website_event_track_quiz/i18n/es.po` (626 lines)
- `addons/website_event_track_quiz/i18n/es_419.po` (625 lines)
- `addons/website_event_track_quiz/i18n/et.po` (622 lines)
- `addons/website_event_track_quiz/i18n/fa.po` (611 lines)
- `addons/website_event_track_quiz/i18n/fi.po` (624 lines)
- `addons/website_event_track_quiz/i18n/fr.po` (627 lines)
- `addons/website_event_track_quiz/i18n/he.po` (612 lines)
- `addons/website_event_track_quiz/i18n/hi.po` (611 lines)
- `addons/website_event_track_quiz/i18n/hr.po` (612 lines)
- `addons/website_event_track_quiz/i18n/hu.po` (612 lines)
- `addons/website_event_track_quiz/i18n/id.po` (626 lines)
- `addons/website_event_track_quiz/i18n/it.po` (624 lines)
- `addons/website_event_track_quiz/i18n/ja.po` (621 lines)
- `addons/website_event_track_quiz/i18n/kab.po` (611 lines)
- `addons/website_event_track_quiz/i18n/ko.po` (614 lines)
- `addons/website_event_track_quiz/i18n/ku.po` (611 lines)
- `addons/website_event_track_quiz/i18n/lo.po` (618 lines)
- `addons/website_event_track_quiz/i18n/lt.po` (613 lines)
- `addons/website_event_track_quiz/i18n/lv.po` (611 lines)
- `addons/website_event_track_quiz/i18n/mn.po` (611 lines)
- `addons/website_event_track_quiz/i18n/my.po` (612 lines)
- `addons/website_event_track_quiz/i18n/nb.po` (611 lines)
- `addons/website_event_track_quiz/i18n/nl.po` (625 lines)
- `addons/website_event_track_quiz/i18n/pl.po` (627 lines)
- `addons/website_event_track_quiz/i18n/pt.po` (626 lines)
- `addons/website_event_track_quiz/i18n/pt_BR.po` (627 lines)
- `addons/website_event_track_quiz/i18n/ro.po` (627 lines)
- `addons/website_event_track_quiz/i18n/ru.po` (628 lines)
- `addons/website_event_track_quiz/i18n/sk.po` (610 lines)
- `addons/website_event_track_quiz/i18n/sl.po` (612 lines)
- `addons/website_event_track_quiz/i18n/sr@latin.po` (622 lines)
- `addons/website_event_track_quiz/i18n/sv.po` (623 lines)
- `addons/website_event_track_quiz/i18n/th.po` (614 lines)
- `addons/website_event_track_quiz/i18n/tr.po` (623 lines)
- `addons/website_event_track_quiz/i18n/uk.po` (624 lines)
- `addons/website_event_track_quiz/i18n/uz.po` (730 lines)
- `addons/website_event_track_quiz/i18n/vi.po` (621 lines)
- `addons/website_event_track_quiz/i18n/website_event_track_quiz.pot` (606 lines)
- `addons/website_event_track_quiz/i18n/zh_CN.po` (616 lines)
- `addons/website_event_track_quiz/i18n/zh_TW.po` (616 lines)
- `addons/website_event_track_quiz/models/__init__.py` (7 lines)
- `addons/website_event_track_quiz/models/event_event.py` (19 lines)
- `addons/website_event_track_quiz/models/event_quiz.py` (67 lines)
- `addons/website_event_track_quiz/models/event_track.py` (99 lines)
- `addons/website_event_track_quiz/models/event_track_visitor.py` (11 lines)
- `addons/website_event_track_quiz/security/ir.access.csv` (4 lines)
- `addons/website_event_track_quiz/static/src/interactions/leaderboard.js` (14 lines)
- `addons/website_event_track_quiz/static/src/interactions/quiz.js` (240 lines)
- `addons/website_event_track_quiz/static/src/scss/event_quiz.scss` (78 lines)
- `addons/website_event_track_quiz/static/src/xml/quiz_templates.xml` (94 lines)
- `addons/website_event_track_quiz/views/event_event_views.xml` (15 lines)
- `addons/website_event_track_quiz/views/event_leaderboard_templates.xml` (131 lines)
- `addons/website_event_track_quiz/views/event_menus.xml` (17 lines)
- `addons/website_event_track_quiz/views/event_quiz_question_views.xml` (94 lines)
- `addons/website_event_track_quiz/views/event_quiz_templates.xml` (50 lines)
- `addons/website_event_track_quiz/views/event_quiz_views.xml` (75 lines)
- `addons/website_event_track_quiz/views/event_track_templates_page.xml` (28 lines)
- `addons/website_event_track_quiz/views/event_track_views.xml` (24 lines)
- `addons/website_event_track_quiz/views/event_track_visitor_views.xml` (39 lines)
- `addons/website_event_track_quiz/views/event_type_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
