# Module: website_customer

- **Module ID:** MOD-605
- **Path:** `addons/website_customer`
- **Manifest:** `addons/website_customer/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Publish your customer references


Publish your customers as business references on your website to attract new potential prospects.
    

Declared dependencies: `website_crm_partner_assign`, `website_partner`, `website_google_map`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_crm_partner_assign",
    "website_partner",
    "website_google_map"
  ],
  "data": [
    "views/website_customer_templates.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/res_partner_demo.xml"
  ],
  "assets": {
    "website.website_builder_assets": [
      "website_customer/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_customer/__init__.py` (5 lines)
- `addons/website_customer/__manifest__.py` (30 lines)
- `addons/website_customer/controllers/__init__.py` (4 lines)
- `addons/website_customer/controllers/main.py` (177 lines)
- `addons/website_customer/data/res_partner_demo.xml` (122 lines)
- `addons/website_customer/i18n/af.po` (393 lines)
- `addons/website_customer/i18n/am.po` (389 lines)
- `addons/website_customer/i18n/ar.po` (411 lines)
- `addons/website_customer/i18n/az.po` (397 lines)
- `addons/website_customer/i18n/bg.po` (399 lines)
- `addons/website_customer/i18n/bs.po` (397 lines)
- `addons/website_customer/i18n/ca.po` (416 lines)
- `addons/website_customer/i18n/cs.po` (410 lines)
- `addons/website_customer/i18n/da.po` (408 lines)
- `addons/website_customer/i18n/de.po` (417 lines)
- `addons/website_customer/i18n/el.po` (398 lines)
- `addons/website_customer/i18n/es.po` (415 lines)
- `addons/website_customer/i18n/es_419.po` (408 lines)
- `addons/website_customer/i18n/es_CL.po` (80 lines)
- `addons/website_customer/i18n/et.po` (409 lines)
- `addons/website_customer/i18n/eu.po` (391 lines)
- `addons/website_customer/i18n/fa.po` (404 lines)
- `addons/website_customer/i18n/fi.po` (419 lines)
- `addons/website_customer/i18n/fo.po` (391 lines)
- `addons/website_customer/i18n/fr.po` (411 lines)
- `addons/website_customer/i18n/fr_BE.po` (51 lines)
- `addons/website_customer/i18n/fr_CA.po` (68 lines)
- `addons/website_customer/i18n/gl.po` (391 lines)
- `addons/website_customer/i18n/gu.po` (393 lines)
- `addons/website_customer/i18n/he.po` (407 lines)
- `addons/website_customer/i18n/hi.po` (396 lines)
- `addons/website_customer/i18n/hr.po` (404 lines)
- `addons/website_customer/i18n/hu.po` (404 lines)
- `addons/website_customer/i18n/id.po` (410 lines)
- `addons/website_customer/i18n/is.po` (389 lines)
- `addons/website_customer/i18n/it.po` (409 lines)
- `addons/website_customer/i18n/ja.po` (408 lines)
- `addons/website_customer/i18n/ka.po` (391 lines)
- `addons/website_customer/i18n/kab.po` (393 lines)
- `addons/website_customer/i18n/kk.po` (391 lines)
- `addons/website_customer/i18n/km.po` (392 lines)
- `addons/website_customer/i18n/ko.po` (407 lines)
- `addons/website_customer/i18n/ku.po` (393 lines)
- `addons/website_customer/i18n/lo.po` (403 lines)
- `addons/website_customer/i18n/lt.po` (411 lines)
- `addons/website_customer/i18n/lv.po` (399 lines)
- `addons/website_customer/i18n/mk.po` (396 lines)
- `addons/website_customer/i18n/ml_IN.po` (392 lines)
- `addons/website_customer/i18n/mn.po` (400 lines)
- `addons/website_customer/i18n/my.po` (394 lines)
- `addons/website_customer/i18n/nb.po` (403 lines)
- `addons/website_customer/i18n/nl.po` (413 lines)
- `addons/website_customer/i18n/pl.po` (418 lines)
- `addons/website_customer/i18n/pt.po` (408 lines)
- `addons/website_customer/i18n/pt_BR.po` (414 lines)
- `addons/website_customer/i18n/ro.po` (409 lines)
- `addons/website_customer/i18n/ru.po` (407 lines)
- `addons/website_customer/i18n/sk.po` (399 lines)
- `addons/website_customer/i18n/sl.po` (402 lines)
- `addons/website_customer/i18n/sq.po` (391 lines)
- `addons/website_customer/i18n/sr@latin.po` (402 lines)
- `addons/website_customer/i18n/sv.po` (412 lines)
- `addons/website_customer/i18n/ta.po` (392 lines)
- `addons/website_customer/i18n/th.po` (403 lines)
- `addons/website_customer/i18n/tr.po` (417 lines)
- `addons/website_customer/i18n/uk.po` (405 lines)
- `addons/website_customer/i18n/uz.po` (461 lines)
- `addons/website_customer/i18n/vi.po` (407 lines)
- `addons/website_customer/i18n/website_customer.pot` (387 lines)
- `addons/website_customer/i18n/zh_CN.po` (407 lines)
- `addons/website_customer/i18n/zh_TW.po` (403 lines)
- `addons/website_customer/models/__init__.py` (5 lines)
- `addons/website_customer/models/res_partner.py` (40 lines)
- `addons/website_customer/models/website.py` (13 lines)
- `addons/website_customer/security/ir.access.csv` (5 lines)
- `addons/website_customer/static/description/icon.png` (24 lines)
- `addons/website_customer/static/description/icon.svg` (1 lines)
- `addons/website_customer/static/description/icon_hi.png` (112 lines)
- `addons/website_customer/static/src/website_builder/customer_filter_option.js` (19 lines)
- `addons/website_customer/static/src/website_builder/customer_filter_option.xml` (37 lines)
- `addons/website_customer/tests/__init__.py` (1 lines)
- `addons/website_customer/tests/test_website_customers_technical_page.py` (9 lines)
- `addons/website_customer/views/res_partner_views.xml` (79 lines)
- `addons/website_customer/views/website_customer_templates.xml` (350 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
