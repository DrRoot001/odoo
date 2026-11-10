# Module: pos_edi_ubl

- **Module ID:** MOD-429
- **Path:** `addons/pos_edi_ubl`
- **Manifest:** `addons/pos_edi_ubl/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

UBL in the Point of Sale 



This module provides helpers for exporting POS orders in various UBL 2.1 formats.



Declared dependencies: `point_of_sale`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale",
    "account_edi_ubl_cii"
  ]
}
```

### Representative source files

- `addons/pos_edi_ubl/__init__.py` (1 lines)
- `addons/pos_edi_ubl/__manifest__.py` (14 lines)
- `addons/pos_edi_ubl/i18n/ar.po` (56 lines)
- `addons/pos_edi_ubl/i18n/az.po` (54 lines)
- `addons/pos_edi_ubl/i18n/bg.po` (54 lines)
- `addons/pos_edi_ubl/i18n/bs.po` (55 lines)
- `addons/pos_edi_ubl/i18n/ca.po` (54 lines)
- `addons/pos_edi_ubl/i18n/cs.po` (54 lines)
- `addons/pos_edi_ubl/i18n/da.po` (54 lines)
- `addons/pos_edi_ubl/i18n/de.po` (60 lines)
- `addons/pos_edi_ubl/i18n/el.po` (54 lines)
- `addons/pos_edi_ubl/i18n/es.po` (60 lines)
- `addons/pos_edi_ubl/i18n/es_419.po` (56 lines)
- `addons/pos_edi_ubl/i18n/et.po` (54 lines)
- `addons/pos_edi_ubl/i18n/fa.po` (54 lines)
- `addons/pos_edi_ubl/i18n/fi.po` (55 lines)
- `addons/pos_edi_ubl/i18n/fr.po` (55 lines)
- `addons/pos_edi_ubl/i18n/he.po` (55 lines)
- `addons/pos_edi_ubl/i18n/hi.po` (54 lines)
- `addons/pos_edi_ubl/i18n/hr.po` (55 lines)
- `addons/pos_edi_ubl/i18n/hu.po` (54 lines)
- `addons/pos_edi_ubl/i18n/id.po` (55 lines)
- `addons/pos_edi_ubl/i18n/it.po` (60 lines)
- `addons/pos_edi_ubl/i18n/ja.po` (55 lines)
- `addons/pos_edi_ubl/i18n/kab.po` (54 lines)
- `addons/pos_edi_ubl/i18n/ko.po` (54 lines)
- `addons/pos_edi_ubl/i18n/ku.po` (54 lines)
- `addons/pos_edi_ubl/i18n/lo.po` (54 lines)
- `addons/pos_edi_ubl/i18n/lt.po` (56 lines)
- `addons/pos_edi_ubl/i18n/lv.po` (55 lines)
- `addons/pos_edi_ubl/i18n/mn.po` (54 lines)
- `addons/pos_edi_ubl/i18n/my.po` (54 lines)
- `addons/pos_edi_ubl/i18n/nb.po` (54 lines)
- `addons/pos_edi_ubl/i18n/nl.po` (55 lines)
- `addons/pos_edi_ubl/i18n/pl.po` (56 lines)
- `addons/pos_edi_ubl/i18n/pos_edi_ubl.pot` (50 lines)
- `addons/pos_edi_ubl/i18n/pt.po` (54 lines)
- `addons/pos_edi_ubl/i18n/pt_BR.po` (62 lines)
- `addons/pos_edi_ubl/i18n/ro.po` (55 lines)
- `addons/pos_edi_ubl/i18n/ru.po` (56 lines)
- `addons/pos_edi_ubl/i18n/sk.po` (54 lines)
- `addons/pos_edi_ubl/i18n/sl.po` (55 lines)
- `addons/pos_edi_ubl/i18n/sr@latin.po` (55 lines)
- `addons/pos_edi_ubl/i18n/sv.po` (55 lines)
- `addons/pos_edi_ubl/i18n/th.po` (55 lines)
- `addons/pos_edi_ubl/i18n/tr.po` (54 lines)
- `addons/pos_edi_ubl/i18n/uk.po` (55 lines)
- `addons/pos_edi_ubl/i18n/uz.po` (54 lines)
- `addons/pos_edi_ubl/i18n/vi.po` (54 lines)
- `addons/pos_edi_ubl/i18n/zh_CN.po` (59 lines)
- `addons/pos_edi_ubl/i18n/zh_TW.po` (54 lines)
- `addons/pos_edi_ubl/models/__init__.py` (1 lines)
- `addons/pos_edi_ubl/models/pos_edi_ubl_21.py` (203 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
