# Module: website_event_crm

- **Module ID:** MOD-611
- **Path:** `addons/website_event_crm`
- **Manifest:** `addons/website_event_crm/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Allow per-order lead creation mode

Declared dependencies: `event_crm`, `website_event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_crm",
    "website_event"
  ],
  "data": [
    "views/event_lead_rule_views.xml"
  ],
  "demo": [
    "data/event_crm_demo.xml"
  ]
}
```

### Representative source files

- `addons/website_event_crm/__init__.py` (3 lines)
- `addons/website_event_crm/__manifest__.py` (18 lines)
- `addons/website_event_crm/data/event_crm_demo.xml` (13 lines)
- `addons/website_event_crm/i18n/ar.po` (57 lines)
- `addons/website_event_crm/i18n/az.po` (55 lines)
- `addons/website_event_crm/i18n/bg.po` (55 lines)
- `addons/website_event_crm/i18n/bs.po` (57 lines)
- `addons/website_event_crm/i18n/ca.po` (56 lines)
- `addons/website_event_crm/i18n/cs.po` (56 lines)
- `addons/website_event_crm/i18n/da.po` (57 lines)
- `addons/website_event_crm/i18n/de.po` (57 lines)
- `addons/website_event_crm/i18n/el.po` (56 lines)
- `addons/website_event_crm/i18n/es.po` (57 lines)
- `addons/website_event_crm/i18n/es_419.po` (56 lines)
- `addons/website_event_crm/i18n/et.po` (55 lines)
- `addons/website_event_crm/i18n/fa.po` (55 lines)
- `addons/website_event_crm/i18n/fi.po` (56 lines)
- `addons/website_event_crm/i18n/fr.po` (56 lines)
- `addons/website_event_crm/i18n/he.po` (56 lines)
- `addons/website_event_crm/i18n/hi.po` (55 lines)
- `addons/website_event_crm/i18n/hr.po` (56 lines)
- `addons/website_event_crm/i18n/hu.po` (56 lines)
- `addons/website_event_crm/i18n/id.po` (56 lines)
- `addons/website_event_crm/i18n/it.po` (56 lines)
- `addons/website_event_crm/i18n/ja.po` (57 lines)
- `addons/website_event_crm/i18n/kab.po` (56 lines)
- `addons/website_event_crm/i18n/ko.po` (56 lines)
- `addons/website_event_crm/i18n/ku.po` (55 lines)
- `addons/website_event_crm/i18n/lo.po` (55 lines)
- `addons/website_event_crm/i18n/lt.po` (57 lines)
- `addons/website_event_crm/i18n/lv.po` (56 lines)
- `addons/website_event_crm/i18n/mn.po` (55 lines)
- `addons/website_event_crm/i18n/my.po` (55 lines)
- `addons/website_event_crm/i18n/nb.po` (56 lines)
- `addons/website_event_crm/i18n/nl.po` (56 lines)
- `addons/website_event_crm/i18n/pl.po` (57 lines)
- `addons/website_event_crm/i18n/pt.po` (57 lines)
- `addons/website_event_crm/i18n/pt_BR.po` (57 lines)
- `addons/website_event_crm/i18n/ro.po` (56 lines)
- `addons/website_event_crm/i18n/ru.po` (59 lines)
- `addons/website_event_crm/i18n/sk.po` (55 lines)
- `addons/website_event_crm/i18n/sl.po` (57 lines)
- `addons/website_event_crm/i18n/sr@latin.po` (56 lines)
- `addons/website_event_crm/i18n/sv.po` (57 lines)
- `addons/website_event_crm/i18n/th.po` (56 lines)
- `addons/website_event_crm/i18n/tr.po` (57 lines)
- `addons/website_event_crm/i18n/uk.po` (56 lines)
- `addons/website_event_crm/i18n/uz.po` (68 lines)
- `addons/website_event_crm/i18n/vi.po` (56 lines)
- `addons/website_event_crm/i18n/website_event_crm.pot` (52 lines)
- `addons/website_event_crm/i18n/zh_CN.po` (56 lines)
- `addons/website_event_crm/i18n/zh_TW.po` (59 lines)
- `addons/website_event_crm/models/__init__.py` (4 lines)
- `addons/website_event_crm/models/event_registration.py` (36 lines)
- `addons/website_event_crm/tests/__init__.py` (5 lines)
- `addons/website_event_crm/tests/test_event_registration.py` (185 lines)
- `addons/website_event_crm/tests/test_visitor_propagation.py` (8 lines)
- `addons/website_event_crm/views/event_lead_rule_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
