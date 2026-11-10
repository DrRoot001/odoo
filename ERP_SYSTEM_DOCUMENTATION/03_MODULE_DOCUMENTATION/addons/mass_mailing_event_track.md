# Module: mass_mailing_event_track

- **Module ID:** MOD-367
- **Path:** `addons/mass_mailing_event_track`
- **Manifest:** `addons/mass_mailing_event_track/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Mass mail event track speakers
==============================

Bridge module adding UX requirements to ease mass mailing of event track speakers.
        

Declared dependencies: `website_event_track`, `mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event_track",
    "mass_mailing"
  ],
  "data": [
    "views/event_views.xml"
  ]
}
```

### Representative source files

- `addons/mass_mailing_event_track/__init__.py` (4 lines)
- `addons/mass_mailing_event_track/__manifest__.py` (20 lines)
- `addons/mass_mailing_event_track/i18n/ar.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/az.po` (71 lines)
- `addons/mass_mailing_event_track/i18n/bg.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/bs.po` (71 lines)
- `addons/mass_mailing_event_track/i18n/ca.po` (75 lines)
- `addons/mass_mailing_event_track/i18n/cs.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/da.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/de.po` (80 lines)
- `addons/mass_mailing_event_track/i18n/el.po` (71 lines)
- `addons/mass_mailing_event_track/i18n/es.po` (81 lines)
- `addons/mass_mailing_event_track/i18n/es_419.po` (71 lines)
- `addons/mass_mailing_event_track/i18n/et.po` (74 lines)
- `addons/mass_mailing_event_track/i18n/fa.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/fi.po` (80 lines)
- `addons/mass_mailing_event_track/i18n/fr.po` (74 lines)
- `addons/mass_mailing_event_track/i18n/gu.po` (68 lines)
- `addons/mass_mailing_event_track/i18n/he.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/hi.po` (69 lines)
- `addons/mass_mailing_event_track/i18n/hr.po` (74 lines)
- `addons/mass_mailing_event_track/i18n/hu.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/id.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/is.po` (65 lines)
- `addons/mass_mailing_event_track/i18n/it.po` (81 lines)
- `addons/mass_mailing_event_track/i18n/ja.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/kab.po` (68 lines)
- `addons/mass_mailing_event_track/i18n/km.po` (68 lines)
- `addons/mass_mailing_event_track/i18n/ko.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/ku.po` (69 lines)
- `addons/mass_mailing_event_track/i18n/lo.po` (68 lines)
- `addons/mass_mailing_event_track/i18n/lt.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/lv.po` (71 lines)
- `addons/mass_mailing_event_track/i18n/mass_mailing_event_track.pot` (64 lines)
- `addons/mass_mailing_event_track/i18n/mn.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/my.po` (69 lines)
- `addons/mass_mailing_event_track/i18n/nb.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/nl.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/pl.po` (75 lines)
- `addons/mass_mailing_event_track/i18n/pt.po` (75 lines)
- `addons/mass_mailing_event_track/i18n/pt_BR.po` (80 lines)
- `addons/mass_mailing_event_track/i18n/ro.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/ru.po` (74 lines)
- `addons/mass_mailing_event_track/i18n/sk.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/sl.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/sr@latin.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/sv.po` (74 lines)
- `addons/mass_mailing_event_track/i18n/th.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/tr.po` (75 lines)
- `addons/mass_mailing_event_track/i18n/uk.po` (75 lines)
- `addons/mass_mailing_event_track/i18n/uz.po` (82 lines)
- `addons/mass_mailing_event_track/i18n/vi.po` (72 lines)
- `addons/mass_mailing_event_track/i18n/zh_CN.po` (73 lines)
- `addons/mass_mailing_event_track/i18n/zh_TW.po` (73 lines)
- `addons/mass_mailing_event_track/models/__init__.py` (5 lines)
- `addons/mass_mailing_event_track/models/event_event.py` (26 lines)
- `addons/mass_mailing_event_track/models/event_track.py` (12 lines)
- `addons/mass_mailing_event_track/views/event_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
