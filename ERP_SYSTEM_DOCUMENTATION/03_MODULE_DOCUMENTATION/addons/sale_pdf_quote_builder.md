# Module: sale_pdf_quote_builder

- **Module ID:** MOD-522
- **Path:** `addons/sale_pdf_quote_builder`
- **Manifest:** `addons/sale_pdf_quote_builder/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Build nice quotations

Declared dependencies: `sale_management`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 6 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_management"
  ],
  "data": [
    "data/ir_cron.xml",
    "data/sale_pdf_form_field.xml",
    "report/ir_actions_report.xml",
    "views/product_document_views.xml",
    "views/quotation_document_views.xml",
    "views/sale_order_template_views.xml",
    "views/sale_order_views.xml",
    "views/sale_pdf_form_field_views.xml",
    "views/sale_pdf_quote_builder_menus.xml",
    "wizards/res_config_settings_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/sale_pdf_quote_builder_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_pdf_quote_builder/static/src/js/**/*"
    ],
    "web.assets_tests": [
      "sale_pdf_quote_builder/static/tests/tours/**/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_pdf_quote_builder/__init__.py` (3 lines)
- `addons/sale_pdf_quote_builder/__manifest__.py` (29 lines)
- `addons/sale_pdf_quote_builder/controllers/__init__.py` (3 lines)
- `addons/sale_pdf_quote_builder/controllers/quotation_document.py` (56 lines)
- `addons/sale_pdf_quote_builder/data/ir_cron.xml` (14 lines)
- `addons/sale_pdf_quote_builder/data/sale_pdf_form_field.xml` (6 lines)
- `addons/sale_pdf_quote_builder/data/sale_pdf_quote_builder_demo.xml` (73 lines)
- `addons/sale_pdf_quote_builder/i18n/ar.po` (692 lines)
- `addons/sale_pdf_quote_builder/i18n/az.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/bg.po` (667 lines)
- `addons/sale_pdf_quote_builder/i18n/bs.po` (666 lines)
- `addons/sale_pdf_quote_builder/i18n/ca.po` (673 lines)
- `addons/sale_pdf_quote_builder/i18n/cs.po` (670 lines)
- `addons/sale_pdf_quote_builder/i18n/da.po` (693 lines)
- `addons/sale_pdf_quote_builder/i18n/de.po` (703 lines)
- `addons/sale_pdf_quote_builder/i18n/el.po` (667 lines)
- `addons/sale_pdf_quote_builder/i18n/es.po` (700 lines)
- `addons/sale_pdf_quote_builder/i18n/es_419.po` (701 lines)
- `addons/sale_pdf_quote_builder/i18n/et.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/fa.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/fi.po` (694 lines)
- `addons/sale_pdf_quote_builder/i18n/fr.po` (707 lines)
- `addons/sale_pdf_quote_builder/i18n/he.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/hi.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/hr.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/hu.po` (692 lines)
- `addons/sale_pdf_quote_builder/i18n/id.po` (696 lines)
- `addons/sale_pdf_quote_builder/i18n/it.po` (702 lines)
- `addons/sale_pdf_quote_builder/i18n/ja.po` (696 lines)
- `addons/sale_pdf_quote_builder/i18n/kab.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/ko.po` (684 lines)
- `addons/sale_pdf_quote_builder/i18n/ku.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/lo.po` (686 lines)
- `addons/sale_pdf_quote_builder/i18n/lt.po` (666 lines)
- `addons/sale_pdf_quote_builder/i18n/lv.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/mn.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/my.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/nb.po` (669 lines)
- `addons/sale_pdf_quote_builder/i18n/nl.po` (699 lines)
- `addons/sale_pdf_quote_builder/i18n/pl.po` (672 lines)
- `addons/sale_pdf_quote_builder/i18n/pt.po` (695 lines)
- `addons/sale_pdf_quote_builder/i18n/pt_BR.po` (699 lines)
- `addons/sale_pdf_quote_builder/i18n/ro.po` (698 lines)
- `addons/sale_pdf_quote_builder/i18n/ru.po` (703 lines)
- `addons/sale_pdf_quote_builder/i18n/sale_pdf_quote_builder.pot` (661 lines)
- `addons/sale_pdf_quote_builder/i18n/sk.po` (664 lines)
- `addons/sale_pdf_quote_builder/i18n/sl.po` (670 lines)
- `addons/sale_pdf_quote_builder/i18n/sr@latin.po` (666 lines)
- `addons/sale_pdf_quote_builder/i18n/sv.po` (694 lines)
- `addons/sale_pdf_quote_builder/i18n/th.po` (683 lines)
- `addons/sale_pdf_quote_builder/i18n/tr.po` (699 lines)
- `addons/sale_pdf_quote_builder/i18n/uk.po` (665 lines)
- `addons/sale_pdf_quote_builder/i18n/uz.po` (810 lines)
- `addons/sale_pdf_quote_builder/i18n/vi.po` (691 lines)
- `addons/sale_pdf_quote_builder/i18n/zh_CN.po` (678 lines)
- `addons/sale_pdf_quote_builder/i18n/zh_TW.po` (680 lines)
- `addons/sale_pdf_quote_builder/models/__init__.py` (11 lines)
- `addons/sale_pdf_quote_builder/models/ir_actions_report.py` (287 lines)
- `addons/sale_pdf_quote_builder/models/product_document.py` (49 lines)
- `addons/sale_pdf_quote_builder/models/quotation_document.py` (110 lines)
- `addons/sale_pdf_quote_builder/models/sale_order.py` (182 lines)
- `addons/sale_pdf_quote_builder/models/sale_order_line.py` (65 lines)
- `addons/sale_pdf_quote_builder/models/sale_order_template.py` (15 lines)
- `addons/sale_pdf_quote_builder/models/sale_pdf_form_field.py` (250 lines)
- `addons/sale_pdf_quote_builder/report/ir_actions_report.xml` (18 lines)
- `addons/sale_pdf_quote_builder/security/ir.access.csv` (8 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/large_meeting_table_with_form_fields.pdf` (15,484 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/quote_footer_terms.pdf` (899 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/quote_footer_testimonials.pdf` (1,568 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/quote_header.pdf` (10,350 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/quote_header_about_us.pdf` (1,043 lines)
- `addons/sale_pdf_quote_builder/static/quote_builder_pdf/quote_header_project_description.pdf` (10,651 lines)
- `addons/sale_pdf_quote_builder/static/src/js/custom_content_kanban_like_widget/custom_content_kanban_like_widget.js` (136 lines)
- `addons/sale_pdf_quote_builder/static/src/js/custom_content_kanban_like_widget/custom_content_kanban_like_widget.xml` (89 lines)
- `addons/sale_pdf_quote_builder/static/src/js/custom_content_kanban_like_widget/custom_field_card/custom_field_card.js` (27 lines)
- `addons/sale_pdf_quote_builder/static/src/js/custom_content_kanban_like_widget/custom_field_card/custom_field_card.scss` (3 lines)
- `addons/sale_pdf_quote_builder/static/src/js/custom_content_kanban_like_widget/custom_field_card/custom_field_card.xml` (23 lines)
- `addons/sale_pdf_quote_builder/static/src/js/quotation_document_kanban/quotation_document_kanban_controller.js` (18 lines)
- `addons/sale_pdf_quote_builder/static/src/js/quotation_document_kanban/quotation_document_kanban_view.js` (14 lines)
- `addons/sale_pdf_quote_builder/static/src/js/quotation_document_kanban/quotation_document_kanban_widget.js` (31 lines)
- `addons/sale_pdf_quote_builder/static/src/js/quotation_document_kanban/quotation_document_kanban_widget.xml` (17 lines)
- `addons/sale_pdf_quote_builder/static/tests/tours/custom_content_kanban_like_tests.js` (20 lines)
- `addons/sale_pdf_quote_builder/tests/__init__.py` (3 lines)
- `addons/sale_pdf_quote_builder/tests/files/__init__.py` (8 lines)
- `addons/sale_pdf_quote_builder/tests/files/test_AES.pdf` (839 lines)
- `addons/sale_pdf_quote_builder/tests/files/test_forms.pdf` (998 lines)
- `addons/sale_pdf_quote_builder/tests/files/test_plain.pdf` (197 lines)
- `addons/sale_pdf_quote_builder/tests/test_controllers.py` (23 lines)
- `addons/sale_pdf_quote_builder/tests/test_pdf_quote_builder.py` (398 lines)
- `addons/sale_pdf_quote_builder/views/product_document_views.xml` (25 lines)
- `addons/sale_pdf_quote_builder/views/quotation_document_views.xml` (176 lines)
- `addons/sale_pdf_quote_builder/views/sale_order_template_views.xml` (32 lines)
- `addons/sale_pdf_quote_builder/views/sale_order_views.xml` (37 lines)
- `addons/sale_pdf_quote_builder/views/sale_pdf_form_field_views.xml` (38 lines)
- `addons/sale_pdf_quote_builder/views/sale_pdf_quote_builder_menus.xml` (10 lines)
- `addons/sale_pdf_quote_builder/wizards/res_config_settings_views.xml` (21 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
