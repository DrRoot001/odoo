# Module: payment_ecpay

- **Module ID:** MOD-401
- **Path:** `addons/payment_ecpay`
- **Manifest:** `addons/payment_ecpay/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering the Taiwanese market.

 

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
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml",
    "views/payment_provider_views.xml"
  ]
}
```

### Representative source files

- `addons/payment_ecpay/README.md` (59 lines)
- `addons/payment_ecpay/__init__.py` (12 lines)
- `addons/payment_ecpay/__manifest__.py` (19 lines)
- `addons/payment_ecpay/const.py` (55 lines)
- `addons/payment_ecpay/controllers/__init__.py` (3 lines)
- `addons/payment_ecpay/controllers/main.py` (81 lines)
- `addons/payment_ecpay/data/neutralize.sql` (4 lines)
- `addons/payment_ecpay/data/payment_method_data.xml` (144 lines)
- `addons/payment_ecpay/data/payment_provider_data.xml` (9 lines)
- `addons/payment_ecpay/i18n/ar.po` (203 lines)
- `addons/payment_ecpay/i18n/az.po` (201 lines)
- `addons/payment_ecpay/i18n/bg.po` (201 lines)
- `addons/payment_ecpay/i18n/bs.po` (202 lines)
- `addons/payment_ecpay/i18n/ca.po` (201 lines)
- `addons/payment_ecpay/i18n/cs.po` (201 lines)
- `addons/payment_ecpay/i18n/da.po` (201 lines)
- `addons/payment_ecpay/i18n/de.po` (205 lines)
- `addons/payment_ecpay/i18n/el.po` (201 lines)
- `addons/payment_ecpay/i18n/es.po` (205 lines)
- `addons/payment_ecpay/i18n/es_419.po` (204 lines)
- `addons/payment_ecpay/i18n/et.po` (201 lines)
- `addons/payment_ecpay/i18n/fa.po` (201 lines)
- `addons/payment_ecpay/i18n/fi.po` (204 lines)
- `addons/payment_ecpay/i18n/fr.po` (206 lines)
- `addons/payment_ecpay/i18n/he.po` (202 lines)
- `addons/payment_ecpay/i18n/hi.po` (201 lines)
- `addons/payment_ecpay/i18n/hr.po` (202 lines)
- `addons/payment_ecpay/i18n/hu.po` (201 lines)
- `addons/payment_ecpay/i18n/id.po` (201 lines)
- `addons/payment_ecpay/i18n/it.po` (206 lines)
- `addons/payment_ecpay/i18n/ja.po` (205 lines)
- `addons/payment_ecpay/i18n/kab.po` (201 lines)
- `addons/payment_ecpay/i18n/ko.po` (201 lines)
- `addons/payment_ecpay/i18n/ku.po` (201 lines)
- `addons/payment_ecpay/i18n/lo.po` (203 lines)
- `addons/payment_ecpay/i18n/lt.po` (203 lines)
- `addons/payment_ecpay/i18n/lv.po` (202 lines)
- `addons/payment_ecpay/i18n/mn.po` (201 lines)
- `addons/payment_ecpay/i18n/my.po` (201 lines)
- `addons/payment_ecpay/i18n/nb.po` (201 lines)
- `addons/payment_ecpay/i18n/nl.po` (207 lines)
- `addons/payment_ecpay/i18n/payment_ecpay.pot` (198 lines)
- `addons/payment_ecpay/i18n/pl.po` (207 lines)
- `addons/payment_ecpay/i18n/pt.po` (201 lines)
- `addons/payment_ecpay/i18n/pt_BR.po` (207 lines)
- `addons/payment_ecpay/i18n/ro.po` (202 lines)
- `addons/payment_ecpay/i18n/ru.po` (205 lines)
- `addons/payment_ecpay/i18n/sk.po` (201 lines)
- `addons/payment_ecpay/i18n/sl.po` (202 lines)
- `addons/payment_ecpay/i18n/sr@latin.po` (202 lines)
- `addons/payment_ecpay/i18n/sv.po` (202 lines)
- `addons/payment_ecpay/i18n/th.po` (203 lines)
- `addons/payment_ecpay/i18n/tr.po` (201 lines)
- `addons/payment_ecpay/i18n/uk.po` (202 lines)
- `addons/payment_ecpay/i18n/uz.po` (201 lines)
- `addons/payment_ecpay/i18n/vi.po` (201 lines)
- `addons/payment_ecpay/i18n/zh_CN.po` (203 lines)
- `addons/payment_ecpay/i18n/zh_TW.po` (202 lines)
- `addons/payment_ecpay/models/__init__.py` (3 lines)
- `addons/payment_ecpay/models/payment_provider.py` (107 lines)
- `addons/payment_ecpay/models/payment_transaction.py` (138 lines)
- `addons/payment_ecpay/static/description/icon.png` (77 lines)
- `addons/payment_ecpay/tests/__init__.py` (3 lines)
- `addons/payment_ecpay/tests/common.py` (36 lines)
- `addons/payment_ecpay/tests/test_payment_transaction.py` (122 lines)
- `addons/payment_ecpay/tests/test_processing_flows.py` (70 lines)
- `addons/payment_ecpay/views/payment_provider_views.xml` (34 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
