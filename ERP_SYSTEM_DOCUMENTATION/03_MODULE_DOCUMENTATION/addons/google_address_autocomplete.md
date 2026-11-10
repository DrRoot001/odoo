# Module: google_address_autocomplete

- **Module ID:** MOD-077
- **Path:** `addons/google_address_autocomplete`
- **Manifest:** `addons/google_address_autocomplete/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Assist with automatic completion & suggestions when filling address


This module Auto complete the address data.
    

Declared dependencies: `web`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "web"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "views/res_company_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "google_address_autocomplete/static/src/**/*",
      [
        "remove",
        "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete_dark.scss"
      ]
    ],
    "web.assets_web_dark": [
      "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete_dark.scss"
    ],
    "web._assets_core": [
      "google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.scss"
    ],
    "web.assets_tests": [
      "google_address_autocomplete/static/tests/tours/*.js"
    ],
    "web.assets_unit_tests": [
      "google_address_autocomplete/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/google_address_autocomplete/__init__.py` (4 lines)
- `addons/google_address_autocomplete/__manifest__.py` (36 lines)
- `addons/google_address_autocomplete/controllers/__init__.py` (4 lines)
- `addons/google_address_autocomplete/controllers/google_address_autocomplete.py` (220 lines)
- `addons/google_address_autocomplete/data/neutralize.sql` (4 lines)
- `addons/google_address_autocomplete/i18n/ar.po` (164 lines)
- `addons/google_address_autocomplete/i18n/az.po` (148 lines)
- `addons/google_address_autocomplete/i18n/bg.po` (163 lines)
- `addons/google_address_autocomplete/i18n/bs.po` (149 lines)
- `addons/google_address_autocomplete/i18n/ca.po` (163 lines)
- `addons/google_address_autocomplete/i18n/cs.po` (148 lines)
- `addons/google_address_autocomplete/i18n/da.po` (163 lines)
- `addons/google_address_autocomplete/i18n/de.po` (175 lines)
- `addons/google_address_autocomplete/i18n/el.po` (164 lines)
- `addons/google_address_autocomplete/i18n/es.po` (171 lines)
- `addons/google_address_autocomplete/i18n/es_419.po` (171 lines)
- `addons/google_address_autocomplete/i18n/et.po` (162 lines)
- `addons/google_address_autocomplete/i18n/fa.po` (148 lines)
- `addons/google_address_autocomplete/i18n/fi.po` (165 lines)
- `addons/google_address_autocomplete/i18n/fr.po` (172 lines)
- `addons/google_address_autocomplete/i18n/google_address_autocomplete.pot` (144 lines)
- `addons/google_address_autocomplete/i18n/he.po` (149 lines)
- `addons/google_address_autocomplete/i18n/hi.po` (155 lines)
- `addons/google_address_autocomplete/i18n/hr.po` (163 lines)
- `addons/google_address_autocomplete/i18n/hu.po` (162 lines)
- `addons/google_address_autocomplete/i18n/id.po` (164 lines)
- `addons/google_address_autocomplete/i18n/it.po` (170 lines)
- `addons/google_address_autocomplete/i18n/ja.po` (162 lines)
- `addons/google_address_autocomplete/i18n/kab.po` (148 lines)
- `addons/google_address_autocomplete/i18n/ko.po` (163 lines)
- `addons/google_address_autocomplete/i18n/ku.po` (148 lines)
- `addons/google_address_autocomplete/i18n/lo.po` (154 lines)
- `addons/google_address_autocomplete/i18n/lt.po` (150 lines)
- `addons/google_address_autocomplete/i18n/lv.po` (148 lines)
- `addons/google_address_autocomplete/i18n/mn.po` (148 lines)
- `addons/google_address_autocomplete/i18n/my.po` (148 lines)
- `addons/google_address_autocomplete/i18n/nb.po` (148 lines)
- `addons/google_address_autocomplete/i18n/nl.po` (163 lines)
- `addons/google_address_autocomplete/i18n/pl.po` (163 lines)
- `addons/google_address_autocomplete/i18n/pt.po` (165 lines)
- `addons/google_address_autocomplete/i18n/pt_BR.po` (170 lines)
- `addons/google_address_autocomplete/i18n/ro.po` (163 lines)
- `addons/google_address_autocomplete/i18n/ru.po` (165 lines)
- `addons/google_address_autocomplete/i18n/sk.po` (147 lines)
- `addons/google_address_autocomplete/i18n/sl.po` (149 lines)
- `addons/google_address_autocomplete/i18n/sr@latin.po` (163 lines)
- `addons/google_address_autocomplete/i18n/sv.po` (167 lines)
- `addons/google_address_autocomplete/i18n/th.po` (163 lines)
- `addons/google_address_autocomplete/i18n/tr.po` (166 lines)
- `addons/google_address_autocomplete/i18n/uk.po` (164 lines)
- `addons/google_address_autocomplete/i18n/uz.po` (170 lines)
- `addons/google_address_autocomplete/i18n/vi.po` (164 lines)
- `addons/google_address_autocomplete/i18n/zh_CN.po` (171 lines)
- `addons/google_address_autocomplete/i18n/zh_TW.po` (166 lines)
- `addons/google_address_autocomplete/models/__init__.py` (4 lines)
- `addons/google_address_autocomplete/models/res_config_settings.py` (12 lines)
- `addons/google_address_autocomplete/models/res_partner.py` (15 lines)
- `addons/google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.js` (168 lines)
- `addons/google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.scss` (13 lines)
- `addons/google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete.xml` (23 lines)
- `addons/google_address_autocomplete/static/src/address_autocomplete/google_address_autocomplete_dark.scss` (3 lines)
- `addons/google_address_autocomplete/static/src/google_places_session.js` (50 lines)
- `addons/google_address_autocomplete/static/src/img/powered_by_google_on_non_white.png` (16 lines)
- `addons/google_address_autocomplete/static/src/img/powered_by_google_on_white.png` (23 lines)
- `addons/google_address_autocomplete/static/tests/google_address_autocomplete.test.js` (267 lines)
- `addons/google_address_autocomplete/static/tests/tours/autocomplete_address_tour.js` (56 lines)
- `addons/google_address_autocomplete/tests/__init__.py` (4 lines)
- `addons/google_address_autocomplete/tests/mock_google_places.py` (154 lines)
- `addons/google_address_autocomplete/tests/test_ui.py` (262 lines)
- `addons/google_address_autocomplete/views/res_company_views.xml` (15 lines)
- `addons/google_address_autocomplete/views/res_config_settings_views.xml` (26 lines)
- `addons/google_address_autocomplete/views/res_partner_views.xml` (24 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
