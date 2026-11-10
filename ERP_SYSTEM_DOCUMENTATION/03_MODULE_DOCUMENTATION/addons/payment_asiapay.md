# Module: payment_asiapay

- **Module ID:** MOD-395
- **Path:** `addons/payment_asiapay`
- **Manifest:** `addons/payment_asiapay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

An payment provider based in Hong Kong covering most Asian countries.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
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

- `addons/payment_asiapay/README.md` (47 lines)
- `addons/payment_asiapay/__init__.py` (12 lines)
- `addons/payment_asiapay/__manifest__.py` (19 lines)
- `addons/payment_asiapay/const.py` (129 lines)
- `addons/payment_asiapay/controllers/__init__.py` (3 lines)
- `addons/payment_asiapay/controllers/main.py` (45 lines)
- `addons/payment_asiapay/data/neutralize.sql` (5 lines)
- `addons/payment_asiapay/data/payment_method_data.xml` (439 lines)
- `addons/payment_asiapay/data/payment_provider_data.xml` (9 lines)
- `addons/payment_asiapay/i18n/ar.po` (395 lines)
- `addons/payment_asiapay/i18n/az.po` (392 lines)
- `addons/payment_asiapay/i18n/bg.po` (392 lines)
- `addons/payment_asiapay/i18n/bs.po` (394 lines)
- `addons/payment_asiapay/i18n/ca.po` (396 lines)
- `addons/payment_asiapay/i18n/cs.po` (394 lines)
- `addons/payment_asiapay/i18n/da.po` (394 lines)
- `addons/payment_asiapay/i18n/de.po` (397 lines)
- `addons/payment_asiapay/i18n/el.po` (393 lines)
- `addons/payment_asiapay/i18n/es.po` (398 lines)
- `addons/payment_asiapay/i18n/es_419.po` (396 lines)
- `addons/payment_asiapay/i18n/et.po` (392 lines)
- `addons/payment_asiapay/i18n/fa.po` (392 lines)
- `addons/payment_asiapay/i18n/fi.po` (395 lines)
- `addons/payment_asiapay/i18n/fr.po` (396 lines)
- `addons/payment_asiapay/i18n/he.po` (393 lines)
- `addons/payment_asiapay/i18n/hi.po` (392 lines)
- `addons/payment_asiapay/i18n/hr.po` (393 lines)
- `addons/payment_asiapay/i18n/hu.po` (393 lines)
- `addons/payment_asiapay/i18n/id.po` (394 lines)
- `addons/payment_asiapay/i18n/it.po` (396 lines)
- `addons/payment_asiapay/i18n/ja.po` (394 lines)
- `addons/payment_asiapay/i18n/kab.po` (393 lines)
- `addons/payment_asiapay/i18n/ko.po` (394 lines)
- `addons/payment_asiapay/i18n/ku.po` (392 lines)
- `addons/payment_asiapay/i18n/lo.po` (394 lines)
- `addons/payment_asiapay/i18n/lt.po` (394 lines)
- `addons/payment_asiapay/i18n/lv.po` (393 lines)
- `addons/payment_asiapay/i18n/mn.po` (392 lines)
- `addons/payment_asiapay/i18n/my.po` (392 lines)
- `addons/payment_asiapay/i18n/nb.po` (393 lines)
- `addons/payment_asiapay/i18n/nl.po` (396 lines)
- `addons/payment_asiapay/i18n/payment_asiapay.pot` (389 lines)
- `addons/payment_asiapay/i18n/pl.po` (396 lines)
- `addons/payment_asiapay/i18n/pt.po` (395 lines)
- `addons/payment_asiapay/i18n/pt_BR.po` (402 lines)
- `addons/payment_asiapay/i18n/ro.po` (396 lines)
- `addons/payment_asiapay/i18n/ru.po` (399 lines)
- `addons/payment_asiapay/i18n/sk.po` (392 lines)
- `addons/payment_asiapay/i18n/sl.po` (394 lines)
- `addons/payment_asiapay/i18n/sr@latin.po` (393 lines)
- `addons/payment_asiapay/i18n/sv.po` (394 lines)
- `addons/payment_asiapay/i18n/th.po` (394 lines)
- `addons/payment_asiapay/i18n/tr.po` (397 lines)
- `addons/payment_asiapay/i18n/uk.po` (393 lines)
- `addons/payment_asiapay/i18n/uz.po` (430 lines)
- `addons/payment_asiapay/i18n/vi.po` (394 lines)
- `addons/payment_asiapay/i18n/zh_CN.po` (395 lines)
- `addons/payment_asiapay/i18n/zh_TW.po` (396 lines)
- `addons/payment_asiapay/models/__init__.py` (3 lines)
- `addons/payment_asiapay/models/payment_provider.py` (112 lines)
- `addons/payment_asiapay/models/payment_transaction.py` (139 lines)
- `addons/payment_asiapay/static/description/icon.png` (13 lines)
- `addons/payment_asiapay/static/description/icon.svg` (1 lines)
- `addons/payment_asiapay/static/description/icon_hi.png` (122 lines)
- `addons/payment_asiapay/tests/__init__.py` (3 lines)
- `addons/payment_asiapay/tests/common.py` (36 lines)
- `addons/payment_asiapay/tests/test_payment_provider.py` (39 lines)
- `addons/payment_asiapay/tests/test_payment_transaction.py` (121 lines)
- `addons/payment_asiapay/tests/test_processing_flows.py` (54 lines)
- `addons/payment_asiapay/views/payment_provider_views.xml` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
