# Module: sale_gelato

- **Module ID:** MOD-514
- **Path:** `addons/sale_gelato`
- **Manifest:** `addons/sale_gelato/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Place orders through Gelato's print-on-demand service

No manifest description declared.

Declared dependencies: `sale`, `delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 22 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "delivery"
  ],
  "data": [
    "data/product_data.xml",
    "data/delivery_carrier_data.xml",
    "data/mail_template_data.xml",
    "views/delivery_carrier_views.xml",
    "views/product_document_views.xml",
    "views/product_product_views.xml",
    "views/product_template_views.xml",
    "wizards/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/sale_gelato/__init__.py` (3 lines)
- `addons/sale_gelato/__manifest__.py` (20 lines)
- `addons/sale_gelato/const.py` (70 lines)
- `addons/sale_gelato/controllers/__init__.py` (3 lines)
- `addons/sale_gelato/controllers/main.py` (138 lines)
- `addons/sale_gelato/data/delivery_carrier_data.xml` (22 lines)
- `addons/sale_gelato/data/mail_template_data.xml` (46 lines)
- `addons/sale_gelato/data/neutralize.sql` (4 lines)
- `addons/sale_gelato/data/product_data.xml` (24 lines)
- `addons/sale_gelato/i18n/ar.po` (542 lines)
- `addons/sale_gelato/i18n/az.po` (451 lines)
- `addons/sale_gelato/i18n/bg.po` (451 lines)
- `addons/sale_gelato/i18n/bs.po` (452 lines)
- `addons/sale_gelato/i18n/ca.po` (541 lines)
- `addons/sale_gelato/i18n/cs.po` (452 lines)
- `addons/sale_gelato/i18n/da.po` (464 lines)
- `addons/sale_gelato/i18n/de.po` (558 lines)
- `addons/sale_gelato/i18n/el.po` (452 lines)
- `addons/sale_gelato/i18n/es.po` (547 lines)
- `addons/sale_gelato/i18n/es_419.po` (553 lines)
- `addons/sale_gelato/i18n/et.po` (451 lines)
- `addons/sale_gelato/i18n/fa.po` (451 lines)
- `addons/sale_gelato/i18n/fi.po` (554 lines)
- `addons/sale_gelato/i18n/fr.po` (559 lines)
- `addons/sale_gelato/i18n/he.po` (452 lines)
- `addons/sale_gelato/i18n/hi.po` (451 lines)
- `addons/sale_gelato/i18n/hr.po` (452 lines)
- `addons/sale_gelato/i18n/hu.po` (461 lines)
- `addons/sale_gelato/i18n/id.po` (552 lines)
- `addons/sale_gelato/i18n/it.po` (556 lines)
- `addons/sale_gelato/i18n/ja.po` (550 lines)
- `addons/sale_gelato/i18n/kab.po` (451 lines)
- `addons/sale_gelato/i18n/ko.po` (544 lines)
- `addons/sale_gelato/i18n/ku.po` (451 lines)
- `addons/sale_gelato/i18n/lo.po` (545 lines)
- `addons/sale_gelato/i18n/lt.po` (453 lines)
- `addons/sale_gelato/i18n/lv.po` (451 lines)
- `addons/sale_gelato/i18n/mn.po` (451 lines)
- `addons/sale_gelato/i18n/my.po` (451 lines)
- `addons/sale_gelato/i18n/nb.po` (452 lines)
- `addons/sale_gelato/i18n/nl.po` (552 lines)
- `addons/sale_gelato/i18n/pl.po` (468 lines)
- `addons/sale_gelato/i18n/pt.po` (537 lines)
- `addons/sale_gelato/i18n/pt_BR.po` (545 lines)
- `addons/sale_gelato/i18n/ro.po` (466 lines)
- `addons/sale_gelato/i18n/ru.po` (552 lines)
- `addons/sale_gelato/i18n/sale_gelato.pot` (436 lines)
- `addons/sale_gelato/i18n/sk.po` (450 lines)
- `addons/sale_gelato/i18n/sl.po` (453 lines)
- `addons/sale_gelato/i18n/sr@latin.po` (452 lines)
- `addons/sale_gelato/i18n/sv.po` (453 lines)
- `addons/sale_gelato/i18n/th.po` (544 lines)
- `addons/sale_gelato/i18n/tr.po` (465 lines)
- `addons/sale_gelato/i18n/uk.po` (452 lines)
- `addons/sale_gelato/i18n/uz.po` (516 lines)
- `addons/sale_gelato/i18n/vi.po` (465 lines)
- `addons/sale_gelato/i18n/zh_CN.po` (546 lines)
- `addons/sale_gelato/i18n/zh_TW.po` (465 lines)
- `addons/sale_gelato/models/__init__.py` (12 lines)
- `addons/sale_gelato/models/delivery_carrier.py` (109 lines)
- `addons/sale_gelato/models/product_document.py` (29 lines)
- `addons/sale_gelato/models/product_product.py` (51 lines)
- `addons/sale_gelato/models/product_template.py` (215 lines)
- `addons/sale_gelato/models/res_company.py` (10 lines)
- `addons/sale_gelato/models/res_partner.py` (88 lines)
- `addons/sale_gelato/models/sale_order.py` (248 lines)
- `addons/sale_gelato/models/sale_order_line.py` (32 lines)
- `addons/sale_gelato/static/description/icon.png` (8 lines)
- `addons/sale_gelato/static/description/icon.svg` (18 lines)
- `addons/sale_gelato/tests/__init__.py` (3 lines)
- `addons/sale_gelato/tests/common.py` (58 lines)
- `addons/sale_gelato/tests/test_delivery_carrier.py` (81 lines)
- `addons/sale_gelato/tests/test_product_template.py` (140 lines)
- `addons/sale_gelato/tests/test_sale_order.py` (58 lines)
- `addons/sale_gelato/utils.py` (45 lines)
- `addons/sale_gelato/views/delivery_carrier_views.xml` (24 lines)
- `addons/sale_gelato/views/product_document_views.xml` (18 lines)
- `addons/sale_gelato/views/product_product_views.xml` (53 lines)
- `addons/sale_gelato/views/product_template_views.xml` (66 lines)
- `addons/sale_gelato/wizards/__init__.py` (3 lines)
- `addons/sale_gelato/wizards/res_config_settings.py` (10 lines)
- `addons/sale_gelato/wizards/res_config_settings_views.xml` (31 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
