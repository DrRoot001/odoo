# Module: mass_mailing_slides

- **Module ID:** MOD-371
- **Path:** `addons/mass_mailing_slides`
- **Manifest:** `addons/mass_mailing_slides/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Mass mail course members
========================

Bridge module adding UX requirements to ease mass mailing of course members.
        

Declared dependencies: `website_slides`, `mass_mailing`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "website_slides",
    "mass_mailing"
  ],
  "data": [
    "views/slide_channel_views.xml"
  ]
}
```

### Representative source files

- `addons/mass_mailing_slides/__init__.py` (4 lines)
- `addons/mass_mailing_slides/__manifest__.py` (20 lines)
- `addons/mass_mailing_slides/i18n/ar.po` (67 lines)
- `addons/mass_mailing_slides/i18n/az.po` (63 lines)
- `addons/mass_mailing_slides/i18n/bg.po` (63 lines)
- `addons/mass_mailing_slides/i18n/bs.po` (64 lines)
- `addons/mass_mailing_slides/i18n/ca.po` (64 lines)
- `addons/mass_mailing_slides/i18n/cs.po` (67 lines)
- `addons/mass_mailing_slides/i18n/da.po` (68 lines)
- `addons/mass_mailing_slides/i18n/de.po` (74 lines)
- `addons/mass_mailing_slides/i18n/el.po` (64 lines)
- `addons/mass_mailing_slides/i18n/es.po` (74 lines)
- `addons/mass_mailing_slides/i18n/es_419.po` (70 lines)
- `addons/mass_mailing_slides/i18n/et.po` (63 lines)
- `addons/mass_mailing_slides/i18n/fa.po` (63 lines)
- `addons/mass_mailing_slides/i18n/fi.po` (71 lines)
- `addons/mass_mailing_slides/i18n/fr.po` (68 lines)
- `addons/mass_mailing_slides/i18n/he.po` (68 lines)
- `addons/mass_mailing_slides/i18n/hi.po` (63 lines)
- `addons/mass_mailing_slides/i18n/hr.po` (66 lines)
- `addons/mass_mailing_slides/i18n/hu.po` (65 lines)
- `addons/mass_mailing_slides/i18n/id.po` (64 lines)
- `addons/mass_mailing_slides/i18n/it.po` (74 lines)
- `addons/mass_mailing_slides/i18n/ja.po` (64 lines)
- `addons/mass_mailing_slides/i18n/kab.po` (63 lines)
- `addons/mass_mailing_slides/i18n/ko.po` (64 lines)
- `addons/mass_mailing_slides/i18n/ku.po` (63 lines)
- `addons/mass_mailing_slides/i18n/lo.po` (62 lines)
- `addons/mass_mailing_slides/i18n/lt.po` (67 lines)
- `addons/mass_mailing_slides/i18n/lv.po` (63 lines)
- `addons/mass_mailing_slides/i18n/mass_mailing_slides.pot` (58 lines)
- `addons/mass_mailing_slides/i18n/mn.po` (65 lines)
- `addons/mass_mailing_slides/i18n/my.po` (63 lines)
- `addons/mass_mailing_slides/i18n/nb.po` (65 lines)
- `addons/mass_mailing_slides/i18n/nl.po` (67 lines)
- `addons/mass_mailing_slides/i18n/pl.po` (68 lines)
- `addons/mass_mailing_slides/i18n/pt.po` (66 lines)
- `addons/mass_mailing_slides/i18n/pt_BR.po` (75 lines)
- `addons/mass_mailing_slides/i18n/ro.po` (68 lines)
- `addons/mass_mailing_slides/i18n/ru.po` (67 lines)
- `addons/mass_mailing_slides/i18n/sk.po` (62 lines)
- `addons/mass_mailing_slides/i18n/sl.po` (65 lines)
- `addons/mass_mailing_slides/i18n/sr@latin.po` (64 lines)
- `addons/mass_mailing_slides/i18n/sv.po` (65 lines)
- `addons/mass_mailing_slides/i18n/th.po` (64 lines)
- `addons/mass_mailing_slides/i18n/tr.po` (67 lines)
- `addons/mass_mailing_slides/i18n/uk.po` (69 lines)
- `addons/mass_mailing_slides/i18n/uz.po` (75 lines)
- `addons/mass_mailing_slides/i18n/vi.po` (66 lines)
- `addons/mass_mailing_slides/i18n/zh_CN.po` (66 lines)
- `addons/mass_mailing_slides/i18n/zh_TW.po` (66 lines)
- `addons/mass_mailing_slides/models/__init__.py` (4 lines)
- `addons/mass_mailing_slides/models/slide_channel.py` (26 lines)
- `addons/mass_mailing_slides/views/slide_channel_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
