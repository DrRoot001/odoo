# Module: website_crm

- **Module ID:** MOD-600
- **Path:** `addons/website_crm`
- **Manifest:** `addons/website_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Generate leads from a contact form


Add capability to your website forms to generate leads or opportunities in the CRM app.
Forms has to be customized inside the *Website Builder* in order to generate leads.

This module includes contact phone and mobile numbers validation.

Declared dependencies: `website`, `crm`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website",
    "crm"
  ],
  "data": [
    "data/crm_lead_merge_template.xml",
    "data/ir_actions_data.xml",
    "data/ir_model_data.xml",
    "views/crm_lead_views.xml",
    "views/website_visitor_views.xml",
    "views/website_templates_contactus.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_crm/static/src/js/website_crm_editor.js"
    ],
    "website.assets_inside_builder_iframe": [
      "website_crm/static/src/js/*.edit.js"
    ],
    "web.assets_tests": [
      "website_crm/static/tests/**/*"
    ],
    "web.assets_backend": [
      "website_crm/static/src/**/*",
      [
        "remove",
        "website_crm/static/src/js/website_crm_editor.*"
      ]
    ]
  }
}
```

### Representative source files

- `addons/website_crm/README.md` (15 lines)
- `addons/website_crm/__init__.py` (5 lines)
- `addons/website_crm/__manifest__.py` (42 lines)
- `addons/website_crm/controllers/__init__.py` (4 lines)
- `addons/website_crm/controllers/website_form.py` (91 lines)
- `addons/website_crm/data/crm_lead_merge_template.xml` (16 lines)
- `addons/website_crm/data/ir_actions_data.xml` (15 lines)
- `addons/website_crm/data/ir_model_data.xml` (26 lines)
- `addons/website_crm/i18n/af.po` (204 lines)
- `addons/website_crm/i18n/ar.po` (213 lines)
- `addons/website_crm/i18n/az.po` (211 lines)
- `addons/website_crm/i18n/bg.po` (210 lines)
- `addons/website_crm/i18n/bs.po` (207 lines)
- `addons/website_crm/i18n/ca.po` (217 lines)
- `addons/website_crm/i18n/cs.po` (214 lines)
- `addons/website_crm/i18n/da.po` (208 lines)
- `addons/website_crm/i18n/de.po` (220 lines)
- `addons/website_crm/i18n/el.po` (210 lines)
- `addons/website_crm/i18n/es.po` (221 lines)
- `addons/website_crm/i18n/es_419.po` (209 lines)
- `addons/website_crm/i18n/et.po` (212 lines)
- `addons/website_crm/i18n/fa.po` (210 lines)
- `addons/website_crm/i18n/fi.po` (215 lines)
- `addons/website_crm/i18n/fr.po` (214 lines)
- `addons/website_crm/i18n/gu.po` (204 lines)
- `addons/website_crm/i18n/he.po` (214 lines)
- `addons/website_crm/i18n/hi.po` (204 lines)
- `addons/website_crm/i18n/hr.po` (214 lines)
- `addons/website_crm/i18n/hu.po` (209 lines)
- `addons/website_crm/i18n/id.po` (211 lines)
- `addons/website_crm/i18n/is.po` (200 lines)
- `addons/website_crm/i18n/it.po` (220 lines)
- `addons/website_crm/i18n/ja.po` (209 lines)
- `addons/website_crm/i18n/kab.po` (204 lines)
- `addons/website_crm/i18n/km.po` (204 lines)
- `addons/website_crm/i18n/ko.po` (210 lines)
- `addons/website_crm/i18n/ku.po` (203 lines)
- `addons/website_crm/i18n/lo.po` (211 lines)
- `addons/website_crm/i18n/lt.po` (217 lines)
- `addons/website_crm/i18n/lv.po` (207 lines)
- `addons/website_crm/i18n/mk.po` (203 lines)
- `addons/website_crm/i18n/mn.po` (214 lines)
- `addons/website_crm/i18n/my.po` (204 lines)
- `addons/website_crm/i18n/nb.po` (208 lines)
- `addons/website_crm/i18n/nl.po` (213 lines)
- `addons/website_crm/i18n/pl.po` (220 lines)
- `addons/website_crm/i18n/pt.po` (214 lines)
- `addons/website_crm/i18n/pt_BR.po` (223 lines)
- `addons/website_crm/i18n/ro.po` (216 lines)
- `addons/website_crm/i18n/ru.po` (218 lines)
- `addons/website_crm/i18n/sk.po` (215 lines)
- `addons/website_crm/i18n/sl.po` (213 lines)
- `addons/website_crm/i18n/sr@latin.po` (212 lines)
- `addons/website_crm/i18n/sv.po` (213 lines)
- `addons/website_crm/i18n/th.po` (208 lines)
- `addons/website_crm/i18n/tr.po` (218 lines)
- `addons/website_crm/i18n/uk.po` (213 lines)
- `addons/website_crm/i18n/uz.po` (244 lines)
- `addons/website_crm/i18n/vi.po` (209 lines)
- `addons/website_crm/i18n/website_crm.pot` (198 lines)
- `addons/website_crm/i18n/zh_CN.po` (209 lines)
- `addons/website_crm/i18n/zh_TW.po` (206 lines)
- `addons/website_crm/models/__init__.py` (6 lines)
- `addons/website_crm/models/crm_lead.py` (64 lines)
- `addons/website_crm/models/website.py` (21 lines)
- `addons/website_crm/models/website_visitor.py` (69 lines)
- `addons/website_crm/security/ir.access.csv` (3 lines)
- `addons/website_crm/static/description/icon.png` (13 lines)
- `addons/website_crm/static/description/icon.svg` (1 lines)
- `addons/website_crm/static/description/icon_hi.png` (36 lines)
- `addons/website_crm/static/src/components/lead_generation_dropdown/crm_lead_gen_element.js` (24 lines)
- `addons/website_crm/static/src/js/website_crm_editor.edit.js` (39 lines)
- `addons/website_crm/static/src/js/website_crm_editor.js` (20 lines)
- `addons/website_crm/static/tests/tours/website_crm.js` (151 lines)
- `addons/website_crm/tests/__init__.py` (6 lines)
- `addons/website_crm/tests/test_crm_lead_merge.py` (42 lines)
- `addons/website_crm/tests/test_website_crm.py` (65 lines)
- `addons/website_crm/tests/test_website_visitor.py` (123 lines)
- `addons/website_crm/views/crm_lead_views.xml` (29 lines)
- `addons/website_crm/views/website_templates_contactus.xml` (14 lines)
- `addons/website_crm/views/website_visitor_views.xml` (58 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
