# Module: event_booth

- **Module ID:** MOD-065
- **Path:** `addons/event_booth`
- **Manifest:** `addons/event_booth/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage event booths


Create booths for your favorite event.
    

Declared dependencies: `event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 11 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event"
  ],
  "data": [
    "views/event_booth_category_views.xml",
    "views/event_type_booth_views.xml",
    "views/event_booth_views.xml",
    "views/event_type_views.xml",
    "views/event_event_views.xml",
    "views/event_menus.xml",
    "data/event_booth_category_data.xml",
    "data/mail_message_subtype_data.xml",
    "data/mail_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_booth_demo.xml",
    "data/event_type_demo.xml"
  ]
}
```

### Representative source files

- `addons/event_booth/__init__.py` (4 lines)
- `addons/event_booth/__manifest__.py` (30 lines)
- `addons/event_booth/data/event_booth_category_data.xml` (91 lines)
- `addons/event_booth/data/event_booth_demo.xml` (128 lines)
- `addons/event_booth/data/event_type_demo.xml` (25 lines)
- `addons/event_booth/data/mail_message_subtype_data.xml` (10 lines)
- `addons/event_booth/data/mail_templates.xml` (35 lines)
- `addons/event_booth/i18n/ar.po` (725 lines)
- `addons/event_booth/i18n/az.po` (721 lines)
- `addons/event_booth/i18n/bg.po` (722 lines)
- `addons/event_booth/i18n/bs.po` (712 lines)
- `addons/event_booth/i18n/ca.po` (726 lines)
- `addons/event_booth/i18n/cs.po` (723 lines)
- `addons/event_booth/i18n/da.po` (726 lines)
- `addons/event_booth/i18n/de.po` (730 lines)
- `addons/event_booth/i18n/el.po` (722 lines)
- `addons/event_booth/i18n/es.po` (728 lines)
- `addons/event_booth/i18n/es_419.po` (729 lines)
- `addons/event_booth/i18n/et.po` (725 lines)
- `addons/event_booth/i18n/event_booth.pot` (707 lines)
- `addons/event_booth/i18n/fa.po` (724 lines)
- `addons/event_booth/i18n/fi.po` (730 lines)
- `addons/event_booth/i18n/fr.po` (731 lines)
- `addons/event_booth/i18n/he.po` (724 lines)
- `addons/event_booth/i18n/hi.po` (721 lines)
- `addons/event_booth/i18n/hr.po` (722 lines)
- `addons/event_booth/i18n/hu.po` (721 lines)
- `addons/event_booth/i18n/id.po` (726 lines)
- `addons/event_booth/i18n/it.po` (729 lines)
- `addons/event_booth/i18n/ja.po` (724 lines)
- `addons/event_booth/i18n/kab.po` (711 lines)
- `addons/event_booth/i18n/ko.po` (726 lines)
- `addons/event_booth/i18n/ku.po` (721 lines)
- `addons/event_booth/i18n/lo.po` (718 lines)
- `addons/event_booth/i18n/lt.po` (723 lines)
- `addons/event_booth/i18n/lv.po` (711 lines)
- `addons/event_booth/i18n/mn.po` (721 lines)
- `addons/event_booth/i18n/my.po` (712 lines)
- `addons/event_booth/i18n/nb.po` (721 lines)
- `addons/event_booth/i18n/nl.po` (725 lines)
- `addons/event_booth/i18n/pl.po` (728 lines)
- `addons/event_booth/i18n/pt.po` (725 lines)
- `addons/event_booth/i18n/pt_BR.po` (727 lines)
- `addons/event_booth/i18n/ro.po` (726 lines)
- `addons/event_booth/i18n/ru.po` (731 lines)
- `addons/event_booth/i18n/sk.po` (710 lines)
- `addons/event_booth/i18n/sl.po` (726 lines)
- `addons/event_booth/i18n/sr@latin.po` (722 lines)
- `addons/event_booth/i18n/sv.po` (730 lines)
- `addons/event_booth/i18n/th.po` (721 lines)
- `addons/event_booth/i18n/tr.po` (726 lines)
- `addons/event_booth/i18n/uk.po` (726 lines)
- `addons/event_booth/i18n/uz.po` (851 lines)
- `addons/event_booth/i18n/vi.po` (725 lines)
- `addons/event_booth/i18n/zh_CN.po` (725 lines)
- `addons/event_booth/i18n/zh_TW.po` (725 lines)
- `addons/event_booth/models/__init__.py` (8 lines)
- `addons/event_booth/models/event_booth.py` (87 lines)
- `addons/event_booth/models/event_booth_category.py` (18 lines)
- `addons/event_booth/models/event_event.py` (89 lines)
- `addons/event_booth/models/event_type.py` (12 lines)
- `addons/event_booth/models/event_type_booth.py` (27 lines)
- `addons/event_booth/security/ir.access.csv` (7 lines)
- `addons/event_booth/static/src/img/premium-booth.jpeg` (284 lines)
- `addons/event_booth/static/src/img/standard-booth.jpeg` (220 lines)
- `addons/event_booth/static/src/img/vip-booth.jpeg` (285 lines)
- `addons/event_booth/tests/__init__.py` (5 lines)
- `addons/event_booth/tests/common.py` (20 lines)
- `addons/event_booth/tests/test_event_booth_internals.py` (56 lines)
- `addons/event_booth/tests/test_event_internals.py` (93 lines)
- `addons/event_booth/views/event_booth_category_views.xml` (65 lines)
- `addons/event_booth/views/event_booth_views.xml` (230 lines)
- `addons/event_booth/views/event_event_views.xml` (27 lines)
- `addons/event_booth/views/event_menus.xml` (16 lines)
- `addons/event_booth/views/event_type_booth_views.xml` (85 lines)
- `addons/event_booth/views/event_type_views.xml` (22 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
