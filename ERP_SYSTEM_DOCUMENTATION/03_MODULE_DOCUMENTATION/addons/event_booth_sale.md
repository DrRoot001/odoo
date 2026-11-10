# Module: event_booth_sale

- **Module ID:** MOD-066
- **Path:** `addons/event_booth_sale`
- **Manifest:** `addons/event_booth_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Manage event booths sale


Sell your event booths and track payments on sale orders.
    

Declared dependencies: `event_booth`, `event_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_booth",
    "event_sale"
  ],
  "data": [
    "data/product_data.xml",
    "data/event_booth_category_data.xml",
    "views/sale_order_views.xml",
    "views/event_type_booth_views.xml",
    "views/event_booth_category_views.xml",
    "views/event_booth_registration_views.xml",
    "views/event_booth_views.xml",
    "wizard/event_booth_configurator_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "event_booth_sale/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/event_booth_sale/__init__.py` (5 lines)
- `addons/event_booth_sale/__manifest__.py` (31 lines)
- `addons/event_booth_sale/data/event_booth_category_data.xml` (19 lines)
- `addons/event_booth_sale/data/product_data.xml` (15 lines)
- `addons/event_booth_sale/i18n/ar.po` (439 lines)
- `addons/event_booth_sale/i18n/az.po` (426 lines)
- `addons/event_booth_sale/i18n/bg.po` (425 lines)
- `addons/event_booth_sale/i18n/bs.po` (455 lines)
- `addons/event_booth_sale/i18n/ca.po` (438 lines)
- `addons/event_booth_sale/i18n/cs.po` (436 lines)
- `addons/event_booth_sale/i18n/da.po` (444 lines)
- `addons/event_booth_sale/i18n/de.po` (450 lines)
- `addons/event_booth_sale/i18n/el.po` (426 lines)
- `addons/event_booth_sale/i18n/es.po` (453 lines)
- `addons/event_booth_sale/i18n/es_419.po` (450 lines)
- `addons/event_booth_sale/i18n/et.po` (431 lines)
- `addons/event_booth_sale/i18n/event_booth_sale.pot` (422 lines)
- `addons/event_booth_sale/i18n/fa.po` (431 lines)
- `addons/event_booth_sale/i18n/fi.po` (453 lines)
- `addons/event_booth_sale/i18n/fr.po` (454 lines)
- `addons/event_booth_sale/i18n/he.po` (426 lines)
- `addons/event_booth_sale/i18n/hi.po` (430 lines)
- `addons/event_booth_sale/i18n/hr.po` (426 lines)
- `addons/event_booth_sale/i18n/hu.po` (425 lines)
- `addons/event_booth_sale/i18n/id.po` (445 lines)
- `addons/event_booth_sale/i18n/it.po` (452 lines)
- `addons/event_booth_sale/i18n/ja.po` (439 lines)
- `addons/event_booth_sale/i18n/kab.po` (449 lines)
- `addons/event_booth_sale/i18n/ko.po` (441 lines)
- `addons/event_booth_sale/i18n/ku.po` (425 lines)
- `addons/event_booth_sale/i18n/lo.po` (437 lines)
- `addons/event_booth_sale/i18n/lt.po` (427 lines)
- `addons/event_booth_sale/i18n/lv.po` (458 lines)
- `addons/event_booth_sale/i18n/mn.po` (425 lines)
- `addons/event_booth_sale/i18n/my.po` (426 lines)
- `addons/event_booth_sale/i18n/nb.po` (425 lines)
- `addons/event_booth_sale/i18n/nl.po` (445 lines)
- `addons/event_booth_sale/i18n/pl.po` (450 lines)
- `addons/event_booth_sale/i18n/pt.po` (445 lines)
- `addons/event_booth_sale/i18n/pt_BR.po` (447 lines)
- `addons/event_booth_sale/i18n/ro.po` (446 lines)
- `addons/event_booth_sale/i18n/ru.po` (448 lines)
- `addons/event_booth_sale/i18n/sk.po` (456 lines)
- `addons/event_booth_sale/i18n/sl.po` (448 lines)
- `addons/event_booth_sale/i18n/sr@latin.po` (426 lines)
- `addons/event_booth_sale/i18n/sv.po` (448 lines)
- `addons/event_booth_sale/i18n/th.po` (437 lines)
- `addons/event_booth_sale/i18n/tr.po` (445 lines)
- `addons/event_booth_sale/i18n/uk.po` (437 lines)
- `addons/event_booth_sale/i18n/uz.po` (518 lines)
- `addons/event_booth_sale/i18n/vi.po` (441 lines)
- `addons/event_booth_sale/i18n/zh_CN.po` (432 lines)
- `addons/event_booth_sale/i18n/zh_TW.po` (436 lines)
- `addons/event_booth_sale/models/__init__.py` (11 lines)
- `addons/event_booth_sale/models/account_move.py` (16 lines)
- `addons/event_booth_sale/models/event_booth.py` (49 lines)
- `addons/event_booth_sale/models/event_booth_category.py` (112 lines)
- `addons/event_booth_sale/models/event_booth_registration.py` (74 lines)
- `addons/event_booth_sale/models/event_type_booth.py` (17 lines)
- `addons/event_booth_sale/models/product_product.py` (25 lines)
- `addons/event_booth_sale/models/product_template.py` (43 lines)
- `addons/event_booth_sale/models/sale_order.py` (42 lines)
- `addons/event_booth_sale/models/sale_order_line.py` (106 lines)
- `addons/event_booth_sale/security/ir.access.csv` (5 lines)
- `addons/event_booth_sale/static/src/js/event_booth_configurator_controller.js` (38 lines)
- `addons/event_booth_sale/static/src/js/sale_product_mixin.js` (82 lines)
- `addons/event_booth_sale/tests/__init__.py` (5 lines)
- `addons/event_booth_sale/tests/common.py` (46 lines)
- `addons/event_booth_sale/tests/test_event_booth_sale.py` (213 lines)
- `addons/event_booth_sale/tests/test_event_internals.py` (95 lines)
- `addons/event_booth_sale/views/event_booth_category_views.xml` (39 lines)
- `addons/event_booth_sale/views/event_booth_registration_views.xml` (44 lines)
- `addons/event_booth_sale/views/event_booth_views.xml` (95 lines)
- `addons/event_booth_sale/views/event_type_booth_views.xml` (30 lines)
- `addons/event_booth_sale/views/sale_order_views.xml` (30 lines)
- `addons/event_booth_sale/wizard/__init__.py` (4 lines)
- `addons/event_booth_sale/wizard/event_booth_configurator.py` (34 lines)
- `addons/event_booth_sale/wizard/event_booth_configurator_views.xml` (44 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
