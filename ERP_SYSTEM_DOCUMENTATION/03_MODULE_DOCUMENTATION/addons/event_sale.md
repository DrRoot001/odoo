# Module: event_sale

- **Module ID:** MOD-070
- **Path:** `addons/event_sale`
- **Manifest:** `addons/event_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Creating registration with sales orders.
========================================

This module allows you to automate and connect your registration creation with
your main sale flow and therefore, to enable the invoicing feature of registrations.

It defines a new kind of service products that offers you the possibility to
choose an event category associated with it. When you encode a sales order for
that product, you will be able to choose an existing event of that category and
when you confirm your sales order it will automatically create a registration for
this event.


Declared dependencies: `event_product`, `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 13 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "event_product",
    "sale_management"
  ],
  "data": [
    "views/event_registration_views.xml",
    "views/event_views.xml",
    "views/product_template_views.xml",
    "views/sale_order_views.xml",
    "data/event_sale_data.xml",
    "data/mail_templates.xml",
    "report/event_sale_report_views.xml",
    "security/event_security.xml",
    "wizard/event_edit_registration.xml",
    "wizard/event_configurator_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/event_sale_demo.xml",
    "data/event_registration_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "event_sale/static/src/**/*"
    ],
    "web.assets_tests": [
      "event_sale/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/event_sale/__init__.py` (7 lines)
- `addons/event_sale/__manifest__.py` (49 lines)
- `addons/event_sale/controllers/__init__.py` (1 lines)
- `addons/event_sale/controllers/portal.py` (18 lines)
- `addons/event_sale/data/event_registration_demo.xml` (70 lines)
- `addons/event_sale/data/event_sale_data.xml` (8 lines)
- `addons/event_sale/data/event_sale_demo.xml` (175 lines)
- `addons/event_sale/data/mail_templates.xml` (23 lines)
- `addons/event_sale/i18n/af.po` (700 lines)
- `addons/event_sale/i18n/am.po` (696 lines)
- `addons/event_sale/i18n/ar.po` (721 lines)
- `addons/event_sale/i18n/az.po` (706 lines)
- `addons/event_sale/i18n/bg.po` (728 lines)
- `addons/event_sale/i18n/bs.po` (704 lines)
- `addons/event_sale/i18n/ca.po` (731 lines)
- `addons/event_sale/i18n/cs.po` (717 lines)
- `addons/event_sale/i18n/da.po` (730 lines)
- `addons/event_sale/i18n/de.po` (752 lines)
- `addons/event_sale/i18n/el.po` (710 lines)
- `addons/event_sale/i18n/es.po` (751 lines)
- `addons/event_sale/i18n/es_419.po` (744 lines)
- `addons/event_sale/i18n/es_CL.po` (104 lines)
- `addons/event_sale/i18n/et.po` (725 lines)
- `addons/event_sale/i18n/eu.po` (699 lines)
- `addons/event_sale/i18n/event_sale.pot` (688 lines)
- `addons/event_sale/i18n/fa.po` (721 lines)
- `addons/event_sale/i18n/fi.po` (762 lines)
- `addons/event_sale/i18n/fo.po` (699 lines)
- `addons/event_sale/i18n/fr.po` (757 lines)
- `addons/event_sale/i18n/fr_BE.po` (97 lines)
- `addons/event_sale/i18n/fr_CA.po` (97 lines)
- `addons/event_sale/i18n/gl.po` (699 lines)
- `addons/event_sale/i18n/gu.po` (700 lines)
- `addons/event_sale/i18n/he.po` (719 lines)
- `addons/event_sale/i18n/hi.po` (714 lines)
- `addons/event_sale/i18n/hr.po` (719 lines)
- `addons/event_sale/i18n/hu.po` (729 lines)
- `addons/event_sale/i18n/id.po` (735 lines)
- `addons/event_sale/i18n/is.po` (700 lines)
- `addons/event_sale/i18n/it.po` (750 lines)
- `addons/event_sale/i18n/ja.po` (725 lines)
- `addons/event_sale/i18n/ka.po` (699 lines)
- `addons/event_sale/i18n/kab.po` (701 lines)
- `addons/event_sale/i18n/km.po` (700 lines)
- `addons/event_sale/i18n/ko.po` (717 lines)
- `addons/event_sale/i18n/ku.po` (700 lines)
- `addons/event_sale/i18n/lo.po` (730 lines)
- `addons/event_sale/i18n/lt.po` (720 lines)
- `addons/event_sale/i18n/lv.po` (709 lines)
- `addons/event_sale/i18n/mk.po` (699 lines)
- `addons/event_sale/i18n/mn.po` (712 lines)
- `addons/event_sale/i18n/my.po` (701 lines)
- `addons/event_sale/i18n/nb.po` (707 lines)
- `addons/event_sale/i18n/nl.po` (750 lines)
- `addons/event_sale/i18n/pl.po` (749 lines)
- `addons/event_sale/i18n/pt.po` (733 lines)
- `addons/event_sale/i18n/pt_BR.po` (752 lines)
- `addons/event_sale/i18n/ro.po` (728 lines)
- `addons/event_sale/i18n/ru.po` (747 lines)
- `addons/event_sale/i18n/sk.po` (712 lines)
- `addons/event_sale/i18n/sl.po` (731 lines)
- `addons/event_sale/i18n/sq.po` (699 lines)
- `addons/event_sale/i18n/sr@latin.po` (719 lines)
- `addons/event_sale/i18n/sv.po` (743 lines)
- `addons/event_sale/i18n/ta.po` (700 lines)
- `addons/event_sale/i18n/th.po` (714 lines)
- `addons/event_sale/i18n/tr.po` (748 lines)
- `addons/event_sale/i18n/uk.po` (719 lines)
- `addons/event_sale/i18n/uz.po` (840 lines)
- `addons/event_sale/i18n/vi.po` (722 lines)
- `addons/event_sale/i18n/zh_CN.po` (713 lines)
- `addons/event_sale/i18n/zh_TW.po` (714 lines)
- `addons/event_sale/models/__init__.py` (6 lines)
- `addons/event_sale/models/event_event.py` (55 lines)
- `addons/event_sale/models/event_registration.py` (169 lines)
- `addons/event_sale/models/event_ticket.py` (14 lines)
- `addons/event_sale/models/product_template.py` (15 lines)
- `addons/event_sale/models/sale_order.py` (59 lines)
- `addons/event_sale/models/sale_order_line.py` (135 lines)
- `addons/event_sale/report/__init__.py` (4 lines)
- `addons/event_sale/report/event_sale_report.py` (148 lines)
- `addons/event_sale/report/event_sale_report_views.xml` (155 lines)
- `addons/event_sale/security/event_security.xml` (8 lines)
- `addons/event_sale/security/ir.access.csv` (8 lines)
- `addons/event_sale/static/img/event_product-image.jpg` (42 lines)
- `addons/event_sale/static/src/client_action/event_registration_summary_dialog.xml` (12 lines)
- `addons/event_sale/static/src/js/event_configurator_controller.js` (49 lines)
- `addons/event_sale/static/src/js/sale_product_mixin.js` (91 lines)
- `addons/event_sale/static/tests/tours/event_configurator_ui.js` (57 lines)
- `addons/event_sale/tests/__init__.py` (7 lines)
- `addons/event_sale/tests/common.py` (22 lines)
- `addons/event_sale/tests/test_event_internals.py` (124 lines)
- `addons/event_sale/tests/test_event_sale.py` (616 lines)
- `addons/event_sale/tests/test_event_sale_ui.py` (42 lines)
- `addons/event_sale/tests/test_event_specific.py` (53 lines)
- `addons/event_sale/views/event_registration_views.xml` (40 lines)
- `addons/event_sale/views/event_views.xml` (29 lines)
- `addons/event_sale/views/product_template_views.xml` (13 lines)
- `addons/event_sale/views/sale_order_views.xml` (73 lines)
- `addons/event_sale/wizard/__init__.py` (2 lines)
- `addons/event_sale/wizard/event_configurator.py` (64 lines)
- `addons/event_sale/wizard/event_configurator_views.xml` (64 lines)
- `addons/event_sale/wizard/event_edit_registration.py` (107 lines)
- `addons/event_sale/wizard/event_edit_registration.xml` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
