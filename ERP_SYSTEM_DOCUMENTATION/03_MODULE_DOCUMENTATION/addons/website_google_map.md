# Module: website_google_map

- **Module ID:** MOD-619
- **Path:** `addons/website_google_map`
- **Manifest:** `addons/website_google_map/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Show your company address on Google Maps


Show your company address/partner address on Google Maps. Configure an API key in the Website settings.
    

Declared dependencies: `base_geolocalize`, `website_partner`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_geolocalize",
    "website_partner"
  ],
  "data": [
    "views/google_map_templates.xml"
  ]
}
```

### Representative source files

- `addons/website_google_map/__init__.py` (3 lines)
- `addons/website_google_map/__manifest__.py` (15 lines)
- `addons/website_google_map/controllers/__init__.py` (4 lines)
- `addons/website_google_map/controllers/main.py` (74 lines)
- `addons/website_google_map/i18n/ar.po` (33 lines)
- `addons/website_google_map/i18n/az.po` (33 lines)
- `addons/website_google_map/i18n/bg.po` (33 lines)
- `addons/website_google_map/i18n/bs.po` (33 lines)
- `addons/website_google_map/i18n/ca.po` (33 lines)
- `addons/website_google_map/i18n/cs.po` (33 lines)
- `addons/website_google_map/i18n/da.po` (33 lines)
- `addons/website_google_map/i18n/de.po` (40 lines)
- `addons/website_google_map/i18n/el.po` (33 lines)
- `addons/website_google_map/i18n/es.po` (40 lines)
- `addons/website_google_map/i18n/es_419.po` (33 lines)
- `addons/website_google_map/i18n/et.po` (33 lines)
- `addons/website_google_map/i18n/fa.po` (33 lines)
- `addons/website_google_map/i18n/fi.po` (33 lines)
- `addons/website_google_map/i18n/fr.po` (33 lines)
- `addons/website_google_map/i18n/he.po` (33 lines)
- `addons/website_google_map/i18n/hi.po` (33 lines)
- `addons/website_google_map/i18n/hr.po` (33 lines)
- `addons/website_google_map/i18n/hu.po` (33 lines)
- `addons/website_google_map/i18n/id.po` (33 lines)
- `addons/website_google_map/i18n/it.po` (33 lines)
- `addons/website_google_map/i18n/ja.po` (33 lines)
- `addons/website_google_map/i18n/kab.po` (33 lines)
- `addons/website_google_map/i18n/ko.po` (33 lines)
- `addons/website_google_map/i18n/ku.po` (33 lines)
- `addons/website_google_map/i18n/lo.po` (33 lines)
- `addons/website_google_map/i18n/lt.po` (33 lines)
- `addons/website_google_map/i18n/lv.po` (33 lines)
- `addons/website_google_map/i18n/mn.po` (33 lines)
- `addons/website_google_map/i18n/my.po` (33 lines)
- `addons/website_google_map/i18n/nb.po` (33 lines)
- `addons/website_google_map/i18n/nl.po` (33 lines)
- `addons/website_google_map/i18n/pl.po` (38 lines)
- `addons/website_google_map/i18n/pt.po` (33 lines)
- `addons/website_google_map/i18n/pt_BR.po` (41 lines)
- `addons/website_google_map/i18n/ro.po` (33 lines)
- `addons/website_google_map/i18n/ru.po` (33 lines)
- `addons/website_google_map/i18n/sk.po` (33 lines)
- `addons/website_google_map/i18n/sl.po` (33 lines)
- `addons/website_google_map/i18n/sr@latin.po` (33 lines)
- `addons/website_google_map/i18n/sv.po` (33 lines)
- `addons/website_google_map/i18n/th.po` (33 lines)
- `addons/website_google_map/i18n/tr.po` (33 lines)
- `addons/website_google_map/i18n/uk.po` (33 lines)
- `addons/website_google_map/i18n/uz.po` (33 lines)
- `addons/website_google_map/i18n/vi.po` (33 lines)
- `addons/website_google_map/i18n/website_google_map.pot` (33 lines)
- `addons/website_google_map/i18n/zh_CN.po` (33 lines)
- `addons/website_google_map/i18n/zh_TW.po` (33 lines)
- `addons/website_google_map/static/description/icon.png` (14 lines)
- `addons/website_google_map/static/description/icon.svg` (1 lines)
- `addons/website_google_map/static/description/icon_hi.png` (110 lines)
- `addons/website_google_map/static/src/css/website_google_map.css` (28 lines)
- `addons/website_google_map/static/src/img/partners.png` (9 lines)
- `addons/website_google_map/static/src/js/website_google_map.js` (122 lines)
- `addons/website_google_map/static/src/lib/images/conv30.png` (8 lines)
- `addons/website_google_map/static/src/lib/images/conv40.png` (10 lines)
- `addons/website_google_map/static/src/lib/images/conv50.png` (14 lines)
- `addons/website_google_map/static/src/lib/images/heart30.png` (11 lines)
- `addons/website_google_map/static/src/lib/images/heart40.png` (13 lines)
- `addons/website_google_map/static/src/lib/images/heart50.png` (14 lines)
- `addons/website_google_map/static/src/lib/images/m1.png` (28 lines)
- `addons/website_google_map/static/src/lib/images/m2.png` (30 lines)
- `addons/website_google_map/static/src/lib/images/m3.png` (34 lines)
- `addons/website_google_map/static/src/lib/images/m4.png` (63 lines)
- `addons/website_google_map/static/src/lib/images/m5.png` (63 lines)
- `addons/website_google_map/static/src/lib/images/people35.png` (11 lines)
- `addons/website_google_map/static/src/lib/images/people45.png` (22 lines)
- `addons/website_google_map/static/src/lib/images/people55.png` (25 lines)
- `addons/website_google_map/static/src/lib/images/pin.png` (8 lines)
- `addons/website_google_map/static/src/lib/markerclusterer.js` (1,317 lines)
- `addons/website_google_map/views/google_map_templates.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
