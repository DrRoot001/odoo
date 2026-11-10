# Module: payment_iyzico

- **Module ID:** MOD-403
- **Path:** `addons/payment_iyzico`
- **Manifest:** `addons/payment_iyzico/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering Turkey.

 

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
    "data/payment_method_data.xml",
    "data/payment_provider_data.xml",
    "views/payment_provider_views.xml"
  ]
}
```

### Representative source files

- `addons/payment_iyzico/README.md` (29 lines)
- `addons/payment_iyzico/__init__.py` (12 lines)
- `addons/payment_iyzico/__manifest__.py` (19 lines)
- `addons/payment_iyzico/const.py` (27 lines)
- `addons/payment_iyzico/controllers/__init__.py` (3 lines)
- `addons/payment_iyzico/controllers/main.py` (96 lines)
- `addons/payment_iyzico/data/neutralize.sql` (4 lines)
- `addons/payment_iyzico/data/payment_method_data.xml` (57 lines)
- `addons/payment_iyzico/data/payment_provider_data.xml` (9 lines)
- `addons/payment_iyzico/i18n/ar.po` (145 lines)
- `addons/payment_iyzico/i18n/az.po` (139 lines)
- `addons/payment_iyzico/i18n/bg.po` (139 lines)
- `addons/payment_iyzico/i18n/bs.po` (140 lines)
- `addons/payment_iyzico/i18n/ca.po` (142 lines)
- `addons/payment_iyzico/i18n/cs.po` (139 lines)
- `addons/payment_iyzico/i18n/da.po` (140 lines)
- `addons/payment_iyzico/i18n/de.po` (144 lines)
- `addons/payment_iyzico/i18n/el.po` (139 lines)
- `addons/payment_iyzico/i18n/es.po` (144 lines)
- `addons/payment_iyzico/i18n/es_419.po` (145 lines)
- `addons/payment_iyzico/i18n/et.po` (139 lines)
- `addons/payment_iyzico/i18n/fa.po` (139 lines)
- `addons/payment_iyzico/i18n/fi.po` (144 lines)
- `addons/payment_iyzico/i18n/fr.po` (144 lines)
- `addons/payment_iyzico/i18n/he.po` (140 lines)
- `addons/payment_iyzico/i18n/hi.po` (139 lines)
- `addons/payment_iyzico/i18n/hr.po` (140 lines)
- `addons/payment_iyzico/i18n/hu.po` (139 lines)
- `addons/payment_iyzico/i18n/id.po` (144 lines)
- `addons/payment_iyzico/i18n/it.po` (144 lines)
- `addons/payment_iyzico/i18n/ja.po` (144 lines)
- `addons/payment_iyzico/i18n/kab.po` (139 lines)
- `addons/payment_iyzico/i18n/ko.po` (142 lines)
- `addons/payment_iyzico/i18n/ku.po` (139 lines)
- `addons/payment_iyzico/i18n/lo.po` (143 lines)
- `addons/payment_iyzico/i18n/lt.po` (141 lines)
- `addons/payment_iyzico/i18n/lv.po` (139 lines)
- `addons/payment_iyzico/i18n/mn.po` (139 lines)
- `addons/payment_iyzico/i18n/my.po` (139 lines)
- `addons/payment_iyzico/i18n/nb.po` (139 lines)
- `addons/payment_iyzico/i18n/nl.po` (144 lines)
- `addons/payment_iyzico/i18n/payment_iyzico.pot` (135 lines)
- `addons/payment_iyzico/i18n/pl.po` (145 lines)
- `addons/payment_iyzico/i18n/pt.po` (140 lines)
- `addons/payment_iyzico/i18n/pt_BR.po` (146 lines)
- `addons/payment_iyzico/i18n/ro.po` (140 lines)
- `addons/payment_iyzico/i18n/ru.po` (145 lines)
- `addons/payment_iyzico/i18n/sk.po` (138 lines)
- `addons/payment_iyzico/i18n/sl.po` (140 lines)
- `addons/payment_iyzico/i18n/sr@latin.po` (140 lines)
- `addons/payment_iyzico/i18n/sv.po` (144 lines)
- `addons/payment_iyzico/i18n/th.po` (142 lines)
- `addons/payment_iyzico/i18n/tr.po` (145 lines)
- `addons/payment_iyzico/i18n/uk.po` (140 lines)
- `addons/payment_iyzico/i18n/uz.po` (158 lines)
- `addons/payment_iyzico/i18n/vi.po` (140 lines)
- `addons/payment_iyzico/i18n/zh_CN.po` (143 lines)
- `addons/payment_iyzico/i18n/zh_TW.po` (139 lines)
- `addons/payment_iyzico/models/__init__.py` (3 lines)
- `addons/payment_iyzico/models/payment_provider.py` (120 lines)
- `addons/payment_iyzico/models/payment_transaction.py` (146 lines)
- `addons/payment_iyzico/static/description/icon.png` (13 lines)
- `addons/payment_iyzico/static/description/icon.svg` (19 lines)
- `addons/payment_iyzico/tests/__init__.py` (3 lines)
- `addons/payment_iyzico/tests/common.py` (25 lines)
- `addons/payment_iyzico/tests/test_payment_provider.py` (16 lines)
- `addons/payment_iyzico/tests/test_payment_transaction.py` (120 lines)
- `addons/payment_iyzico/tests/test_processing_flows.py` (66 lines)
- `addons/payment_iyzico/views/payment_provider_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
