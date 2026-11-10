# Module: partner_autocomplete

- **Module ID:** MOD-390
- **Path:** `addons/partner_autocomplete`
- **Manifest:** `addons/partner_autocomplete/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Auto-complete partner companies' data


Auto-complete partner companies' data
    

Declared dependencies: `iap_mail`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 8 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "iap_mail"
  ],
  "data": [
    "views/res_company_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "data/iap_service_data.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "partner_autocomplete/static/src/scss/*",
      "partner_autocomplete/static/src/js/*",
      "partner_autocomplete/static/src/xml/*"
    ],
    "web.jsvat_lib": [
      "partner_autocomplete/static/lib/**/*"
    ],
    "web.assets_unit_tests": [
      "partner_autocomplete/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/partner_autocomplete/__init__.py` (4 lines)
- `addons/partner_autocomplete/__manifest__.py` (38 lines)
- `addons/partner_autocomplete/data/iap_service_data.xml` (12 lines)
- `addons/partner_autocomplete/i18n/af.po` (162 lines)
- `addons/partner_autocomplete/i18n/ar.po` (191 lines)
- `addons/partner_autocomplete/i18n/az.po` (189 lines)
- `addons/partner_autocomplete/i18n/bg.po` (190 lines)
- `addons/partner_autocomplete/i18n/bs.po` (190 lines)
- `addons/partner_autocomplete/i18n/ca.po` (194 lines)
- `addons/partner_autocomplete/i18n/cs.po` (192 lines)
- `addons/partner_autocomplete/i18n/da.po` (190 lines)
- `addons/partner_autocomplete/i18n/de.po` (198 lines)
- `addons/partner_autocomplete/i18n/el.po` (188 lines)
- `addons/partner_autocomplete/i18n/es.po` (193 lines)
- `addons/partner_autocomplete/i18n/es_419.po` (189 lines)
- `addons/partner_autocomplete/i18n/et.po` (193 lines)
- `addons/partner_autocomplete/i18n/fa.po` (191 lines)
- `addons/partner_autocomplete/i18n/fi.po` (195 lines)
- `addons/partner_autocomplete/i18n/fr.po` (195 lines)
- `addons/partner_autocomplete/i18n/gu.po` (162 lines)
- `addons/partner_autocomplete/i18n/he.po` (194 lines)
- `addons/partner_autocomplete/i18n/hi.po` (185 lines)
- `addons/partner_autocomplete/i18n/hr.po` (192 lines)
- `addons/partner_autocomplete/i18n/hu.po` (194 lines)
- `addons/partner_autocomplete/i18n/id.po` (191 lines)
- `addons/partner_autocomplete/i18n/is.po` (158 lines)
- `addons/partner_autocomplete/i18n/it.po` (192 lines)
- `addons/partner_autocomplete/i18n/ja.po` (190 lines)
- `addons/partner_autocomplete/i18n/kab.po` (185 lines)
- `addons/partner_autocomplete/i18n/km.po` (161 lines)
- `addons/partner_autocomplete/i18n/ko.po` (190 lines)
- `addons/partner_autocomplete/i18n/ku.po` (185 lines)
- `addons/partner_autocomplete/i18n/lo.po` (188 lines)
- `addons/partner_autocomplete/i18n/lt.po` (195 lines)
- `addons/partner_autocomplete/i18n/lv.po` (192 lines)
- `addons/partner_autocomplete/i18n/mn.po` (190 lines)
- `addons/partner_autocomplete/i18n/my.po` (186 lines)
- `addons/partner_autocomplete/i18n/nb.po` (189 lines)
- `addons/partner_autocomplete/i18n/nl.po` (195 lines)
- `addons/partner_autocomplete/i18n/partner_autocomplete.pot` (183 lines)
- `addons/partner_autocomplete/i18n/pl.po` (201 lines)
- `addons/partner_autocomplete/i18n/pt.po` (193 lines)
- `addons/partner_autocomplete/i18n/pt_BR.po` (200 lines)
- `addons/partner_autocomplete/i18n/ro.po` (194 lines)
- `addons/partner_autocomplete/i18n/ru.po` (190 lines)
- `addons/partner_autocomplete/i18n/sk.po` (190 lines)
- `addons/partner_autocomplete/i18n/sl.po` (195 lines)
- `addons/partner_autocomplete/i18n/sr@latin.po` (191 lines)
- `addons/partner_autocomplete/i18n/sv.po` (196 lines)
- `addons/partner_autocomplete/i18n/th.po` (191 lines)
- `addons/partner_autocomplete/i18n/tr.po` (197 lines)
- `addons/partner_autocomplete/i18n/uk.po` (192 lines)
- `addons/partner_autocomplete/i18n/uz.po` (212 lines)
- `addons/partner_autocomplete/i18n/vi.po` (192 lines)
- `addons/partner_autocomplete/i18n/zh_CN.po` (193 lines)
- `addons/partner_autocomplete/i18n/zh_TW.po` (189 lines)
- `addons/partner_autocomplete/models/__init__.py` (8 lines)
- `addons/partner_autocomplete/models/iap_autocomplete_api.py` (55 lines)
- `addons/partner_autocomplete/models/ir_http.py` (15 lines)
- `addons/partner_autocomplete/models/res_company.py` (76 lines)
- `addons/partner_autocomplete/models/res_config_settings.py` (21 lines)
- `addons/partner_autocomplete/models/res_partner.py` (380 lines)
- `addons/partner_autocomplete/static/description/icon.png` (5 lines)
- `addons/partner_autocomplete/static/description/icon.svg` (1 lines)
- `addons/partner_autocomplete/static/description/icon_hi.png` (17 lines)
- `addons/partner_autocomplete/static/lib/jsvat.js` (1,328 lines)
- `addons/partner_autocomplete/static/src/js/partner_autocomplete_additional_identifiers_list.js` (123 lines)
- `addons/partner_autocomplete/static/src/js/partner_autocomplete_component.js` (27 lines)
- `addons/partner_autocomplete/static/src/js/partner_autocomplete_core.js` (227 lines)
- `addons/partner_autocomplete/static/src/js/partner_autocomplete_fieldchar.js` (100 lines)
- `addons/partner_autocomplete/static/src/js/partner_autocomplete_many2one.js` (122 lines)
- `addons/partner_autocomplete/static/src/js/web_company_autocomplete.js` (17 lines)
- `addons/partner_autocomplete/static/src/scss/partner_autocomplete.scss` (10 lines)
- `addons/partner_autocomplete/static/src/xml/partner_autocomplete.xml` (103 lines)
- `addons/partner_autocomplete/static/tests/partner_autocomplete.test.js` (346 lines)
- `addons/partner_autocomplete/tests/__init__.py` (5 lines)
- `addons/partner_autocomplete/tests/common.py` (71 lines)
- `addons/partner_autocomplete/tests/test_autocomplete_address_extended.py` (129 lines)
- `addons/partner_autocomplete/tests/test_res_company.py` (132 lines)
- `addons/partner_autocomplete/views/res_company_views.xml` (16 lines)
- `addons/partner_autocomplete/views/res_config_settings_views.xml` (13 lines)
- `addons/partner_autocomplete/views/res_partner_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
