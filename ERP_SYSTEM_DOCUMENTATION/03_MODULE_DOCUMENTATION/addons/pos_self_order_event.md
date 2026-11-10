# Module: pos_self_order_event

- **Module ID:** MOD-457
- **Path:** `addons/pos_self_order_event`
- **Manifest:** `addons/pos_self_order_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between PoS Self Order and PoS Event

No manifest description declared.

Declared dependencies: `pos_self_order`, `pos_event`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 14 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 2 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "pos_self_order",
    "pos_event"
  ],
  "assets": {
    "pos_self_order.assets": [
      "pos_self_order_event/static/src/**/*",
      "pos_event/static/src/app/models/**/*",
      "pos_event/static/src/app/utils/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_self_order_event/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_self_order_event/__init__.py` (4 lines)
- `addons/pos_self_order_event/__manifest__.py` (21 lines)
- `addons/pos_self_order_event/controllers/__init__.py` (3 lines)
- `addons/pos_self_order_event/controllers/main.py` (41 lines)
- `addons/pos_self_order_event/i18n/ar.po` (249 lines)
- `addons/pos_self_order_event/i18n/az.po` (248 lines)
- `addons/pos_self_order_event/i18n/bg.po` (248 lines)
- `addons/pos_self_order_event/i18n/bs.po` (249 lines)
- `addons/pos_self_order_event/i18n/ca.po` (248 lines)
- `addons/pos_self_order_event/i18n/cs.po` (249 lines)
- `addons/pos_self_order_event/i18n/da.po` (248 lines)
- `addons/pos_self_order_event/i18n/de.po` (254 lines)
- `addons/pos_self_order_event/i18n/el.po` (248 lines)
- `addons/pos_self_order_event/i18n/es.po` (252 lines)
- `addons/pos_self_order_event/i18n/es_419.po` (250 lines)
- `addons/pos_self_order_event/i18n/et.po` (248 lines)
- `addons/pos_self_order_event/i18n/fa.po` (248 lines)
- `addons/pos_self_order_event/i18n/fi.po` (249 lines)
- `addons/pos_self_order_event/i18n/fr.po` (252 lines)
- `addons/pos_self_order_event/i18n/he.po` (249 lines)
- `addons/pos_self_order_event/i18n/hi.po` (248 lines)
- `addons/pos_self_order_event/i18n/hr.po` (249 lines)
- `addons/pos_self_order_event/i18n/hu.po` (248 lines)
- `addons/pos_self_order_event/i18n/id.po` (252 lines)
- `addons/pos_self_order_event/i18n/it.po` (251 lines)
- `addons/pos_self_order_event/i18n/ja.po` (249 lines)
- `addons/pos_self_order_event/i18n/kab.po` (248 lines)
- `addons/pos_self_order_event/i18n/ko.po` (249 lines)
- `addons/pos_self_order_event/i18n/ku.po` (248 lines)
- `addons/pos_self_order_event/i18n/lo.po` (248 lines)
- `addons/pos_self_order_event/i18n/lt.po` (250 lines)
- `addons/pos_self_order_event/i18n/lv.po` (249 lines)
- `addons/pos_self_order_event/i18n/mn.po` (248 lines)
- `addons/pos_self_order_event/i18n/my.po` (248 lines)
- `addons/pos_self_order_event/i18n/nb.po` (248 lines)
- `addons/pos_self_order_event/i18n/nl.po` (251 lines)
- `addons/pos_self_order_event/i18n/pl.po` (249 lines)
- `addons/pos_self_order_event/i18n/pos_self_order_event.pot` (246 lines)
- `addons/pos_self_order_event/i18n/pt.po` (248 lines)
- `addons/pos_self_order_event/i18n/pt_BR.po` (252 lines)
- `addons/pos_self_order_event/i18n/ro.po` (249 lines)
- `addons/pos_self_order_event/i18n/ru.po` (249 lines)
- `addons/pos_self_order_event/i18n/sk.po` (248 lines)
- `addons/pos_self_order_event/i18n/sl.po` (249 lines)
- `addons/pos_self_order_event/i18n/sr@latin.po` (250 lines)
- `addons/pos_self_order_event/i18n/sv.po` (249 lines)
- `addons/pos_self_order_event/i18n/th.po` (249 lines)
- `addons/pos_self_order_event/i18n/tr.po` (248 lines)
- `addons/pos_self_order_event/i18n/uk.po` (249 lines)
- `addons/pos_self_order_event/i18n/uz.po` (248 lines)
- `addons/pos_self_order_event/i18n/vi.po` (248 lines)
- `addons/pos_self_order_event/i18n/zh_CN.po` (250 lines)
- `addons/pos_self_order_event/i18n/zh_TW.po` (248 lines)
- `addons/pos_self_order_event/models/__init__.py` (5 lines)
- `addons/pos_self_order_event/models/event_event.py` (18 lines)
- `addons/pos_self_order_event/models/pos_config.py` (11 lines)
- `addons/pos_self_order_event/models/pos_order.py` (96 lines)
- `addons/pos_self_order_event/static/src/app/components/product_card/product_card.js` (37 lines)
- `addons/pos_self_order_event/static/src/app/components/product_card/product_card.xml` (17 lines)
- `addons/pos_self_order_event/static/src/app/models/pos_category.js` (9 lines)
- `addons/pos_self_order_event/static/src/app/pages/cart_page/cart_page.js` (20 lines)
- `addons/pos_self_order_event/static/src/app/pages/confirmation_page/confirmation_page.js` (11 lines)
- `addons/pos_self_order_event/static/src/app/pages/confirmation_page/confirmation_page.xml` (13 lines)
- `addons/pos_self_order_event/static/src/app/pages/event_page/event_page.js` (462 lines)
- `addons/pos_self_order_event/static/src/app/pages/event_page/event_page.scss` (99 lines)
- `addons/pos_self_order_event/static/src/app/pages/event_page/event_page.xml` (234 lines)
- `addons/pos_self_order_event/static/src/app/pages/order_history_page/order_history_page.js` (35 lines)
- `addons/pos_self_order_event/static/src/app/pages/order_history_page/order_history_page.xml` (15 lines)
- `addons/pos_self_order_event/static/src/app/self_order_index.js` (10 lines)
- `addons/pos_self_order_event/static/src/app/self_order_index.xml` (10 lines)
- `addons/pos_self_order_event/static/src/app/services/card_utils.js` (28 lines)
- `addons/pos_self_order_event/static/src/app/services/self_order_service.js` (48 lines)
- `addons/pos_self_order_event/static/src/img/event_ticket_placeholder_thumbnail.png` (33 lines)
- `addons/pos_self_order_event/static/src/img/placeholder_thumbnail.png` (23 lines)
- `addons/pos_self_order_event/static/tests/unit/components/product_card.test.js` (65 lines)
- `addons/pos_self_order_event/static/tests/unit/data/pos_config.data.js` (17 lines)
- `addons/pos_self_order_event/static/tests/unit/pages/cart_page.test.js` (28 lines)
- `addons/pos_self_order_event/static/tests/unit/pages/event_page.test.js` (160 lines)
- `addons/pos_self_order_event/static/tests/unit/services/self_order_service.test.js` (19 lines)
- `addons/pos_self_order_event/tests/__init__.py` (3 lines)
- `addons/pos_self_order_event/tests/test_self_order_event.py` (156 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
