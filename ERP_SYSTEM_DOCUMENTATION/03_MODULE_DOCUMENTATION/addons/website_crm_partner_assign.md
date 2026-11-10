# Module: website_crm_partner_assign

- **Module ID:** MOD-603
- **Path:** `addons/website_crm_partner_assign`
- **Manifest:** `addons/website_crm_partner_assign/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Publish your resellers/partners and forward leads to them


This module allows to forward incoming leads/opportunities to your resellers/partners.

Forwarding leads can be done for one or several leads at a time. The action is available in the *Assigned Partner* section of the lead/opportunity form view and in the *Action* menu of the list view.

The automatic assignment is figured from the weight of partner levels and the geolocalization. Partners get leads that are located around them.

    

Declared dependencies: `base_geolocalize`, `crm`, `account`, `website_partnership`, `website_partner`, `website_google_map`, `portal`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 17 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 5 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base_geolocalize",
    "crm",
    "account",
    "website_partnership",
    "website_partner",
    "website_google_map",
    "portal"
  ],
  "data": [
    "data/crm_lead_merge_template.xml",
    "data/crm_tag_data.xml",
    "data/mail_template_data.xml",
    "data/res_partner_activation_data.xml",
    "data/portal_entry_data.xml",
    "wizard/crm_forward_to_partner_view.xml",
    "views/res_partner_views.xml",
    "views/website_page_views.xml",
    "views/res_partner_activation_views.xml",
    "views/res_partner_grade_views.xml",
    "views/crm_lead_views.xml",
    "views/website_crm_partner_assign_templates.xml",
    "views/partner_assign_menus.xml",
    "report/crm_partner_report_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_partner_demo.xml",
    "data/crm_lead_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_crm_partner_assign/static/src/interactions/**/*"
    ],
    "website.website_builder_assets": [
      "website_crm_partner_assign/static/src/website_builder/**/*"
    ],
    "html_builder.assets_inside_builder_iframe": [
      "website_crm_partner_assign/static/src/scss/crm_partner_assign.scss"
    ]
  }
}
```

### Representative source files

- `addons/website_crm_partner_assign/__init__.py` (7 lines)
- `addons/website_crm_partner_assign/__manifest__.py` (52 lines)
- `addons/website_crm_partner_assign/controllers/__init__.py` (4 lines)
- `addons/website_crm_partner_assign/controllers/main.py` (355 lines)
- `addons/website_crm_partner_assign/data/crm_lead_demo.xml` (33 lines)
- `addons/website_crm_partner_assign/data/crm_lead_merge_template.xml` (27 lines)
- `addons/website_crm_partner_assign/data/crm_tag_data.xml` (17 lines)
- `addons/website_crm_partner_assign/data/mail_template_data.xml` (42 lines)
- `addons/website_crm_partner_assign/data/portal_entry_data.xml` (22 lines)
- `addons/website_crm_partner_assign/data/res_partner_activation_data.xml` (15 lines)
- `addons/website_crm_partner_assign/data/res_partner_demo.xml` (43 lines)
- `addons/website_crm_partner_assign/i18n/af.po` (1,301 lines)
- `addons/website_crm_partner_assign/i18n/am.po` (1,297 lines)
- `addons/website_crm_partner_assign/i18n/ar.po` (1,334 lines)
- `addons/website_crm_partner_assign/i18n/az.po` (1,304 lines)
- `addons/website_crm_partner_assign/i18n/bg.po` (1,320 lines)
- `addons/website_crm_partner_assign/i18n/bs.po` (1,311 lines)
- `addons/website_crm_partner_assign/i18n/ca.po` (1,434 lines)
- `addons/website_crm_partner_assign/i18n/cs.po` (1,335 lines)
- `addons/website_crm_partner_assign/i18n/da.po` (1,338 lines)
- `addons/website_crm_partner_assign/i18n/de.po` (1,455 lines)
- `addons/website_crm_partner_assign/i18n/el.po` (1,319 lines)
- `addons/website_crm_partner_assign/i18n/es.po` (1,436 lines)
- `addons/website_crm_partner_assign/i18n/es_419.po` (1,444 lines)
- `addons/website_crm_partner_assign/i18n/es_CL.po` (41 lines)
- `addons/website_crm_partner_assign/i18n/et.po` (1,349 lines)
- `addons/website_crm_partner_assign/i18n/eu.po` (1,310 lines)
- `addons/website_crm_partner_assign/i18n/fa.po` (1,318 lines)
- `addons/website_crm_partner_assign/i18n/fi.po` (1,458 lines)
- `addons/website_crm_partner_assign/i18n/fr.po` (1,435 lines)
- `addons/website_crm_partner_assign/i18n/fr_BE.po` (47 lines)
- `addons/website_crm_partner_assign/i18n/fr_CA.po` (36 lines)
- `addons/website_crm_partner_assign/i18n/gl.po` (1,310 lines)
- `addons/website_crm_partner_assign/i18n/gu.po` (1,301 lines)
- `addons/website_crm_partner_assign/i18n/he.po` (1,340 lines)
- `addons/website_crm_partner_assign/i18n/hi.po` (1,306 lines)
- `addons/website_crm_partner_assign/i18n/hr.po` (1,323 lines)
- `addons/website_crm_partner_assign/i18n/hu.po` (1,315 lines)
- `addons/website_crm_partner_assign/i18n/hy.po` (1,299 lines)
- `addons/website_crm_partner_assign/i18n/id.po` (1,433 lines)
- `addons/website_crm_partner_assign/i18n/is.po` (1,297 lines)
- `addons/website_crm_partner_assign/i18n/it.po` (1,444 lines)
- `addons/website_crm_partner_assign/i18n/ja.po` (1,432 lines)
- `addons/website_crm_partner_assign/i18n/ka.po` (1,299 lines)
- `addons/website_crm_partner_assign/i18n/kab.po` (1,308 lines)
- `addons/website_crm_partner_assign/i18n/kk.po` (1,310 lines)
- `addons/website_crm_partner_assign/i18n/km.po` (1,302 lines)
- `addons/website_crm_partner_assign/i18n/ko.po` (1,427 lines)
- `addons/website_crm_partner_assign/i18n/ku.po` (1,304 lines)
- `addons/website_crm_partner_assign/i18n/lo.po` (1,423 lines)
- `addons/website_crm_partner_assign/i18n/lt.po` (1,340 lines)
- `addons/website_crm_partner_assign/i18n/lv.po` (1,308 lines)
- `addons/website_crm_partner_assign/i18n/mk.po` (1,313 lines)
- `addons/website_crm_partner_assign/i18n/mn.po` (1,322 lines)
- `addons/website_crm_partner_assign/i18n/my.po` (1,303 lines)
- `addons/website_crm_partner_assign/i18n/nb.po` (1,319 lines)
- `addons/website_crm_partner_assign/i18n/nl.po` (1,437 lines)
- `addons/website_crm_partner_assign/i18n/pl.po` (1,440 lines)
- `addons/website_crm_partner_assign/i18n/pt.po` (1,428 lines)
- `addons/website_crm_partner_assign/i18n/pt_BR.po` (1,449 lines)
- `addons/website_crm_partner_assign/i18n/ro.po` (1,341 lines)
- `addons/website_crm_partner_assign/i18n/ru.po` (1,446 lines)
- `addons/website_crm_partner_assign/i18n/sk.po` (1,328 lines)
- `addons/website_crm_partner_assign/i18n/sl.po` (1,319 lines)
- `addons/website_crm_partner_assign/i18n/sq.po` (1,310 lines)
- `addons/website_crm_partner_assign/i18n/sr@latin.po` (1,311 lines)
- `addons/website_crm_partner_assign/i18n/sv.po` (1,346 lines)
- `addons/website_crm_partner_assign/i18n/ta.po` (1,310 lines)
- `addons/website_crm_partner_assign/i18n/th.po` (1,418 lines)
- `addons/website_crm_partner_assign/i18n/tr.po` (1,355 lines)
- `addons/website_crm_partner_assign/i18n/uk.po` (1,328 lines)
- `addons/website_crm_partner_assign/i18n/uz.po` (1,524 lines)
- `addons/website_crm_partner_assign/i18n/vi.po` (1,336 lines)
- `addons/website_crm_partner_assign/i18n/website_crm_partner_assign.pot` (1,268 lines)
- `addons/website_crm_partner_assign/i18n/zh_CN.po` (1,428 lines)
- `addons/website_crm_partner_assign/i18n/zh_TW.po` (1,420 lines)
- `addons/website_crm_partner_assign/models/__init__.py` (9 lines)
- `addons/website_crm_partner_assign/models/crm_lead.py` (368 lines)
- `addons/website_crm_partner_assign/models/portal_entry.py` (15 lines)
- `addons/website_crm_partner_assign/models/res_partner.py` (102 lines)
- `addons/website_crm_partner_assign/models/res_partner_activation.py` (14 lines)
- `addons/website_crm_partner_assign/models/res_partner_grade.py` (12 lines)
- `addons/website_crm_partner_assign/models/website.py` (13 lines)
- `addons/website_crm_partner_assign/report/__init__.py` (4 lines)
- `addons/website_crm_partner_assign/report/crm_partner_report.py` (60 lines)
- `addons/website_crm_partner_assign/report/crm_partner_report_view.xml` (60 lines)
- `addons/website_crm_partner_assign/security/ir.access.csv` (11 lines)
- `addons/website_crm_partner_assign/static/description/icon.png` (27 lines)
- `addons/website_crm_partner_assign/static/description/icon.svg` (1 lines)
- `addons/website_crm_partner_assign/static/description/icon_hi.png` (84 lines)
- `addons/website_crm_partner_assign/static/src/img/leads.svg` (10 lines)
- `addons/website_crm_partner_assign/static/src/img/quotation.svg` (19 lines)
- `addons/website_crm_partner_assign/static/src/interactions/crm_partner_assign.js` (163 lines)
- `addons/website_crm_partner_assign/static/src/scss/crm_partner_assign.scss` (7 lines)
- `addons/website_crm_partner_assign/static/src/website_builder/website_crm_partner_assign_option.js` (24 lines)
- `addons/website_crm_partner_assign/static/src/website_builder/website_crm_partner_assign_option.xml` (26 lines)
- `addons/website_crm_partner_assign/tests/__init__.py` (6 lines)
- `addons/website_crm_partner_assign/tests/test_partner_assign.py` (480 lines)
- `addons/website_crm_partner_assign/tests/test_res_partner.py` (39 lines)
- `addons/website_crm_partner_assign/tests/test_website_crm_partner_technical_page.py` (9 lines)
- `addons/website_crm_partner_assign/views/crm_lead_views.xml` (184 lines)
- `addons/website_crm_partner_assign/views/partner_assign_menus.xml` (9 lines)
- `addons/website_crm_partner_assign/views/res_partner_activation_views.xml` (52 lines)
- `addons/website_crm_partner_assign/views/res_partner_grade_views.xml` (16 lines)
- `addons/website_crm_partner_assign/views/res_partner_views.xml` (42 lines)
- `addons/website_crm_partner_assign/views/website_crm_partner_assign_templates.xml` (830 lines)
- `addons/website_crm_partner_assign/views/website_page_views.xml` (68 lines)
- `addons/website_crm_partner_assign/wizard/__init__.py` (4 lines)
- `addons/website_crm_partner_assign/wizard/crm_forward_to_partner.py` (166 lines)
- `addons/website_crm_partner_assign/wizard/crm_forward_to_partner_view.xml` (58 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
