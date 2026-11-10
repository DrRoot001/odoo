# Module: product

- **Module ID:** MOD-470
- **Path:** `addons/product`
- **Manifest:** `addons/product/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module for managing products and pricelists in Odoo.
========================================================================

Products support variants, different pricing methods, vendors information,
make to stock/order, different units of measure, packaging and properties.

Pricelists support:
-------------------
    * Multiple-level of discount (by product, category, quantities)
    * Compute price based on different criteria:
        * Other pricelist
        * Cost price
        * List price
        * Vendor price

Pricelists preferences by product and/or partners.

Print product labels with barcode.
    

Declared dependencies: `base`, `mail`, `uom`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 57 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 28 | Files under `models/` or `models.py`. |
| Controller-path Python files | 4 | Files under `controllers/` or `controllers.py`. |
| XML files | 44 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 22 | Client behavior/assets. |
| Tests | 17 | Test files found by path/name convention. |
| Security artifacts | 2 | Access CSV and/or security XML. |
| Route declarations | 4 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "mail",
    "uom"
  ],
  "data": [
    "data/product_data.xml",
    "security/product_security.xml",
    "data/product_attribute_data.xml",
    "wizard/product_label_layout_views.xml",
    "wizard/update_product_attribute_value_views.xml",
    "views/product_tag_views.xml",
    "views/product_views.xml",
    "views/res_config_settings_views.xml",
    "views/product_attribute_views.xml",
    "views/product_attribute_value_views.xml",
    "views/product_base_unit_views.xml",
    "views/product_category_views.xml",
    "views/product_combo_views.xml",
    "views/product_document_views.xml",
    "views/product_pricelist_item_views.xml",
    "views/product_pricelist_views.xml",
    "views/product_supplierinfo_views.xml",
    "views/product_template_attribute_line_views.xml",
    "views/product_template_views.xml",
    "views/res_country_group_views.xml",
    "views/res_partner_views.xml",
    "views/uom_views.xml",
    "report/product_reports.xml",
    "report/product_product_templates.xml",
    "report/product_template_templates.xml",
    "report/product_pricelist_report_templates.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/product_attribute_demo.xml",
    "data/product_category_demo.xml",
    "data/product_demo.xml",
    "data/product_document_demo.xml",
    "data/product_supplierinfo_demo.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "product/static/src/js/**/*",
      "product/static/src/product_catalog/**/*.js",
      "product/static/src/product_catalog/**/*.xml",
      "product/static/src/product_catalog/**/*.scss",
      "product/static/src/scss/product_template_views.scss"
    ],
    "web.report_assets_common": [
      "product/static/src/scss/report_label_sheet.scss"
    ],
    "web.assets_unit_tests": [
      "product/static/tests/**/*"
    ]
  }
}
```

### Representative source files

- `addons/product/__init__.py` (7 lines)
- `addons/product/__manifest__.py` (84 lines)
- `addons/product/controllers/__init__.py` (3 lines)
- `addons/product/controllers/catalog.py` (54 lines)
- `addons/product/controllers/pricelist_report.py` (95 lines)
- `addons/product/controllers/product_document.py` (44 lines)
- `addons/product/data/product_attribute_data.xml` (32 lines)
- `addons/product/data/product_attribute_demo.xml` (572 lines)
- `addons/product/data/product_category_demo.xml` (20 lines)
- `addons/product/data/product_data.xml` (43 lines)
- `addons/product/data/product_demo.xml` (904 lines)
- `addons/product/data/product_document_demo.xml` (19 lines)
- `addons/product/data/product_supplierinfo_demo.xml` (256 lines)
- `addons/product/i18n/af.po` (5,205 lines)
- `addons/product/i18n/am.po` (5,204 lines)
- `addons/product/i18n/ar.po` (5,745 lines)
- `addons/product/i18n/az.po` (5,443 lines)
- `addons/product/i18n/bg.po` (5,493 lines)
- `addons/product/i18n/bs.po` (5,449 lines)
- `addons/product/i18n/ca.po` (5,767 lines)
- `addons/product/i18n/cs.po` (5,577 lines)
- `addons/product/i18n/da.po` (5,930 lines)
- `addons/product/i18n/de.po` (5,986 lines)
- `addons/product/i18n/el.po` (5,542 lines)
- `addons/product/i18n/es.po` (5,787 lines)
- `addons/product/i18n/es_419.po` (5,927 lines)
- `addons/product/i18n/es_CL.po` (638 lines)
- `addons/product/i18n/et.po` (5,722 lines)
- `addons/product/i18n/eu.po` (5,209 lines)
- `addons/product/i18n/fa.po` (5,518 lines)
- `addons/product/i18n/fi.po` (5,873 lines)
- `addons/product/i18n/fr.po` (5,915 lines)
- `addons/product/i18n/gl.po` (5,203 lines)
- `addons/product/i18n/gu.po` (5,209 lines)
- `addons/product/i18n/he.po` (5,618 lines)
- `addons/product/i18n/hi.po` (5,442 lines)
- `addons/product/i18n/hr.po` (5,572 lines)
- `addons/product/i18n/hu.po` (5,523 lines)
- `addons/product/i18n/id.po` (5,865 lines)
- `addons/product/i18n/is.po` (5,206 lines)
- `addons/product/i18n/it.po` (5,933 lines)
- `addons/product/i18n/ja.po` (5,766 lines)
- `addons/product/i18n/kab.po` (5,440 lines)
- `addons/product/i18n/km.po` (5,208 lines)
- `addons/product/i18n/ko.po` (5,713 lines)
- `addons/product/i18n/ku.po` (5,441 lines)
- `addons/product/i18n/lb.po` (5,206 lines)
- `addons/product/i18n/lo.po` (5,608 lines)
- `addons/product/i18n/lt.po` (5,526 lines)
- `addons/product/i18n/lv.po` (5,481 lines)
- `addons/product/i18n/mk.po` (5,223 lines)
- `addons/product/i18n/mn.po` (5,523 lines)
- `addons/product/i18n/my.po` (5,428 lines)
- `addons/product/i18n/nb.po` (5,506 lines)
- `addons/product/i18n/nl.po` (5,951 lines)
- `addons/product/i18n/pl.po` (5,896 lines)
- `addons/product/i18n/product.pot` (5,390 lines)
- `addons/product/i18n/pt.po` (5,742 lines)
- `addons/product/i18n/pt_BR.po` (6,030 lines)
- `addons/product/i18n/ro.po` (5,778 lines)
- `addons/product/i18n/ru.po` (5,745 lines)
- `addons/product/i18n/sk.po` (5,481 lines)
- `addons/product/i18n/sl.po` (5,494 lines)
- `addons/product/i18n/sr@latin.po` (5,453 lines)
- `addons/product/i18n/sv.po` (5,718 lines)
- `addons/product/i18n/th.po` (5,772 lines)
- `addons/product/i18n/tr.po` (5,742 lines)
- `addons/product/i18n/uk.po` (5,620 lines)
- `addons/product/i18n/uz.po` (6,419 lines)
- `addons/product/i18n/vi.po` (5,758 lines)
- `addons/product/i18n/zh_CN.po` (5,837 lines)
- `addons/product/i18n/zh_TW.po` (5,718 lines)
- `addons/product/models/__init__.py` (35 lines)
- `addons/product/models/ir_attachment.py` (26 lines)
- `addons/product/models/product_attribute.py` (169 lines)
- `addons/product/models/product_attribute_custom_value.py` (30 lines)
- `addons/product/models/product_attribute_value.py` (180 lines)
- `addons/product/models/product_base_unit.py` (13 lines)
- `addons/product/models/product_catalog_line_mixin.py` (100 lines)
- `addons/product/models/product_catalog_mixin.py` (250 lines)
- `addons/product/models/product_category.py` (104 lines)
- `addons/product/models/product_combo.py` (84 lines)
- `addons/product/models/product_combo_item.py` (34 lines)
- `addons/product/models/product_document.py` (75 lines)
- `addons/product/models/product_pricelist.py` (533 lines)
- `addons/product/models/product_pricelist_item.py` (677 lines)
- `addons/product/models/product_product.py` (1,464 lines)
- `addons/product/models/product_supplierinfo.py` (145 lines)
- `addons/product/models/product_tag.py` (58 lines)
- `addons/product/models/product_template.py` (1,892 lines)
- `addons/product/models/product_template_attribute_line.py` (283 lines)
- `addons/product/models/product_template_attribute_value.py` (217 lines)
- `addons/product/models/product_uom.py` (52 lines)
- `addons/product/models/res_company.py` (69 lines)
- `addons/product/models/res_config_settings.py` (45 lines)
- `addons/product/models/res_country_group.py` (15 lines)
- `addons/product/models/res_currency.py` (25 lines)
- `addons/product/models/res_groups.py` (15 lines)
- `addons/product/models/res_partner.py` (68 lines)
- `addons/product/models/uom_uom.py` (32 lines)
- `addons/product/populate/benchmarks.xml` (298 lines)
- `addons/product/populate/common.xml` (19 lines)
- `addons/product/populate/config_parameter.xml` (8 lines)
- `addons/product/populate/populate_demo.xml` (128 lines)
- `addons/product/report/__init__.py` (5 lines)
- `addons/product/report/product_label_report.py` (114 lines)
- `addons/product/report/product_pricelist_report.py` (96 lines)
- `addons/product/report/product_pricelist_report_templates.xml` (153 lines)
- `addons/product/report/product_product_templates.xml` (589 lines)
- `addons/product/report/product_reports.xml` (71 lines)
- `addons/product/report/product_template_templates.xml` (24 lines)
- `addons/product/security/ir.access.csv` (49 lines)
- `addons/product/security/product_security.xml` (35 lines)
- `addons/product/static/demo/acoustic_bloc_screen_document.pdf` (1,649 lines)
- `addons/product/static/demo/customizable_desk_document.pdf` (1,733 lines)
- `addons/product/static/description/icon.png` (28 lines)
- `addons/product/static/description/icon.svg` (1 lines)
- `addons/product/static/description/icon_hi.png` (109 lines)
- `addons/product/static/img/desk_organizer.jpg` (281 lines)
- `addons/product/static/img/desk_pad.jpg` (162 lines)
- `addons/product/static/img/dining_table.png` (626 lines)
- `addons/product/static/img/glass.png` (272 lines)
- `addons/product/static/img/leather.png` (258 lines)
- `addons/product/static/img/linen.png` (393 lines)
- `addons/product/static/img/maroon.png` (340 lines)
- `addons/product/static/img/membership_0-image.jpg` (20 lines)
- `addons/product/static/img/membership_1-image.jpg` (24 lines)
- `addons/product/static/img/membership_2-image.jpg` (27 lines)
- `addons/product/static/img/metal.png` (172 lines)
- `addons/product/static/img/monitor_stand.jpg` (267 lines)
- `addons/product/static/img/office_combo.jpg` (1,034 lines)
- `addons/product/static/img/placeholder.png` (254 lines)
- `addons/product/static/img/placeholder_thumbnail.png` (23 lines)
- `addons/product/static/img/product_chair.jpg` (78 lines)
- `addons/product/static/img/product_lamp.png` (77 lines)
- `addons/product/static/img/product_product_10-image.jpg` (120 lines)
- `addons/product/static/img/product_product_11-image.jpg` (1,125 lines)
- `addons/product/static/img/product_product_11b-image.jpg` (1,444 lines)
- `addons/product/static/img/product_product_12-image.jpg` (179 lines)
- `addons/product/static/img/product_product_13-image.jpg` (719 lines)
- `addons/product/static/img/product_product_16-image.jpg` (88 lines)
- `addons/product/static/img/product_product_20-image.png` (243 lines)
- `addons/product/static/img/product_product_22-image.png` (128 lines)
- `addons/product/static/img/product_product_24-image.jpg` (810 lines)
- `addons/product/static/img/product_product_25-image.jpg` (346 lines)
- `addons/product/static/img/product_product_25_black-image.jpg` (563 lines)
- `addons/product/static/img/product_product_27-image.jpg` (86 lines)
- `addons/product/static/img/product_product_3-image.jpg` (42 lines)
- `addons/product/static/img/product_product_43-image.jpg` (147 lines)
- `addons/product/static/img/product_product_46-image.jpg` (903 lines)
- `addons/product/static/img/product_product_5-image.jpg` (700 lines)
- `addons/product/static/img/product_product_6-image.jpg` (89 lines)
- `addons/product/static/img/product_product_7-image.png` (143 lines)
- `addons/product/static/img/product_product_8-image.jpg` (1,611 lines)
- `addons/product/static/img/product_product_8_glass-image.jpg` (646 lines)
- `addons/product/static/img/product_product_8_metal-image.jpg` (296 lines)
- `addons/product/static/img/product_product_9-image.jpg` (79 lines)
- `addons/product/static/img/product_product_d01-image.jpg` (120 lines)
- `addons/product/static/img/product_product_d01b-image.jpg` (152 lines)
- `addons/product/static/img/product_product_d01c-image.jpg` (129 lines)

Additional files not expanded here: 97. Full paths are in `01_CODEBASE_ANALYSIS/Repository_Inventory.csv`.

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
