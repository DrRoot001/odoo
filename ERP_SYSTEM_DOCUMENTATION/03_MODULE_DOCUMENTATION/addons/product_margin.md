# Module: product_margin

- **Module ID:** MOD-473
- **Path:** `addons/product_margin`
- **Manifest:** `addons/product_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Adds a reporting menu in products that computes sales, purchases, margins and other interesting indicators based on invoices.
=============================================================================================================================

The wizard to launch the report has several options to help you get the data you need.


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "wizard/product_margin_view.xml",
    "views/product_product_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/product_margin/__init__.py` (5 lines)
- `addons/product_margin/__manifest__.py` (21 lines)
- `addons/product_margin/i18n/af.po` (339 lines)
- `addons/product_margin/i18n/am.po` (335 lines)
- `addons/product_margin/i18n/ar.po` (343 lines)
- `addons/product_margin/i18n/az.po` (342 lines)
- `addons/product_margin/i18n/bg.po` (351 lines)
- `addons/product_margin/i18n/bs.po` (343 lines)
- `addons/product_margin/i18n/ca.po` (354 lines)
- `addons/product_margin/i18n/cs.po` (346 lines)
- `addons/product_margin/i18n/da.po` (345 lines)
- `addons/product_margin/i18n/de.po` (356 lines)
- `addons/product_margin/i18n/el.po` (344 lines)
- `addons/product_margin/i18n/es.po` (359 lines)
- `addons/product_margin/i18n/es_419.po` (348 lines)
- `addons/product_margin/i18n/es_CL.po` (92 lines)
- `addons/product_margin/i18n/et.po` (348 lines)
- `addons/product_margin/i18n/eu.po` (337 lines)
- `addons/product_margin/i18n/fa.po` (346 lines)
- `addons/product_margin/i18n/fi.po` (349 lines)
- `addons/product_margin/i18n/fo.po` (337 lines)
- `addons/product_margin/i18n/fr.po` (352 lines)
- `addons/product_margin/i18n/fr_BE.po` (45 lines)
- `addons/product_margin/i18n/fr_CA.po` (66 lines)
- `addons/product_margin/i18n/gl.po` (337 lines)
- `addons/product_margin/i18n/gu.po` (339 lines)
- `addons/product_margin/i18n/he.po` (348 lines)
- `addons/product_margin/i18n/hi.po` (339 lines)
- `addons/product_margin/i18n/hr.po` (347 lines)
- `addons/product_margin/i18n/hu.po` (353 lines)
- `addons/product_margin/i18n/id.po` (343 lines)
- `addons/product_margin/i18n/is.po` (335 lines)
- `addons/product_margin/i18n/it.po` (348 lines)
- `addons/product_margin/i18n/ja.po` (343 lines)
- `addons/product_margin/i18n/ka.po` (337 lines)
- `addons/product_margin/i18n/kab.po` (339 lines)
- `addons/product_margin/i18n/km.po` (339 lines)
- `addons/product_margin/i18n/ko.po` (343 lines)
- `addons/product_margin/i18n/ku.po` (339 lines)
- `addons/product_margin/i18n/lo.po` (345 lines)
- `addons/product_margin/i18n/lt.po` (351 lines)
- `addons/product_margin/i18n/lv.po` (345 lines)
- `addons/product_margin/i18n/mk.po` (341 lines)
- `addons/product_margin/i18n/mn.po` (351 lines)
- `addons/product_margin/i18n/my.po` (340 lines)
- `addons/product_margin/i18n/nb.po` (343 lines)
- `addons/product_margin/i18n/nl.po` (359 lines)
- `addons/product_margin/i18n/pl.po` (353 lines)
- `addons/product_margin/i18n/product_margin.pot` (334 lines)
- `addons/product_margin/i18n/pt.po` (357 lines)
- `addons/product_margin/i18n/pt_BR.po` (357 lines)
- `addons/product_margin/i18n/ro.po` (349 lines)
- `addons/product_margin/i18n/ru.po` (344 lines)
- `addons/product_margin/i18n/sk.po` (346 lines)
- `addons/product_margin/i18n/sl.po` (348 lines)
- `addons/product_margin/i18n/sq.po` (337 lines)
- `addons/product_margin/i18n/sr@latin.po` (343 lines)
- `addons/product_margin/i18n/sv.po` (354 lines)
- `addons/product_margin/i18n/ta.po` (339 lines)
- `addons/product_margin/i18n/th.po` (344 lines)
- `addons/product_margin/i18n/tr.po` (353 lines)
- `addons/product_margin/i18n/uk.po` (347 lines)
- `addons/product_margin/i18n/uz.po` (411 lines)
- `addons/product_margin/i18n/vi.po` (343 lines)
- `addons/product_margin/i18n/zh_CN.po` (348 lines)
- `addons/product_margin/i18n/zh_TW.po` (343 lines)
- `addons/product_margin/models/__init__.py` (4 lines)
- `addons/product_margin/models/product_product.py` (219 lines)
- `addons/product_margin/security/ir.access.csv` (2 lines)
- `addons/product_margin/tests/__init__.py` (4 lines)
- `addons/product_margin/tests/test_product_margin.py` (308 lines)
- `addons/product_margin/views/product_product_views.xml` (89 lines)
- `addons/product_margin/wizard/__init__.py` (4 lines)
- `addons/product_margin/wizard/product_margin.py` (56 lines)
- `addons/product_margin/wizard/product_margin_view.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
