# Module: website_mass_mailing_event

- **Module ID:** MOD-627
- **Path:** `addons/website_mass_mailing_event`
- **Manifest:** `addons/website_mass_mailing_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Add pre-filled snippets in mass_mailing with an event snapshot


    Add pre-filled event snippets for the mass_mailing html builder, with links to the matching website event page.
    The snippet is linked to specified events and will load a snapshot of their data to be sent by email.
    

Declared dependencies: `mass_mailing`, `website_event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mass_mailing",
    "website_event"
  ],
  "assets": {
    "mass_mailing.assets_builder": [
      "website_mass_mailing_event/static/src/builder/**/*",
      "website_mass_mailing_event/static/src/snippets/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_mass_mailing_event/__init__.py` (0 lines)
- `addons/website_mass_mailing_event/__manifest__.py` (19 lines)
- `addons/website_mass_mailing_event/i18n/ar.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/az.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/bg.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/bs.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/ca.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/cs.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/da.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/de.po` (70 lines)
- `addons/website_mass_mailing_event/i18n/el.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/es.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/es_419.po` (65 lines)
- `addons/website_mass_mailing_event/i18n/et.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/fa.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/fi.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/fr.po` (65 lines)
- `addons/website_mass_mailing_event/i18n/he.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/hi.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/hr.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/hu.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/id.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/it.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/ja.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/kab.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/ko.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/ku.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/lo.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/lt.po` (65 lines)
- `addons/website_mass_mailing_event/i18n/lv.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/mn.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/my.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/nb.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/nl.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/pl.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/pt.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/pt_BR.po` (73 lines)
- `addons/website_mass_mailing_event/i18n/ro.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/ru.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/sk.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/sl.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/sr@latin.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/sv.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/th.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/tr.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/uk.po` (64 lines)
- `addons/website_mass_mailing_event/i18n/uz.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/vi.po` (63 lines)
- `addons/website_mass_mailing_event/i18n/website_mass_mailing_event.pot` (58 lines)
- `addons/website_mass_mailing_event/i18n/zh_CN.po` (69 lines)
- `addons/website_mass_mailing_event/i18n/zh_TW.po` (64 lines)
- `addons/website_mass_mailing_event/static/src/builder/options/event_snapshot_fragments.xml` (126 lines)
- `addons/website_mass_mailing_event/static/src/builder/options/event_snapshot_snippet_info.js` (90 lines)
- `addons/website_mass_mailing_event/static/src/snippets/s_event_snapshot.xml` (67 lines)
- `addons/website_mass_mailing_event/static/src/snippets/snippet_categories.xml` (9 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
