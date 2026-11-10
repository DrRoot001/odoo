# Module: purchase_alternative

- **Module ID:** MOD-494
- **Path:** `addons/purchase_alternative`
- **Manifest:** `addons/purchase_alternative/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This module allows you to manage your Purchase Alternative.
===========================================================

It helps users compare product lines across RFQs and decide to order specific products
from different vendors, enabling more flexible and cost-effective purchasing decisions.
create a call for tender by adding alternative requests for quotation to different vendors.
Make your choice by selecting the best combination of lead time, OTD and/or total amount.
By comparing product lines you can also decide to order some products from
one vendor and others from another vendor.


Declared dependencies: `purchase`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase"
  ],
  "data": [
    "views/purchase_views.xml",
    "wizard/purchase_alternative_warning.xml",
    "wizard/purchase_alternative_create.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/purchase_alternative_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "purchase_alternative/static/src/*/**.js",
      "purchase_alternative/static/src/*/**.scss",
      "purchase_alternative/static/src/*/**.xml"
    ]
  }
}
```

### Representative source files

- `addons/purchase_alternative/__init__.py` (4 lines)
- `addons/purchase_alternative/__manifest__.py` (34 lines)
- `addons/purchase_alternative/data/purchase_alternative_demo.xml` (37 lines)
- `addons/purchase_alternative/i18n/ar.po` (342 lines)
- `addons/purchase_alternative/i18n/az.po` (341 lines)
- `addons/purchase_alternative/i18n/bg.po` (341 lines)
- `addons/purchase_alternative/i18n/bs.po` (342 lines)
- `addons/purchase_alternative/i18n/ca.po` (341 lines)
- `addons/purchase_alternative/i18n/cs.po` (341 lines)
- `addons/purchase_alternative/i18n/da.po` (341 lines)
- `addons/purchase_alternative/i18n/de.po` (376 lines)
- `addons/purchase_alternative/i18n/el.po` (341 lines)
- `addons/purchase_alternative/i18n/es.po` (342 lines)
- `addons/purchase_alternative/i18n/es_419.po` (379 lines)
- `addons/purchase_alternative/i18n/et.po` (366 lines)
- `addons/purchase_alternative/i18n/fa.po` (341 lines)
- `addons/purchase_alternative/i18n/fi.po` (356 lines)
- `addons/purchase_alternative/i18n/fr.po` (362 lines)
- `addons/purchase_alternative/i18n/he.po` (342 lines)
- `addons/purchase_alternative/i18n/hi.po` (341 lines)
- `addons/purchase_alternative/i18n/hr.po` (342 lines)
- `addons/purchase_alternative/i18n/hu.po` (341 lines)
- `addons/purchase_alternative/i18n/id.po` (342 lines)
- `addons/purchase_alternative/i18n/it.po` (376 lines)
- `addons/purchase_alternative/i18n/ja.po` (353 lines)
- `addons/purchase_alternative/i18n/kab.po` (341 lines)
- `addons/purchase_alternative/i18n/ko.po` (342 lines)
- `addons/purchase_alternative/i18n/ku.po` (341 lines)
- `addons/purchase_alternative/i18n/lo.po` (361 lines)
- `addons/purchase_alternative/i18n/lt.po` (343 lines)
- `addons/purchase_alternative/i18n/lv.po` (342 lines)
- `addons/purchase_alternative/i18n/mn.po` (341 lines)
- `addons/purchase_alternative/i18n/my.po` (342 lines)
- `addons/purchase_alternative/i18n/nb.po` (341 lines)
- `addons/purchase_alternative/i18n/nl.po` (376 lines)
- `addons/purchase_alternative/i18n/pl.po` (342 lines)
- `addons/purchase_alternative/i18n/pt.po` (341 lines)
- `addons/purchase_alternative/i18n/pt_BR.po` (376 lines)
- `addons/purchase_alternative/i18n/purchase_alternative.pot` (334 lines)
- `addons/purchase_alternative/i18n/ro.po` (342 lines)
- `addons/purchase_alternative/i18n/ru.po` (342 lines)
- `addons/purchase_alternative/i18n/sk.po` (341 lines)
- `addons/purchase_alternative/i18n/sl.po` (342 lines)
- `addons/purchase_alternative/i18n/sr@latin.po` (342 lines)
- `addons/purchase_alternative/i18n/sv.po` (342 lines)
- `addons/purchase_alternative/i18n/th.po` (342 lines)
- `addons/purchase_alternative/i18n/tr.po` (341 lines)
- `addons/purchase_alternative/i18n/uk.po` (342 lines)
- `addons/purchase_alternative/i18n/uz.po` (341 lines)
- `addons/purchase_alternative/i18n/vi.po` (348 lines)
- `addons/purchase_alternative/i18n/zh_CN.po` (350 lines)
- `addons/purchase_alternative/i18n/zh_TW.po` (341 lines)
- `addons/purchase_alternative/models/__init__.py` (3 lines)
- `addons/purchase_alternative/models/purchase.py` (211 lines)
- `addons/purchase_alternative/security/ir.access.csv` (4 lines)
- `addons/purchase_alternative/static/src/views/purchase_order_line_compare_list_renderer.js` (51 lines)
- `addons/purchase_alternative/static/src/views/purchase_order_line_compare_list_view.js` (11 lines)
- `addons/purchase_alternative/static/src/widgets/purchase_order_alternatives_widget.js` (51 lines)
- `addons/purchase_alternative/static/src/widgets/purchase_order_alternatives_widget.scss` (3 lines)
- `addons/purchase_alternative/static/src/widgets/purchase_order_alternatives_widget.xml` (11 lines)
- `addons/purchase_alternative/tests/__init__.py` (4 lines)
- `addons/purchase_alternative/tests/common.py` (32 lines)
- `addons/purchase_alternative/tests/test_purchase_alternative.py` (619 lines)
- `addons/purchase_alternative/views/purchase_views.xml` (73 lines)
- `addons/purchase_alternative/wizard/__init__.py` (2 lines)
- `addons/purchase_alternative/wizard/purchase_alternative_create.py` (99 lines)
- `addons/purchase_alternative/wizard/purchase_alternative_create.xml` (27 lines)
- `addons/purchase_alternative/wizard/purchase_alternative_warning.py` (22 lines)
- `addons/purchase_alternative/wizard/purchase_alternative_warning.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
