# Module: website_mass_mailing_sms

- **Module ID:** MOD-628
- **Path:** `addons/website_mass_mailing_sms`
- **Manifest:** `addons/website_mass_mailing_sms/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Attract visitors to subscribe to mailing lists


This module adds a new template to the Newsletter Block to allow
your visitors to subscribe with their phone number.
    

Declared dependencies: `website_mass_mailing`, `mass_mailing_sms`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_mass_mailing",
    "mass_mailing_sms"
  ],
  "data": [
    "views/snippets/snippets_templates.xml",
    "data/ir_model_data.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_mass_mailing_sms/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_mass_mailing_sms/__init__.py` (4 lines)
- `addons/website_mass_mailing_sms/__manifest__.py` (24 lines)
- `addons/website_mass_mailing_sms/controllers/__init__.py` (4 lines)
- `addons/website_mass_mailing_sms/controllers/main.py` (23 lines)
- `addons/website_mass_mailing_sms/data/ir_model_data.xml` (11 lines)
- `addons/website_mass_mailing_sms/i18n/ar.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/az.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/bg.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/bs.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/ca.po` (91 lines)
- `addons/website_mass_mailing_sms/i18n/cs.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/da.po` (93 lines)
- `addons/website_mass_mailing_sms/i18n/de.po` (102 lines)
- `addons/website_mass_mailing_sms/i18n/el.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/es.po` (91 lines)
- `addons/website_mass_mailing_sms/i18n/es_419.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/et.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/fa.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/fi.po` (92 lines)
- `addons/website_mass_mailing_sms/i18n/fr.po` (92 lines)
- `addons/website_mass_mailing_sms/i18n/he.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/hi.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/hr.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/hu.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/id.po` (90 lines)
- `addons/website_mass_mailing_sms/i18n/it.po` (93 lines)
- `addons/website_mass_mailing_sms/i18n/ja.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/kab.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/ko.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/ku.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/lo.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/lt.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/lv.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/mn.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/my.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/nb.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/nl.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/pl.po` (93 lines)
- `addons/website_mass_mailing_sms/i18n/pt.po` (90 lines)
- `addons/website_mass_mailing_sms/i18n/pt_BR.po` (106 lines)
- `addons/website_mass_mailing_sms/i18n/ro.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/ru.po` (93 lines)
- `addons/website_mass_mailing_sms/i18n/sk.po` (87 lines)
- `addons/website_mass_mailing_sms/i18n/sl.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/sr@latin.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/sv.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/th.po` (89 lines)
- `addons/website_mass_mailing_sms/i18n/tr.po` (90 lines)
- `addons/website_mass_mailing_sms/i18n/uk.po` (90 lines)
- `addons/website_mass_mailing_sms/i18n/uz.po` (105 lines)
- `addons/website_mass_mailing_sms/i18n/vi.po` (88 lines)
- `addons/website_mass_mailing_sms/i18n/website_mass_mailing_sms.pot` (84 lines)
- `addons/website_mass_mailing_sms/i18n/zh_CN.po` (94 lines)
- `addons/website_mass_mailing_sms/i18n/zh_TW.po` (91 lines)
- `addons/website_mass_mailing_sms/static/shapes/s_newsletter_sms_notifications.svg` (316 lines)
- `addons/website_mass_mailing_sms/static/src/website_builder/newsletter_layout_option.xml` (17 lines)
- `addons/website_mass_mailing_sms/tests/__init__.py` (1 lines)
- `addons/website_mass_mailing_sms/tests/test_website_mass_mailing_sms.py` (51 lines)
- `addons/website_mass_mailing_sms/views/snippets/snippets_templates.xml` (60 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
