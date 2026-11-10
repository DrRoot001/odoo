# Module: pos_event

- **Module ID:** MOD-430
- **Path:** `addons/pos_event`
- **Manifest:** `addons/pos_event/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Link module between Point of Sale and Event

No manifest description declared.

Declared dependencies: `point_of_sale`, `event_product`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 34 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "event_product"
  ],
  "data": [
    "data/point_of_sale_data.xml",
    "data/event_product_data.xml",
    "views/event_registration_views.xml",
    "views/event_event_views.xml",
    "views/pos_order_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_product_demo.xml",
    "data/point_of_sale_demo.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_event/static/src/**/*"
    ],
    "web.assets_tests": [
      "pos_event/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_event/static/tests/unit/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_event/__init__.py` (2 lines)
- `addons/pos_event/__manifest__.py` (34 lines)
- `addons/pos_event/data/event_product_data.xml` (9 lines)
- `addons/pos_event/data/event_product_demo.xml` (13 lines)
- `addons/pos_event/data/point_of_sale_data.xml` (9 lines)
- `addons/pos_event/data/point_of_sale_demo.xml` (8 lines)
- `addons/pos_event/i18n/ar.po` (415 lines)
- `addons/pos_event/i18n/az.po` (405 lines)
- `addons/pos_event/i18n/bg.po` (405 lines)
- `addons/pos_event/i18n/bs.po` (406 lines)
- `addons/pos_event/i18n/ca.po` (410 lines)
- `addons/pos_event/i18n/cs.po` (406 lines)
- `addons/pos_event/i18n/da.po` (413 lines)
- `addons/pos_event/i18n/de.po` (420 lines)
- `addons/pos_event/i18n/el.po` (406 lines)
- `addons/pos_event/i18n/es.po` (413 lines)
- `addons/pos_event/i18n/es_419.po` (416 lines)
- `addons/pos_event/i18n/et.po` (405 lines)
- `addons/pos_event/i18n/fa.po` (405 lines)
- `addons/pos_event/i18n/fi.po` (414 lines)
- `addons/pos_event/i18n/fr.po` (421 lines)
- `addons/pos_event/i18n/he.po` (410 lines)
- `addons/pos_event/i18n/hi.po` (405 lines)
- `addons/pos_event/i18n/hr.po` (406 lines)
- `addons/pos_event/i18n/hu.po` (406 lines)
- `addons/pos_event/i18n/id.po` (414 lines)
- `addons/pos_event/i18n/it.po` (418 lines)
- `addons/pos_event/i18n/ja.po` (412 lines)
- `addons/pos_event/i18n/kab.po` (405 lines)
- `addons/pos_event/i18n/ko.po` (411 lines)
- `addons/pos_event/i18n/ku.po` (405 lines)
- `addons/pos_event/i18n/lo.po` (410 lines)
- `addons/pos_event/i18n/lt.po` (407 lines)
- `addons/pos_event/i18n/lv.po` (405 lines)
- `addons/pos_event/i18n/mn.po` (405 lines)
- `addons/pos_event/i18n/my.po` (405 lines)
- `addons/pos_event/i18n/nb.po` (406 lines)
- `addons/pos_event/i18n/nl.po` (420 lines)
- `addons/pos_event/i18n/pl.po` (413 lines)
- `addons/pos_event/i18n/pos_event.pot` (402 lines)
- `addons/pos_event/i18n/pt.po` (415 lines)
- `addons/pos_event/i18n/pt_BR.po` (426 lines)
- `addons/pos_event/i18n/ro.po` (417 lines)
- `addons/pos_event/i18n/ru.po` (416 lines)
- `addons/pos_event/i18n/sk.po` (404 lines)
- `addons/pos_event/i18n/sl.po` (407 lines)
- `addons/pos_event/i18n/sr@latin.po` (407 lines)
- `addons/pos_event/i18n/sv.po` (407 lines)
- `addons/pos_event/i18n/th.po` (407 lines)
- `addons/pos_event/i18n/tr.po` (414 lines)
- `addons/pos_event/i18n/uk.po` (406 lines)
- `addons/pos_event/i18n/uz.po` (448 lines)
- `addons/pos_event/i18n/vi.po` (413 lines)
- `addons/pos_event/i18n/zh_CN.po` (415 lines)
- `addons/pos_event/i18n/zh_TW.po` (413 lines)
- `addons/pos_event/models/__init__.py` (12 lines)
- `addons/pos_event/models/event_event.py` (58 lines)
- `addons/pos_event/models/event_question.py` (20 lines)
- `addons/pos_event/models/event_question_answer.py` (20 lines)
- `addons/pos_event/models/event_registration.py` (86 lines)
- `addons/pos_event/models/event_registration_answer.py` (19 lines)
- `addons/pos_event/models/event_slot.py` (20 lines)
- `addons/pos_event/models/event_ticket.py` (26 lines)
- `addons/pos_event/models/pos_config.py` (25 lines)
- `addons/pos_event/models/pos_order.py` (71 lines)
- `addons/pos_event/models/pos_order_line.py` (15 lines)
- `addons/pos_event/models/pos_session.py` (12 lines)
- `addons/pos_event/security/ir.access.csv` (4 lines)
- `addons/pos_event/static/img/event_category.png` (126 lines)
- `addons/pos_event/static/src/app/components/popup/event_configurator_popup/event_configurator_popup.js` (150 lines)
- `addons/pos_event/static/src/app/components/popup/event_configurator_popup/event_configurator_popup.xml` (43 lines)
- `addons/pos_event/static/src/app/components/popup/event_registration_popup/event_registration_popup.js` (187 lines)
- `addons/pos_event/static/src/app/components/popup/event_registration_popup/event_registration_popup.xml` (53 lines)
- `addons/pos_event/static/src/app/components/popup/event_slot_selection_popup/event_slot_selection_popup.js` (91 lines)
- `addons/pos_event/static/src/app/components/popup/event_slot_selection_popup/event_slot_selection_popup.xml` (32 lines)
- `addons/pos_event/static/src/app/components/popup/print_popup/print_popup.js` (51 lines)
- `addons/pos_event/static/src/app/components/product_card/product_card.js` (50 lines)
- `addons/pos_event/static/src/app/components/product_card/product_card.xml` (23 lines)
- `addons/pos_event/static/src/app/models/data_service_options.js` (28 lines)
- `addons/pos_event/static/src/app/models/pos_order.js` (9 lines)
- `addons/pos_event/static/src/app/models/pos_order_line.js` (27 lines)
- `addons/pos_event/static/src/app/models/product_template.js` (21 lines)
- `addons/pos_event/static/src/app/screens/product_screen/order_summary/order_summary.js` (113 lines)
- `addons/pos_event/static/src/app/screens/product_screen/order_summary/order_summary.xml` (13 lines)
- `addons/pos_event/static/src/app/screens/product_screen/product_screen.js` (304 lines)
- `addons/pos_event/static/src/app/services/pos_store.js` (15 lines)
- `addons/pos_event/static/src/app/utils/event_util.js` (97 lines)
- `addons/pos_event/static/tests/tours/pos_event_tour.js` (334 lines)
- `addons/pos_event/static/tests/tours/pos_multi_slot_event_tour.js` (206 lines)
- `addons/pos_event/static/tests/tours/utils/event_tour_utils.js` (72 lines)
- `addons/pos_event/static/tests/tours/utils/slot_selection_screen_utils.js` (19 lines)
- `addons/pos_event/static/tests/unit/components/event_configurator_popup.test.js` (34 lines)
- `addons/pos_event/static/tests/unit/components/event_registration_popup.test.js` (137 lines)
- `addons/pos_event/static/tests/unit/components/event_slot_selection_popup.test.js` (32 lines)
- `addons/pos_event/static/tests/unit/components/product_card.test.js` (86 lines)
- `addons/pos_event/static/tests/unit/data/event_event.data.js` (115 lines)
- `addons/pos_event/static/tests/unit/data/event_event_ticket.data.js` (63 lines)
- `addons/pos_event/static/tests/unit/data/event_question.data.js` (79 lines)
- `addons/pos_event/static/tests/unit/data/event_question_answer.data.js` (30 lines)
- `addons/pos_event/static/tests/unit/data/event_registration.data.js` (26 lines)
- `addons/pos_event/static/tests/unit/data/event_registration_answer.data.js` (22 lines)
- `addons/pos_event/static/tests/unit/data/event_slot.data.js` (34 lines)
- `addons/pos_event/static/tests/unit/data/pos_order_line.data.js` (8 lines)
- `addons/pos_event/static/tests/unit/data/pos_session.data.js` (17 lines)
- `addons/pos_event/static/tests/unit/data/product_product.data.js` (16 lines)
- `addons/pos_event/static/tests/unit/data/product_template.data.js` (20 lines)
- `addons/pos_event/static/tests/unit/data_service_options.test.js` (74 lines)
- `addons/pos_event/static/tests/unit/services/pos_store.test.js` (18 lines)
- `addons/pos_event/tests/__init__.py` (2 lines)
- `addons/pos_event/tests/test_frontend.py` (396 lines)
- `addons/pos_event/views/event_event_views.xml` (30 lines)
- `addons/pos_event/views/event_registration_views.xml` (26 lines)
- `addons/pos_event/views/pos_order_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
