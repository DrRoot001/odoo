# Module: mass_mailing_event_sms

- **Module ID:** MOD-366
- **Path:** `addons/mass_mailing_event_sms`
- **Manifest:** `addons/mass_mailing_event_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


SMS Marketing on event attendees
================================

Bridge module adding UX requirements to ease SMS marketing o, event attendees.
        

Declared dependencies: `event`, `mass_mailing`, `mass_mailing_event`, `mass_mailing_sms`, `sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event",
    "mass_mailing",
    "mass_mailing_event",
    "mass_mailing_sms",
    "sms"
  ]
}
```

### Representative source files

- `addons/mass_mailing_event_sms/__init__.py` (4 lines)
- `addons/mass_mailing_event_sms/__manifest__.py` (23 lines)
- `addons/mass_mailing_event_sms/i18n/ar.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/az.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/bg.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/bs.po` (56 lines)
- `addons/mass_mailing_event_sms/i18n/ca.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/cs.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/da.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/de.po` (58 lines)
- `addons/mass_mailing_event_sms/i18n/el.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/es.po` (59 lines)
- `addons/mass_mailing_event_sms/i18n/es_419.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/et.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/fa.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/fi.po` (59 lines)
- `addons/mass_mailing_event_sms/i18n/fr.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/he.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/hi.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/hr.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/hu.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/id.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/it.po` (59 lines)
- `addons/mass_mailing_event_sms/i18n/ja.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/kab.po` (55 lines)
- `addons/mass_mailing_event_sms/i18n/ko.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/ku.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/lo.po` (54 lines)
- `addons/mass_mailing_event_sms/i18n/lt.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/lv.po` (55 lines)
- `addons/mass_mailing_event_sms/i18n/mass_mailing_event_sms.pot` (46 lines)
- `addons/mass_mailing_event_sms/i18n/mn.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/my.po` (51 lines)
- `addons/mass_mailing_event_sms/i18n/nb.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/nl.po` (59 lines)
- `addons/mass_mailing_event_sms/i18n/pl.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/pt.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/pt_BR.po` (60 lines)
- `addons/mass_mailing_event_sms/i18n/ro.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/ru.po` (54 lines)
- `addons/mass_mailing_event_sms/i18n/sk.po` (54 lines)
- `addons/mass_mailing_event_sms/i18n/sl.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/sr@latin.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/sv.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/th.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/tr.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/uk.po` (52 lines)
- `addons/mass_mailing_event_sms/i18n/uz.po` (61 lines)
- `addons/mass_mailing_event_sms/i18n/vi.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/zh_CN.po` (53 lines)
- `addons/mass_mailing_event_sms/i18n/zh_TW.po` (54 lines)
- `addons/mass_mailing_event_sms/models/__init__.py` (4 lines)
- `addons/mass_mailing_event_sms/models/event.py` (20 lines)
- `addons/mass_mailing_event_sms/tests/__init__.py` (1 lines)
- `addons/mass_mailing_event_sms/tests/test_mailing_event.py` (42 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
