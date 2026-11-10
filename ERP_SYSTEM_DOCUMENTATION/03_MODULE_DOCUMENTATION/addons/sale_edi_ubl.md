# Module: sale_edi_ubl

- **Module ID:** MOD-511
- **Path:** `addons/sale_edi_ubl`
- **Manifest:** `addons/sale_edi_ubl/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Electronic ordering module
===========================

Allows to import formats: UBL Bis 3.
When uploading or pasting Files in order list view with order related data inside XML file or PDF
File with embedded xml data will allow seller to retrieve Order data from Files.
    

Declared dependencies: `sale`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "account_edi_ubl_cii"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/sale_edi_ubl/__init__.py` (1 lines)
- `addons/sale_edi_ubl/__manifest__.py` (19 lines)
- `addons/sale_edi_ubl/i18n/ar.po` (139 lines)
- `addons/sale_edi_ubl/i18n/az.po` (135 lines)
- `addons/sale_edi_ubl/i18n/bg.po` (135 lines)
- `addons/sale_edi_ubl/i18n/bs.po` (137 lines)
- `addons/sale_edi_ubl/i18n/ca.po` (136 lines)
- `addons/sale_edi_ubl/i18n/cs.po` (137 lines)
- `addons/sale_edi_ubl/i18n/da.po` (137 lines)
- `addons/sale_edi_ubl/i18n/de.po` (147 lines)
- `addons/sale_edi_ubl/i18n/el.po` (136 lines)
- `addons/sale_edi_ubl/i18n/es.po` (147 lines)
- `addons/sale_edi_ubl/i18n/es_419.po` (147 lines)
- `addons/sale_edi_ubl/i18n/et.po` (136 lines)
- `addons/sale_edi_ubl/i18n/fa.po` (135 lines)
- `addons/sale_edi_ubl/i18n/fi.po` (146 lines)
- `addons/sale_edi_ubl/i18n/fr.po` (138 lines)
- `addons/sale_edi_ubl/i18n/he.po` (136 lines)
- `addons/sale_edi_ubl/i18n/hi.po` (135 lines)
- `addons/sale_edi_ubl/i18n/hr.po` (136 lines)
- `addons/sale_edi_ubl/i18n/hu.po` (136 lines)
- `addons/sale_edi_ubl/i18n/id.po` (138 lines)
- `addons/sale_edi_ubl/i18n/it.po` (137 lines)
- `addons/sale_edi_ubl/i18n/ja.po` (137 lines)
- `addons/sale_edi_ubl/i18n/kab.po` (136 lines)
- `addons/sale_edi_ubl/i18n/ko.po` (137 lines)
- `addons/sale_edi_ubl/i18n/ku.po` (135 lines)
- `addons/sale_edi_ubl/i18n/lo.po` (135 lines)
- `addons/sale_edi_ubl/i18n/lt.po` (137 lines)
- `addons/sale_edi_ubl/i18n/lv.po` (136 lines)
- `addons/sale_edi_ubl/i18n/mn.po` (135 lines)
- `addons/sale_edi_ubl/i18n/my.po` (136 lines)
- `addons/sale_edi_ubl/i18n/nb.po` (136 lines)
- `addons/sale_edi_ubl/i18n/nl.po` (138 lines)
- `addons/sale_edi_ubl/i18n/pl.po` (139 lines)
- `addons/sale_edi_ubl/i18n/pt.po` (136 lines)
- `addons/sale_edi_ubl/i18n/pt_BR.po` (147 lines)
- `addons/sale_edi_ubl/i18n/ro.po` (137 lines)
- `addons/sale_edi_ubl/i18n/ru.po` (138 lines)
- `addons/sale_edi_ubl/i18n/sale_edi_ubl.pot` (130 lines)
- `addons/sale_edi_ubl/i18n/sk.po` (135 lines)
- `addons/sale_edi_ubl/i18n/sl.po` (137 lines)
- `addons/sale_edi_ubl/i18n/sr@latin.po` (136 lines)
- `addons/sale_edi_ubl/i18n/sv.po` (137 lines)
- `addons/sale_edi_ubl/i18n/th.po` (137 lines)
- `addons/sale_edi_ubl/i18n/tr.po` (140 lines)
- `addons/sale_edi_ubl/i18n/uk.po` (136 lines)
- `addons/sale_edi_ubl/i18n/uz.po` (150 lines)
- `addons/sale_edi_ubl/i18n/vi.po` (137 lines)
- `addons/sale_edi_ubl/i18n/zh_CN.po` (145 lines)
- `addons/sale_edi_ubl/i18n/zh_TW.po` (139 lines)
- `addons/sale_edi_ubl/models/__init__.py` (6 lines)
- `addons/sale_edi_ubl/models/customer_product_reference.py` (75 lines)
- `addons/sale_edi_ubl/models/product_product.py` (48 lines)
- `addons/sale_edi_ubl/models/sale_edi_xml_ubl_bis3.py` (410 lines)
- `addons/sale_edi_ubl/models/sale_order.py` (75 lines)
- `addons/sale_edi_ubl/models/sale_order_line.py` (9 lines)
- `addons/sale_edi_ubl/security/ir.access.csv` (2 lines)
- `addons/sale_edi_ubl/tests/__init__.py` (1 lines)
- `addons/sale_edi_ubl/tests/data/test_so_edi.xml` (148 lines)
- `addons/sale_edi_ubl/tests/test_sale_order_edi_gen.py` (55 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
