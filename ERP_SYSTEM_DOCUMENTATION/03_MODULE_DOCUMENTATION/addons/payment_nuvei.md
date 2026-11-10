# Module: payment_nuvei

- **Module ID:** MOD-406
- **Path:** `addons/payment_nuvei`
- **Manifest:** `addons/payment_nuvei/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A payment provider covering Latin America.

 

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

- `addons/payment_nuvei/README.md` (43 lines)
- `addons/payment_nuvei/__init__.py` (12 lines)
- `addons/payment_nuvei/__manifest__.py` (19 lines)
- `addons/payment_nuvei/const.py` (43 lines)
- `addons/payment_nuvei/controllers/__init__.py` (3 lines)
- `addons/payment_nuvei/controllers/main.py` (71 lines)
- `addons/payment_nuvei/data/neutralize.sql` (5 lines)
- `addons/payment_nuvei/data/payment_method_data.xml` (212 lines)
- `addons/payment_nuvei/data/payment_provider_data.xml` (9 lines)
- `addons/payment_nuvei/i18n/ar.po` (249 lines)
- `addons/payment_nuvei/i18n/az.po` (247 lines)
- `addons/payment_nuvei/i18n/bg.po` (247 lines)
- `addons/payment_nuvei/i18n/bs.po` (248 lines)
- `addons/payment_nuvei/i18n/ca.po` (248 lines)
- `addons/payment_nuvei/i18n/cs.po` (248 lines)
- `addons/payment_nuvei/i18n/da.po` (249 lines)
- `addons/payment_nuvei/i18n/de.po` (250 lines)
- `addons/payment_nuvei/i18n/el.po` (248 lines)
- `addons/payment_nuvei/i18n/es.po` (253 lines)
- `addons/payment_nuvei/i18n/es_419.po` (252 lines)
- `addons/payment_nuvei/i18n/et.po` (247 lines)
- `addons/payment_nuvei/i18n/fa.po` (247 lines)
- `addons/payment_nuvei/i18n/fi.po` (249 lines)
- `addons/payment_nuvei/i18n/fr.po` (250 lines)
- `addons/payment_nuvei/i18n/he.po` (248 lines)
- `addons/payment_nuvei/i18n/hi.po` (247 lines)
- `addons/payment_nuvei/i18n/hr.po` (248 lines)
- `addons/payment_nuvei/i18n/hu.po` (248 lines)
- `addons/payment_nuvei/i18n/id.po` (248 lines)
- `addons/payment_nuvei/i18n/it.po` (250 lines)
- `addons/payment_nuvei/i18n/ja.po` (248 lines)
- `addons/payment_nuvei/i18n/kab.po` (247 lines)
- `addons/payment_nuvei/i18n/ko.po` (249 lines)
- `addons/payment_nuvei/i18n/ku.po` (247 lines)
- `addons/payment_nuvei/i18n/lo.po` (247 lines)
- `addons/payment_nuvei/i18n/lt.po` (249 lines)
- `addons/payment_nuvei/i18n/lv.po` (247 lines)
- `addons/payment_nuvei/i18n/mn.po` (247 lines)
- `addons/payment_nuvei/i18n/my.po` (247 lines)
- `addons/payment_nuvei/i18n/nb.po` (248 lines)
- `addons/payment_nuvei/i18n/nl.po` (251 lines)
- `addons/payment_nuvei/i18n/payment_nuvei.pot` (244 lines)
- `addons/payment_nuvei/i18n/pl.po` (252 lines)
- `addons/payment_nuvei/i18n/pt.po` (250 lines)
- `addons/payment_nuvei/i18n/pt_BR.po` (251 lines)
- `addons/payment_nuvei/i18n/ro.po` (249 lines)
- `addons/payment_nuvei/i18n/ru.po` (249 lines)
- `addons/payment_nuvei/i18n/sk.po` (246 lines)
- `addons/payment_nuvei/i18n/sl.po` (249 lines)
- `addons/payment_nuvei/i18n/sr@latin.po` (248 lines)
- `addons/payment_nuvei/i18n/sv.po` (249 lines)
- `addons/payment_nuvei/i18n/th.po` (249 lines)
- `addons/payment_nuvei/i18n/tr.po` (248 lines)
- `addons/payment_nuvei/i18n/uk.po` (249 lines)
- `addons/payment_nuvei/i18n/uz.po` (274 lines)
- `addons/payment_nuvei/i18n/vi.po` (250 lines)
- `addons/payment_nuvei/i18n/zh_CN.po` (250 lines)
- `addons/payment_nuvei/i18n/zh_TW.po` (250 lines)
- `addons/payment_nuvei/models/__init__.py` (3 lines)
- `addons/payment_nuvei/models/payment_provider.py` (77 lines)
- `addons/payment_nuvei/models/payment_transaction.py` (170 lines)
- `addons/payment_nuvei/static/description/icon.png` (25 lines)
- `addons/payment_nuvei/static/description/icon.svg` (1 lines)
- `addons/payment_nuvei/tests/__init__.py` (3 lines)
- `addons/payment_nuvei/tests/common.py` (39 lines)
- `addons/payment_nuvei/tests/test_payment_provider.py` (44 lines)
- `addons/payment_nuvei/tests/test_payment_transaction.py` (173 lines)
- `addons/payment_nuvei/tests/test_processing_flows.py` (96 lines)
- `addons/payment_nuvei/views/payment_provider_views.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
