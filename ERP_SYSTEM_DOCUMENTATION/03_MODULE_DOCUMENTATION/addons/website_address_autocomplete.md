# Module: website_address_autocomplete

- **Module ID:** MOD-597
- **Path:** `addons/website_address_autocomplete`
- **Manifest:** `addons/website_address_autocomplete/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Assist your users with automatic completion & suggestions when filling their address

Assist your users with automatic completion & suggestions when filling their address

Declared dependencies: `website`, `google_address_autocomplete`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "google_address_autocomplete"
  ],
  "data": [
    "views/templates.xml",
    "views/res_config_settings_views.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "google_address_autocomplete/static/src/google_places_session.js",
      "website_address_autocomplete/static/src/interactions/address_form.js",
      "website_address_autocomplete/static/src/xml/autocomplete.xml"
    ],
    "web.assets_tests": [
      "website_address_autocomplete/static/tests/**/*.js"
    ]
  }
}
```

### Representative source files

- `addons/website_address_autocomplete/__init__.py` (4 lines)
- `addons/website_address_autocomplete/__manifest__.py` (29 lines)
- `addons/website_address_autocomplete/controllers/__init__.py` (3 lines)
- `addons/website_address_autocomplete/controllers/main.py` (9 lines)
- `addons/website_address_autocomplete/data/neutralize.sql` (3 lines)
- `addons/website_address_autocomplete/i18n/ar.po` (95 lines)
- `addons/website_address_autocomplete/i18n/az.po` (89 lines)
- `addons/website_address_autocomplete/i18n/bg.po` (89 lines)
- `addons/website_address_autocomplete/i18n/bs.po` (91 lines)
- `addons/website_address_autocomplete/i18n/ca.po` (94 lines)
- `addons/website_address_autocomplete/i18n/cs.po` (90 lines)
- `addons/website_address_autocomplete/i18n/da.po` (95 lines)
- `addons/website_address_autocomplete/i18n/de.po` (99 lines)
- `addons/website_address_autocomplete/i18n/el.po` (96 lines)
- `addons/website_address_autocomplete/i18n/es.po` (95 lines)
- `addons/website_address_autocomplete/i18n/es_419.po` (95 lines)
- `addons/website_address_autocomplete/i18n/et.po` (89 lines)
- `addons/website_address_autocomplete/i18n/fa.po` (89 lines)
- `addons/website_address_autocomplete/i18n/fi.po` (94 lines)
- `addons/website_address_autocomplete/i18n/fr.po` (94 lines)
- `addons/website_address_autocomplete/i18n/he.po` (90 lines)
- `addons/website_address_autocomplete/i18n/hi.po` (89 lines)
- `addons/website_address_autocomplete/i18n/hr.po` (90 lines)
- `addons/website_address_autocomplete/i18n/hu.po` (94 lines)
- `addons/website_address_autocomplete/i18n/id.po` (94 lines)
- `addons/website_address_autocomplete/i18n/it.po` (97 lines)
- `addons/website_address_autocomplete/i18n/ja.po` (95 lines)
- `addons/website_address_autocomplete/i18n/kab.po` (90 lines)
- `addons/website_address_autocomplete/i18n/ko.po` (94 lines)
- `addons/website_address_autocomplete/i18n/ku.po` (89 lines)
- `addons/website_address_autocomplete/i18n/lo.po` (89 lines)
- `addons/website_address_autocomplete/i18n/lt.po` (91 lines)
- `addons/website_address_autocomplete/i18n/lv.po` (90 lines)
- `addons/website_address_autocomplete/i18n/mn.po` (89 lines)
- `addons/website_address_autocomplete/i18n/my.po` (89 lines)
- `addons/website_address_autocomplete/i18n/nb.po` (90 lines)
- `addons/website_address_autocomplete/i18n/nl.po` (94 lines)
- `addons/website_address_autocomplete/i18n/pl.po` (96 lines)
- `addons/website_address_autocomplete/i18n/pt.po` (97 lines)
- `addons/website_address_autocomplete/i18n/pt_BR.po` (99 lines)
- `addons/website_address_autocomplete/i18n/ro.po` (95 lines)
- `addons/website_address_autocomplete/i18n/ru.po` (97 lines)
- `addons/website_address_autocomplete/i18n/sk.po` (89 lines)
- `addons/website_address_autocomplete/i18n/sl.po` (91 lines)
- `addons/website_address_autocomplete/i18n/sr@latin.po` (90 lines)
- `addons/website_address_autocomplete/i18n/sv.po` (95 lines)
- `addons/website_address_autocomplete/i18n/th.po` (94 lines)
- `addons/website_address_autocomplete/i18n/tr.po` (99 lines)
- `addons/website_address_autocomplete/i18n/uk.po` (90 lines)
- `addons/website_address_autocomplete/i18n/uz.po` (105 lines)
- `addons/website_address_autocomplete/i18n/vi.po` (96 lines)
- `addons/website_address_autocomplete/i18n/website_address_autocomplete.pot` (86 lines)
- `addons/website_address_autocomplete/i18n/zh_CN.po` (95 lines)
- `addons/website_address_autocomplete/i18n/zh_TW.po` (98 lines)
- `addons/website_address_autocomplete/models/__init__.py` (4 lines)
- `addons/website_address_autocomplete/models/res_config_settings.py` (10 lines)
- `addons/website_address_autocomplete/models/website.py` (14 lines)
- `addons/website_address_autocomplete/static/src/interactions/address_form.js` (115 lines)
- `addons/website_address_autocomplete/static/src/xml/autocomplete.xml` (14 lines)
- `addons/website_address_autocomplete/static/tests/autocomplete_tour.js` (42 lines)
- `addons/website_address_autocomplete/tests/__init__.py` (3 lines)
- `addons/website_address_autocomplete/tests/test_ui.py` (48 lines)
- `addons/website_address_autocomplete/views/res_config_settings_views.xml` (31 lines)
- `addons/website_address_autocomplete/views/templates.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
