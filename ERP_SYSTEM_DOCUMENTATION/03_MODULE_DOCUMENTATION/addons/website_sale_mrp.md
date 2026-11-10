# Module: website_sale_mrp

- **Module ID:** MOD-639
- **Path:** `addons/website_sale_mrp`
- **Manifest:** `addons/website_sale_mrp/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage Kit product inventory & availability


Manage the inventory of your Kit products and display their availability status in your eCommerce store.
    

Declared dependencies: `website_sale_stock`, `sale_mrp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale_stock",
    "sale_mrp"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale_mrp/static/src/interactions/**/*"
    ],
    "web.assets_tests": [
      "website_sale_mrp/static/tests/tours/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_mrp/__init__.py` (4 lines)
- `addons/website_sale_mrp/__manifest__.py` (25 lines)
- `addons/website_sale_mrp/controllers/__init__.py` (3 lines)
- `addons/website_sale_mrp/controllers/variant.py` (28 lines)
- `addons/website_sale_mrp/i18n/ar.po` (54 lines)
- `addons/website_sale_mrp/i18n/az.po` (52 lines)
- `addons/website_sale_mrp/i18n/bg.po` (52 lines)
- `addons/website_sale_mrp/i18n/bs.po` (53 lines)
- `addons/website_sale_mrp/i18n/ca.po` (52 lines)
- `addons/website_sale_mrp/i18n/cs.po` (53 lines)
- `addons/website_sale_mrp/i18n/da.po` (52 lines)
- `addons/website_sale_mrp/i18n/de.po` (57 lines)
- `addons/website_sale_mrp/i18n/el.po` (52 lines)
- `addons/website_sale_mrp/i18n/es.po` (53 lines)
- `addons/website_sale_mrp/i18n/es_419.po` (56 lines)
- `addons/website_sale_mrp/i18n/et.po` (52 lines)
- `addons/website_sale_mrp/i18n/fa.po` (52 lines)
- `addons/website_sale_mrp/i18n/fi.po` (53 lines)
- `addons/website_sale_mrp/i18n/fr.po` (53 lines)
- `addons/website_sale_mrp/i18n/he.po` (53 lines)
- `addons/website_sale_mrp/i18n/hi.po` (52 lines)
- `addons/website_sale_mrp/i18n/hr.po` (53 lines)
- `addons/website_sale_mrp/i18n/hu.po` (52 lines)
- `addons/website_sale_mrp/i18n/id.po` (53 lines)
- `addons/website_sale_mrp/i18n/it.po` (53 lines)
- `addons/website_sale_mrp/i18n/ja.po` (53 lines)
- `addons/website_sale_mrp/i18n/kab.po` (52 lines)
- `addons/website_sale_mrp/i18n/ko.po` (53 lines)
- `addons/website_sale_mrp/i18n/ku.po` (52 lines)
- `addons/website_sale_mrp/i18n/lo.po` (52 lines)
- `addons/website_sale_mrp/i18n/lt.po` (54 lines)
- `addons/website_sale_mrp/i18n/lv.po` (53 lines)
- `addons/website_sale_mrp/i18n/mn.po` (52 lines)
- `addons/website_sale_mrp/i18n/my.po` (52 lines)
- `addons/website_sale_mrp/i18n/nb.po` (52 lines)
- `addons/website_sale_mrp/i18n/nl.po` (53 lines)
- `addons/website_sale_mrp/i18n/pl.po` (54 lines)
- `addons/website_sale_mrp/i18n/pt.po` (52 lines)
- `addons/website_sale_mrp/i18n/pt_BR.po` (60 lines)
- `addons/website_sale_mrp/i18n/ro.po` (53 lines)
- `addons/website_sale_mrp/i18n/ru.po` (54 lines)
- `addons/website_sale_mrp/i18n/sk.po` (52 lines)
- `addons/website_sale_mrp/i18n/sl.po` (53 lines)
- `addons/website_sale_mrp/i18n/sr@latin.po` (53 lines)
- `addons/website_sale_mrp/i18n/sv.po` (53 lines)
- `addons/website_sale_mrp/i18n/th.po` (53 lines)
- `addons/website_sale_mrp/i18n/tr.po` (52 lines)
- `addons/website_sale_mrp/i18n/uk.po` (53 lines)
- `addons/website_sale_mrp/i18n/uz.po` (63 lines)
- `addons/website_sale_mrp/i18n/vi.po` (53 lines)
- `addons/website_sale_mrp/i18n/website_sale_mrp.pot` (48 lines)
- `addons/website_sale_mrp/i18n/zh_CN.po` (53 lines)
- `addons/website_sale_mrp/i18n/zh_TW.po` (53 lines)
- `addons/website_sale_mrp/models/__init__.py` (3 lines)
- `addons/website_sale_mrp/models/sale_order.py` (60 lines)
- `addons/website_sale_mrp/static/src/interactions/product_page.js` (16 lines)
- `addons/website_sale_mrp/static/tests/tours/test_website_sale_product_availability.js` (37 lines)
- `addons/website_sale_mrp/tests/__init__.py` (3 lines)
- `addons/website_sale_mrp/tests/test_website_sale_product_availability.py` (86 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
