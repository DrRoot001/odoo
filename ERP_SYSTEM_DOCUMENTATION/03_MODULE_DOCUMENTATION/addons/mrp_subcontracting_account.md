# Module: mrp_subcontracting_account

- **Module ID:** MOD-384
- **Path:** `addons/mrp_subcontracting_account`
- **Manifest:** `addons/mrp_subcontracting_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This bridge module allows to manage subcontracting with valuation.
    

Declared dependencies: `mrp_subcontracting`, `mrp_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp_subcontracting",
    "mrp_account"
  ],
  "data": [
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/mrp_subcontracting_account/__init__.py` (4 lines)
- `addons/mrp_subcontracting_account/__manifest__.py` (17 lines)
- `addons/mrp_subcontracting_account/i18n/ar.po` (59 lines)
- `addons/mrp_subcontracting_account/i18n/az.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/bg.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/bs.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/ca.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/cs.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/da.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/de.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/el.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/es.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/es_419.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/et.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/fa.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/fi.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/fr.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/he.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/hi.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/hr.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/hu.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/id.po` (56 lines)
- `addons/mrp_subcontracting_account/i18n/it.po` (57 lines)
- `addons/mrp_subcontracting_account/i18n/ja.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/kab.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/ko.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/ku.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/lo.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/lt.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/lv.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/mn.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/mrp_subcontracting_account.pot` (50 lines)
- `addons/mrp_subcontracting_account/i18n/my.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/nb.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/nl.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/pl.po` (56 lines)
- `addons/mrp_subcontracting_account/i18n/pt.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/pt_BR.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/ro.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/ru.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/sk.po` (53 lines)
- `addons/mrp_subcontracting_account/i18n/sl.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/sr@latin.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/sv.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/th.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/tr.po` (58 lines)
- `addons/mrp_subcontracting_account/i18n/uk.po` (54 lines)
- `addons/mrp_subcontracting_account/i18n/uz.po` (65 lines)
- `addons/mrp_subcontracting_account/i18n/vi.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/zh_CN.po` (55 lines)
- `addons/mrp_subcontracting_account/i18n/zh_TW.po` (57 lines)
- `addons/mrp_subcontracting_account/models/__init__.py` (5 lines)
- `addons/mrp_subcontracting_account/models/mrp_production.py` (23 lines)
- `addons/mrp_subcontracting_account/models/product_product.py` (19 lines)
- `addons/mrp_subcontracting_account/security/ir.access.csv` (3 lines)
- `addons/mrp_subcontracting_account/tests/__init__.py` (4 lines)
- `addons/mrp_subcontracting_account/tests/test_subcontracting_account.py` (383 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
