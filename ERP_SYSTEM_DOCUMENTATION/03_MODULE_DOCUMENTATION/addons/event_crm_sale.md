# Module: event_crm_sale

- **Module ID:** MOD-068
- **Path:** `addons/event_crm_sale`
- **Manifest:** `addons/event_crm_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Add information of sale order linked to the registration for the creation of the lead.

Declared dependencies: `event_crm`, `event_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_crm",
    "event_sale"
  ],
  "data": [
    "views/event_lead_rule_views.xml"
  ]
}
```

### Representative source files

- `addons/event_crm_sale/__init__.py` (4 lines)
- `addons/event_crm_sale/__manifest__.py` (15 lines)
- `addons/event_crm_sale/i18n/ar.po` (49 lines)
- `addons/event_crm_sale/i18n/az.po` (47 lines)
- `addons/event_crm_sale/i18n/bg.po` (47 lines)
- `addons/event_crm_sale/i18n/bs.po` (48 lines)
- `addons/event_crm_sale/i18n/ca.po` (48 lines)
- `addons/event_crm_sale/i18n/cs.po` (48 lines)
- `addons/event_crm_sale/i18n/da.po` (49 lines)
- `addons/event_crm_sale/i18n/de.po` (50 lines)
- `addons/event_crm_sale/i18n/el.po` (48 lines)
- `addons/event_crm_sale/i18n/es.po` (51 lines)
- `addons/event_crm_sale/i18n/es_419.po` (50 lines)
- `addons/event_crm_sale/i18n/et.po` (47 lines)
- `addons/event_crm_sale/i18n/event_crm_sale.pot` (43 lines)
- `addons/event_crm_sale/i18n/fa.po` (47 lines)
- `addons/event_crm_sale/i18n/fi.po` (51 lines)
- `addons/event_crm_sale/i18n/fr.po` (51 lines)
- `addons/event_crm_sale/i18n/he.po` (48 lines)
- `addons/event_crm_sale/i18n/hi.po` (47 lines)
- `addons/event_crm_sale/i18n/hr.po` (48 lines)
- `addons/event_crm_sale/i18n/hu.po` (48 lines)
- `addons/event_crm_sale/i18n/id.po` (48 lines)
- `addons/event_crm_sale/i18n/it.po` (50 lines)
- `addons/event_crm_sale/i18n/ja.po` (48 lines)
- `addons/event_crm_sale/i18n/kab.po` (47 lines)
- `addons/event_crm_sale/i18n/ko.po` (48 lines)
- `addons/event_crm_sale/i18n/ku.po` (47 lines)
- `addons/event_crm_sale/i18n/lo.po` (46 lines)
- `addons/event_crm_sale/i18n/lt.po` (49 lines)
- `addons/event_crm_sale/i18n/lv.po` (47 lines)
- `addons/event_crm_sale/i18n/mn.po` (47 lines)
- `addons/event_crm_sale/i18n/my.po` (47 lines)
- `addons/event_crm_sale/i18n/nb.po` (48 lines)
- `addons/event_crm_sale/i18n/nl.po` (48 lines)
- `addons/event_crm_sale/i18n/pl.po` (49 lines)
- `addons/event_crm_sale/i18n/pt.po` (49 lines)
- `addons/event_crm_sale/i18n/pt_BR.po` (50 lines)
- `addons/event_crm_sale/i18n/ro.po` (48 lines)
- `addons/event_crm_sale/i18n/ru.po` (52 lines)
- `addons/event_crm_sale/i18n/sk.po` (46 lines)
- `addons/event_crm_sale/i18n/sl.po` (49 lines)
- `addons/event_crm_sale/i18n/sr@latin.po` (48 lines)
- `addons/event_crm_sale/i18n/sv.po` (49 lines)
- `addons/event_crm_sale/i18n/th.po` (48 lines)
- `addons/event_crm_sale/i18n/tr.po` (48 lines)
- `addons/event_crm_sale/i18n/uk.po` (48 lines)
- `addons/event_crm_sale/i18n/uz.po` (57 lines)
- `addons/event_crm_sale/i18n/vi.po` (49 lines)
- `addons/event_crm_sale/i18n/zh_CN.po` (49 lines)
- `addons/event_crm_sale/i18n/zh_TW.po` (50 lines)
- `addons/event_crm_sale/models/__init__.py` (4 lines)
- `addons/event_crm_sale/models/event_registration.py` (49 lines)
- `addons/event_crm_sale/tests/__init__.py` (1 lines)
- `addons/event_crm_sale/tests/test_event_crm_flow.py` (45 lines)
- `addons/event_crm_sale/views/event_lead_rule_views.xml` (23 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
