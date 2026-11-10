# Module: base_geolocalize

- **Module ID:** MOD-036
- **Path:** `addons/base_geolocalize`
- **Manifest:** `addons/base_geolocalize/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Partners Geolocation
========================
    

Declared dependencies: `base_setup`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_setup"
  ],
  "data": [
    "views/geo_provider_view.xml",
    "views/res_partner_views.xml",
    "views/res_config_settings_views.xml",
    "data/data.xml",
    "data/ir_cron.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/base_geolocalize/README.md` (13 lines)
- `addons/base_geolocalize/__init__.py` (3 lines)
- `addons/base_geolocalize/__manifest__.py` (21 lines)
- `addons/base_geolocalize/data/data.xml` (12 lines)
- `addons/base_geolocalize/data/ir_cron.xml` (14 lines)
- `addons/base_geolocalize/i18n/af.po` (226 lines)
- `addons/base_geolocalize/i18n/ar.po` (262 lines)
- `addons/base_geolocalize/i18n/az.po` (247 lines)
- `addons/base_geolocalize/i18n/base_geolocalize.pot` (240 lines)
- `addons/base_geolocalize/i18n/bg.po` (251 lines)
- `addons/base_geolocalize/i18n/bs.po` (249 lines)
- `addons/base_geolocalize/i18n/ca.po` (267 lines)
- `addons/base_geolocalize/i18n/cs.po` (267 lines)
- `addons/base_geolocalize/i18n/da.po` (261 lines)
- `addons/base_geolocalize/i18n/de.po` (267 lines)
- `addons/base_geolocalize/i18n/el.po` (250 lines)
- `addons/base_geolocalize/i18n/es.po` (267 lines)
- `addons/base_geolocalize/i18n/es_419.po` (264 lines)
- `addons/base_geolocalize/i18n/et.po` (267 lines)
- `addons/base_geolocalize/i18n/fa.po` (263 lines)
- `addons/base_geolocalize/i18n/fi.po` (267 lines)
- `addons/base_geolocalize/i18n/fr.po` (270 lines)
- `addons/base_geolocalize/i18n/gu.po` (226 lines)
- `addons/base_geolocalize/i18n/he.po` (266 lines)
- `addons/base_geolocalize/i18n/hi.po` (245 lines)
- `addons/base_geolocalize/i18n/hr.po` (250 lines)
- `addons/base_geolocalize/i18n/hu.po` (265 lines)
- `addons/base_geolocalize/i18n/id.po` (261 lines)
- `addons/base_geolocalize/i18n/is.po` (222 lines)
- `addons/base_geolocalize/i18n/it.po` (268 lines)
- `addons/base_geolocalize/i18n/ja.po` (266 lines)
- `addons/base_geolocalize/i18n/kab.po` (245 lines)
- `addons/base_geolocalize/i18n/km.po` (225 lines)
- `addons/base_geolocalize/i18n/ko.po` (260 lines)
- `addons/base_geolocalize/i18n/ku.po` (245 lines)
- `addons/base_geolocalize/i18n/lo.po` (261 lines)
- `addons/base_geolocalize/i18n/lt.po` (256 lines)
- `addons/base_geolocalize/i18n/lv.po` (250 lines)
- `addons/base_geolocalize/i18n/mn.po` (248 lines)
- `addons/base_geolocalize/i18n/my.po` (246 lines)
- `addons/base_geolocalize/i18n/nb.po` (248 lines)
- `addons/base_geolocalize/i18n/nl.po` (263 lines)
- `addons/base_geolocalize/i18n/pl.po` (272 lines)
- `addons/base_geolocalize/i18n/pt.po` (266 lines)
- `addons/base_geolocalize/i18n/pt_BR.po` (269 lines)
- `addons/base_geolocalize/i18n/ro.po` (265 lines)
- `addons/base_geolocalize/i18n/ru.po` (262 lines)
- `addons/base_geolocalize/i18n/sk.po` (261 lines)
- `addons/base_geolocalize/i18n/sl.po` (267 lines)
- `addons/base_geolocalize/i18n/sr@latin.po` (262 lines)
- `addons/base_geolocalize/i18n/sv.po` (265 lines)
- `addons/base_geolocalize/i18n/th.po` (261 lines)
- `addons/base_geolocalize/i18n/tr.po` (271 lines)
- `addons/base_geolocalize/i18n/uk.po` (264 lines)
- `addons/base_geolocalize/i18n/uz.po` (290 lines)
- `addons/base_geolocalize/i18n/vi.po` (261 lines)
- `addons/base_geolocalize/i18n/zh_CN.po` (265 lines)
- `addons/base_geolocalize/i18n/zh_TW.po` (260 lines)
- `addons/base_geolocalize/models/__init__.py` (5 lines)
- `addons/base_geolocalize/models/base_geocoder.py` (266 lines)
- `addons/base_geolocalize/models/res_config_settings.py` (27 lines)
- `addons/base_geolocalize/models/res_partner.py` (86 lines)
- `addons/base_geolocalize/security/ir.access.csv` (2 lines)
- `addons/base_geolocalize/tests/__init__.py` (3 lines)
- `addons/base_geolocalize/tests/test_geolocalize.py` (107 lines)
- `addons/base_geolocalize/views/geo_provider_view.xml` (25 lines)
- `addons/base_geolocalize/views/res_config_settings_views.xml` (21 lines)
- `addons/base_geolocalize/views/res_partner_views.xml` (29 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
