# Module: payment_mollie

- **Module ID:** MOD-405
- **Path:** `addons/payment_mollie`
- **Manifest:** `addons/payment_mollie/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A Dutch payment provider covering several European countries.

 

Declared dependencies: `payment`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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

- `addons/payment_mollie/README.md` (38 lines)
- `addons/payment_mollie/__init__.py` (12 lines)
- `addons/payment_mollie/__manifest__.py` (20 lines)
- `addons/payment_mollie/const.py` (76 lines)
- `addons/payment_mollie/controllers/__init__.py` (3 lines)
- `addons/payment_mollie/controllers/main.py` (80 lines)
- `addons/payment_mollie/data/neutralize.sql` (3 lines)
- `addons/payment_mollie/data/payment_method_data.xml` (460 lines)
- `addons/payment_mollie/data/payment_provider_data.xml` (10 lines)
- `addons/payment_mollie/i18n/ar.po` (241 lines)
- `addons/payment_mollie/i18n/az.po` (237 lines)
- `addons/payment_mollie/i18n/bg.po` (237 lines)
- `addons/payment_mollie/i18n/bs.po` (238 lines)
- `addons/payment_mollie/i18n/ca.po` (238 lines)
- `addons/payment_mollie/i18n/cs.po` (238 lines)
- `addons/payment_mollie/i18n/da.po` (239 lines)
- `addons/payment_mollie/i18n/de.po` (239 lines)
- `addons/payment_mollie/i18n/el.po` (238 lines)
- `addons/payment_mollie/i18n/es.po` (239 lines)
- `addons/payment_mollie/i18n/es_419.po` (238 lines)
- `addons/payment_mollie/i18n/et.po` (237 lines)
- `addons/payment_mollie/i18n/fa.po` (237 lines)
- `addons/payment_mollie/i18n/fi.po` (239 lines)
- `addons/payment_mollie/i18n/fr.po` (238 lines)
- `addons/payment_mollie/i18n/he.po` (238 lines)
- `addons/payment_mollie/i18n/hi.po` (237 lines)
- `addons/payment_mollie/i18n/hr.po` (238 lines)
- `addons/payment_mollie/i18n/hu.po` (238 lines)
- `addons/payment_mollie/i18n/id.po` (239 lines)
- `addons/payment_mollie/i18n/it.po` (239 lines)
- `addons/payment_mollie/i18n/ja.po` (238 lines)
- `addons/payment_mollie/i18n/kab.po` (237 lines)
- `addons/payment_mollie/i18n/ko.po` (239 lines)
- `addons/payment_mollie/i18n/ku.po` (237 lines)
- `addons/payment_mollie/i18n/lo.po` (238 lines)
- `addons/payment_mollie/i18n/lt.po` (239 lines)
- `addons/payment_mollie/i18n/lv.po` (237 lines)
- `addons/payment_mollie/i18n/mn.po` (237 lines)
- `addons/payment_mollie/i18n/my.po` (237 lines)
- `addons/payment_mollie/i18n/nb.po` (238 lines)
- `addons/payment_mollie/i18n/nl.po` (240 lines)
- `addons/payment_mollie/i18n/payment_mollie.pot` (234 lines)
- `addons/payment_mollie/i18n/pl.po` (241 lines)
- `addons/payment_mollie/i18n/pt.po` (240 lines)
- `addons/payment_mollie/i18n/pt_BR.po` (242 lines)
- `addons/payment_mollie/i18n/ro.po` (238 lines)
- `addons/payment_mollie/i18n/ru.po` (242 lines)
- `addons/payment_mollie/i18n/sk.po` (236 lines)
- `addons/payment_mollie/i18n/sl.po` (239 lines)
- `addons/payment_mollie/i18n/sr@latin.po` (238 lines)
- `addons/payment_mollie/i18n/sv.po` (239 lines)
- `addons/payment_mollie/i18n/th.po` (239 lines)
- `addons/payment_mollie/i18n/tr.po` (241 lines)
- `addons/payment_mollie/i18n/uk.po` (238 lines)
- `addons/payment_mollie/i18n/uz.po` (256 lines)
- `addons/payment_mollie/i18n/vi.po` (241 lines)
- `addons/payment_mollie/i18n/zh_CN.po` (240 lines)
- `addons/payment_mollie/i18n/zh_TW.po` (240 lines)
- `addons/payment_mollie/models/__init__.py` (3 lines)
- `addons/payment_mollie/models/payment_provider.py` (79 lines)
- `addons/payment_mollie/models/payment_token.py` (9 lines)
- `addons/payment_mollie/models/payment_transaction.py` (228 lines)
- `addons/payment_mollie/static/description/icon.png` (11 lines)
- `addons/payment_mollie/static/description/icon.svg` (1 lines)
- `addons/payment_mollie/static/description/icon_hi.png` (41 lines)
- `addons/payment_mollie/tests/__init__.py` (3 lines)
- `addons/payment_mollie/tests/common.py` (15 lines)
- `addons/payment_mollie/tests/test_mollie.py` (148 lines)
- `addons/payment_mollie/views/payment_provider_views.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
