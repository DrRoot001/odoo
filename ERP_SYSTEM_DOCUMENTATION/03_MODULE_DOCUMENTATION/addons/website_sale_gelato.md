# Module: website_sale_gelato

- **Module ID:** MOD-636
- **Path:** `addons/website_sale_gelato`
- **Manifest:** `addons/website_sale_gelato/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `sale_gelato`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_gelato",
    "website_sale"
  ],
  "data": [
    "data/delivery_carrier_data.xml",
    "views/address_templates.xml"
  ]
}
```

### Representative source files

- `addons/website_sale_gelato/__init__.py` (3 lines)
- `addons/website_sale_gelato/__manifest__.py` (11 lines)
- `addons/website_sale_gelato/data/delivery_carrier_data.xml` (14 lines)
- `addons/website_sale_gelato/i18n/ar.po` (109 lines)
- `addons/website_sale_gelato/i18n/az.po` (105 lines)
- `addons/website_sale_gelato/i18n/bg.po` (105 lines)
- `addons/website_sale_gelato/i18n/bs.po` (107 lines)
- `addons/website_sale_gelato/i18n/ca.po` (108 lines)
- `addons/website_sale_gelato/i18n/cs.po` (106 lines)
- `addons/website_sale_gelato/i18n/da.po` (111 lines)
- `addons/website_sale_gelato/i18n/de.po` (114 lines)
- `addons/website_sale_gelato/i18n/el.po` (106 lines)
- `addons/website_sale_gelato/i18n/es.po` (114 lines)
- `addons/website_sale_gelato/i18n/es_419.po` (113 lines)
- `addons/website_sale_gelato/i18n/et.po` (105 lines)
- `addons/website_sale_gelato/i18n/fa.po` (105 lines)
- `addons/website_sale_gelato/i18n/fi.po` (111 lines)
- `addons/website_sale_gelato/i18n/fr.po` (115 lines)
- `addons/website_sale_gelato/i18n/he.po` (106 lines)
- `addons/website_sale_gelato/i18n/hi.po` (105 lines)
- `addons/website_sale_gelato/i18n/hr.po` (106 lines)
- `addons/website_sale_gelato/i18n/hu.po` (106 lines)
- `addons/website_sale_gelato/i18n/id.po` (113 lines)
- `addons/website_sale_gelato/i18n/it.po` (114 lines)
- `addons/website_sale_gelato/i18n/ja.po` (109 lines)
- `addons/website_sale_gelato/i18n/kab.po` (106 lines)
- `addons/website_sale_gelato/i18n/ko.po` (108 lines)
- `addons/website_sale_gelato/i18n/ku.po` (105 lines)
- `addons/website_sale_gelato/i18n/lo.po` (105 lines)
- `addons/website_sale_gelato/i18n/lt.po` (107 lines)
- `addons/website_sale_gelato/i18n/lv.po` (106 lines)
- `addons/website_sale_gelato/i18n/mn.po` (105 lines)
- `addons/website_sale_gelato/i18n/my.po` (105 lines)
- `addons/website_sale_gelato/i18n/nb.po` (106 lines)
- `addons/website_sale_gelato/i18n/nl.po` (114 lines)
- `addons/website_sale_gelato/i18n/pl.po` (114 lines)
- `addons/website_sale_gelato/i18n/pt.po` (113 lines)
- `addons/website_sale_gelato/i18n/pt_BR.po` (115 lines)
- `addons/website_sale_gelato/i18n/ro.po` (113 lines)
- `addons/website_sale_gelato/i18n/ru.po` (115 lines)
- `addons/website_sale_gelato/i18n/sk.po` (105 lines)
- `addons/website_sale_gelato/i18n/sl.po` (107 lines)
- `addons/website_sale_gelato/i18n/sr@latin.po` (106 lines)
- `addons/website_sale_gelato/i18n/sv.po` (110 lines)
- `addons/website_sale_gelato/i18n/th.po` (110 lines)
- `addons/website_sale_gelato/i18n/tr.po` (113 lines)
- `addons/website_sale_gelato/i18n/uk.po` (106 lines)
- `addons/website_sale_gelato/i18n/uz.po` (127 lines)
- `addons/website_sale_gelato/i18n/vi.po` (108 lines)
- `addons/website_sale_gelato/i18n/website_sale_gelato.pot` (102 lines)
- `addons/website_sale_gelato/i18n/zh_CN.po` (109 lines)
- `addons/website_sale_gelato/i18n/zh_TW.po` (111 lines)
- `addons/website_sale_gelato/models/__init__.py` (3 lines)
- `addons/website_sale_gelato/models/product_document.py` (22 lines)
- `addons/website_sale_gelato/models/product_template.py` (25 lines)
- `addons/website_sale_gelato/models/res_partner.py` (27 lines)
- `addons/website_sale_gelato/models/sale_order.py` (46 lines)
- `addons/website_sale_gelato/tests/__init__.py` (3 lines)
- `addons/website_sale_gelato/tests/test_address.py` (46 lines)
- `addons/website_sale_gelato/tests/test_product_template.py` (36 lines)
- `addons/website_sale_gelato/views/address_templates.xml` (47 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
