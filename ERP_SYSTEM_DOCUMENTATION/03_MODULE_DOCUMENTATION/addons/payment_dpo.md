# Module: payment_dpo

- **Module ID:** MOD-400
- **Path:** `addons/payment_dpo`
- **Manifest:** `addons/payment_dpo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A Kenyan payment provider covering several African countries.

 

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
| Route declarations | 1 | Static decorator matches. |

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

- `addons/payment_dpo/README.md` (23 lines)
- `addons/payment_dpo/__init__.py` (12 lines)
- `addons/payment_dpo/__manifest__.py` (19 lines)
- `addons/payment_dpo/const.py` (17 lines)
- `addons/payment_dpo/controllers/__init__.py` (3 lines)
- `addons/payment_dpo/controllers/main.py` (60 lines)
- `addons/payment_dpo/data/neutralize.sql` (4 lines)
- `addons/payment_dpo/data/payment_method_data.xml` (75 lines)
- `addons/payment_dpo/data/payment_provider_data.xml` (9 lines)
- `addons/payment_dpo/i18n/ar.po` (129 lines)
- `addons/payment_dpo/i18n/az.po` (125 lines)
- `addons/payment_dpo/i18n/bg.po` (125 lines)
- `addons/payment_dpo/i18n/bs.po` (127 lines)
- `addons/payment_dpo/i18n/ca.po` (128 lines)
- `addons/payment_dpo/i18n/cs.po` (126 lines)
- `addons/payment_dpo/i18n/da.po` (125 lines)
- `addons/payment_dpo/i18n/de.po` (129 lines)
- `addons/payment_dpo/i18n/el.po` (125 lines)
- `addons/payment_dpo/i18n/es.po` (128 lines)
- `addons/payment_dpo/i18n/es_419.po` (129 lines)
- `addons/payment_dpo/i18n/et.po` (125 lines)
- `addons/payment_dpo/i18n/fa.po` (125 lines)
- `addons/payment_dpo/i18n/fi.po` (128 lines)
- `addons/payment_dpo/i18n/fr.po` (128 lines)
- `addons/payment_dpo/i18n/he.po` (126 lines)
- `addons/payment_dpo/i18n/hi.po` (125 lines)
- `addons/payment_dpo/i18n/hr.po` (126 lines)
- `addons/payment_dpo/i18n/hu.po` (125 lines)
- `addons/payment_dpo/i18n/id.po` (128 lines)
- `addons/payment_dpo/i18n/it.po` (128 lines)
- `addons/payment_dpo/i18n/ja.po` (128 lines)
- `addons/payment_dpo/i18n/kab.po` (126 lines)
- `addons/payment_dpo/i18n/ko.po` (128 lines)
- `addons/payment_dpo/i18n/ku.po` (125 lines)
- `addons/payment_dpo/i18n/lo.po` (128 lines)
- `addons/payment_dpo/i18n/lt.po` (127 lines)
- `addons/payment_dpo/i18n/lv.po` (126 lines)
- `addons/payment_dpo/i18n/mn.po` (125 lines)
- `addons/payment_dpo/i18n/my.po` (125 lines)
- `addons/payment_dpo/i18n/nb.po` (125 lines)
- `addons/payment_dpo/i18n/nl.po` (128 lines)
- `addons/payment_dpo/i18n/payment_dpo.pot` (122 lines)
- `addons/payment_dpo/i18n/pl.po` (129 lines)
- `addons/payment_dpo/i18n/pt.po` (125 lines)
- `addons/payment_dpo/i18n/pt_BR.po` (131 lines)
- `addons/payment_dpo/i18n/ro.po` (129 lines)
- `addons/payment_dpo/i18n/ru.po` (129 lines)
- `addons/payment_dpo/i18n/sk.po` (125 lines)
- `addons/payment_dpo/i18n/sl.po` (126 lines)
- `addons/payment_dpo/i18n/sr@latin.po` (126 lines)
- `addons/payment_dpo/i18n/sv.po` (128 lines)
- `addons/payment_dpo/i18n/th.po` (128 lines)
- `addons/payment_dpo/i18n/tr.po` (130 lines)
- `addons/payment_dpo/i18n/uk.po` (126 lines)
- `addons/payment_dpo/i18n/uz.po` (148 lines)
- `addons/payment_dpo/i18n/vi.po` (126 lines)
- `addons/payment_dpo/i18n/zh_CN.po` (128 lines)
- `addons/payment_dpo/i18n/zh_TW.po` (131 lines)
- `addons/payment_dpo/models/__init__.py` (3 lines)
- `addons/payment_dpo/models/payment_provider.py` (54 lines)
- `addons/payment_dpo/models/payment_transaction.py` (136 lines)
- `addons/payment_dpo/static/description/icon.png` (507 lines)
- `addons/payment_dpo/static/description/icon.svg` (1 lines)
- `addons/payment_dpo/tests/__init__.py` (3 lines)
- `addons/payment_dpo/tests/common.py` (23 lines)
- `addons/payment_dpo/tests/test_payment_transaction.py` (39 lines)
- `addons/payment_dpo/tests/test_processing_flows.py` (25 lines)
- `addons/payment_dpo/views/payment_provider_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
