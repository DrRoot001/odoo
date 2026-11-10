# Module: payment_redsys

- **Module ID:** MOD-411
- **Path:** `addons/payment_redsys`
- **Manifest:** `addons/payment_redsys/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering the Spanish market.

 

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

- `addons/payment_redsys/README.md` (36 lines)
- `addons/payment_redsys/__init__.py` (12 lines)
- `addons/payment_redsys/__manifest__.py` (19 lines)
- `addons/payment_redsys/const.py` (48 lines)
- `addons/payment_redsys/controllers/__init__.py` (3 lines)
- `addons/payment_redsys/controllers/main.py` (61 lines)
- `addons/payment_redsys/data/neutralize.sql` (5 lines)
- `addons/payment_redsys/data/payment_method_data.xml` (75 lines)
- `addons/payment_redsys/data/payment_provider_data.xml` (10 lines)
- `addons/payment_redsys/i18n/ar.po` (187 lines)
- `addons/payment_redsys/i18n/az.po` (184 lines)
- `addons/payment_redsys/i18n/bg.po` (185 lines)
- `addons/payment_redsys/i18n/bs.po` (186 lines)
- `addons/payment_redsys/i18n/ca.po` (195 lines)
- `addons/payment_redsys/i18n/cs.po` (187 lines)
- `addons/payment_redsys/i18n/da.po` (192 lines)
- `addons/payment_redsys/i18n/de.po` (187 lines)
- `addons/payment_redsys/i18n/el.po` (185 lines)
- `addons/payment_redsys/i18n/es.po` (184 lines)
- `addons/payment_redsys/i18n/es_419.po` (185 lines)
- `addons/payment_redsys/i18n/et.po` (186 lines)
- `addons/payment_redsys/i18n/fa.po` (186 lines)
- `addons/payment_redsys/i18n/fi.po` (184 lines)
- `addons/payment_redsys/i18n/fr.po` (186 lines)
- `addons/payment_redsys/i18n/he.po` (189 lines)
- `addons/payment_redsys/i18n/hi.po` (193 lines)
- `addons/payment_redsys/i18n/hr.po` (187 lines)
- `addons/payment_redsys/i18n/hu.po` (185 lines)
- `addons/payment_redsys/i18n/id.po` (187 lines)
- `addons/payment_redsys/i18n/it.po` (187 lines)
- `addons/payment_redsys/i18n/ja.po` (184 lines)
- `addons/payment_redsys/i18n/kab.po` (184 lines)
- `addons/payment_redsys/i18n/ko.po` (186 lines)
- `addons/payment_redsys/i18n/ku.po` (183 lines)
- `addons/payment_redsys/i18n/lo.po` (186 lines)
- `addons/payment_redsys/i18n/lt.po` (187 lines)
- `addons/payment_redsys/i18n/lv.po` (187 lines)
- `addons/payment_redsys/i18n/mn.po` (185 lines)
- `addons/payment_redsys/i18n/my.po` (184 lines)
- `addons/payment_redsys/i18n/nb.po` (185 lines)
- `addons/payment_redsys/i18n/nl.po` (187 lines)
- `addons/payment_redsys/i18n/payment_redsys.pot` (175 lines)
- `addons/payment_redsys/i18n/pl.po` (185 lines)
- `addons/payment_redsys/i18n/pt.po` (195 lines)
- `addons/payment_redsys/i18n/pt_BR.po` (188 lines)
- `addons/payment_redsys/i18n/ro.po` (187 lines)
- `addons/payment_redsys/i18n/ru.po` (189 lines)
- `addons/payment_redsys/i18n/sk.po` (187 lines)
- `addons/payment_redsys/i18n/sl.po` (187 lines)
- `addons/payment_redsys/i18n/sr@latin.po` (185 lines)
- `addons/payment_redsys/i18n/sv.po` (185 lines)
- `addons/payment_redsys/i18n/th.po` (193 lines)
- `addons/payment_redsys/i18n/tr.po` (186 lines)
- `addons/payment_redsys/i18n/uk.po` (196 lines)
- `addons/payment_redsys/i18n/uz.po` (208 lines)
- `addons/payment_redsys/i18n/vi.po` (194 lines)
- `addons/payment_redsys/i18n/zh_CN.po` (187 lines)
- `addons/payment_redsys/i18n/zh_TW.po` (194 lines)
- `addons/payment_redsys/models/__init__.py` (3 lines)
- `addons/payment_redsys/models/payment_provider.py` (100 lines)
- `addons/payment_redsys/models/payment_transaction.py` (207 lines)
- `addons/payment_redsys/static/description/icon.png` (396 lines)
- `addons/payment_redsys/static/description/icon.svg` (33 lines)
- `addons/payment_redsys/tests/__init__.py` (3 lines)
- `addons/payment_redsys/tests/common.py` (42 lines)
- `addons/payment_redsys/tests/test_payment_transaction.py` (88 lines)
- `addons/payment_redsys/tests/test_processing_flows.py` (85 lines)
- `addons/payment_redsys/views/payment_provider_views.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
