# Module: website_partnership

- **Module ID:** MOD-630
- **Path:** `addons/website_partnership`
- **Manifest:** `addons/website_partnership/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Publish your partners on your website


This module allows to publish your members/partners on your website.

To publish a member, set a *Level* in their contact form and click the *Publish* button.
    

Declared dependencies: `partnership`, `website_partner`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "partnership",
    "website_partner"
  ],
  "data": [
    "views/res_partner_grade_views.xml",
    "views/website_partnership_templates.xml",
    "views/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/res_partner_grade_demo.xml",
    "demo/res_partner_demo.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_partnership/static/src/website_builder/**/*"
    ],
    "web.assets_tests": [
      "website_partnership/static/tests/tours/*"
    ]
  }
}
```

### Representative source files

- `addons/website_partnership/__init__.py` (4 lines)
- `addons/website_partnership/__manifest__.py` (33 lines)
- `addons/website_partnership/controllers/__init__.py` (3 lines)
- `addons/website_partnership/controllers/main.py` (120 lines)
- `addons/website_partnership/demo/res_partner_demo.xml` (21 lines)
- `addons/website_partnership/demo/res_partner_grade_demo.xml` (14 lines)
- `addons/website_partnership/i18n/ar.po` (254 lines)
- `addons/website_partnership/i18n/az.po` (253 lines)
- `addons/website_partnership/i18n/bg.po` (253 lines)
- `addons/website_partnership/i18n/bs.po` (254 lines)
- `addons/website_partnership/i18n/ca.po` (253 lines)
- `addons/website_partnership/i18n/cs.po` (253 lines)
- `addons/website_partnership/i18n/da.po` (253 lines)
- `addons/website_partnership/i18n/de.po` (268 lines)
- `addons/website_partnership/i18n/el.po` (253 lines)
- `addons/website_partnership/i18n/es.po` (254 lines)
- `addons/website_partnership/i18n/es_419.po` (259 lines)
- `addons/website_partnership/i18n/et.po` (253 lines)
- `addons/website_partnership/i18n/fa.po` (253 lines)
- `addons/website_partnership/i18n/fi.po` (254 lines)
- `addons/website_partnership/i18n/fr.po` (256 lines)
- `addons/website_partnership/i18n/he.po` (254 lines)
- `addons/website_partnership/i18n/hi.po` (253 lines)
- `addons/website_partnership/i18n/hr.po` (254 lines)
- `addons/website_partnership/i18n/hu.po` (253 lines)
- `addons/website_partnership/i18n/id.po` (256 lines)
- `addons/website_partnership/i18n/it.po` (262 lines)
- `addons/website_partnership/i18n/ja.po` (258 lines)
- `addons/website_partnership/i18n/kab.po` (253 lines)
- `addons/website_partnership/i18n/ko.po` (254 lines)
- `addons/website_partnership/i18n/ku.po` (253 lines)
- `addons/website_partnership/i18n/lo.po` (260 lines)
- `addons/website_partnership/i18n/lt.po` (255 lines)
- `addons/website_partnership/i18n/lv.po` (254 lines)
- `addons/website_partnership/i18n/mn.po` (253 lines)
- `addons/website_partnership/i18n/my.po` (253 lines)
- `addons/website_partnership/i18n/nb.po` (253 lines)
- `addons/website_partnership/i18n/nl.po` (260 lines)
- `addons/website_partnership/i18n/pl.po` (254 lines)
- `addons/website_partnership/i18n/pt.po` (253 lines)
- `addons/website_partnership/i18n/pt_BR.po` (263 lines)
- `addons/website_partnership/i18n/ro.po` (254 lines)
- `addons/website_partnership/i18n/ru.po` (254 lines)
- `addons/website_partnership/i18n/sk.po` (253 lines)
- `addons/website_partnership/i18n/sl.po` (254 lines)
- `addons/website_partnership/i18n/sr@latin.po` (254 lines)
- `addons/website_partnership/i18n/sv.po` (254 lines)
- `addons/website_partnership/i18n/th.po` (254 lines)
- `addons/website_partnership/i18n/tr.po` (253 lines)
- `addons/website_partnership/i18n/uk.po` (254 lines)
- `addons/website_partnership/i18n/uz.po` (253 lines)
- `addons/website_partnership/i18n/vi.po` (253 lines)
- `addons/website_partnership/i18n/website_partnership.pot` (249 lines)
- `addons/website_partnership/i18n/zh_CN.po` (261 lines)
- `addons/website_partnership/i18n/zh_TW.po` (256 lines)
- `addons/website_partnership/models/__init__.py` (4 lines)
- `addons/website_partnership/models/res_partner_grade.py` (16 lines)
- `addons/website_partnership/models/website.py` (12 lines)
- `addons/website_partnership/security/ir.access.csv` (2 lines)
- `addons/website_partnership/static/src/website_builder/partner_page_option.xml` (21 lines)
- `addons/website_partnership/static/src/website_builder/website_partnership_option.xml` (38 lines)
- `addons/website_partnership/static/tests/tours/publish.js` (67 lines)
- `addons/website_partnership/views/res_config_settings_views.xml` (17 lines)
- `addons/website_partnership/views/res_partner_grade_views.xml` (13 lines)
- `addons/website_partnership/views/website_partnership_templates.xml` (233 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
