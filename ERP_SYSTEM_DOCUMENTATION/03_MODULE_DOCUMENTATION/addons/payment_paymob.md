# Module: payment_paymob

- **Module ID:** MOD-407
- **Path:** `addons/payment_paymob`
- **Manifest:** `addons/payment_paymob/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An Egyptian payment provider for the Middle East.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
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
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ]
}
```

### Representative source files

- `addons/payment_paymob/README.md` (31 lines)
- `addons/payment_paymob/__init__.py` (12 lines)
- `addons/payment_paymob/__manifest__.py` (19 lines)
- `addons/payment_paymob/const.py` (59 lines)
- `addons/payment_paymob/controllers/__init__.py` (3 lines)
- `addons/payment_paymob/controllers/main.py` (120 lines)
- `addons/payment_paymob/data/neutralize.sql` (6 lines)
- `addons/payment_paymob/data/payment_method_data.xml` (181 lines)
- `addons/payment_paymob/data/payment_provider_data.xml` (9 lines)
- `addons/payment_paymob/i18n/ar.po` (293 lines)
- `addons/payment_paymob/i18n/az.po` (295 lines)
- `addons/payment_paymob/i18n/bg.po` (296 lines)
- `addons/payment_paymob/i18n/bs.po` (295 lines)
- `addons/payment_paymob/i18n/ca.po` (301 lines)
- `addons/payment_paymob/i18n/cs.po` (300 lines)
- `addons/payment_paymob/i18n/da.po` (319 lines)
- `addons/payment_paymob/i18n/de.po` (294 lines)
- `addons/payment_paymob/i18n/el.po` (296 lines)
- `addons/payment_paymob/i18n/es.po` (292 lines)
- `addons/payment_paymob/i18n/es_419.po` (292 lines)
- `addons/payment_paymob/i18n/et.po` (299 lines)
- `addons/payment_paymob/i18n/fa.po` (298 lines)
- `addons/payment_paymob/i18n/fi.po` (289 lines)
- `addons/payment_paymob/i18n/fr.po` (293 lines)
- `addons/payment_paymob/i18n/he.po` (300 lines)
- `addons/payment_paymob/i18n/hi.po` (299 lines)
- `addons/payment_paymob/i18n/hr.po` (299 lines)
- `addons/payment_paymob/i18n/hu.po` (296 lines)
- `addons/payment_paymob/i18n/id.po` (296 lines)
- `addons/payment_paymob/i18n/it.po` (292 lines)
- `addons/payment_paymob/i18n/ja.po` (292 lines)
- `addons/payment_paymob/i18n/kab.po` (293 lines)
- `addons/payment_paymob/i18n/ko.po` (292 lines)
- `addons/payment_paymob/i18n/ku.po` (294 lines)
- `addons/payment_paymob/i18n/lo.po` (291 lines)
- `addons/payment_paymob/i18n/lt.po` (298 lines)
- `addons/payment_paymob/i18n/lv.po` (298 lines)
- `addons/payment_paymob/i18n/mn.po` (296 lines)
- `addons/payment_paymob/i18n/my.po` (294 lines)
- `addons/payment_paymob/i18n/nb.po` (296 lines)
- `addons/payment_paymob/i18n/nl.po` (293 lines)
- `addons/payment_paymob/i18n/payment_paymob.pot` (285 lines)
- `addons/payment_paymob/i18n/pl.po` (294 lines)
- `addons/payment_paymob/i18n/pt.po` (299 lines)
- `addons/payment_paymob/i18n/pt_BR.po` (295 lines)
- `addons/payment_paymob/i18n/ro.po` (292 lines)
- `addons/payment_paymob/i18n/ru.po` (293 lines)
- `addons/payment_paymob/i18n/sk.po` (300 lines)
- `addons/payment_paymob/i18n/sl.po` (299 lines)
- `addons/payment_paymob/i18n/sr@latin.po` (296 lines)
- `addons/payment_paymob/i18n/sv.po` (299 lines)
- `addons/payment_paymob/i18n/th.po` (299 lines)
- `addons/payment_paymob/i18n/tr.po` (294 lines)
- `addons/payment_paymob/i18n/uk.po` (302 lines)
- `addons/payment_paymob/i18n/uz.po` (326 lines)
- `addons/payment_paymob/i18n/vi.po` (301 lines)
- `addons/payment_paymob/i18n/zh_CN.po` (290 lines)
- `addons/payment_paymob/i18n/zh_TW.po` (291 lines)
- `addons/payment_paymob/models/__init__.py` (3 lines)
- `addons/payment_paymob/models/payment_provider.py` (281 lines)
- `addons/payment_paymob/models/payment_transaction.py` (157 lines)
- `addons/payment_paymob/static/description/icon.png` (13 lines)
- `addons/payment_paymob/static/description/icon.svg` (10 lines)
- `addons/payment_paymob/static/description/icon_hi.png` (54 lines)
- `addons/payment_paymob/tests/__init__.py` (3 lines)
- `addons/payment_paymob/tests/common.py` (80 lines)
- `addons/payment_paymob/tests/test_paymob.py` (85 lines)
- `addons/payment_paymob/tests/test_processing_flows.py` (114 lines)
- `addons/payment_paymob/views/payment_provider_views.xml` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
