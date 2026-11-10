# Module: sale_management

- **Module ID:** MOD-518
- **Path:** `addons/sale_management`
- **Manifest:** `addons/sale_management/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `True`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

From quotations to invoices


Manage sales quotations and orders
==================================

This application allows you to manage your sales goals in an effective and efficient manner by
keeping track of all sales orders and history.

It handles the full sales workflow:

* **Quotation** -> **Sales order** -> **Invoice**

Preferences (only with Warehouse Management installed)
------------------------------------------------------

If you also installed the Warehouse Management, you can deal with the following preferences:

* Shipping: Choice of delivery at once or partial delivery
* Invoicing: choose how invoices will be paid
* Incoterms: International Commercial terms


With this module you can personnalize the sales order and invoice report with
categories, subtotals or page-breaks.

The Dashboard for the Sales Manager will include
------------------------------------------------
* My Quotations
* Monthly Turnover (Graph)
    

Declared dependencies: `sale`, `digest`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 24 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "digest"
  ],
  "data": [
    "data/digest_data.xml",
    "views/sale_order_template_views.xml",
    "views/digest_views.xml",
    "views/res_config_settings_views.xml",
    "views/sale_order_views.xml",
    "views/sale_portal_templates.xml",
    "views/sale_management_menus.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/sale_order_template_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_management/static/src/components/**/*",
      "sale_management/static/src/fields/**/*",
      "sale_management/static/src/views/**/*"
    ],
    "web.assets_frontend": [
      "sale_management/static/src/interactions/**/*"
    ],
    "web.assets_tests": [
      "sale_management/static/tests/tours/**/*"
    ],
    "web.assets_unit_tests": [
      "sale_management/static/tests/mock_server/**/*",
      "sale_management/static/tests/sale_management_test_helpers.js",
      "sale_management/static/tests/**/*.test.js"
    ]
  }
}
```

### Representative source files

- `addons/sale_management/__init__.py` (21 lines)
- `addons/sale_management/__manifest__.py` (70 lines)
- `addons/sale_management/controllers/__init__.py` (3 lines)
- `addons/sale_management/controllers/portal.py` (69 lines)
- `addons/sale_management/data/digest_data.xml` (34 lines)
- `addons/sale_management/data/sale_order_template_demo.xml` (10 lines)
- `addons/sale_management/i18n/ar.po` (929 lines)
- `addons/sale_management/i18n/az.po` (891 lines)
- `addons/sale_management/i18n/bg.po` (887 lines)
- `addons/sale_management/i18n/bs.po` (892 lines)
- `addons/sale_management/i18n/ca.po` (938 lines)
- `addons/sale_management/i18n/cs.po` (919 lines)
- `addons/sale_management/i18n/da.po` (925 lines)
- `addons/sale_management/i18n/de.po` (1,006 lines)
- `addons/sale_management/i18n/el.po` (926 lines)
- `addons/sale_management/i18n/es.po` (996 lines)
- `addons/sale_management/i18n/es_419.po` (989 lines)
- `addons/sale_management/i18n/et.po` (932 lines)
- `addons/sale_management/i18n/fa.po` (921 lines)
- `addons/sale_management/i18n/fi.po` (990 lines)
- `addons/sale_management/i18n/fr.po` (966 lines)
- `addons/sale_management/i18n/gu.po` (766 lines)
- `addons/sale_management/i18n/he.po` (917 lines)
- `addons/sale_management/i18n/hi.po` (887 lines)
- `addons/sale_management/i18n/hr.po` (933 lines)
- `addons/sale_management/i18n/hu.po` (933 lines)
- `addons/sale_management/i18n/id.po` (1,000 lines)
- `addons/sale_management/i18n/is.po` (759 lines)
- `addons/sale_management/i18n/it.po` (990 lines)
- `addons/sale_management/i18n/ja.po` (947 lines)
- `addons/sale_management/i18n/kab.po` (888 lines)
- `addons/sale_management/i18n/km.po` (764 lines)
- `addons/sale_management/i18n/ko.po` (932 lines)
- `addons/sale_management/i18n/ku.po` (887 lines)
- `addons/sale_management/i18n/lo.po` (947 lines)
- `addons/sale_management/i18n/lt.po` (925 lines)
- `addons/sale_management/i18n/lv.po` (897 lines)
- `addons/sale_management/i18n/mn.po` (984 lines)
- `addons/sale_management/i18n/my.po` (888 lines)
- `addons/sale_management/i18n/nb.po` (903 lines)
- `addons/sale_management/i18n/nl.po` (1,000 lines)
- `addons/sale_management/i18n/pl.po` (967 lines)
- `addons/sale_management/i18n/pt.po` (932 lines)
- `addons/sale_management/i18n/pt_BR.po` (994 lines)
- `addons/sale_management/i18n/ro.po` (932 lines)
- `addons/sale_management/i18n/ru.po` (939 lines)
- `addons/sale_management/i18n/sale_management.pot` (874 lines)
- `addons/sale_management/i18n/sk.po` (919 lines)
- `addons/sale_management/i18n/sl.po` (912 lines)
- `addons/sale_management/i18n/sr@latin.po` (924 lines)
- `addons/sale_management/i18n/sv.po` (935 lines)
- `addons/sale_management/i18n/th.po` (937 lines)
- `addons/sale_management/i18n/tr.po` (976 lines)
- `addons/sale_management/i18n/uk.po` (925 lines)
- `addons/sale_management/i18n/uz.po` (1,001 lines)
- `addons/sale_management/i18n/vi.po` (933 lines)
- `addons/sale_management/i18n/zh_CN.po` (944 lines)
- `addons/sale_management/i18n/zh_TW.po` (913 lines)
- `addons/sale_management/models/__init__.py` (10 lines)
- `addons/sale_management/models/digest.py` (29 lines)
- `addons/sale_management/models/product_attribute_custom_value.py` (19 lines)
- `addons/sale_management/models/sale_order.py` (172 lines)
- `addons/sale_management/models/sale_order_line.py` (137 lines)
- `addons/sale_management/models/sale_order_template.py` (416 lines)
- `addons/sale_management/models/sale_order_template_line.py` (434 lines)
- `addons/sale_management/security/ir.access.csv` (7 lines)
- `addons/sale_management/static/description/icon.png` (15 lines)
- `addons/sale_management/static/description/icon.svg` (1 lines)
- `addons/sale_management/static/description/icon_hi.png` (20 lines)
- `addons/sale_management/static/src/components/product_catalog/kanban_controller.js` (20 lines)
- `addons/sale_management/static/src/fields/sale_order_line_field/sale_order_line_field.js` (512 lines)
- `addons/sale_management/static/src/fields/sale_order_line_field/sale_order_line_field.scss` (3 lines)
- `addons/sale_management/static/src/fields/sale_order_line_field/sale_order_line_field.xml` (97 lines)
- `addons/sale_management/static/src/fields/sale_order_template_label_text/sale_order_template_label_text.js` (148 lines)
- `addons/sale_management/static/src/fields/sale_order_template_label_text/sale_order_template_label_text.scss` (7 lines)
- `addons/sale_management/static/src/fields/sale_order_template_line_field/sale_order_template_line_field.js` (424 lines)
- `addons/sale_management/static/src/fields/sale_order_template_line_field/sale_order_template_line_field.scss` (14 lines)
- `addons/sale_management/static/src/fields/sale_order_template_line_field/sale_order_template_line_field.xml` (21 lines)
- `addons/sale_management/static/src/fields/sale_order_template_product_field/sale_order_template_product_field.js` (139 lines)
- `addons/sale_management/static/src/fields/sale_product_mixin.js` (28 lines)
- `addons/sale_management/static/src/img/milk-Sales-configure-products.gif` (173 lines)
- `addons/sale_management/static/src/img/milk-t-shirts.png` (151 lines)
- `addons/sale_management/static/src/img/online_training.png` (90 lines)
- `addons/sale_management/static/src/img/openerp_gold_partner.png` (149 lines)
- `addons/sale_management/static/src/img/partner_icon_01.png` (158 lines)
- `addons/sale_management/static/src/img/partner_icon_02.png` (124 lines)
- `addons/sale_management/static/src/img/partner_icon_04.png` (147 lines)
- `addons/sale_management/static/src/img/partner_sc_01.png` (366 lines)
- `addons/sale_management/static/src/interactions/sale_update_line_button.js` (63 lines)
- `addons/sale_management/static/src/views/components/template_dropdown.js` (104 lines)
- `addons/sale_management/static/src/views/components/template_dropdown.scss` (25 lines)
- `addons/sale_management/static/src/views/components/template_dropdown.xml` (50 lines)
- `addons/sale_management/static/src/views/file_upload_kanban/file_upload_kanban_controller.js` (10 lines)
- `addons/sale_management/static/src/views/file_upload_kanban/file_upload_kanban_view.js` (6 lines)
- `addons/sale_management/static/src/views/file_upload_list/file_upload_list_controller.js` (10 lines)
- `addons/sale_management/static/src/views/file_upload_list/file_upload_list_view.js` (6 lines)
- `addons/sale_management/static/src/views/onboarding_kanban/onboarding_kanban_view.js` (6 lines)
- `addons/sale_management/static/src/views/onboarding_list/onboarding_list_view.js` (6 lines)
- `addons/sale_management/static/src/views/order_form/order_form_controller.js` (10 lines)
- `addons/sale_management/static/src/views/order_form/order_form_controller.xml` (13 lines)
- `addons/sale_management/static/src/views/order_form/order_form_view.js` (5 lines)
- `addons/sale_management/static/src/views/sale_order_template_form/sale_order_template_form_view.js` (15 lines)
- `addons/sale_management/static/src/views/sale_order_template_form/sale_order_template_static_list.js` (57 lines)
- `addons/sale_management/static/src/views/template_kanban_buttons/template_kanban_buttons.xml` (12 lines)
- `addons/sale_management/static/src/views/template_list_buttons/template_list_buttons.xml` (12 lines)
- `addons/sale_management/static/tests/mock_server/mock_models/sale_order_template.js` (60 lines)
- `addons/sale_management/static/tests/mock_server/mock_models/sale_order_template_line.js` (30 lines)
- `addons/sale_management/static/tests/sale_management_test_helpers.js` (14 lines)
- `addons/sale_management/static/tests/sale_order_line_field.test.js` (482 lines)
- `addons/sale_management/static/tests/sale_order_template_line_field.test.js` (642 lines)
- `addons/sale_management/static/tests/tours/sale_flow_tour.js` (47 lines)
- `addons/sale_management/tests/__init__.py` (3 lines)
- `addons/sale_management/tests/common.py` (25 lines)
- `addons/sale_management/tests/test_sale_order.py` (677 lines)
- `addons/sale_management/tests/test_sale_order_template.py` (179 lines)
- `addons/sale_management/tests/test_sale_section_templates.py` (216 lines)
- `addons/sale_management/tests/test_sale_ui.py` (85 lines)
- `addons/sale_management/views/digest_views.xml` (21 lines)
- `addons/sale_management/views/res_config_settings_views.xml` (15 lines)
- `addons/sale_management/views/sale_management_menus.xml` (16 lines)
- `addons/sale_management/views/sale_order_template_views.xml` (310 lines)
- `addons/sale_management/views/sale_order_views.xml` (47 lines)
- `addons/sale_management/views/sale_portal_templates.xml` (66 lines)
- `addons/sale_management/wizard/__init__.py` (3 lines)
- `addons/sale_management/wizard/res_config_settings.py` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
