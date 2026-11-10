# Module: website_event_booth_sale

- **Module ID:** MOD-609
- **Path:** `addons/website_event_booth_sale`
- **Manifest:** `addons/website_event_booth_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Events, sell your booths online


Use the e-commerce to sell your event booths.
    

Declared dependencies: `event_booth_sale`, `website_event_booth`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 4 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_booth_sale",
    "website_event_booth",
    "website_sale"
  ],
  "data": [
    "views/event_booth_registration_templates.xml",
    "views/event_booth_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "/website_event_booth_sale/static/src/interactions/*"
    ],
    "web.assets_tests": [
      "/website_event_booth_sale/static/tests/tours/**/*.js"
    ]
  }
}
```

### Representative source files

- `addons/website_event_booth_sale/__init__.py` (5 lines)
- `addons/website_event_booth_sale/__manifest__.py` (25 lines)
- `addons/website_event_booth_sale/controllers/__init__.py` (4 lines)
- `addons/website_event_booth_sale/controllers/event_booth.py` (56 lines)
- `addons/website_event_booth_sale/i18n/ar.po` (96 lines)
- `addons/website_event_booth_sale/i18n/az.po` (94 lines)
- `addons/website_event_booth_sale/i18n/bg.po` (94 lines)
- `addons/website_event_booth_sale/i18n/bs.po` (96 lines)
- `addons/website_event_booth_sale/i18n/ca.po` (97 lines)
- `addons/website_event_booth_sale/i18n/cs.po` (95 lines)
- `addons/website_event_booth_sale/i18n/da.po` (98 lines)
- `addons/website_event_booth_sale/i18n/de.po` (99 lines)
- `addons/website_event_booth_sale/i18n/el.po` (95 lines)
- `addons/website_event_booth_sale/i18n/es.po` (100 lines)
- `addons/website_event_booth_sale/i18n/es_419.po` (97 lines)
- `addons/website_event_booth_sale/i18n/et.po` (94 lines)
- `addons/website_event_booth_sale/i18n/fa.po` (94 lines)
- `addons/website_event_booth_sale/i18n/fi.po` (96 lines)
- `addons/website_event_booth_sale/i18n/fr.po` (97 lines)
- `addons/website_event_booth_sale/i18n/he.po` (95 lines)
- `addons/website_event_booth_sale/i18n/hi.po` (94 lines)
- `addons/website_event_booth_sale/i18n/hr.po` (95 lines)
- `addons/website_event_booth_sale/i18n/hu.po` (95 lines)
- `addons/website_event_booth_sale/i18n/id.po` (96 lines)
- `addons/website_event_booth_sale/i18n/it.po` (98 lines)
- `addons/website_event_booth_sale/i18n/ja.po` (95 lines)
- `addons/website_event_booth_sale/i18n/kab.po` (95 lines)
- `addons/website_event_booth_sale/i18n/ko.po` (96 lines)
- `addons/website_event_booth_sale/i18n/ku.po` (94 lines)
- `addons/website_event_booth_sale/i18n/lo.po` (94 lines)
- `addons/website_event_booth_sale/i18n/lt.po` (96 lines)
- `addons/website_event_booth_sale/i18n/lv.po` (95 lines)
- `addons/website_event_booth_sale/i18n/mn.po` (94 lines)
- `addons/website_event_booth_sale/i18n/my.po` (94 lines)
- `addons/website_event_booth_sale/i18n/nb.po` (95 lines)
- `addons/website_event_booth_sale/i18n/nl.po` (96 lines)
- `addons/website_event_booth_sale/i18n/pl.po` (97 lines)
- `addons/website_event_booth_sale/i18n/pt.po` (98 lines)
- `addons/website_event_booth_sale/i18n/pt_BR.po` (101 lines)
- `addons/website_event_booth_sale/i18n/ro.po` (95 lines)
- `addons/website_event_booth_sale/i18n/ru.po` (99 lines)
- `addons/website_event_booth_sale/i18n/sk.po` (94 lines)
- `addons/website_event_booth_sale/i18n/sl.po` (96 lines)
- `addons/website_event_booth_sale/i18n/sr@latin.po` (95 lines)
- `addons/website_event_booth_sale/i18n/sv.po` (96 lines)
- `addons/website_event_booth_sale/i18n/th.po` (95 lines)
- `addons/website_event_booth_sale/i18n/tr.po` (98 lines)
- `addons/website_event_booth_sale/i18n/uk.po` (95 lines)
- `addons/website_event_booth_sale/i18n/uz.po` (113 lines)
- `addons/website_event_booth_sale/i18n/vi.po` (97 lines)
- `addons/website_event_booth_sale/i18n/website_event_booth_sale.pot` (91 lines)
- `addons/website_event_booth_sale/i18n/zh_CN.po` (95 lines)
- `addons/website_event_booth_sale/i18n/zh_TW.po` (98 lines)
- `addons/website_event_booth_sale/models/__init__.py` (4 lines)
- `addons/website_event_booth_sale/models/product_template.py` (12 lines)
- `addons/website_event_booth_sale/models/sale_order.py` (79 lines)
- `addons/website_event_booth_sale/models/sale_order_line.py` (14 lines)
- `addons/website_event_booth_sale/static/src/interactions/booth_registration.js` (29 lines)
- `addons/website_event_booth_sale/static/tests/tours/helpers/WebsiteEventBoothSaleTourMethods.js` (58 lines)
- `addons/website_event_booth_sale/static/tests/tours/website_event_booth.js` (58 lines)
- `addons/website_event_booth_sale/static/tests/tours/website_event_booth_sale_pricelists.js` (62 lines)
- `addons/website_event_booth_sale/tests/__init__.py` (5 lines)
- `addons/website_event_booth_sale/tests/test_event_booth_sale.py` (96 lines)
- `addons/website_event_booth_sale/tests/test_website_event_booth_sale_pricelist.py` (70 lines)
- `addons/website_event_booth_sale/views/event_booth_registration_templates.xml` (11 lines)
- `addons/website_event_booth_sale/views/event_booth_templates.xml` (54 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
