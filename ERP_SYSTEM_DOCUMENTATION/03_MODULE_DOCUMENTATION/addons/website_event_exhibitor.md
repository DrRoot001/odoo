# Module: website_event_exhibitor

- **Module ID:** MOD-612
- **Path:** `addons/website_event_exhibitor`
- **Manifest:** `addons/website_event_exhibitor/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Event: manage sponsors and exhibitors

No manifest description declared.

Declared dependencies: `website_event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_event"
  ],
  "data": [
    "data/event_sponsor_data.xml",
    "report/website_event_exhibitor_reports.xml",
    "report/website_event_exhibitor_templates.xml",
    "views/event_templates_sponsor.xml",
    "views/event_sponsor_views.xml",
    "views/event_event_views.xml",
    "views/event_exhibitor_templates_list.xml",
    "views/event_exhibitor_templates_page.xml",
    "views/event_type_views.xml",
    "views/event_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_demo.xml",
    "data/event_sponsor_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_event_exhibitor/static/src/scss/event_templates_sponsor.scss",
      "website_event_exhibitor/static/src/scss/event_exhibitor_templates.scss",
      "website_event_exhibitor/static/src/interactions/**/*",
      "website_event_exhibitor/static/src/components/exhibitor_connect_closed_dialog/**/*"
    ],
    "web.report_assets_common": [
      "/website_event_exhibitor/static/src/scss/event_full_page_ticket_report.scss"
    ],
    "website.website_builder_assets": [
      "website_event_exhibitor/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_event_exhibitor/__init__.py` (5 lines)
- `addons/website_event_exhibitor/__manifest__.py` (46 lines)
- `addons/website_event_exhibitor/controllers/__init__.py` (4 lines)
- `addons/website_event_exhibitor/controllers/exhibitor.py` (237 lines)
- `addons/website_event_exhibitor/data/event_demo.xml` (8 lines)
- `addons/website_event_exhibitor/data/event_sponsor_data.xml` (20 lines)
- `addons/website_event_exhibitor/data/event_sponsor_demo.xml` (114 lines)
- `addons/website_event_exhibitor/i18n/ar.po` (991 lines)
- `addons/website_event_exhibitor/i18n/az.po` (1,046 lines)
- `addons/website_event_exhibitor/i18n/bg.po` (1,056 lines)
- `addons/website_event_exhibitor/i18n/bs.po` (1,053 lines)
- `addons/website_event_exhibitor/i18n/ca.po` (1,005 lines)
- `addons/website_event_exhibitor/i18n/cs.po` (990 lines)
- `addons/website_event_exhibitor/i18n/da.po` (999 lines)
- `addons/website_event_exhibitor/i18n/de.po` (1,001 lines)
- `addons/website_event_exhibitor/i18n/el.po` (983 lines)
- `addons/website_event_exhibitor/i18n/es.po` (1,000 lines)
- `addons/website_event_exhibitor/i18n/es_419.po` (997 lines)
- `addons/website_event_exhibitor/i18n/et.po` (1,128 lines)
- `addons/website_event_exhibitor/i18n/fa.po` (1,057 lines)
- `addons/website_event_exhibitor/i18n/fi.po` (1,001 lines)
- `addons/website_event_exhibitor/i18n/fr.po` (994 lines)
- `addons/website_event_exhibitor/i18n/he.po` (1,068 lines)
- `addons/website_event_exhibitor/i18n/hi.po` (1,059 lines)
- `addons/website_event_exhibitor/i18n/hr.po` (1,060 lines)
- `addons/website_event_exhibitor/i18n/hu.po` (982 lines)
- `addons/website_event_exhibitor/i18n/id.po` (999 lines)
- `addons/website_event_exhibitor/i18n/it.po` (995 lines)
- `addons/website_event_exhibitor/i18n/ja.po` (990 lines)
- `addons/website_event_exhibitor/i18n/kab.po` (1,006 lines)
- `addons/website_event_exhibitor/i18n/ko.po` (994 lines)
- `addons/website_event_exhibitor/i18n/ku.po` (1,027 lines)
- `addons/website_event_exhibitor/i18n/lo.po` (987 lines)
- `addons/website_event_exhibitor/i18n/lt.po` (1,069 lines)
- `addons/website_event_exhibitor/i18n/lv.po` (1,050 lines)
- `addons/website_event_exhibitor/i18n/mn.po` (1,058 lines)
- `addons/website_event_exhibitor/i18n/my.po` (1,004 lines)
- `addons/website_event_exhibitor/i18n/nb.po` (984 lines)
- `addons/website_event_exhibitor/i18n/nl.po` (997 lines)
- `addons/website_event_exhibitor/i18n/pl.po` (998 lines)
- `addons/website_event_exhibitor/i18n/pt.po` (998 lines)
- `addons/website_event_exhibitor/i18n/pt_BR.po` (994 lines)
- `addons/website_event_exhibitor/i18n/ro.po` (1,145 lines)
- `addons/website_event_exhibitor/i18n/ru.po` (1,004 lines)
- `addons/website_event_exhibitor/i18n/sk.po` (1,069 lines)
- `addons/website_event_exhibitor/i18n/sl.po` (984 lines)
- `addons/website_event_exhibitor/i18n/sr@latin.po` (1,069 lines)
- `addons/website_event_exhibitor/i18n/sv.po` (1,007 lines)
- `addons/website_event_exhibitor/i18n/th.po` (995 lines)
- `addons/website_event_exhibitor/i18n/tr.po` (1,003 lines)
- `addons/website_event_exhibitor/i18n/uk.po` (1,134 lines)
- `addons/website_event_exhibitor/i18n/uz.po` (1,146 lines)
- `addons/website_event_exhibitor/i18n/vi.po` (1,000 lines)
- `addons/website_event_exhibitor/i18n/website_event_exhibitor.pot` (964 lines)
- `addons/website_event_exhibitor/i18n/zh_CN.po` (988 lines)
- `addons/website_event_exhibitor/i18n/zh_TW.po` (998 lines)
- `addons/website_event_exhibitor/models/__init__.py` (9 lines)
- `addons/website_event_exhibitor/models/event_event.py` (67 lines)
- `addons/website_event_exhibitor/models/event_sponsor.py` (268 lines)
- `addons/website_event_exhibitor/models/event_sponsor_type.py` (20 lines)
- `addons/website_event_exhibitor/models/event_type.py` (18 lines)
- `addons/website_event_exhibitor/models/website.py` (11 lines)
- `addons/website_event_exhibitor/models/website_event_menu.py` (12 lines)
- `addons/website_event_exhibitor/report/website_event_exhibitor_reports.xml` (9 lines)
- `addons/website_event_exhibitor/report/website_event_exhibitor_templates.xml` (19 lines)
- `addons/website_event_exhibitor/security/ir.access.csv` (5 lines)
- `addons/website_event_exhibitor/static/src/components/exhibitor_connect_closed_dialog/exhibitor_connect_closed_dialog.js` (36 lines)
- `addons/website_event_exhibitor/static/src/components/exhibitor_connect_closed_dialog/exhibitor_connect_closed_dialog.xml` (84 lines)
- `addons/website_event_exhibitor/static/src/img/event_sponsor_default.svg` (5 lines)
- `addons/website_event_exhibitor/static/src/interactions/exhibitor_connect.js` (38 lines)
- `addons/website_event_exhibitor/static/src/scss/event_exhibitor_templates.scss` (112 lines)
- `addons/website_event_exhibitor/static/src/scss/event_full_page_ticket_report.scss` (9 lines)
- `addons/website_event_exhibitor/static/src/scss/event_templates_sponsor.scss` (69 lines)
- `addons/website_event_exhibitor/static/src/website_builder/event_page_option.xml` (32 lines)
- `addons/website_event_exhibitor/tests/__init__.py` (4 lines)
- `addons/website_event_exhibitor/tests/common.py` (31 lines)
- `addons/website_event_exhibitor/tests/test_sponsor_internals.py` (93 lines)
- `addons/website_event_exhibitor/views/event_event_views.xml` (38 lines)
- `addons/website_event_exhibitor/views/event_exhibitor_templates_list.xml` (317 lines)
- `addons/website_event_exhibitor/views/event_exhibitor_templates_page.xml` (175 lines)
- `addons/website_event_exhibitor/views/event_menus.xml` (11 lines)
- `addons/website_event_exhibitor/views/event_sponsor_views.xml` (204 lines)
- `addons/website_event_exhibitor/views/event_templates_sponsor.xml` (42 lines)
- `addons/website_event_exhibitor/views/event_type_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
