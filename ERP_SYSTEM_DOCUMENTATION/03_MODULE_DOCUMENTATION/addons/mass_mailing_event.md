# Module: mass_mailing_event

- **Module ID:** MOD-365
- **Path:** `addons/mass_mailing_event`
- **Manifest:** `addons/mass_mailing_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Mass mail event attendees
=========================

Bridge module adding UX requirements to ease mass mailing of event attendees.
        

Declared dependencies: `event`, `mass_mailing`.

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
    "event",
    "mass_mailing"
  ],
  "data": [
    "views/event_views.xml"
  ]
}
```

### Representative source files

- `addons/mass_mailing_event/__init__.py` (4 lines)
- `addons/mass_mailing_event/__manifest__.py` (20 lines)
- `addons/mass_mailing_event/i18n/ar.po` (78 lines)
- `addons/mass_mailing_event/i18n/az.po` (78 lines)
- `addons/mass_mailing_event/i18n/bg.po` (79 lines)
- `addons/mass_mailing_event/i18n/bs.po` (81 lines)
- `addons/mass_mailing_event/i18n/ca.po` (81 lines)
- `addons/mass_mailing_event/i18n/cs.po` (79 lines)
- `addons/mass_mailing_event/i18n/da.po` (80 lines)
- `addons/mass_mailing_event/i18n/de.po` (84 lines)
- `addons/mass_mailing_event/i18n/el.po` (79 lines)
- `addons/mass_mailing_event/i18n/es.po` (86 lines)
- `addons/mass_mailing_event/i18n/es_419.po` (75 lines)
- `addons/mass_mailing_event/i18n/et.po` (81 lines)
- `addons/mass_mailing_event/i18n/fa.po` (82 lines)
- `addons/mass_mailing_event/i18n/fi.po` (84 lines)
- `addons/mass_mailing_event/i18n/fr.po` (79 lines)
- `addons/mass_mailing_event/i18n/gu.po` (73 lines)
- `addons/mass_mailing_event/i18n/he.po` (81 lines)
- `addons/mass_mailing_event/i18n/hi.po` (80 lines)
- `addons/mass_mailing_event/i18n/hr.po` (80 lines)
- `addons/mass_mailing_event/i18n/hu.po` (81 lines)
- `addons/mass_mailing_event/i18n/id.po` (77 lines)
- `addons/mass_mailing_event/i18n/is.po` (70 lines)
- `addons/mass_mailing_event/i18n/it.po` (85 lines)
- `addons/mass_mailing_event/i18n/ja.po` (78 lines)
- `addons/mass_mailing_event/i18n/kab.po` (77 lines)
- `addons/mass_mailing_event/i18n/km.po` (73 lines)
- `addons/mass_mailing_event/i18n/ko.po` (77 lines)
- `addons/mass_mailing_event/i18n/ku.po` (75 lines)
- `addons/mass_mailing_event/i18n/lo.po` (80 lines)
- `addons/mass_mailing_event/i18n/lt.po` (79 lines)
- `addons/mass_mailing_event/i18n/lv.po` (81 lines)
- `addons/mass_mailing_event/i18n/mass_mailing_event.pot` (69 lines)
- `addons/mass_mailing_event/i18n/mn.po` (79 lines)
- `addons/mass_mailing_event/i18n/my.po` (78 lines)
- `addons/mass_mailing_event/i18n/nb.po` (77 lines)
- `addons/mass_mailing_event/i18n/nl.po` (78 lines)
- `addons/mass_mailing_event/i18n/pl.po` (80 lines)
- `addons/mass_mailing_event/i18n/pt.po` (82 lines)
- `addons/mass_mailing_event/i18n/pt_BR.po` (85 lines)
- `addons/mass_mailing_event/i18n/ro.po` (82 lines)
- `addons/mass_mailing_event/i18n/ru.po` (79 lines)
- `addons/mass_mailing_event/i18n/sk.po` (80 lines)
- `addons/mass_mailing_event/i18n/sl.po` (78 lines)
- `addons/mass_mailing_event/i18n/sr@latin.po` (79 lines)
- `addons/mass_mailing_event/i18n/sv.po` (79 lines)
- `addons/mass_mailing_event/i18n/th.po` (78 lines)
- `addons/mass_mailing_event/i18n/tr.po` (81 lines)
- `addons/mass_mailing_event/i18n/uk.po` (83 lines)
- `addons/mass_mailing_event/i18n/uz.po` (88 lines)
- `addons/mass_mailing_event/i18n/vi.po` (77 lines)
- `addons/mass_mailing_event/i18n/zh_CN.po` (77 lines)
- `addons/mass_mailing_event/i18n/zh_TW.po` (77 lines)
- `addons/mass_mailing_event/models/__init__.py` (5 lines)
- `addons/mass_mailing_event/models/event_event.py` (38 lines)
- `addons/mass_mailing_event/models/event_registration.py` (18 lines)
- `addons/mass_mailing_event/views/event_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
