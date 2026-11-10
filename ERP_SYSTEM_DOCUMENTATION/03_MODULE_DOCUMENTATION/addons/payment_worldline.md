# Module: payment_worldline

- **Module ID:** MOD-414
- **Path:** `addons/payment_worldline`
- **Manifest:** `addons/payment_worldline/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A French payment provider covering several European countries.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml",
    "views/payment_provider_views.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "payment_worldline/static/src/interactions/payment_form.js"
    ]
  }
}
```

### Representative source files

- `addons/payment_worldline/README.md` (44 lines)
- `addons/payment_worldline/__init__.py` (12 lines)
- `addons/payment_worldline/__manifest__.py` (22 lines)
- `addons/payment_worldline/const.py` (72 lines)
- `addons/payment_worldline/controllers/__init__.py` (3 lines)
- `addons/payment_worldline/controllers/main.py` (81 lines)
- `addons/payment_worldline/data/neutralize.sql` (7 lines)
- `addons/payment_worldline/data/payment_method_data.xml` (496 lines)
- `addons/payment_worldline/data/payment_provider_data.xml` (10 lines)
- `addons/payment_worldline/i18n/ar.po` (313 lines)
- `addons/payment_worldline/i18n/az.po` (310 lines)
- `addons/payment_worldline/i18n/bg.po` (310 lines)
- `addons/payment_worldline/i18n/bs.po` (311 lines)
- `addons/payment_worldline/i18n/ca.po` (311 lines)
- `addons/payment_worldline/i18n/cs.po` (311 lines)
- `addons/payment_worldline/i18n/da.po` (312 lines)
- `addons/payment_worldline/i18n/de.po` (314 lines)
- `addons/payment_worldline/i18n/el.po` (311 lines)
- `addons/payment_worldline/i18n/es.po` (314 lines)
- `addons/payment_worldline/i18n/es_419.po` (313 lines)
- `addons/payment_worldline/i18n/et.po` (310 lines)
- `addons/payment_worldline/i18n/fa.po` (310 lines)
- `addons/payment_worldline/i18n/fi.po` (314 lines)
- `addons/payment_worldline/i18n/fr.po` (313 lines)
- `addons/payment_worldline/i18n/he.po` (311 lines)
- `addons/payment_worldline/i18n/hi.po` (310 lines)
- `addons/payment_worldline/i18n/hr.po` (311 lines)
- `addons/payment_worldline/i18n/hu.po` (311 lines)
- `addons/payment_worldline/i18n/id.po` (313 lines)
- `addons/payment_worldline/i18n/it.po` (313 lines)
- `addons/payment_worldline/i18n/ja.po` (312 lines)
- `addons/payment_worldline/i18n/kab.po` (310 lines)
- `addons/payment_worldline/i18n/ko.po` (312 lines)
- `addons/payment_worldline/i18n/ku.po` (310 lines)
- `addons/payment_worldline/i18n/lo.po` (311 lines)
- `addons/payment_worldline/i18n/lt.po` (312 lines)
- `addons/payment_worldline/i18n/lv.po` (310 lines)
- `addons/payment_worldline/i18n/mn.po` (310 lines)
- `addons/payment_worldline/i18n/my.po` (310 lines)
- `addons/payment_worldline/i18n/nb.po` (311 lines)
- `addons/payment_worldline/i18n/nl.po` (312 lines)
- `addons/payment_worldline/i18n/payment_worldline.pot` (306 lines)
- `addons/payment_worldline/i18n/pl.po` (315 lines)
- `addons/payment_worldline/i18n/pt.po` (314 lines)
- `addons/payment_worldline/i18n/pt_BR.po` (315 lines)
- `addons/payment_worldline/i18n/ro.po` (313 lines)
- `addons/payment_worldline/i18n/ru.po` (314 lines)
- `addons/payment_worldline/i18n/sk.po` (309 lines)
- `addons/payment_worldline/i18n/sl.po` (312 lines)
- `addons/payment_worldline/i18n/sr@latin.po` (311 lines)
- `addons/payment_worldline/i18n/sv.po` (314 lines)
- `addons/payment_worldline/i18n/th.po` (312 lines)
- `addons/payment_worldline/i18n/tr.po` (314 lines)
- `addons/payment_worldline/i18n/uk.po` (311 lines)
- `addons/payment_worldline/i18n/uz.po` (340 lines)
- `addons/payment_worldline/i18n/vi.po` (314 lines)
- `addons/payment_worldline/i18n/zh_CN.po` (313 lines)
- `addons/payment_worldline/i18n/zh_TW.po` (313 lines)
- `addons/payment_worldline/models/__init__.py` (3 lines)
- `addons/payment_worldline/models/payment_provider.py` (129 lines)
- `addons/payment_worldline/models/payment_transaction.py` (315 lines)
- `addons/payment_worldline/static/description/icon.png` (11 lines)
- `addons/payment_worldline/static/description/icon.svg` (1 lines)
- `addons/payment_worldline/static/src/interactions/payment_form.js` (25 lines)
- `addons/payment_worldline/tests/__init__.py` (3 lines)
- `addons/payment_worldline/tests/common.py` (166 lines)
- `addons/payment_worldline/tests/test_processing_flows.py` (55 lines)
- `addons/payment_worldline/tests/test_worldline.py` (83 lines)
- `addons/payment_worldline/views/payment_provider_views.xml` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
