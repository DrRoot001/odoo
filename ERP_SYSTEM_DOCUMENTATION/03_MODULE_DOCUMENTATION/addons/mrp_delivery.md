# Module: mrp_delivery

- **Module ID:** MOD-379
- **Path:** `addons/mrp_delivery`
- **Manifest:** `addons/mrp_delivery/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Carrier with kits

Manage datas of carriers with kit products

Declared dependencies: `mrp`, `stock_delivery`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp",
    "stock_delivery"
  ]
}
```

### Representative source files

- `addons/mrp_delivery/__init__.py` (3 lines)
- `addons/mrp_delivery/__manifest__.py` (12 lines)
- `addons/mrp_delivery/i18n/ar.po` (50 lines)
- `addons/mrp_delivery/i18n/az.po` (49 lines)
- `addons/mrp_delivery/i18n/bg.po` (49 lines)
- `addons/mrp_delivery/i18n/bs.po` (50 lines)
- `addons/mrp_delivery/i18n/ca.po` (49 lines)
- `addons/mrp_delivery/i18n/cs.po` (49 lines)
- `addons/mrp_delivery/i18n/da.po` (50 lines)
- `addons/mrp_delivery/i18n/de.po` (50 lines)
- `addons/mrp_delivery/i18n/el.po` (49 lines)
- `addons/mrp_delivery/i18n/es.po` (50 lines)
- `addons/mrp_delivery/i18n/es_419.po` (50 lines)
- `addons/mrp_delivery/i18n/et.po` (49 lines)
- `addons/mrp_delivery/i18n/fa.po` (49 lines)
- `addons/mrp_delivery/i18n/fi.po` (50 lines)
- `addons/mrp_delivery/i18n/fr.po` (50 lines)
- `addons/mrp_delivery/i18n/he.po` (50 lines)
- `addons/mrp_delivery/i18n/hi.po` (49 lines)
- `addons/mrp_delivery/i18n/hr.po` (50 lines)
- `addons/mrp_delivery/i18n/hu.po` (49 lines)
- `addons/mrp_delivery/i18n/id.po` (49 lines)
- `addons/mrp_delivery/i18n/it.po` (50 lines)
- `addons/mrp_delivery/i18n/ja.po` (50 lines)
- `addons/mrp_delivery/i18n/kab.po` (49 lines)
- `addons/mrp_delivery/i18n/ko.po` (49 lines)
- `addons/mrp_delivery/i18n/ku.po` (49 lines)
- `addons/mrp_delivery/i18n/lo.po` (49 lines)
- `addons/mrp_delivery/i18n/lt.po` (51 lines)
- `addons/mrp_delivery/i18n/lv.po` (50 lines)
- `addons/mrp_delivery/i18n/mn.po` (49 lines)
- `addons/mrp_delivery/i18n/mrp_delivery.pot` (46 lines)
- `addons/mrp_delivery/i18n/my.po` (49 lines)
- `addons/mrp_delivery/i18n/nb.po` (49 lines)
- `addons/mrp_delivery/i18n/nl.po` (50 lines)
- `addons/mrp_delivery/i18n/pl.po` (50 lines)
- `addons/mrp_delivery/i18n/pt.po` (49 lines)
- `addons/mrp_delivery/i18n/pt_BR.po` (51 lines)
- `addons/mrp_delivery/i18n/ro.po` (50 lines)
- `addons/mrp_delivery/i18n/ru.po` (50 lines)
- `addons/mrp_delivery/i18n/sk.po` (49 lines)
- `addons/mrp_delivery/i18n/sl.po` (50 lines)
- `addons/mrp_delivery/i18n/sr@latin.po` (50 lines)
- `addons/mrp_delivery/i18n/sv.po` (50 lines)
- `addons/mrp_delivery/i18n/th.po` (50 lines)
- `addons/mrp_delivery/i18n/tr.po` (49 lines)
- `addons/mrp_delivery/i18n/uk.po` (50 lines)
- `addons/mrp_delivery/i18n/uz.po` (49 lines)
- `addons/mrp_delivery/i18n/vi.po` (49 lines)
- `addons/mrp_delivery/i18n/zh_CN.po` (50 lines)
- `addons/mrp_delivery/i18n/zh_TW.po` (49 lines)
- `addons/mrp_delivery/models/__init__.py` (3 lines)
- `addons/mrp_delivery/models/stock_move_line.py` (34 lines)
- `addons/mrp_delivery/tests/__init__.py` (3 lines)
- `addons/mrp_delivery/tests/test_delivery_mrp_kit.py` (162 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
