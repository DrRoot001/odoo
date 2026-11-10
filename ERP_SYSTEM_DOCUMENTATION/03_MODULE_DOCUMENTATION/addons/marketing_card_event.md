# Module: marketing_card_event

- **Module ID:** MOD-361
- **Path:** `addons/marketing_card_event`
- **Manifest:** `addons/marketing_card_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate dynamic shareable cards for entities linked to events.

No manifest description declared.

Declared dependencies: `marketing_card`, `event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "marketing_card",
    "event"
  ],
  "data": [
    "views/event_event_views.xml",
    "views/mailing_mailing_views.xml"
  ]
}
```

### Representative source files

- `addons/marketing_card_event/__init__.py` (1 lines)
- `addons/marketing_card_event/__manifest__.py` (14 lines)
- `addons/marketing_card_event/i18n/ar.po` (78 lines)
- `addons/marketing_card_event/i18n/az.po` (77 lines)
- `addons/marketing_card_event/i18n/bg.po` (77 lines)
- `addons/marketing_card_event/i18n/bs.po` (78 lines)
- `addons/marketing_card_event/i18n/ca.po` (77 lines)
- `addons/marketing_card_event/i18n/cs.po` (77 lines)
- `addons/marketing_card_event/i18n/da.po` (77 lines)
- `addons/marketing_card_event/i18n/de.po` (80 lines)
- `addons/marketing_card_event/i18n/el.po` (77 lines)
- `addons/marketing_card_event/i18n/es.po` (78 lines)
- `addons/marketing_card_event/i18n/es_419.po` (78 lines)
- `addons/marketing_card_event/i18n/et.po` (77 lines)
- `addons/marketing_card_event/i18n/fa.po` (77 lines)
- `addons/marketing_card_event/i18n/fi.po` (79 lines)
- `addons/marketing_card_event/i18n/fr.po` (78 lines)
- `addons/marketing_card_event/i18n/he.po` (78 lines)
- `addons/marketing_card_event/i18n/hi.po` (77 lines)
- `addons/marketing_card_event/i18n/hr.po` (78 lines)
- `addons/marketing_card_event/i18n/hu.po` (77 lines)
- `addons/marketing_card_event/i18n/id.po` (77 lines)
- `addons/marketing_card_event/i18n/it.po` (78 lines)
- `addons/marketing_card_event/i18n/ja.po` (78 lines)
- `addons/marketing_card_event/i18n/kab.po` (77 lines)
- `addons/marketing_card_event/i18n/ko.po` (77 lines)
- `addons/marketing_card_event/i18n/ku.po` (77 lines)
- `addons/marketing_card_event/i18n/lo.po` (77 lines)
- `addons/marketing_card_event/i18n/lt.po` (79 lines)
- `addons/marketing_card_event/i18n/lv.po` (78 lines)
- `addons/marketing_card_event/i18n/marketing_card_event.pot` (74 lines)
- `addons/marketing_card_event/i18n/mn.po` (77 lines)
- `addons/marketing_card_event/i18n/my.po` (77 lines)
- `addons/marketing_card_event/i18n/nb.po` (77 lines)
- `addons/marketing_card_event/i18n/nl.po` (80 lines)
- `addons/marketing_card_event/i18n/pl.po` (78 lines)
- `addons/marketing_card_event/i18n/pt.po` (77 lines)
- `addons/marketing_card_event/i18n/pt_BR.po` (82 lines)
- `addons/marketing_card_event/i18n/ro.po` (78 lines)
- `addons/marketing_card_event/i18n/ru.po` (79 lines)
- `addons/marketing_card_event/i18n/sk.po` (77 lines)
- `addons/marketing_card_event/i18n/sl.po` (78 lines)
- `addons/marketing_card_event/i18n/sr@latin.po` (78 lines)
- `addons/marketing_card_event/i18n/sv.po` (78 lines)
- `addons/marketing_card_event/i18n/th.po` (78 lines)
- `addons/marketing_card_event/i18n/tr.po` (77 lines)
- `addons/marketing_card_event/i18n/uk.po` (78 lines)
- `addons/marketing_card_event/i18n/uz.po` (77 lines)
- `addons/marketing_card_event/i18n/vi.po` (77 lines)
- `addons/marketing_card_event/i18n/zh_CN.po` (79 lines)
- `addons/marketing_card_event/i18n/zh_TW.po` (77 lines)
- `addons/marketing_card_event/models/__init__.py` (3 lines)
- `addons/marketing_card_event/models/card_campaign.py` (39 lines)
- `addons/marketing_card_event/models/event_event.py` (22 lines)
- `addons/marketing_card_event/models/mailing_mailing.py` (57 lines)
- `addons/marketing_card_event/tests/__init__.py` (1 lines)
- `addons/marketing_card_event/tests/test_mailing.py` (85 lines)
- `addons/marketing_card_event/views/event_event_views.xml` (15 lines)
- `addons/marketing_card_event/views/mailing_mailing_views.xml` (17 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
