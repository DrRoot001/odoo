# Module: payment_payu

- **Module ID:** MOD-409
- **Path:** `addons/payment_payu`
- **Manifest:** `addons/payment_payu/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering India.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 3 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "payment"
  ],
  "data": [
    "views/payment_payu_templates.xml",
    "views/payment_provider_views.xml",
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml"
  ]
}
```

### Representative source files

- `addons/payment_payu/README.md` (46 lines)
- `addons/payment_payu/__init__.py` (12 lines)
- `addons/payment_payu/__manifest__.py` (20 lines)
- `addons/payment_payu/const.py` (89 lines)
- `addons/payment_payu/controllers/__init__.py` (3 lines)
- `addons/payment_payu/controllers/main.py` (61 lines)
- `addons/payment_payu/controllers/onboarding.py` (84 lines)
- `addons/payment_payu/data/neutralize.sql` (4 lines)
- `addons/payment_payu/data/payment_method_data.xml` (97 lines)
- `addons/payment_payu/data/payment_provider_data.xml` (9 lines)
- `addons/payment_payu/i18n/ar.po` (207 lines)
- `addons/payment_payu/i18n/az.po` (203 lines)
- `addons/payment_payu/i18n/bg.po` (203 lines)
- `addons/payment_payu/i18n/bs.po` (203 lines)
- `addons/payment_payu/i18n/ca.po` (203 lines)
- `addons/payment_payu/i18n/cs.po` (203 lines)
- `addons/payment_payu/i18n/da.po` (203 lines)
- `addons/payment_payu/i18n/de.po` (211 lines)
- `addons/payment_payu/i18n/el.po` (203 lines)
- `addons/payment_payu/i18n/es.po` (206 lines)
- `addons/payment_payu/i18n/es_419.po` (209 lines)
- `addons/payment_payu/i18n/et.po` (203 lines)
- `addons/payment_payu/i18n/fa.po` (203 lines)
- `addons/payment_payu/i18n/fi.po` (206 lines)
- `addons/payment_payu/i18n/fr.po` (203 lines)
- `addons/payment_payu/i18n/he.po` (203 lines)
- `addons/payment_payu/i18n/hi.po` (203 lines)
- `addons/payment_payu/i18n/hr.po` (203 lines)
- `addons/payment_payu/i18n/hu.po` (203 lines)
- `addons/payment_payu/i18n/id.po` (203 lines)
- `addons/payment_payu/i18n/it.po` (206 lines)
- `addons/payment_payu/i18n/ja.po` (203 lines)
- `addons/payment_payu/i18n/kab.po` (203 lines)
- `addons/payment_payu/i18n/ko.po` (203 lines)
- `addons/payment_payu/i18n/ku.po` (203 lines)
- `addons/payment_payu/i18n/lo.po` (208 lines)
- `addons/payment_payu/i18n/lt.po` (203 lines)
- `addons/payment_payu/i18n/lv.po` (203 lines)
- `addons/payment_payu/i18n/mn.po` (203 lines)
- `addons/payment_payu/i18n/my.po` (203 lines)
- `addons/payment_payu/i18n/nb.po` (203 lines)
- `addons/payment_payu/i18n/nl.po` (209 lines)
- `addons/payment_payu/i18n/payment_payu.pot` (202 lines)
- `addons/payment_payu/i18n/pl.po` (203 lines)
- `addons/payment_payu/i18n/pt.po` (203 lines)
- `addons/payment_payu/i18n/pt_BR.po` (210 lines)
- `addons/payment_payu/i18n/ro.po` (203 lines)
- `addons/payment_payu/i18n/ru.po` (203 lines)
- `addons/payment_payu/i18n/sk.po` (203 lines)
- `addons/payment_payu/i18n/sl.po` (203 lines)
- `addons/payment_payu/i18n/sr@latin.po` (203 lines)
- `addons/payment_payu/i18n/sv.po` (206 lines)
- `addons/payment_payu/i18n/th.po` (203 lines)
- `addons/payment_payu/i18n/tr.po` (203 lines)
- `addons/payment_payu/i18n/uk.po` (203 lines)
- `addons/payment_payu/i18n/uz.po` (203 lines)
- `addons/payment_payu/i18n/vi.po` (203 lines)
- `addons/payment_payu/i18n/zh_CN.po` (207 lines)
- `addons/payment_payu/i18n/zh_TW.po` (203 lines)
- `addons/payment_payu/models/__init__.py` (3 lines)
- `addons/payment_payu/models/payment_provider.py` (156 lines)
- `addons/payment_payu/models/payment_transaction.py` (108 lines)
- `addons/payment_payu/static/description/icon.png` (22 lines)
- `addons/payment_payu/tests/__init__.py` (3 lines)
- `addons/payment_payu/tests/common.py` (27 lines)
- `addons/payment_payu/tests/test_payment_provider.py` (28 lines)
- `addons/payment_payu/tests/test_payment_transaction.py` (67 lines)
- `addons/payment_payu/tests/test_processing_flows.py` (57 lines)
- `addons/payment_payu/views/payment_payu_templates.xml` (23 lines)
- `addons/payment_payu/views/payment_provider_views.xml` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
