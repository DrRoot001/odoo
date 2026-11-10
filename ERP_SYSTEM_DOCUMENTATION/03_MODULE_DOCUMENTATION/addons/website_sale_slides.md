# Module: website_sale_slides

- **Module ID:** MOD-641
- **Path:** `addons/website_sale_slides`
- **Manifest:** `addons/website_sale_slides/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Sell your courses online

Sell your courses using the e-commerce features of the website.

Declared dependencies: `website_slides`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 14 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 3 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 5 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_slides",
    "website_sale"
  ],
  "data": [
    "data/product_data.xml",
    "report/sale_report_views.xml",
    "views/website_slides_menu_views.xml",
    "views/product_template_views.xml",
    "views/slide_channel_views.xml",
    "views/website_sale_templates.xml",
    "views/website_slides_templates.xml"
  ],
  "demo": [
    "data/product_demo.xml",
    "data/slide_demo.xml",
    "data/sale_order_demo.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "website_sale_slides/static/src/interactions/**/*",
      "website_sale_slides/static/src/xml/**/*"
    ],
    "web.assets_tests": [
      "website_sale_slides/static/tests/tours/*.js"
    ],
    "website.website_builder_assets": [
      "website_sale_slides/static/src/website_builder/**/*"
    ]
  }
}
```

### Representative source files

- `addons/website_sale_slides/__init__.py` (5 lines)
- `addons/website_sale_slides/__manifest__.py` (37 lines)
- `addons/website_sale_slides/controllers/__init__.py` (5 lines)
- `addons/website_sale_slides/controllers/sale.py` (21 lines)
- `addons/website_sale_slides/controllers/slides.py` (31 lines)
- `addons/website_sale_slides/data/product_data.xml` (13 lines)
- `addons/website_sale_slides/data/product_demo.xml` (44 lines)
- `addons/website_sale_slides/data/sale_order_demo.xml` (90 lines)
- `addons/website_sale_slides/data/slide_demo.xml` (23 lines)
- `addons/website_sale_slides/i18n/ar.po` (343 lines)
- `addons/website_sale_slides/i18n/az.po` (335 lines)
- `addons/website_sale_slides/i18n/bg.po` (335 lines)
- `addons/website_sale_slides/i18n/bs.po` (337 lines)
- `addons/website_sale_slides/i18n/ca.po` (339 lines)
- `addons/website_sale_slides/i18n/cs.po` (342 lines)
- `addons/website_sale_slides/i18n/da.po` (343 lines)
- `addons/website_sale_slides/i18n/de.po` (348 lines)
- `addons/website_sale_slides/i18n/el.po` (336 lines)
- `addons/website_sale_slides/i18n/es.po` (347 lines)
- `addons/website_sale_slides/i18n/es_419.po` (341 lines)
- `addons/website_sale_slides/i18n/et.po` (336 lines)
- `addons/website_sale_slides/i18n/fa.po` (335 lines)
- `addons/website_sale_slides/i18n/fi.po` (340 lines)
- `addons/website_sale_slides/i18n/fr.po` (347 lines)
- `addons/website_sale_slides/i18n/he.po` (344 lines)
- `addons/website_sale_slides/i18n/hi.po` (335 lines)
- `addons/website_sale_slides/i18n/hr.po` (344 lines)
- `addons/website_sale_slides/i18n/hu.po` (348 lines)
- `addons/website_sale_slides/i18n/id.po` (342 lines)
- `addons/website_sale_slides/i18n/it.po` (346 lines)
- `addons/website_sale_slides/i18n/ja.po` (339 lines)
- `addons/website_sale_slides/i18n/kab.po` (336 lines)
- `addons/website_sale_slides/i18n/ko.po` (337 lines)
- `addons/website_sale_slides/i18n/ku.po` (335 lines)
- `addons/website_sale_slides/i18n/lo.po` (338 lines)
- `addons/website_sale_slides/i18n/lt.po` (350 lines)
- `addons/website_sale_slides/i18n/lv.po` (336 lines)
- `addons/website_sale_slides/i18n/mn.po` (343 lines)
- `addons/website_sale_slides/i18n/my.po` (336 lines)
- `addons/website_sale_slides/i18n/nb.po` (341 lines)
- `addons/website_sale_slides/i18n/nl.po` (348 lines)
- `addons/website_sale_slides/i18n/pl.po` (352 lines)
- `addons/website_sale_slides/i18n/pt.po` (349 lines)
- `addons/website_sale_slides/i18n/pt_BR.po` (349 lines)
- `addons/website_sale_slides/i18n/ro.po` (344 lines)
- `addons/website_sale_slides/i18n/ru.po` (343 lines)
- `addons/website_sale_slides/i18n/sk.po` (335 lines)
- `addons/website_sale_slides/i18n/sl.po` (337 lines)
- `addons/website_sale_slides/i18n/sr@latin.po` (337 lines)
- `addons/website_sale_slides/i18n/sv.po` (341 lines)
- `addons/website_sale_slides/i18n/th.po` (337 lines)
- `addons/website_sale_slides/i18n/tr.po` (353 lines)
- `addons/website_sale_slides/i18n/uk.po` (342 lines)
- `addons/website_sale_slides/i18n/uz.po` (396 lines)
- `addons/website_sale_slides/i18n/vi.po` (345 lines)
- `addons/website_sale_slides/i18n/website_sale_slides.pot` (332 lines)
- `addons/website_sale_slides/i18n/zh_CN.po` (344 lines)
- `addons/website_sale_slides/i18n/zh_TW.po` (340 lines)
- `addons/website_sale_slides/models/__init__.py` (7 lines)
- `addons/website_sale_slides/models/product_product.py` (28 lines)
- `addons/website_sale_slides/models/product_template.py` (24 lines)
- `addons/website_sale_slides/models/sale_order.py` (40 lines)
- `addons/website_sale_slides/models/sale_order_line.py` (11 lines)
- `addons/website_sale_slides/models/slide_channel.py` (94 lines)
- `addons/website_sale_slides/report/sale_report_views.xml` (28 lines)
- `addons/website_sale_slides/static/img/channel_demo_furniture_2.jpg` (498 lines)
- `addons/website_sale_slides/static/img/channel_demo_tree_1.jpg` (354 lines)
- `addons/website_sale_slides/static/img/default_course_product.jpg` (419 lines)
- `addons/website_sale_slides/static/img/flower_pot.jpg` (279 lines)
- `addons/website_sale_slides/static/img/product_course.jpg` (450 lines)
- `addons/website_sale_slides/static/img/water_can.jpg` (584 lines)
- `addons/website_sale_slides/static/src/interactions/slides_course_fullscreen.js` (16 lines)
- `addons/website_sale_slides/static/src/interactions/slides_course_join.js` (31 lines)
- `addons/website_sale_slides/static/src/interactions/slides_course_quiz_edit.js` (19 lines)
- `addons/website_sale_slides/static/src/website_builder/course_page_option.xml` (21 lines)
- `addons/website_sale_slides/static/src/xml/slide_course_join.xml` (15 lines)
- `addons/website_sale_slides/static/src/xml/website_sale_slides_quiz.xml` (15 lines)
- `addons/website_sale_slides/static/src/xml/website_slides_unsubscribe.xml` (18 lines)
- `addons/website_sale_slides/static/tests/tours/slides_course_member_invited_logged.js` (41 lines)
- `addons/website_sale_slides/static/tests/tours/slides_course_member_invited_public.js` (58 lines)
- `addons/website_sale_slides/tests/__init__.py` (5 lines)
- `addons/website_sale_slides/tests/test_course_purchase_flow.py` (126 lines)
- `addons/website_sale_slides/tests/test_ui_website_sale_slides.py` (39 lines)
- `addons/website_sale_slides/views/product_template_views.xml` (13 lines)
- `addons/website_sale_slides/views/slide_channel_views.xml` (80 lines)
- `addons/website_sale_slides/views/website_sale_templates.xml` (56 lines)
- `addons/website_sale_slides/views/website_slides_menu_views.xml` (8 lines)
- `addons/website_sale_slides/views/website_slides_templates.xml` (198 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
