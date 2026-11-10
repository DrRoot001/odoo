# Module: pos_restaurant

- **Module ID:** MOD-447
- **Path:** `addons/pos_restaurant`
- **Manifest:** `addons/pos_restaurant/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Restaurant extensions for the Point of Sale 



This module adds several features to the Point of Sale that are specific to restaurant management:
- Bill Printing: Allows you to print a receipt before the order is paid
- Bill Splitting: Allows you to split an order into different orders
- Kitchen Order Printing: allows you to print orders updates to kitchen or bar printers



Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 12 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 42 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 108 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "data/scenarios/restaurant_preset.xml",
    "views/pos_category_view.xml",
    "views/pos_course_views.xml",
    "views/pos_order_views.xml",
    "views/pos_restaurant_views.xml",
    "views/pos_preset_views.xml",
    "views/res_config_settings_views.xml",
    "receipt/pos_order_receipt.xml",
    "receipt/pos_order_change_receipt.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/demo_data.xml"
  ],
  "assets": {
    "point_of_sale._assets_pos": [
      "pos_restaurant/static/src/**/*",
      [
        "after",
        "point_of_sale/static/src/scss/pos.scss",
        "pos_restaurant/static/src/scss/restaurant.scss"
      ]
    ],
    "web.assets_backend": [
      "point_of_sale/static/src/scss/pos_dashboard.scss"
    ],
    "web.assets_tests": [
      "pos_restaurant/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "pos_restaurant/static/tests/unit/**/*"
    ],
    "point_of_sale.assets_debug": [
      "pos_restaurant/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/pos_restaurant/__init__.py` (17 lines)
- `addons/pos_restaurant/__manifest__.py` (65 lines)
- `addons/pos_restaurant/data/demo_data.xml` (7 lines)
- `addons/pos_restaurant/data/scenarios/bar_category_data.xml` (24 lines)
- `addons/pos_restaurant/data/scenarios/bar_demo_data.xml` (201 lines)
- `addons/pos_restaurant/data/scenarios/restaurant_category_data.xml` (21 lines)
- `addons/pos_restaurant/data/scenarios/restaurant_demo_data.xml` (651 lines)
- `addons/pos_restaurant/data/scenarios/restaurant_demo_session.xml` (384 lines)
- `addons/pos_restaurant/data/scenarios/restaurant_floor.xml` (382 lines)
- `addons/pos_restaurant/data/scenarios/restaurant_preset.xml` (36 lines)
- `addons/pos_restaurant/i18n/af.po` (1,714 lines)
- `addons/pos_restaurant/i18n/ar.po` (1,753 lines)
- `addons/pos_restaurant/i18n/az.po` (1,733 lines)
- `addons/pos_restaurant/i18n/bg.po` (1,748 lines)
- `addons/pos_restaurant/i18n/bs.po` (1,728 lines)
- `addons/pos_restaurant/i18n/ca.po` (1,758 lines)
- `addons/pos_restaurant/i18n/cs.po` (1,750 lines)
- `addons/pos_restaurant/i18n/da.po` (1,751 lines)
- `addons/pos_restaurant/i18n/de.po` (1,789 lines)
- `addons/pos_restaurant/i18n/el.po` (1,743 lines)
- `addons/pos_restaurant/i18n/es.po` (1,785 lines)
- `addons/pos_restaurant/i18n/es_419.po` (1,776 lines)
- `addons/pos_restaurant/i18n/es_CL.po` (103 lines)
- `addons/pos_restaurant/i18n/et.po` (1,754 lines)
- `addons/pos_restaurant/i18n/eu.po` (1,712 lines)
- `addons/pos_restaurant/i18n/fa.po` (1,742 lines)
- `addons/pos_restaurant/i18n/fi.po` (1,777 lines)
- `addons/pos_restaurant/i18n/fr.po` (1,777 lines)
- `addons/pos_restaurant/i18n/fr_CA.po` (100 lines)
- `addons/pos_restaurant/i18n/gl.po` (1,712 lines)
- `addons/pos_restaurant/i18n/gu.po` (1,714 lines)
- `addons/pos_restaurant/i18n/he.po` (1,746 lines)
- `addons/pos_restaurant/i18n/hi.po` (1,730 lines)
- `addons/pos_restaurant/i18n/hr.po` (1,743 lines)
- `addons/pos_restaurant/i18n/hu.po` (1,748 lines)
- `addons/pos_restaurant/i18n/id.po` (1,782 lines)
- `addons/pos_restaurant/i18n/is.po` (1,710 lines)
- `addons/pos_restaurant/i18n/it.po` (1,780 lines)
- `addons/pos_restaurant/i18n/ja.po` (1,769 lines)
- `addons/pos_restaurant/i18n/ka.po` (1,712 lines)
- `addons/pos_restaurant/i18n/kab.po` (1,724 lines)
- `addons/pos_restaurant/i18n/km.po` (1,715 lines)
- `addons/pos_restaurant/i18n/ko.po` (1,756 lines)
- `addons/pos_restaurant/i18n/ku.po` (1,727 lines)
- `addons/pos_restaurant/i18n/lo.po` (1,739 lines)
- `addons/pos_restaurant/i18n/lt.po` (1,748 lines)
- `addons/pos_restaurant/i18n/lv.po` (1,738 lines)
- `addons/pos_restaurant/i18n/mk.po` (1,721 lines)
- `addons/pos_restaurant/i18n/mn.po` (1,745 lines)
- `addons/pos_restaurant/i18n/my.po` (1,729 lines)
- `addons/pos_restaurant/i18n/nb.po` (1,736 lines)
- `addons/pos_restaurant/i18n/nl.po` (1,789 lines)
- `addons/pos_restaurant/i18n/pl.po` (1,788 lines)
- `addons/pos_restaurant/i18n/pos_restaurant.pot` (1,712 lines)
- `addons/pos_restaurant/i18n/pt.po` (1,768 lines)
- `addons/pos_restaurant/i18n/pt_BR.po` (1,782 lines)
- `addons/pos_restaurant/i18n/ro.po` (1,767 lines)
- `addons/pos_restaurant/i18n/ru.po` (1,753 lines)
- `addons/pos_restaurant/i18n/sk.po` (1,734 lines)
- `addons/pos_restaurant/i18n/sl.po` (1,741 lines)
- `addons/pos_restaurant/i18n/sq.po` (1,713 lines)
- `addons/pos_restaurant/i18n/sr@latin.po` (1,736 lines)
- `addons/pos_restaurant/i18n/sv.po` (1,767 lines)
- `addons/pos_restaurant/i18n/th.po` (1,751 lines)
- `addons/pos_restaurant/i18n/tr.po` (1,778 lines)
- `addons/pos_restaurant/i18n/uk.po` (1,748 lines)
- `addons/pos_restaurant/i18n/uz.po` (1,931 lines)
- `addons/pos_restaurant/i18n/vi.po` (1,754 lines)
- `addons/pos_restaurant/i18n/zh_CN.po` (1,760 lines)
- `addons/pos_restaurant/i18n/zh_TW.po` (1,746 lines)
- `addons/pos_restaurant/models/__init__.py` (13 lines)
- `addons/pos_restaurant/models/pos_category.py` (11 lines)
- `addons/pos_restaurant/models/pos_config.py` (334 lines)
- `addons/pos_restaurant/models/pos_course.py` (30 lines)
- `addons/pos_restaurant/models/pos_order.py` (52 lines)
- `addons/pos_restaurant/models/pos_order_line.py` (13 lines)
- `addons/pos_restaurant/models/pos_preset.py` (22 lines)
- `addons/pos_restaurant/models/pos_restaurant.py` (175 lines)
- `addons/pos_restaurant/models/pos_session.py` (15 lines)
- `addons/pos_restaurant/models/product_template.py` (18 lines)
- `addons/pos_restaurant/models/res_config_settings.py` (12 lines)
- `addons/pos_restaurant/models/restaurant_order_course.py` (43 lines)
- `addons/pos_restaurant/receipt/__init__.py` (1 lines)
- `addons/pos_restaurant/receipt/pos_order_change_receipt.xml` (19 lines)
- `addons/pos_restaurant/receipt/pos_order_receipt.py` (27 lines)
- `addons/pos_restaurant/receipt/pos_order_receipt.xml` (12 lines)
- `addons/pos_restaurant/security/ir.access.csv` (8 lines)
- `addons/pos_restaurant/static/description/icon.png` (25 lines)
- `addons/pos_restaurant/static/description/icon.svg` (1 lines)
- `addons/pos_restaurant/static/description/icon_hi.png` (67 lines)
- `addons/pos_restaurant/static/floor_plan/door.svg` (4 lines)
- `addons/pos_restaurant/static/floor_plan/plant.svg` (14 lines)
- `addons/pos_restaurant/static/floor_plan/tile-1.jpg` (116 lines)
- `addons/pos_restaurant/static/floor_plan/tile-1p.png` (41 lines)
- `addons/pos_restaurant/static/floor_plan/tile-2.jpg` (132 lines)
- `addons/pos_restaurant/static/floor_plan/tile-2p.jpg` (12 lines)
- `addons/pos_restaurant/static/floor_plan/tile-3.jpg` (91 lines)
- `addons/pos_restaurant/static/floor_plan/tile-3p.jpg` (9 lines)
- `addons/pos_restaurant/static/floor_plan/toilet.svg` (1 lines)
- `addons/pos_restaurant/static/floor_plan/wood-h.jpg` (143 lines)
- `addons/pos_restaurant/static/floor_plan/wood-hp.png` (19 lines)
- `addons/pos_restaurant/static/floor_plan/wood-v.jpg` (187 lines)
- `addons/pos_restaurant/static/floor_plan/wood-vp.png` (48 lines)
- `addons/pos_restaurant/static/img/combo-hamb.png` (569 lines)
- `addons/pos_restaurant/static/img/drink_category.jpg` (428 lines)
- `addons/pos_restaurant/static/img/floor_main.jpeg` (674 lines)
- `addons/pos_restaurant/static/img/food_category.jpg` (597 lines)
- `addons/pos_restaurant/static/img/plan.svg` (1 lines)
- `addons/pos_restaurant/static/img/product_aperol_spritz.png` (276 lines)
- `addons/pos_restaurant/static/img/product_cosmopolitan.png` (289 lines)
- `addons/pos_restaurant/static/img/product_mai_tai.png` (481 lines)
- `addons/pos_restaurant/static/img/product_margarita.png` (331 lines)
- `addons/pos_restaurant/static/img/product_mojito.png` (399 lines)
- `addons/pos_restaurant/static/img/product_moscow_mule.png` (691 lines)
- `addons/pos_restaurant/static/img/product_negroni.png` (197 lines)
- `addons/pos_restaurant/static/img/product_old_fashioned.png` (182 lines)
- `addons/pos_restaurant/static/img/product_pina_colada.png` (319 lines)
- `addons/pos_restaurant/static/img/product_whiskey_sour.png` (419 lines)
- `addons/pos_restaurant/static/img/soft-drink-icon.png` (83 lines)
- `addons/pos_restaurant/static/img/sushi-combo.png` (683 lines)
- `addons/pos_restaurant/static/img/table.svg` (1 lines)
- `addons/pos_restaurant/static/img/th-burger.png` (696 lines)
- `addons/pos_restaurant/static/img/th-cheeseburger.png` (574 lines)
- `addons/pos_restaurant/static/img/th-club.png` (748 lines)
- `addons/pos_restaurant/static/img/th-coke.png` (304 lines)
- `addons/pos_restaurant/static/img/th-espresso.png` (434 lines)
- `addons/pos_restaurant/static/img/th-fanta.png` (331 lines)
- `addons/pos_restaurant/static/img/th-green_tea.png` (303 lines)
- `addons/pos_restaurant/static/img/th-ice_tea.png` (290 lines)
- `addons/pos_restaurant/static/img/th-maki.png` (613 lines)
- `addons/pos_restaurant/static/img/th-milkshake_banana.png` (437 lines)
- `addons/pos_restaurant/static/img/th-minute_maid.png` (239 lines)
- `addons/pos_restaurant/static/img/th-mozza.png` (611 lines)
- `addons/pos_restaurant/static/img/th-pasta-4f.png` (585 lines)
- `addons/pos_restaurant/static/img/th-pasta.png` (763 lines)
- `addons/pos_restaurant/static/img/th-pizza-fu.png` (672 lines)
- `addons/pos_restaurant/static/img/th-pizza-ma.png` (631 lines)
- `addons/pos_restaurant/static/img/th-pizza-ve.png` (578 lines)
- `addons/pos_restaurant/static/img/th-pizza.png` (775 lines)
- `addons/pos_restaurant/static/img/th-salmon-avocado.png` (781 lines)
- `addons/pos_restaurant/static/img/th-salmon.png` (507 lines)
- `addons/pos_restaurant/static/img/th-sandwich.png` (785 lines)
- `addons/pos_restaurant/static/img/th-schweppes.png` (223 lines)
- `addons/pos_restaurant/static/img/th-temaki.png` (444 lines)
- `addons/pos_restaurant/static/img/th-tuna.png` (735 lines)
- `addons/pos_restaurant/static/img/th-water.png` (320 lines)
- `addons/pos_restaurant/static/src/app/components/navbar/navbar.js` (59 lines)
- `addons/pos_restaurant/static/src/app/components/navbar/navbar.xml` (46 lines)
- `addons/pos_restaurant/static/src/app/components/numpad_dropdown/numpad_dropdown.js` (65 lines)
- `addons/pos_restaurant/static/src/app/components/numpad_dropdown/numpad_dropdown.scss` (22 lines)
- `addons/pos_restaurant/static/src/app/components/numpad_dropdown/numpad_dropdown.xml` (33 lines)
- `addons/pos_restaurant/static/src/app/components/order_course/order_course.js` (37 lines)
- `addons/pos_restaurant/static/src/app/components/order_course/order_course.xml` (19 lines)
- `addons/pos_restaurant/static/src/app/components/order_display/order_display.js` (23 lines)
- `addons/pos_restaurant/static/src/app/components/order_display/order_display.xml` (25 lines)
- `addons/pos_restaurant/static/src/app/components/order_tabs/order_tabs.xml` (19 lines)
- `addons/pos_restaurant/static/src/app/components/orderline/orderline.xml` (8 lines)
- `addons/pos_restaurant/static/src/app/components/popup/edit_order_name_popup/edit_order_name_popup.js` (29 lines)
- `addons/pos_restaurant/static/src/app/components/popup/edit_order_name_popup/edit_order_name_popup.xml` (29 lines)
- `addons/pos_restaurant/static/src/app/hooks/floor_plan_hook.js` (5 lines)

Additional files not expanded here: 137. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
