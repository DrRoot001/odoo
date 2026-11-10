# Module: payment_buckaroo

- **Module ID:** MOD-397
- **Path:** `addons/payment_buckaroo`
- **Manifest:** `addons/payment_buckaroo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

A Dutch payment provider covering several countries in Europe.

 

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

- `addons/payment_buckaroo/README.md` (27 lines)
- `addons/payment_buckaroo/__init__.py` (12 lines)
- `addons/payment_buckaroo/__manifest__.py` (20 lines)
- `addons/payment_buckaroo/const.py` (50 lines)
- `addons/payment_buckaroo/controllers/__init__.py` (3 lines)
- `addons/payment_buckaroo/controllers/main.py` (81 lines)
- `addons/payment_buckaroo/data/neutralize.sql` (4 lines)
- `addons/payment_buckaroo/data/payment_method_data.xml` (399 lines)
- `addons/payment_buckaroo/data/payment_provider_data.xml` (9 lines)
- `addons/payment_buckaroo/i18n/ar.po` (269 lines)
- `addons/payment_buckaroo/i18n/az.po` (268 lines)
- `addons/payment_buckaroo/i18n/bg.po` (270 lines)
- `addons/payment_buckaroo/i18n/bs.po` (270 lines)
- `addons/payment_buckaroo/i18n/ca.po` (272 lines)
- `addons/payment_buckaroo/i18n/cs.po` (269 lines)
- `addons/payment_buckaroo/i18n/da.po` (271 lines)
- `addons/payment_buckaroo/i18n/de.po` (270 lines)
- `addons/payment_buckaroo/i18n/el.po` (270 lines)
- `addons/payment_buckaroo/i18n/es.po` (268 lines)
- `addons/payment_buckaroo/i18n/es_419.po` (265 lines)
- `addons/payment_buckaroo/i18n/et.po` (275 lines)
- `addons/payment_buckaroo/i18n/fa.po` (273 lines)
- `addons/payment_buckaroo/i18n/fi.po` (269 lines)
- `addons/payment_buckaroo/i18n/fr.po` (267 lines)
- `addons/payment_buckaroo/i18n/he.po` (275 lines)
- `addons/payment_buckaroo/i18n/hi.po` (271 lines)
- `addons/payment_buckaroo/i18n/hr.po` (274 lines)
- `addons/payment_buckaroo/i18n/hu.po` (270 lines)
- `addons/payment_buckaroo/i18n/id.po` (267 lines)
- `addons/payment_buckaroo/i18n/is.po` (263 lines)
- `addons/payment_buckaroo/i18n/it.po` (269 lines)
- `addons/payment_buckaroo/i18n/ja.po` (268 lines)
- `addons/payment_buckaroo/i18n/kab.po` (267 lines)
- `addons/payment_buckaroo/i18n/ko.po` (267 lines)
- `addons/payment_buckaroo/i18n/ku.po` (267 lines)
- `addons/payment_buckaroo/i18n/lo.po` (264 lines)
- `addons/payment_buckaroo/i18n/lt.po` (269 lines)
- `addons/payment_buckaroo/i18n/lv.po` (271 lines)
- `addons/payment_buckaroo/i18n/mn.po` (271 lines)
- `addons/payment_buckaroo/i18n/my.po` (268 lines)
- `addons/payment_buckaroo/i18n/nb.po` (266 lines)
- `addons/payment_buckaroo/i18n/nl.po` (269 lines)
- `addons/payment_buckaroo/i18n/payment_buckaroo.pot` (259 lines)
- `addons/payment_buckaroo/i18n/pl.po` (273 lines)
- `addons/payment_buckaroo/i18n/pt.po` (269 lines)
- `addons/payment_buckaroo/i18n/pt_BR.po` (273 lines)
- `addons/payment_buckaroo/i18n/ro.po` (279 lines)
- `addons/payment_buckaroo/i18n/ru.po` (269 lines)
- `addons/payment_buckaroo/i18n/sk.po` (274 lines)
- `addons/payment_buckaroo/i18n/sl.po` (264 lines)
- `addons/payment_buckaroo/i18n/sr@latin.po` (270 lines)
- `addons/payment_buckaroo/i18n/sv.po` (269 lines)
- `addons/payment_buckaroo/i18n/th.po` (266 lines)
- `addons/payment_buckaroo/i18n/tr.po` (272 lines)
- `addons/payment_buckaroo/i18n/uk.po` (281 lines)
- `addons/payment_buckaroo/i18n/uz.po` (286 lines)
- `addons/payment_buckaroo/i18n/vi.po` (267 lines)
- `addons/payment_buckaroo/i18n/zh_CN.po` (269 lines)
- `addons/payment_buckaroo/i18n/zh_TW.po` (266 lines)
- `addons/payment_buckaroo/models/__init__.py` (3 lines)
- `addons/payment_buckaroo/models/payment_provider.py` (98 lines)
- `addons/payment_buckaroo/models/payment_transaction.py` (105 lines)
- `addons/payment_buckaroo/static/description/icon.png` (5 lines)
- `addons/payment_buckaroo/static/description/icon.svg` (1 lines)
- `addons/payment_buckaroo/static/description/icon_hi.png` (61 lines)
- `addons/payment_buckaroo/tests/__init__.py` (3 lines)
- `addons/payment_buckaroo/tests/common.py` (45 lines)
- `addons/payment_buckaroo/tests/test_buckaroo.py` (91 lines)
- `addons/payment_buckaroo/tests/test_processing_flows.py` (85 lines)
- `addons/payment_buckaroo/views/payment_provider_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
