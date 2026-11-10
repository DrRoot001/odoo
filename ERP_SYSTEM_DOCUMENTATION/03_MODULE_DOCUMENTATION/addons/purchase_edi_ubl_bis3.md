# Module: purchase_edi_ubl_bis3

- **Module ID:** MOD-497
- **Path:** `addons/purchase_edi_ubl_bis3`
- **Manifest:** `addons/purchase_edi_ubl_bis3/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Allows to export and import formats: UBL Bis 3.
When generating the PDF on the order, the PDF will be embedded inside the xml for all UBL formats. This allows the
receiver to retrieve the PDF with only the xml file.
    

Declared dependencies: `purchase`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "purchase",
    "account_edi_ubl_cii"
  ]
}
```

### Representative source files

- `addons/purchase_edi_ubl_bis3/__init__.py` (1 lines)
- `addons/purchase_edi_ubl_bis3/__manifest__.py` (13 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ar.po` (87 lines)
- `addons/purchase_edi_ubl_bis3/i18n/az.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/bg.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/bs.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ca.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/cs.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/da.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/de.po` (91 lines)
- `addons/purchase_edi_ubl_bis3/i18n/el.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/es.po` (92 lines)
- `addons/purchase_edi_ubl_bis3/i18n/es_419.po` (87 lines)
- `addons/purchase_edi_ubl_bis3/i18n/et.po` (90 lines)
- `addons/purchase_edi_ubl_bis3/i18n/fa.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/fi.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/i18n/fr.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/i18n/he.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/hi.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/hr.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/hu.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/id.po` (85 lines)
- `addons/purchase_edi_ubl_bis3/i18n/it.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ja.po` (85 lines)
- `addons/purchase_edi_ubl_bis3/i18n/kab.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ko.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ku.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/lo.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/lt.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/lv.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/mn.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/my.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/nb.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/nl.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/i18n/pl.po` (85 lines)
- `addons/purchase_edi_ubl_bis3/i18n/pt.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/pt_BR.po` (92 lines)
- `addons/purchase_edi_ubl_bis3/i18n/purchase_edi_ubl_bis3.pot` (78 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ro.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/ru.po` (87 lines)
- `addons/purchase_edi_ubl_bis3/i18n/sk.po` (82 lines)
- `addons/purchase_edi_ubl_bis3/i18n/sl.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/sr@latin.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/sv.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/i18n/th.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/tr.po` (89 lines)
- `addons/purchase_edi_ubl_bis3/i18n/uk.po` (83 lines)
- `addons/purchase_edi_ubl_bis3/i18n/uz.po` (96 lines)
- `addons/purchase_edi_ubl_bis3/i18n/vi.po` (84 lines)
- `addons/purchase_edi_ubl_bis3/i18n/zh_CN.po` (89 lines)
- `addons/purchase_edi_ubl_bis3/i18n/zh_TW.po` (86 lines)
- `addons/purchase_edi_ubl_bis3/models/__init__.py` (3 lines)
- `addons/purchase_edi_ubl_bis3/models/account_move.py` (12 lines)
- `addons/purchase_edi_ubl_bis3/models/purchase_edi_xml_ubl_bis3.py` (399 lines)
- `addons/purchase_edi_ubl_bis3/models/purchase_order.py` (57 lines)
- `addons/purchase_edi_ubl_bis3/tests/__init__.py` (2 lines)
- `addons/purchase_edi_ubl_bis3/tests/data/test_po_edi.xml` (146 lines)
- `addons/purchase_edi_ubl_bis3/tests/test_account_move_import.py` (179 lines)
- `addons/purchase_edi_ubl_bis3/tests/test_files/ubl_bis3_PO.xml` (154 lines)
- `addons/purchase_edi_ubl_bis3/tests/test_files/ubl_bis3_PO_description.xml` (152 lines)
- `addons/purchase_edi_ubl_bis3/tests/test_purchase_order_edi_gen.py` (55 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
